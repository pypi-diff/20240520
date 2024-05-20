# Comparing `tmp/kohlrahbi-1.0.0.tar.gz` & `tmp/kohlrahbi-1.1.0.tar.gz`

## Comparing `kohlrahbi-1.0.0.tar` & `kohlrahbi-1.1.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.gitattributes
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/README.md
--rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/kohlrahbi-image.png
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/requirements.txt
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/tox.ini
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/wip.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxfilefinder.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0    11369 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/table_header.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/version.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahb/command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/__init__.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbcondtions.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbpackagetable.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbsubtable.py
--rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtable.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtablerow.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/changehistory/__init__.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/changehistory/changehistorytable.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/changehistory/command.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/conditions/__init__.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/conditions/command.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/ahbexportfileformat.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
--rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
--rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
--rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
--rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    19261 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/LICENSE
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.gitattributes
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/README.md
+-rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/kohlrahbi-image.png
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/tox.ini
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/wip.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxfilefinder.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/table_header.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/version.py
+-rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahb/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/__init__.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbcondtions.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbpackagetable.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbsubtable.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtable.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtablerow.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/changehistory/__init__.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/changehistory/changehistorytable.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/changehistory/command.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/conditions/__init__.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/conditions/command.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/ahbexportfileformat.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
+-rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
+-rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
+-rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
+-rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    20365 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/PKG-INFO
```

### Comparing `kohlrahbi-1.0.0/.pre-commit-config.yaml` & `kohlrahbi-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/README.md` & `kohlrahbi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/kohlrahbi-image.png` & `kohlrahbi-1.1.0/kohlrahbi-image.png`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/requirements.txt` & `kohlrahbi-1.1.0/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # via kohlrahbi (pyproject.toml)
 et-xmlfile==1.1.0
     # via openpyxl
 lxml==5.2.2
     # via python-docx
 marshmallow==3.21.2
     # via maus
-maus==0.4.2
+maus==0.5.0
     # via kohlrahbi (pyproject.toml)
 more-itertools==10.2.0
     # via maus
 numpy==1.26.4
     # via pandas
 openpyxl==3.1.2
     # via kohlrahbi (pyproject.toml)
@@ -36,15 +36,15 @@
     # via kohlrahbi (pyproject.toml)
 pydantic==2.7.1
     # via kohlrahbi (pyproject.toml)
 pydantic-core==2.18.2
     # via pydantic
 python-dateutil==2.9.0.post0
     # via pandas
-python-docx==1.1.0
+python-docx==1.1.2
     # via kohlrahbi (pyproject.toml)
 pytz==2024.1
     # via
     #   kohlrahbi (pyproject.toml)
     #   pandas
 six==1.16.0
     # via python-dateutil
```

### Comparing `kohlrahbi-1.0.0/tox.ini` & `kohlrahbi-1.1.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [testenv:type_check]
 # the type_check environment checks the type hints using mypy
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
     -rrequirements.txt
      -r dev_requirements/requirements-type_check.txt
 commands =
-    mypy --show-error-codes src/kohlrahbi
+    mypy --show-error-codes src/kohlrahbi --strict
     mypy --show-error-codes unittests
 # mypy --show-error-codes unittests # does not work yet, sadly; Some tox/packaging problems
 # add single files (ending with .py) or packages here
 
 [testenv:coverage]
 # the coverage environment is called by the Github Action that runs the coverage measurement
 deps =
@@ -60,18 +60,23 @@
     {[testenv:linting]deps}
     {[testenv:coverage]deps}
     -r dev_requirements/requirements-formatting.txt
     pip-tools
     pre-commit
 commands =
     python -m pip install --upgrade pip
-    pip-compile pyproject.toml
     pip install -r requirements.txt
     pre-commit install
 
+[testenv:compile_requirements]
+deps =
+    pip-compile-multi
+commands =
+    pip-compile-multi -d dev_requirements --autoresolve
+
 [testenv:test_packaging]
 skip_install = true
 deps =
     -r dev_requirements/requirements-test_packaging.txt
 commands =
     python -m build
     twine check dist/*
```

### Comparing `kohlrahbi-1.0.0/wip.md` & `kohlrahbi-1.1.0/wip.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/dependabot.yml` & `kohlrahbi-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/coverage.yml` & `kohlrahbi-1.1.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/dependabot_automerge.yml` & `kohlrahbi-1.1.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/formatting.yml` & `kohlrahbi-1.1.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/packaging_test.yml` & `kohlrahbi-1.1.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/python-publish.yml` & `kohlrahbi-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/pythonlint.yml` & `kohlrahbi-1.1.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/.github/workflows/unittests.yml` & `kohlrahbi-1.1.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/dev_requirements/requirements-tests.txt` & `kohlrahbi-1.1.0/dev_requirements/requirements-tests.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     # via -r dev_requirements/requirements-tests.in
 iniconfig==2.0.0
     # via pytest
 packaging==24.0
     # via pytest
 pluggy==1.5.0
     # via pytest
-pytest==8.2.0
+pytest==8.2.1
     # via
     #   -r dev_requirements/requirements-tests.in
     #   pytest-datafiles
 pytest-datafiles==3.0.0
     # via -r dev_requirements/requirements-tests.in
 python-dateutil==2.9.0.post0
     # via freezegun
```

### Comparing `kohlrahbi-1.0.0/dev_requirements/requirements-type_check.txt` & `kohlrahbi-1.1.0/dev_requirements/requirements-type_check.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     # via
     #   pandas
     #   pandas-stubs
 packaging==24.0
     # via pytest
 pandas==2.2.2
     # via -r dev_requirements/requirements-type_check.in
-pandas-stubs==2.2.1.240316
+pandas-stubs==2.2.2.240514
     # via -r dev_requirements/requirements-type_check.in
 pluggy==1.5.0
     # via pytest
-pytest==8.2.0
+pytest==8.2.1
     # via -r dev_requirements/requirements-type_check.in
 python-dateutil==2.9.0.post0
     # via pandas
 pytz==2024.1
     # via pandas
 six==1.16.0
     # via python-dateutil
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/__init__.py` & `kohlrahbi-1.1.0/src/kohlrahbi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from kohlrahbi.changehistory.command import changehistory
 from kohlrahbi.conditions.command import conditions
 from kohlrahbi.version import version
 
 
 @click.group()
 @click.version_option(version=version)
-def cli():
+def cli() -> None:
     """Kohlrahbi CLI tool"""
 
 
 # Add commands to the CLI group
 cli.add_command(ahb)
 cli.add_command(changehistory)
 cli.add_command(conditions)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/docxfilefinder.py` & `kohlrahbi-1.1.0/src/kohlrahbi/docxfilefinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         """
         Returns a list of docx files which contain the given edifact format.
         This method is not pure. It changes the state of the object.
         """
 
         self.paths_to_docx_files = [path for path in self.paths_to_docx_files if str(edifact_format) in path.name]
 
-    def remove_temporary_files(self):
+    def remove_temporary_files(self) -> None:
         """
         This method removes all temporary files from paths_to_docx_files.
         Temporary files lead to the exception `BadZipFile: File is not a zip file`.
         It appears if a docx file is opened by Word.
         """
 
         self.paths_to_docx_files = [path for path in self.paths_to_docx_files if not path.name.startswith("~")]
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/read_functions.py` & `kohlrahbi-1.1.0/src/kohlrahbi/read_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 A collection of functions to get information from AHB tables.
 """
 
-from typing import Generator, Optional, Tuple, Union
+from typing import Generator, Optional, Tuple, TypeGuard, Union
 
-from docx.document import Document  # type:ignore[import]
-from docx.oxml.table import CT_Tbl  # type:ignore[import]
-from docx.oxml.text.paragraph import CT_P  # type:ignore[import]
-from docx.table import Table, _Cell  # type:ignore[import]
-from docx.text.paragraph import Paragraph  # type:ignore[import]
+from docx.document import Document
+from docx.oxml.table import CT_Tbl
+from docx.oxml.text.paragraph import CT_P
+from docx.table import Table, _Cell
+from docx.text.paragraph import Paragraph
 from maus.edifact import EdifactFormat, get_format_of_pruefidentifikator
 
 from kohlrahbi.ahbtable.ahbcondtions import AhbConditions
 from kohlrahbi.ahbtable.ahbpackagetable import AhbPackageTable
 from kohlrahbi.ahbtable.ahbsubtable import AhbSubTable
 from kohlrahbi.ahbtable.ahbtable import AhbTable
 from kohlrahbi.logger import logger
@@ -44,79 +44,78 @@
 def table_header_starts_with_text_edifact_struktur(table: Table) -> bool:
     """
     Check if the table header starts with the text "EDIFACT Struktur".
     """
     return table.cell(row_idx=0, col_idx=0).text.strip() == "EDIFACT Struktur"
 
 
-def is_item_header_of_change_history_section(item: Paragraph | Table | None, style_name: str) -> bool:
+def is_item_header_of_change_history_section(item: Paragraph | Table | None, style_name: str) -> TypeGuard[Paragraph]:
     """
     Checks if the given item is a header of the change history section.
     """
     # checking the style is quite expensive for the CPU because it includes some xpath searches;
     # we should only check the style if the other (easier/cheap) checks returned True so it at least
     return isinstance(item, Paragraph) and "Änderungshistorie" in item.text and "Heading" in style_name
 
 
-def is_item_text_paragraph(item: Paragraph | Table | None, style_name: str) -> bool:
+def is_item_text_paragraph(item: Paragraph | Table | None, style_name: str) -> TypeGuard[Paragraph]:
     """
     Checks if the given item is a text paragraph.
     """
     return isinstance(item, Paragraph) and "Heading" not in style_name
 
 
-def is_item_table_with_pruefidentifikatoren(item: Paragraph | Table | None) -> bool:
+def is_item_table_with_pruefidentifikatoren(item: Paragraph | Table | None) -> TypeGuard[Table]:
     """
     Check if the item is a Table and contains Pruefidentifikatoren.
 
     Args:
     item (Paragraph | Table | None): The item to check.
 
     Returns:
     bool: True if the item is a Table and contains Pruefidentifikatoren, False otherwise.
     """
     return isinstance(item, Table) and table_header_starts_with_text_edifact_struktur(table=item)
 
 
 def is_item_headless_table(
-    item: Paragraph | Table | None,
-    # seed: Seed | None,
-    ahb_table: AhbTable | None,
-) -> bool:
+    value: tuple[Union[Paragraph, Table, None], Union[AhbTable, None]]
+) -> TypeGuard[tuple[Table, AhbTable]]:
     """
     Checks if the given item is a headless table.
 
     Args:
         item (Paragraph | Table | None): The item to be checked.
         seed (Seed): The seed object.
         ahb_table (AhbTable): The AhbTable object.
 
     Returns:
         bool: True if the item is a headless table, False otherwise.
     """
+    item, ahb_table = value
     # return isinstance(item, Table) and seed is not None and ahb_table is not None
     return isinstance(item, Table) and ahb_table is not None
 
 
-def get_ahb_table(document, pruefi: str) -> Optional[AhbTable]:
+def get_ahb_table(document: Document, pruefi: str) -> Optional[AhbTable]:
     """
     Reads a docx file and extracts all information for a given Prüfidentifikator.
     If the Prüfidentifikator is not found or we reach the end of the AHB document
     - indicated by the section 'Änderungshistorie' - it returns None.
 
     Args:
         document: AHB word document which is read by python-docx package
         pruefi (str): The Prüfidentifikator to search for
 
     Returns:
         AhbTable or None: The extracted AHB table or None if not found
     """
 
-    ahb_table = None
-    seed = None
+    ahb_table: AhbTable | None = None
+    seed: Seed | None = None
     searched_pruefi_is_found = False
 
     for item in get_all_paragraphs_and_tables(document):
         style_name = get_style_name(item)
 
         if is_item_text_paragraph(item, style_name):
             continue
@@ -129,86 +128,96 @@
 
         if should_end_search(pruefi, seed, searched_pruefi_is_found):
             log_end_of_ahb_table(pruefi)
             break
 
         searched_pruefi_is_found, ahb_table = process_table(item, pruefi, searched_pruefi_is_found, ahb_table, seed)
 
-    if ahb_table:
+    if ahb_table is not None:
         ahb_table.sanitize()
         return ahb_table
 
     log_pruefi_not_found(pruefi)
     return None
 
 
-def get_style_name(item) -> str:
+def get_style_name(item: Paragraph | Table) -> str:
     """Extracts and normalizes the style name of a document item."""
-    return item.style.name if item.style else "None"
+    return item.style.name if item.style else "None"  # type:ignore[no-any-return]
 
 
-def reached_end_of_document(style_name, item) -> bool:
+def reached_end_of_document(style_name: str, item: Paragraph | Table | None) -> bool:
     """Checks if the current item marks the end of the document."""
     return is_item_header_of_change_history_section(item, style_name)
 
 
-def update_seed(item, seed):
+def update_seed(item: Paragraph | Table | None, seed: Seed | None) -> Seed | None:
     """Updates the seed if the current item is a table with Prüfidentifikatoren."""
     if is_item_table_with_pruefidentifikatoren(item):
         return Seed.from_table(docx_table=item)
     return seed
 
 
-def should_end_search(pruefi, seed, searched_pruefi_is_found):
+def should_end_search(pruefi: str, seed: Seed | None, searched_pruefi_is_found: bool) -> bool:
     """Determines if the search for the AHB table should end."""
-    return seed and pruefi not in seed.pruefidentifikatoren and searched_pruefi_is_found
+    if seed is None:
+        return False
+    return pruefi not in seed.pruefidentifikatoren and searched_pruefi_is_found
 
 
-def process_table(item, pruefi, searched_pruefi_is_found, ahb_table, seed=None):
+def process_table(
+    item: Paragraph | Table | None,
+    pruefi: str,
+    searched_pruefi_is_found: bool,
+    ahb_table: AhbTable | None,
+    seed: Seed | None = None,
+) -> tuple[bool, AhbTable]:
     """Processes tables to find and build the AHB table."""
     if is_item_table_with_pruefidentifikatoren(item):
         seed = Seed.from_table(docx_table=item)
 
         if pruefi in seed.pruefidentifikatoren and not searched_pruefi_is_found:
             log_found_pruefi(pruefi)
             ahb_sub_table = AhbSubTable.from_table_with_header(docx_table=item)
             ahb_table = AhbTable.from_ahb_sub_table(ahb_sub_table=ahb_sub_table)
             searched_pruefi_is_found = True
 
-    # elif is_item_headless_table(item, seed, ahb_table):
-    elif is_item_headless_table(item, ahb_table):
+    elif is_item_headless_table((item, ahb_table)):
+        assert ahb_table is not None
+        assert isinstance(item, Table)
+        assert seed is not None
         ahb_sub_table = AhbSubTable.from_headless_table(docx_table=item, tmd=seed)
         ahb_table.append_ahb_sub_table(ahb_sub_table=ahb_sub_table)
-
-    return searched_pruefi_is_found, ahb_table
+    # actually, the ahb_table is none here (see test_kohlrahbi_cli_with_valid_arguments)
+    return searched_pruefi_is_found, ahb_table  # type:ignore[return-value]
 
 
 # Logging functions
-def log_end_of_document(pruefi):
+def log_end_of_document(pruefi: str) -> None:
     """
     Logs that the end of the document was reached before finding the table for a given Prüfi.
     """
     logger.info("Reached the end of the document before finding the table for Prüfi '%s'.", pruefi)
 
 
-def log_end_of_ahb_table(pruefi):
+def log_end_of_ahb_table(pruefi: str) -> None:
     """
     Logs that the end of the AHB table was reached for a given Prüfi.
     """
     logger.info("Reached the end of the AHB table for Prüfi '%s'.", pruefi)
 
 
-def log_found_pruefi(pruefi):
+def log_found_pruefi(pruefi: str) -> None:
     """
     Logs that the AHB table for a given Prüfi was found.
     """
     logger.info("Found the AHB table for Prüfi '%s'.", pruefi)
 
 
-def log_pruefi_not_found(pruefi):
+def log_pruefi_not_found(pruefi: str) -> None:
     """
     Logs that the Prüfi was not found in the provided document.
     """
     logger.warning("Prüfi '%s' was not found in the provided document.", pruefi)
 
 
 # pylint: disable=too-many-branches
@@ -271,15 +280,17 @@
 def is_last_row_unt_0062(item: Table | Paragraph) -> bool:
     """
     Checks if the given table contains UNT segment in last row.
     """
     return isinstance(item, Table) and "UNT\t0062" == item.cell(row_idx=-1, col_idx=0).text.strip()
 
 
-def is_relevant_pruefi_table(item: Paragraph | Table, seed: Seed, edifact_format) -> bool:
+def is_relevant_pruefi_table(
+    item: Paragraph | Table, seed: Seed | None, edifact_format: EdifactFormat
+) -> TypeGuard[Table]:
     """compares new pruefis to last pruefi and thus checks whether new table"""
     return (
         isinstance(item, Table)
         and seed is not None
         and is_pruefi_of_edifact_format(seed.pruefidentifikatoren, edifact_format)
     )
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-1.1.0/src/kohlrahbi/row_type_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 This module contains all functions to define the type of a row of the tables in an AHB.
 """
 
-from docx.oxml.ns import qn  # type:ignore[import]
-from docx.oxml.parser import OxmlElement  # type:ignore[import]
-from docx.shared import RGBColor  # type:ignore[import]
-from docx.table import _Cell  # type:ignore[import]
+from docx.oxml.ns import qn
+from docx.oxml.parser import OxmlElement
+from docx.shared import RGBColor
+from docx.table import _Cell
 
 from kohlrahbi.enums import RowType
 
 
-def set_table_header_bg_color(cell, hex_color: str):
+def set_table_header_bg_color(cell: _Cell, hex_color: str) -> _Cell:
     """
     set background shading for Header Rows
     """
     table_cell = cell._tc  # pylint:disable=protected-access
     table_cell_properties = table_cell.get_or_add_tcPr()
     cl_shading = OxmlElement("w:shd")
     cl_shading.set(qn("w:fill"), hex_color)  # Hex of Dark Blue Shade {R:0x00, G:0x51, B:0x9E}
@@ -44,15 +44,16 @@
     Args:
         edifact_struktur_cell (_Cell): Indicator cell
 
     Returns:
         bool:
     """
     try:
-        return edifact_struktur_cell.paragraphs[0].runs[0].font.color.rgb == RGBColor(128, 128, 128)  # grey
+        colour_is_grey: bool = edifact_struktur_cell.paragraphs[0].runs[0].font.color.rgb == RGBColor(128, 128, 128)
+        return colour_is_grey
     except IndexError:
         return False
 
 
 def is_row_segmentgruppe(edifact_struktur_cell: _Cell, left_indent_position: int) -> bool:
     """Checks if the current row is a segmentgruppe.
        Example: "SG2"
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/seed.py` & `kohlrahbi-1.1.0/src/kohlrahbi/seed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module provides a class to collect information which of need for all parsing functions
 """
 
-from docx.table import Table  # type:ignore[import]
+from docx.table import Table
 from pydantic import BaseModel
 
 from kohlrahbi.enums import RowType
 from kohlrahbi.table_header import PruefiMetaData, TableHeader, get_tabstop_positions
 
 
 # pylint: disable=too-few-public-methods
@@ -52,15 +52,15 @@
         middle_cell_indicator_paragraph = docx_table.cell(row_idx=4, col_idx=1).paragraphs[0]
         middle_cell_left_indent_position = middle_cell_indicator_paragraph.paragraph_format.left_indent
         tabstop_positions = get_tabstop_positions(middle_cell_indicator_paragraph)
 
         # metadata
         metadata = table_header.pruefi_meta_data
 
-        base_column_names: list = [
+        base_column_names: list[str] = [
             "Segment Gruppe",
             "Segment",
             "Datenelement",
             "Codes und Qualifier",
             "Beschreibung",
         ]
         columns = base_column_names + pruefidentifikatoren + ["Bedingung"]
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/table_header.py` & `kohlrahbi-1.1.0/src/kohlrahbi/table_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 This module contains the TableHeader class.
 """
 
 from enum import StrEnum
 from typing import Dict, List, Mapping, cast
 
-from docx.table import _Cell  # type:ignore[import]
-from docx.text.paragraph import Paragraph  # type:ignore[import]
+from docx.table import _Cell
+from docx.text.paragraph import Paragraph
 from more_itertools import first, last
 from pydantic import BaseModel
 
 
 class HeaderSection(StrEnum):
     """
     Enum for the different sections of the table header
@@ -153,15 +153,15 @@
             for pruefi, meta_data in collector.items()
             if isinstance(meta_data[HeaderSection.KOMMUNIKATION_VON.value], str)
         ]
 
         return cls(pruefi_meta_data=pruefi_meta_data)
 
     @staticmethod
-    def initialize_collector(paragraph) -> Dict[str, Dict[str, str | int]]:
+    def initialize_collector(paragraph: Paragraph) -> Dict[str, Dict[str, str | int]]:
         """Initialize the collector"""
         current_tabstop_positions = get_tabstop_positions(paragraph=paragraph)
         splitted_text = paragraph.text.split("\t")
         splitted_text.remove("Prüfidentifikator")
 
         collector: Dict[str, Dict[str, str | int]] = {
             pruefidentifikator: {
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahb/__init__.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import fnmatch
 import re
 from datetime import date
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import click
-import docx  # type: ignore
+import docx
 import tomlkit
-from docx.document import Document  # type:ignore[import]
-from docx.table import Table  # type:ignore[import]
+from docx.document import Document
+from docx.table import Table
 from maus.edifact import EdifactFormatVersion
 
 from kohlrahbi.ahbtable.ahbtable import AhbTable
 from kohlrahbi.docxfilefinder import DocxFileFinder
 from kohlrahbi.enums.ahbexportfileformat import AhbExportFileFormat
 from kohlrahbi.logger import logger
 from kohlrahbi.read_functions import (
@@ -44,15 +44,15 @@
 
 
 def process_ahb_table(
     ahb_table: AhbTable,
     pruefi: str,
     output_path: Path,
     file_type: str,
-):
+) -> None:
     """
     Process the ahb table.
     """
     unfolded_ahb = UnfoldedAhb.from_ahb_table(ahb_table=ahb_table, pruefi=pruefi)
 
     if "xlsx" in file_type:
         unfolded_ahb.dump_xlsx(output_path)
@@ -94,15 +94,15 @@
 
 # pylint: disable=too-many-arguments
 def process_pruefi(
     pruefi: str,
     path_to_ahb_docx_file: Path,
     output_path: Path,
     file_type: str,
-):
+) -> None:
     """
     Process one pruefi.
     If the input path ends with .docx, we assume that the file containing the pruefi is given.
     Therefore we only access that file.
     """
 
     # TODO try to cache document objects cause it is slow to read them from disk # pylint: disable=fixme
@@ -179,15 +179,15 @@
     seed = Seed.from_table(docx_table=table)
     logger.info("Found a table with the following pruefis: %s", seed.pruefidentifikatoren)
     return seed.pruefidentifikatoren
 
 
 def table_header_contains_text_pruefidentifikator(table: Table) -> bool:
     """Checks if the table header contains the text 'Prüfidentifikator'."""
-    return table.row_cells(0)[-1].paragraphs[-1].text.startswith("Prüfidentifikator")
+    return table.row_cells(0)[-1].paragraphs[-1].text.startswith("Prüfidentifikator")  # type:ignore[no-any-return]
 
 
 def get_pruefi_to_file_mapping(basic_input_path: Path, format_version: EdifactFormatVersion) -> dict[str, str]:
     """Returns the pruefi to file mapping. If the cache file does not exist, it creates it."""
     default_path_to_cache_file = Path(__file__).parents[1] / "cache" / f"{format_version}_pruefi_docx_filename_map.toml"
 
     if default_path_to_cache_file.exists():
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahb/command.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahb/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 import click
 from maus.edifact import EdifactFormatVersion
 
 from kohlrahbi.ahb import scrape_pruefis
 from kohlrahbi.enums.ahbexportfileformat import AhbExportFileFormat
 
 
-def check_python_version():
+def check_python_version() -> None:
     """
     Check if the Python interpreter is greater or equal to 3.11
     """
     if sys.version_info.major != 3 or sys.version_info.minor < 11:
         raise click.Abort(
             f"""Python >=3.11 is required to run this script but you use Python
 {sys.version_info.major}.{sys.version_info.minor}"""
         )
 
 
 # pylint: disable=unused-argument
-def validate_path(ctx, param, value):
+def validate_path(ctx, param, value) -> Path:  # type:ignore[no-untyped-def]
     """
     Ensure the path exists or offer to create it.
     """
     path = Path(value)
     if not path.exists():
         if ctx.params.get("assume_yes") or click.confirm(
             f"The path {value} does not exist. Would you like to create it?"
@@ -93,15 +93,15 @@
     pruefis: list[str],
     edi_energy_mirror_path: Path,
     output_path: Path,
     file_type: AhbExportFileFormat,
     format_version: EdifactFormatVersion | str,
     assume_yes: bool,  # pylint: disable=unused-argument
     # it is used by the callback function of the output-path
-):
+) -> None:
     """
     Scrape AHB documents for pruefidentifikatoren.
     This is a command line interface for the pruefis module.
     """
     check_python_version()
     if isinstance(format_version, str):
         format_version = EdifactFormatVersion(format_version)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbcondtions.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbcondtions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains the ahbconditions class."""
 
 import json
 import re
 from pathlib import Path
 
-from docx.table import Table as DocxTable  # type: ignore[import-untyped]
+from docx.table import Table as DocxTable
 from maus.edifact import EdifactFormat
 from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.logger import logger
 
 
 class AhbConditions(BaseModel):
@@ -49,18 +49,19 @@
         conditions_dict: dict[EdifactFormat, dict[str, str]] = {edifact_format: {}}
 
         conditions_str = "".join(conditions_list)
         conditions_dict = parse_conditions_from_string(conditions_str, edifact_format, conditions_dict)
         logger.info("The package conditions for %s were collected.", edifact_format)
         return conditions_dict
 
-    def include_condition_dict(self, to_add=dict[EdifactFormat, dict[str, str]] | None) -> None:
+    def include_condition_dict(self, to_add: dict[EdifactFormat, dict[str, str]] | None) -> None:
         """ " Include a dict of conditions to the conditions_dict"""
         if to_add is None:
             logger.info("Conditions dict to be added is empty.")
+            return
         for edifact_format, edi_cond_dict in to_add.items():
             for condition_key, condition_text in edi_cond_dict.items():
                 if edifact_format in self.conditions_dict:
                     if (
                         condition_key in self.conditions_dict[edifact_format]
                         and len(condition_text) > len(self.conditions_dict[edifact_format][condition_key])
                         or condition_key not in self.conditions_dict[edifact_format]
@@ -113,12 +114,11 @@
         # make text prettier:
         text = match[1].strip()
         text = re.sub(r"\s+", " ", text)
 
         # check whether condition was already collected:
         existing_text = conditions_dict[edifact_format].get(match[0])
         is_condition_key_collected_yet = existing_text is not None
-        if is_condition_key_collected_yet and existing_text is not None:
-            key_exits_but_shorter_text = len(text) > len(existing_text)
+        key_exits_but_shorter_text = existing_text is not None and len(text) > len(existing_text)
         if not is_condition_key_collected_yet or key_exits_but_shorter_text:
             conditions_dict[edifact_format][match[0]] = text
     return conditions_dict
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbpackagetable.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbpackagetable.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import json
 import re
 from pathlib import Path
 
 import pandas as pd
-from docx.table import Table as DocxTable  # type: ignore[import-untyped]
+from docx.table import Table as DocxTable
 from maus.edifact import EdifactFormat
 from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.ahbtable.ahbcondtions import parse_conditions_from_string
 from kohlrahbi.logger import logger
 
 
@@ -48,15 +48,15 @@
         there_are_conditions = (self.table["Bedingungen"] != "").any()
         if there_are_conditions:
             for conditions_text in self.table["Bedingungen"][self.table["Bedingungen"] != ""]:
                 conditions_dict = parse_conditions_from_string(conditions_text, edifact_format, conditions_dict)
         logger.info("The package conditions for %s were collected.", edifact_format)
         return conditions_dict
 
-    def provide_packages(self, edifact_format: EdifactFormat):
+    def provide_packages(self, edifact_format: EdifactFormat) -> None:
         """collect conditions from package table and store them in conditions dict."""
         package_dict: dict[EdifactFormat, dict[str, str]] = {edifact_format: {}}
 
         there_are_packages = (self.table["Paket"] != "").any()
         if there_are_packages:
             for _, row in self.table.iterrows():
                 package = row["Paket"]
@@ -67,28 +67,28 @@
                     # Extract the matched digits
                 package = match.group(1)
                 if package != "1":
                     package_conditions = row["Paketvoraussetzung(en)"].strip()
                     # check whether package was already collected:
                     existing_text = package_dict[edifact_format].get(package)
                     is_package_key_collected_yet = existing_text is not None
-                    if is_package_key_collected_yet:
-                        key_exits_but_shorter_text = len(package_conditions) > len(
-                            existing_text  # type: ignore[arg-type]
-                        )  # type: ignore[arg-type]
+                    key_exits_but_shorter_text = existing_text is not None and len(package_conditions) > len(
+                        existing_text
+                    )
                     if not is_package_key_collected_yet or key_exits_but_shorter_text:
                         package_dict[edifact_format][package] = package_conditions
 
         logger.info("Packages for %s were collected.", edifact_format)
         self.package_dict = package_dict
 
-    def include_package_dict(self, to_add=dict[EdifactFormat, dict[str, str]] | None) -> None:
+    def include_package_dict(self, to_add: dict[EdifactFormat, dict[str, str]] | None) -> None:
         """Include a dict of conditions to the conditions_dict"""
         if to_add is None:
             logger.info("Packages dict to be added is empty.")
+            return
         for edifact_format, edi_cond_dict in to_add.items():
             for package_key, package_conditions in edi_cond_dict.items():
                 if edifact_format in self.package_dict:
                     if (
                         package_key in self.package_dict[edifact_format]
                         and len(package_conditions) > len(self.package_dict[edifact_format][package_key])
                         or package_key not in self.package_dict[edifact_format]
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbsubtable.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbsubtable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 This module contains the AhbSubTable class.
 """
 
 from typing import Generator
 
 import pandas as pd
-from docx.table import Table as DocxTable  # type:ignore[import]
-from docx.table import _Cell  # type:ignore[import]
+from docx.table import Table as DocxTable
+from docx.table import _Cell, _Row
 from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.ahbtable.ahbtablerow import AhbTableRow
-from kohlrahbi.row_type_checker import RowType, get_row_type
+from kohlrahbi.enums import RowType
+from kohlrahbi.row_type_checker import get_row_type
 from kohlrahbi.seed import Seed
 
 
 class AhbSubTable(BaseModel):
     """
     The AHB table for one Pruefidentifikator is separated into small sub tables.
     This class contains the information from such a sub table.
@@ -118,15 +119,15 @@
             ahb_table_dataframe=ahb_table_dataframe,
             docx_table=docx_table,
         )
 
         return cls(table_meta_data=tmd, table=ahb_table_dataframe)
 
     @staticmethod
-    def iter_visible_cells(row) -> Generator[_Cell, None, None]:
+    def iter_visible_cells(row: _Row) -> Generator[_Cell, None, None]:
         """
         This function makes sure that you will iterate over the cells you see in the word document.
         For more information go to https://github.com/python-openxml/python-docx/issues/970#issuecomment-877386927
         """
         table_row = row._tr  # pylint:disable=protected-access
         for table_column in table_row.tc_lst:
             yield _Cell(table_column, row.table)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtable.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         """
         if self.table is None:
             self.table = ahb_sub_table.table
         else:
             self.table = pd.concat([self.table, ahb_sub_table.table], ignore_index=True)
 
     @staticmethod
-    def line_contains_only_segment_gruppe(raw_line: pd.Series) -> bool:
+    def line_contains_only_segment_gruppe(raw_line: pd.Series) -> bool:  # type:ignore[type-arg]
         """
         Returns true if the given raw line only contains some meaningful data in the "Segment Gruppe" key
         """
         for key, value in raw_line.items():
             if key == "Segment Gruppe":
                 continue
             if value is not None and len(value.strip()) > 0:
@@ -108,14 +108,15 @@
         We need to merge the content into one cell and delete the deprecated cell afterwards.
         """
         index_of_lines_to_drop: list[int] = []
 
         iterable_ahb_table = peekable(self.table.iterrows())
         self.table.reset_index(drop=True, inplace=True)
         for _, row in iterable_ahb_table:
+            # pylint: disable=unpacking-non-sequence # it is a tuple indeed
             index_of_next_row, next_row = iterable_ahb_table.peek(
                 (
                     0,
                     pd.Series(
                         {
                             "Segment Gruppe": "",
                             "Segment": "",
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtablerow.py` & `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtablerow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 This module contains the class AhbTableRow
 """
 
 from typing import Optional
 
 import pandas as pd
-from docx.table import _Cell  # type:ignore[import]
+from docx.table import _Cell
 from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.docxtablecells import BedingungCell, BodyCell, EdifactStrukturCell
-from kohlrahbi.row_type_checker import RowType
+from kohlrahbi.enums import RowType
 from kohlrahbi.seed import Seed
 
 
 # pylint:disable=too-few-public-methods
 class AhbTableRow(BaseModel):
     """
     A AhbTableRow is a single row from an AHB table.
@@ -42,15 +42,17 @@
 
         ahb_row_dataframe = pd.DataFrame(
             # pylint: disable=no-member
             columns=self.seed.column_headers,
             dtype="str",
         )
         # pylint: disable=unsubscriptable-object, no-member
-        empty_row: pd.Series[str] = pd.Series(len(ahb_row_dataframe.columns) * [""], index=self.seed.column_headers)
+        empty_row: pd.Series = pd.Series(  # type:ignore[type-arg]
+            len(ahb_row_dataframe.columns) * [""], index=self.seed.column_headers
+        )
 
         ahb_row_dataframe = pd.concat([ahb_row_dataframe, empty_row.to_frame().T], ignore_index=True)
 
         # EDIFACT STRUKTUR
         esc: EdifactStrukturCell = EdifactStrukturCell(
             # pylint: disable=no-member
             table_cell=self.edifact_struktur_cell,
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/changehistory/__init__.py` & `kohlrahbi-1.1.0/src/kohlrahbi/changehistory/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 - `create_sheet_name`: Creates a sheet name from the filename.
 """
 
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Optional
 
-import docx  # type: ignore
+import docx
 import pandas as pd
-from docx.document import Document  # type:ignore[import]
-from docx.table import Table  # type: ignore
+from docx.document import Document
+from docx.table import Table
 
 from kohlrahbi.changehistory.changehistorytable import ChangeHistoryTable
 from kohlrahbi.docxfilefinder import DocxFileFinder
 from kohlrahbi.logger import logger
 from kohlrahbi.read_functions import get_all_paragraphs_and_tables
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/changehistory/changehistorytable.py` & `kohlrahbi-1.1.0/src/kohlrahbi/changehistory/changehistorytable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module provides the ChangeHistoryTable class
 """
 
 import pandas as pd
-from docx.table import Table  # type:ignore[import]
+from docx.table import Table
 from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.ahbtable.ahbsubtable import AhbSubTable
 
 
 class ChangeHistoryTable(BaseModel):
     """
@@ -50,15 +50,15 @@
         def is_empty(val: str) -> bool:
             """
             Checks if the given value is considered empty for our case.
             """
             return pd.isna(val) or val == ""
 
         # Define a function to check if a value is considered empty for our case
-        def is_the_first_column_empty(row: pd.Series) -> bool:
+        def is_the_first_column_empty(row: pd.Series) -> bool:  # type:ignore[type-arg]
             """
             Checks if the first column of the given row is empty.
             This is our indicator if the current row is a continuation of the upper row.
             """
             return is_empty(row.iloc[0])
 
         # Iterate over the DataFrame rows in reverse (to avoid skipping rows after removing them)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/changehistory/command.py` & `kohlrahbi-1.1.0/src/kohlrahbi/changehistory/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 )
 def changehistory(
     edi_energy_mirror_path: Path,
     output_path: Path,
     format_version: EdifactFormatVersion | str,
     assume_yes: bool,  # pylint: disable=unused-argument
     # it is used by the callback function of the output-path
-):
+) -> None:
     """
     Scrape change histories from the input path and save them to the output path.
 
     Args:
         edi_energy_mirror_path (Path): The path to the input file or directory containing change histories.
         output_path (Path): The path to save the scraped change histories.
         format_version (EdifactFormatVersion | str): The version of the EDIFACT format to use for scraping.
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/conditions/__init__.py` & `kohlrahbi-1.1.0/src/kohlrahbi/conditions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains the function to write the collected conditions to a json file.
 """
 
 from pathlib import Path
 
-import docx  # type: ignore[import-untyped]
+import docx
 from maus.edifact import EdifactFormat, EdifactFormatVersion, get_format_of_pruefidentifikator
 
 from kohlrahbi.ahb import get_pruefi_to_file_mapping
 from kohlrahbi.ahbtable.ahbcondtions import AhbConditions
 from kohlrahbi.ahbtable.ahbpackagetable import AhbPackageTable
 from kohlrahbi.logger import logger
 from kohlrahbi.read_functions import get_all_conditions_from_doc
@@ -41,16 +41,16 @@
 
     collected_conditions: AhbConditions = AhbConditions()
     collected_packages: AhbPackageTable = AhbPackageTable()
     all_format_files = find_all_files_from_all_pruefis(pruefi_to_file_mapping)
     for edifact_format, files in all_format_files.items():
         for file in files:
             # pylint: disable=too-many-function-args
-            # type: ignore[call-arg, arg-type]
-            doc = docx.Document(basic_input_path / path_to_file / Path(file))
+            path: Path = basic_input_path / path_to_file / Path(file)
+            doc = docx.Document(str(path.absolute()))
             logger.info("Start scraping conditions for %s in %s", edifact_format, file)
             if not doc:
                 logger.error("Could not open file %s as docx", Path(file))
             packages, cond_table = get_all_conditions_from_doc(doc, edifact_format)
             if packages and packages.table is not None:
                 collected_conditions.include_condition_dict(packages.provide_conditions(edifact_format))
                 collected_packages.include_package_dict(packages.package_dict)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/conditions/command.py` & `kohlrahbi-1.1.0/src/kohlrahbi/conditions/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 
 import click
 from maus.edifact import EdifactFormatVersion
 
 from kohlrahbi.conditions import scrape_conditions
 
 
-def check_python_version():
+def check_python_version() -> None:
     """
     Check if the Python interpreter is greater or equal to 3.11
     """
     if sys.version_info.major != 3 or sys.version_info.minor < 11:
         raise click.Abort(
             f"""Python >=3.11 is required to run this script but you use Python
 {sys.version_info.major}.{sys.version_info.minor}"""
         )
 
 
 # pylint: disable=unused-argument
-def validate_path(ctx, param, value):
+def validate_path(ctx, param, value) -> Path:  # type:ignore[no-untyped-def]
     """
     Ensure the path exists or offer to create it.
     """
     path = Path(value)
     if not path.exists():
         if ctx.params.get("assume_yes") or click.confirm(
             f"The path {value} does not exist. Would you like to create it?"
@@ -87,15 +87,15 @@
     "-y",
     is_flag=True,
     default=False,
     help="Confirm all prompts automatically.",
 )
 def conditions(
     edi_energy_mirror_path: Path, output_path: Path, format_version: EdifactFormatVersion | str, assume_yes: bool
-):
+) -> None:
     """
     Scrape AHB documents for conditions.
     """
     check_python_version()
     if isinstance(format_version, str):
         format_version = EdifactFormatVersion(format_version)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains the class BedingungCell
 """
 
 import re
 
 import pandas as pd
-from docx.table import _Cell  # type:ignore[import]
+from docx.table import _Cell
 from pydantic import BaseModel, ConfigDict
 
 
 class BedingungCell(BaseModel):
     """
     BedingungCell contains all information and a method
     to extract the Bedingungen of an AHB Bedingung cell.
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module contains the class BodyCell
 """
 
 import pandas as pd
-from docx.table import _Cell  # type:ignore[import]
+from docx.table import _Cell
+from docx.text.paragraph import Paragraph
 from maus.reader.flat_ahb_reader import FlatAhbCsvReader
 from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.table_header import get_tabstop_positions
 
 INDEX_OF_CODES_AND_QUALIFIER_COLUMN = 3
 
@@ -99,13 +100,13 @@
                 raise NotImplementedError(f"Could not parse paragraph in middle cell with {paragraph.text}")
 
             # recognize that the first loop is over
             is_first_iteration = False
 
         return ahb_row_dataframe
 
-    def has_paragraph_tabstops(self, paragraph) -> bool:
+    def has_paragraph_tabstops(self, paragraph: Paragraph) -> bool:
         """
         Checks if the given paragraph contains tabstops
         """
         tab_stops = list(paragraph.paragraph_format.tab_stops)
-        return len(tab_stops) > 0
+        return any(tab_stops)
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains the class EdifactStrukturCell
 """
 
 import re
 
 import pandas as pd
-from docx.table import _Cell  # type:ignore[import]
+from docx.table import _Cell
 from pydantic import BaseModel, ConfigDict
 
 _segment_group_pattern = re.compile(r"^SG\d+$")
 _segment_pattern = re.compile(r"^[A-Z]{3}$")
 
 
 # pylint: disable=too-few-public-methods
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-1.1.0/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml` & `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml` & `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml` & `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml` & `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,13 +77,14 @@
 
     # pylint: disable=fixme
     # TODO: add class variable which increments the index with each created instance
     index: int
     segment_name: str  # Ansprechpartner
     segment_gruppe: str | None  # SG3
     segment: str | None  # CTA
+    segment_id: str | None = None  # 00009
     datenelement: str | None  # 3055
     code: str | None  # IC
     qualifier: str | None  # Name vom Ansprechpartner
     beschreibung: str | None  # Informationskontakt
     bedingung_ausdruck: str | None  # Muss / X / X [1P0..1]
     bedingung: str | None  # [492] Wenn MP-ID in NAD+MR (Nachrichtenempfänger) aus Sparte Strom
```

### Comparing `kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains the UnfoldedAhbTable class.
 """
 
 import copy
 import json
 import re
+from functools import lru_cache
 from pathlib import Path
 from uuid import uuid4
 
 import pandas as pd
 from maus.edifact import get_format_of_pruefidentifikator
 from maus.models.anwendungshandbuch import (
     AhbLine,
@@ -22,27 +23,46 @@
 
 from kohlrahbi.ahbtable.ahbtable import AhbTable, _column_letter_width_mapping
 from kohlrahbi.logger import logger
 from kohlrahbi.unfoldedahb.unfoldedahbline import UnfoldedAhbLine
 from kohlrahbi.unfoldedahb.unfoldedahbtablemetadata import UnfoldedAhbTableMetaData
 
 _segment_group_pattern = re.compile(r"^SG\d+$")
+_segment_id_pattern = re.compile(r"^\d{5}$")
 
 
 def _lines_are_equal_when_ignoring_guid(line1: AhbLine, line2: AhbLine) -> bool:
     """
     returns true iff the line1 and line2 are equal except for their guid
     """
     line1_copy = copy.deepcopy(line1)
     line2_copy = copy.deepcopy(line2)
     line1_copy.guid = None
     line2_copy.guid = None
     return line1_copy == line2_copy
 
 
+@lru_cache
+def _split_data_element_and_segment_id(value: str | None) -> tuple[str | None, str | None]:
+    """
+    returns the data element id and segment id
+    """
+    if value is None:
+        return None, None
+    datenelement_id: str | None
+    segment_id: str | None
+    if _segment_id_pattern.match(value):
+        datenelement_id = None
+        segment_id = value
+    else:
+        datenelement_id = value
+        segment_id = None
+    return datenelement_id, segment_id
+
+
 def _keep_guids_of_unchanged_lines_stable(
     updated_ahb: FlatAnwendungshandbuch, existing_ahb: FlatAnwendungshandbuch
 ) -> None:
     """
     Modifies the instance of updated_ahb such that the guids of all lines that are unchanged are the same as in the
     existing_ahb. Only applies if metadata of both AHBs match.
     """
@@ -67,15 +87,15 @@
     The unfolded classes add new columns/attribues to avoid the duplication of information in one column.
     """
 
     meta_data: UnfoldedAhbTableMetaData
     unfolded_ahb_lines: list[UnfoldedAhbLine]
 
     @classmethod
-    def from_ahb_table(cls, ahb_table: AhbTable, pruefi: str):
+    def from_ahb_table(cls, ahb_table: AhbTable, pruefi: str) -> "UnfoldedAhb":
         """
         This function creates an UnfoldedAhb from an AhbTable.
         """
         unfolded_ahb_lines: list[UnfoldedAhbLine] = []
         current_section_name: str = ""
 
         # we need to peek one iteration in front of us
@@ -85,15 +105,15 @@
             row = series[1]
 
             current_section_name = UnfoldedAhb._get_section_name(
                 segment_gruppe_or_section_name=row["Segment Gruppe"], last_section_name=current_section_name
             )
 
             if UnfoldedAhb._is_section_name(ahb_row=row):
-                _, next_row = iterable_ahb_table.peek()
+                _, next_row = iterable_ahb_table.peek()  # pylint: disable=unpacking-non-sequence # it is a tuple indeed
                 ahb_expression = next_row[pruefi]
 
                 if _segment_group_pattern.match(next_row["Segment Gruppe"]):
                     segment_group_key = next_row["Segment Gruppe"]
                 else:
                     segment_group_key = None
 
@@ -155,15 +175,16 @@
                 )
                 unfolded_ahb_lines.append(
                     UnfoldedAhbLine(
                         index=index,
                         segment_name=current_section_name,
                         segment_gruppe=row["Segment Gruppe"] or None,
                         segment=row["Segment"] or None,
-                        datenelement=row["Datenelement"] or None,
+                        datenelement=_split_data_element_and_segment_id(row["Datenelement"])[0],
+                        segment_id=_split_data_element_and_segment_id(row["Datenelement"])[1],
                         code=value_pool_entry,
                         qualifier="",
                         beschreibung=description,
                         bedingung_ausdruck=row[pruefi] or None,
                         bedingung=row["Bedingung"],
                     )
                 )
@@ -232,32 +253,32 @@
         the 'last_section_name' will be returned.
         """
         if not (segment_gruppe_or_section_name.startswith("SG") or segment_gruppe_or_section_name == ""):
             return segment_gruppe_or_section_name
         return last_section_name
 
     @staticmethod
-    def _is_section_name(ahb_row: pd.Series) -> bool:
+    def _is_section_name(ahb_row: pd.Series) -> bool:  # type:ignore[type-arg]
         """
         Checks if the current AHB row is a section name.
         It uses the same logic as the function 'line_contains_only_segment_gruppe'
         So to avoid duplicate code, this function just calls the other function.
         """
         return AhbTable.line_contains_only_segment_gruppe(ahb_row)
 
     @staticmethod
-    def _is_segment_group(ahb_row: pd.Series) -> bool:
+    def _is_segment_group(ahb_row: pd.Series) -> bool:  # type:ignore[type-arg]
         """Checks if the current AHB row is a segment group."""
 
         if _segment_group_pattern.match(ahb_row["Segment Gruppe"]) and not ahb_row["Segment"]:
             return True
         return False
 
     @staticmethod
-    def _is_segment_opening_line(ahb_row: pd.Series) -> bool:
+    def _is_segment_opening_line(ahb_row: pd.Series) -> bool:  # type:ignore[type-arg]
         """Checks if the current AHB row is a segment opening line.
         Example:
 
         SG3    CTA                                         Muss    Muss    Muss
         SG3    CTA    3139    IC    Informationskontakt    X       X       X
 
         The first line in the example is a segment opening line
@@ -269,38 +290,40 @@
             and ahb_row["Segment"]
             and not ahb_row["Datenelement"]
         ):
             return True
         return False
 
     @staticmethod
-    def _is_just_segment(ahb_row: pd.Series) -> bool:
+    def _is_just_segment(ahb_row: pd.Series) -> bool:  # type:ignore[type-arg]
         """
         Checks if the given AHB row is a segment
         """
 
         if (
             _segment_group_pattern.match(ahb_row["Segment Gruppe"])
             and ahb_row["Segment"]
             and not ahb_row["Datenelement"]
         ):
             return True
+        if ahb_row["Datenelement"] is not None and _segment_id_pattern.match(ahb_row["Datenelement"]):
+            return True
         return False
 
     @staticmethod
-    def _is_dataelement(ahb_row: pd.Series) -> bool:
+    def _is_dataelement(ahb_row: pd.Series) -> bool:  # type:ignore[type-arg]
         """
         Checks if the given AHB row is a dataelement
         """
         if ahb_row["Datenelement"]:
             return True
         return False
 
     @staticmethod
-    def _is_just_value_pool_entry(ahb_row: pd.Series) -> bool:
+    def _is_just_value_pool_entry(ahb_row: pd.Series) -> bool:  # type:ignore[type-arg]
         """
         Checks if the given AHB row contains only a value pool entry (w/o Segment (group) and data element)
         """
         return (
             (not ahb_row["Segment Gruppe"])
             and (not ahb_row["Segment"])
             and (not ahb_row["Datenelement"])
@@ -321,14 +344,15 @@
         for unfolded_ahb_line in self.unfolded_ahb_lines:
             lines.append(
                 AhbLine(
                     guid=uuid4(),
                     segment_group_key=unfolded_ahb_line.segment_gruppe,
                     segment_code=unfolded_ahb_line.segment,
                     data_element=unfolded_ahb_line.datenelement,
+                    segment_id=unfolded_ahb_line.segment_id,
                     value_pool_entry=unfolded_ahb_line.code,
                     name=unfolded_ahb_line.beschreibung or unfolded_ahb_line.qualifier,
                     ahb_expression=unfolded_ahb_line.bedingung_ausdruck,
                     section_name=unfolded_ahb_line.segment_name,
                     index=unfolded_ahb_line.index,
                 )
             )
```

### Comparing `kohlrahbi-1.0.0/.gitignore` & `kohlrahbi-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/LICENSE` & `kohlrahbi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.0.0/pyproject.toml` & `kohlrahbi-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [
   "click>=8.0.0",
   "colorlog>=6.7.0",
-  "maus>=0.3.43",
+  "maus>=0.5.0",
   "openpyxl>=3.1.1",
   "pandas>=1.5.3",
   "python-docx>=1.0.0",
   "pytz>=2022.7.1",
   "pydantic>=2.6.0",
   "tomlkit>=0.11.6",
   "xlsxwriter>=3.0.8",
```

### Comparing `kohlrahbi-1.0.0/PKG-INFO` & `kohlrahbi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kohlrahbi
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Requires-Dist: click>=8.0.0
 Requires-Dist: colorlog>=6.7.0
-Requires-Dist: maus>=0.3.43
+Requires-Dist: maus>=0.5.0
 Requires-Dist: openpyxl>=3.1.1
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: python-docx>=1.0.0
 Requires-Dist: pytz>=2022.7.1
 Requires-Dist: tomlkit>=0.11.6
 Requires-Dist: xlsxwriter>=3.0.8
```

