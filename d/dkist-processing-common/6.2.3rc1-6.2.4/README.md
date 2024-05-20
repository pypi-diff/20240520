# Comparing `tmp/dkist-processing-common-6.2.3rc1.tar.gz` & `tmp/dkist-processing-common-6.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-6.2.3rc1.tar", last modified: Thu May  9 16:15:12 2024, max compression
+gzip compressed data, was "dkist-processing-common-6.2.4.tar", last modified: Mon May 20 21:56:03 2024, max compression
```

## Comparing `dkist-processing-common-6.2.3rc1.tar` & `dkist-processing-common-6.2.4.tar`

### file list

```diff
@@ -1,139 +1,136 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    25646 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4394 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3271 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.454883 dkist-processing-common-6.2.3rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/189.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/190.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/191.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.454883 dkist-processing-common-6.2.3rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.458883 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)    10378 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.458883 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/asdf.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/quality.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.458883 dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.462883 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/task_name.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.462883 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6461 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/unique_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.462883 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12776 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    13198 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9891 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.466884 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    14466 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.466884 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8130 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47664 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8266 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19802 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27198 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    16866 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    20569 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)    10946 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8346 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10629 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36887 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16481 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)    24306 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_stems.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_submit_dataset_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4027 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5494 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6658 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6814 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)    20114 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    17411 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.454883 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4394 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5168 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.444500 dkist-processing-common-6.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    26904 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2024-05-20 21:56:03.444500 dkist-processing-common-6.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.432500 dkist-processing-common-6.2.4/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.432500 dkist-processing-common-6.2.4/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.432500 dkist-processing-common-6.2.4/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)    10378 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.432500 dkist-processing-common-6.2.4/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/asdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.436500 dkist-processing-common-6.2.4/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.436500 dkist-processing-common-6.2.4/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.436500 dkist-processing-common-6.2.4/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/unique_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.440500 dkist-processing-common-6.2.4/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    13198 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9891 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.440500 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    14466 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.440500 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8130 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47730 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7986 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8266 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19802 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.444500 dkist-processing-common-6.2.4/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27289 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    16873 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_assemble_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    20569 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    10946 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10629 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    37086 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16481 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_stems.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_submit_dataset_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5494 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6814 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    20114 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    17411 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.432500 dkist-processing-common-6.2.4/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4391 2024-05-20 21:56:03.000000 dkist-processing-common-6.2.4/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5094 2024-05-20 21:56:03.000000 dkist-processing-common-6.2.4/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-20 21:56:03.000000 dkist-processing-common-6.2.4/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-20 21:56:03.000000 dkist-processing-common-6.2.4/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-20 21:56:03.000000 dkist-processing-common-6.2.4/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.444500 dkist-processing-common-6.2.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 21:56:03.444500 dkist-processing-common-6.2.4/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-05-20 21:56:03.444500 dkist-processing-common-6.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-20 21:55:57.000000 dkist-processing-common-6.2.4/setup.py
```

### Comparing `dkist-processing-common-6.2.3rc1/.gitignore` & `dkist-processing-common-6.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/.pre-commit-config.yaml` & `dkist-processing-common-6.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/CHANGELOG.rst` & `dkist-processing-common-6.2.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+v6.2.4 (2024-05-20)
+===================
+
+Bugfixes
+--------
+
+- No longer crash when building polcal metrics where some CS steps had `I_sys` fixed during the polcal fit. (`#193 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/193>`__)
+
+
+Misc
+----
+
+- Change the DKIST site time zone to US/Hawaii to correctly account for daylight savings time. (`#192 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/192>`__)
+- Pin `sphinx-autoapi` to avoid failure in doc build. (`#194 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/194>`__)
+
+
+v6.2.3 (2024-05-09)
+===================
+
+Features
+--------
+
+- Save all floating point arrays as float32. The extra precision of float64 is not needed, especially when lossy quantization is applied before compression. (`#191 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/191>`__)
+
+
+Bugfixes
+--------
+
+- `QualityMixin.avg_noise` is now NaN aware. I.e., it will ignore NaN values when computing the noise. (`#190 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/190>`__)
+
+
+Misc
+----
+
+- Cap the length of browse movies at 60 seconds by default. (`#189 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/189>`__)
+
+
 v6.2.2 (2024-05-07)
 ===================
 
 Features
 --------
 
 - Add the ability to create a quality report from a trial workflow. (`#185 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/185>`__)
```

### Comparing `dkist-processing-common-6.2.3rc1/PKG-INFO` & `dkist-processing-common-6.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.3rc1
+Version: 6.2.4
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.2.3rc1/README.rst` & `dkist-processing-common-6.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/bitbucket-pipelines.yml` & `dkist-processing-common-6.2.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/check_changelog_updated.sh` & `dkist-processing-common-6.2.4/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-6.2.4/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-6.2.4/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-6.2.4/dkist_processing_common/_util/dkist_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from astropy.coordinates import EarthLocation
 
 
 def location_of_dkist() -> EarthLocation:
     """Return hard-coded EarthLocation of the DKIST.
 
     Cartesian geocentric coordinates of DKIST on Earth as retrieved from
-    https://github.com/astropy/astropy-data/blob/gh-pages/coordinates/sites.json#L755
+    https://github.com/astropy/astropy-data/blob/gh-pages/coordinates/sites.json#L838
     """
     _dkist_site_info = {
         "aliases": ["DKIST", "ATST"],
         "name": "Daniel K. Inouye Solar Telescope",
         "elevation": 3067,
         "elevation_unit": "meter",
         "latitude": 20.7067,
         "latitude_unit": "degree",
         "longitude": 203.7436,
         "longitude_unit": "degree",
-        "timezone": "US/Aleutian",
+        "timezone": "US/Hawaii",
         "source": "DKIST website: https://www.nso.edu/telescopes/dki-solar-telescope/",
     }
     location_of_dkist = EarthLocation.from_geodetic(
         _dkist_site_info["longitude"] * u.Unit(_dkist_site_info["longitude_unit"]),
         _dkist_site_info["latitude"] * u.Unit(_dkist_site_info["latitude_unit"]),
         _dkist_site_info["elevation"] * u.Unit(_dkist_site_info["elevation_unit"]),
     )
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-6.2.4/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-6.2.4/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-6.2.4/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/asdf.py` & `dkist-processing-common-6.2.4/dkist_processing_common/codecs/asdf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-6.2.4/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-6.2.4/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/json.py` & `dkist-processing-common-6.2.4/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/quality.py` & `dkist-processing-common-6.2.4/dkist_processing_common/codecs/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/str.py` & `dkist-processing-common-6.2.4/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-6.2.4/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/manual.py` & `dkist-processing-common-6.2.4/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/task_name.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-6.2.4/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/task.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/wavelength.py` & `dkist-processing-common-6.2.4/dkist_processing_common/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/__init__.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -876,15 +876,14 @@
         First, flatten FOV bins dimensions, compute modulation matrices, and record I_sys for all bins.
 
         Then convert to python lists for serialization and write to disk.
         """
         ## Modulation matrices
         fov_shape = polcal_fitter.local_objects.dresser.shape
         num_mod = polcal_fitter.local_objects.dresser.nummod
-        num_steps = polcal_fitter.local_objects.dresser.numsteps
         flattened_demod = np.reshape(
             polcal_fitter.demodulation_matrices, (np.prod(fov_shape), 4, num_mod)
         )
         flattened_mod = np.zeros((np.prod(fov_shape), num_mod, 4))
         for i in range(flattened_demod.shape[0]):
             flattened_mod[i] = np.linalg.pinv(flattened_demod[i])
 
@@ -897,34 +896,38 @@
 
         # Now get the rest of the free variables
         fit_params = polcal_fitter.local_objects.fit_parameters
         init_param = polcal_fitter.local_objects.init_parameters
         param_metadata = fit_params.first_parameters
 
         free_param_data = dict()
+        num_varied_I_sys = 0
         for param in param_metadata.keys():
             # Don't grab modulation matrix values because we got those above.
             # Also don't grab any parameters that were fixed.
             if "modmat" in param or not param_metadata[param].vary:
                 continue
 
+            if param.startswith("I_sys"):
+                num_varied_I_sys += 1
+
             fit_value_list = []
             for point_param in fit_params._all_parameters:
                 fit_value_list.append(point_param[param].value)
 
             init_value = init_param.first_parameters[param].value
 
             free_param_data[param] = {"fit_values": fit_value_list, "init_value": init_value}
 
         data = {
             "task_type": label,
             "bin_1_str": f"{bins_1} {bin_1_type}",
             "bin_2_str": f"{bins_2} {bin_2_type}",
             "total_bins": bins_1 * bins_2,
-            "num_steps": num_steps,
+            "num_varied_I_sys": num_varied_I_sys,
             "modmat_list": mod_list,
             "free_param_dict": free_param_data,
         }
         self._record_values(
             values=data, tags=[Tag.quality("POLCAL_LOCAL_PAR_VALS"), Tag.quality_task(label)]
         )
 
@@ -936,15 +939,15 @@
         with data_file.open() as f:
             data = json.load(f)
 
         modmat_hist = ModulationMatrixHistograms(modmat_list=data["modmat_list"])
         free_param_dict = data["free_param_dict"]
         I_sys_series_data = dict()
         I_sys_vertical_lines = dict()
-        for step in range(data["num_steps"]):
+        for step in range(data["num_varied_I_sys"]):
             I_sys_series_data[f"CS step {step}"] = free_param_dict[f"I_sys_CS00_step{step:02n}"][
                 "fit_values"
             ]
             if step == 0:
                 I_sys_vertical_lines["init value"] = free_param_dict[f"I_sys_CS00_step{step:02n}"][
                     "init_value"
                 ]
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_catalog.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,17 +593,19 @@
 
         out_dict[n] = [InstAccess(h) for h in hdu_list]
         start_time = ds.start_time + timedelta(seconds=60)
 
     return out_dict, data_shape
 
 
-@pytest.fixture(scope="session")
-def pac_fit_mode() -> str:
-    return "use_M12"
+@pytest.fixture(
+    scope="session", params=[pytest.param("use_M12"), pytest.param("use_M12_I_sys_per_step")]
+)
+def pac_fit_mode(request) -> str:
+    return request.param
 
 
 @pytest.fixture(scope="session")
 def pac_init_set() -> str:
     return "OCCal_VIS"
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_quality.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_assemble_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
                     "I_sys_CS00_step00": {"fit_values": [1, 2, 3.0], "init_value": 0.3},
                     "I_sys_CS00_step01": {"fit_values": [10, 20, 30.0], "init_value": 0.33},
                     "param_X": {"fit_values": [5, 6, 7.0], "init_value": 99},
                 },
                 "bin_1_str": "bin1",
                 "bin_2_str": "bin2",
                 "total_bins": 100,
-                "num_steps": 2,
+                "num_varied_I_sys": 2,
             },
             ["QUALITY_POLCAL_LOCAL_PAR_VALS", "QUALITY_TASK_BEAM 1"],
         ),
         Metric(
             {
                 "bin_1_str": "bin1",
                 "bin_2_str": "bin2",
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,25 +690,32 @@
         local_par_dict = json.load(f)
         assert sorted(local_par_dict.keys()) == sorted(
             [
                 "task_type",
                 "bin_1_str",
                 "bin_2_str",
                 "total_bins",
-                "num_steps",
+                "num_varied_I_sys",
                 "modmat_list",
                 "free_param_dict",
             ]
         )
         assert local_par_dict["task_type"] == label
         assert type(local_par_dict["total_bins"]) == int
         assert type(local_par_dict["modmat_list"]) == list
         assert type(local_par_dict["free_param_dict"]) == dict
-        assert type(local_par_dict["free_param_dict"]["I_sys_CS00_step00"]["init_value"]) == float
-        assert type(local_par_dict["free_param_dict"]["I_sys_CS00_step00"]["fit_values"]) == list
+        for step in range(local_par_dict["num_varied_I_sys"]):
+            assert (
+                type(local_par_dict["free_param_dict"][f"I_sys_CS00_step{step:02n}"]["init_value"])
+                == float
+            )
+            assert (
+                type(local_par_dict["free_param_dict"][f"I_sys_CS00_step{step:02n}"]["fit_values"])
+                == list
+            )
 
     # Fit residuals
     fit_res_file = list(
         quality_task.read(tags=[Tag.quality("POLCAL_FIT_RESIDUALS"), Tag.quality_task(label)])
     )
     assert len(fit_res_file) == 1
     with open(fit_res_file[0], "r") as f:
@@ -848,15 +855,15 @@
 def polcal_local_params_json():
     label = "Beam 1"
     data = {
         "task_type": label,
         "bin_1_str": "2 spatial",
         "bin_2_str": "3 radical",
         "total_bins": 6,
-        "num_steps": 2,
+        "num_varied_I_sys": 2,
         "modmat_list": [[[1, 2.0], [2.0, 3.0]], [[10.0, 20.0], [20.0, 30.0]]],
         "free_param_dict": {
             "I_sys_CS00_step00": {"fit_values": [1, 2, 3.0], "init_value": 0.3},
             "I_sys_CS00_step01": {"fit_values": [10, 20, 30.0], "init_value": 0.33},
             "param_X": {"fit_values": [5, 6, 7.0], "init_value": 99},
         },
     }
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_stems.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_stems.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_submit_dataset_metadata.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_submit_dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_name.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_catalog.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-6.2.4/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-6.2.4/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.3rc1
+Version: 6.2.4
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-6.2.4/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/189.misc.rst
-changelog/190.bugfix.rst
-changelog/191.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-6.2.4/dkist_processing_common.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [asdf]
 dkist-inventory[asdf]>=1.3.1
 
 [docs]
 sphinx
 sphinx-astropy
 sphinx-changelog
-sphinx-autoapi
+sphinx-autoapi<3.1.0
 pytest
 towncrier<22.12.0
 dkist-sphinx-theme
 
 [inventory]
 dkist-inventory>=1.3.1
```

### Comparing `dkist-processing-common-6.2.3rc1/docs/Makefile` & `dkist-processing-common-6.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/docs/conf.py` & `dkist-processing-common-6.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/docs/make.bat` & `dkist-processing-common-6.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/licenses/LICENSE.rst` & `dkist-processing-common-6.2.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/pyproject.toml` & `dkist-processing-common-6.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.3rc1/setup.cfg` & `dkist-processing-common-6.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 	%(inventory)s
 	%(asdf)s
 	%(quality)s
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog
-	sphinx-autoapi
+	sphinx-autoapi < 3.1.0
 	pytest
 	towncrier < 22.12.0
 	dkist-sphinx-theme
 inventory = 
 	dkist-inventory >= 1.3.1
 asdf = 
 	dkist-inventory[asdf] >= 1.3.1
```

