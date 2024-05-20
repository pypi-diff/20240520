# Comparing `tmp/kohlrahbi-1.1.0.tar.gz` & `tmp/kohlrahbi-1.1.1.tar.gz`

## Comparing `kohlrahbi-1.1.0.tar` & `kohlrahbi-1.1.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.gitattributes
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/README.md
--rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/kohlrahbi-image.png
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/requirements.txt
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/tox.ini
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/wip.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxfilefinder.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/table_header.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/version.py
--rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahb/command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/__init__.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbcondtions.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbpackagetable.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbsubtable.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtable.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtablerow.py
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/changehistory/__init__.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/changehistory/changehistorytable.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/changehistory/command.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/conditions/__init__.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/conditions/command.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/ahbexportfileformat.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
--rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
--rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
--rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
--rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    20365 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/LICENSE
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 kohlrahbi-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.gitattributes
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/README.md
+-rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/kohlrahbi-image.png
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/requirements.txt
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/tox.ini
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/wip.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxfilefinder.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/table_header.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/version.py
+-rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahb/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/__init__.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbcondtions.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbpackagetable.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbsubtable.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtable.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtablerow.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/changehistory/__init__.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/changehistory/changehistorytable.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/changehistory/command.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/conditions/__init__.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/conditions/command.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/ahbexportfileformat.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
+-rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
+-rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
+-rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
+-rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    20398 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 kohlrahbi-1.1.1/PKG-INFO
```

### Comparing `kohlrahbi-1.1.0/.pre-commit-config.yaml` & `kohlrahbi-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/README.md` & `kohlrahbi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/kohlrahbi-image.png` & `kohlrahbi-1.1.1/kohlrahbi-image.png`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/requirements.txt` & `kohlrahbi-1.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/tox.ini` & `kohlrahbi-1.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/wip.md` & `kohlrahbi-1.1.1/wip.md`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/dependabot.yml` & `kohlrahbi-1.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/coverage.yml` & `kohlrahbi-1.1.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/dependabot_automerge.yml` & `kohlrahbi-1.1.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/formatting.yml` & `kohlrahbi-1.1.1/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/packaging_test.yml` & `kohlrahbi-1.1.1/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/python-publish.yml` & `kohlrahbi-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/pythonlint.yml` & `kohlrahbi-1.1.1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/.github/workflows/unittests.yml` & `kohlrahbi-1.1.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/dev_requirements/requirements-test_packaging.txt` & `kohlrahbi-1.1.1/dev_requirements/requirements-test_packaging.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/dev_requirements/requirements-tests.txt` & `kohlrahbi-1.1.1/dev_requirements/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/dev_requirements/requirements-type_check.txt` & `kohlrahbi-1.1.1/dev_requirements/requirements-type_check.txt`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/__init__.py` & `kohlrahbi-1.1.1/src/kohlrahbi/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/docxfilefinder.py` & `kohlrahbi-1.1.1/src/kohlrahbi/docxfilefinder.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/read_functions.py` & `kohlrahbi-1.1.1/src/kohlrahbi/read_functions.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-1.1.1/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/seed.py` & `kohlrahbi-1.1.1/src/kohlrahbi/seed.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/table_header.py` & `kohlrahbi-1.1.1/src/kohlrahbi/table_header.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahb/__init__.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahb/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahb/command.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahb/command.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbcondtions.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbcondtions.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbpackagetable.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbpackagetable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbsubtable.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtable.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/ahbtable/ahbtablerow.py` & `kohlrahbi-1.1.1/src/kohlrahbi/ahbtable/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/changehistory/__init__.py` & `kohlrahbi-1.1.1/src/kohlrahbi/changehistory/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/changehistory/changehistorytable.py` & `kohlrahbi-1.1.1/src/kohlrahbi/changehistory/changehistorytable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/changehistory/command.py` & `kohlrahbi-1.1.1/src/kohlrahbi/changehistory/command.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/conditions/__init__.py` & `kohlrahbi-1.1.1/src/kohlrahbi/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/conditions/command.py` & `kohlrahbi-1.1.1/src/kohlrahbi/conditions/command.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-1.1.1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-1.1.1/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml` & `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml` & `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml` & `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml` & `kohlrahbi-1.1.1/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-1.1.1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 @lru_cache
 def _split_data_element_and_segment_id(value: str | None) -> tuple[str | None, str | None]:
     """
     returns the data element id and segment id
     """
-    if value is None:
+    if not value:  # covers both None and empty string
         return None, None
     datenelement_id: str | None
     segment_id: str | None
     if _segment_id_pattern.match(value):
         datenelement_id = None
         segment_id = value
     else:
```

### Comparing `kohlrahbi-1.1.0/.gitignore` & `kohlrahbi-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/LICENSE` & `kohlrahbi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/pyproject.toml` & `kohlrahbi-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-1.1.0/PKG-INFO` & `kohlrahbi-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kohlrahbi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
```

