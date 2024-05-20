# Comparing `tmp/hapi_schema-0.8.0.tar.gz` & `tmp/hapi_schema-0.8.2.tar.gz`

## Comparing `hapi_schema-0.8.0.tar` & `hapi_schema-0.8.2.tar`

### file list

```diff
@@ -1,81 +1,97 @@
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/changelog.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/contributing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/initialize_test_db.sh
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/coveragerc
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/ruff.toml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/docker/docker-compose.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_conflict_event.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_funding.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_poverty_rate.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_refugees.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/constraints.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/enums.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/view_as_table_code_generator.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_admin1.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_admin2.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_conflict_event.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_dataset.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_food_security.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_funding.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_location.py
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_national_risk.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_operational_presence.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_org.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_org_type.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_patch.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_population.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_poverty_rate.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_refugees.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_resource.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_conflict_event.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_funding.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_poverty_rate.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_refugees.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_currency.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_food_price.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_views_as_tables.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_wfp_commodity.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_wfp_market.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/hapi_views_code_generator.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_definitions.toml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/conftest.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_admin1.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_admin2.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_currency.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_dataset.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_food_price.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_food_security.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_funding.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_location.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_org_type.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_patch.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_population.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_refugees.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_sector.py
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_views_as_tables.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_wfp_commodity.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_wfp_market.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_currency.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_food_price.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_wfp_commodity.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_wfp_market.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/PKG-INFO
```

### Comparing `hapi_schema-0.8.0/changelog.md` & `hapi_schema-0.8.2/changelog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.8.2
+
+Miscellaneous fixes for pipelines
+
+### Changed
+- added from\_cods column to location, admin1, and admin2
+
+
+## 0.8.1
+
+Implemented the Food Prices subcategory.
+
+### Added
+- New tables and views: food\_price, wfp\_commodity, wfp\_market, currency
+- New enums: PriceFlag, PriceType, CommodityCategory
+- New constraints: non\_negative\_constraint, latlon\_constraint
+
+
 ## 0.8.0
 
 ### Changed
 
 - Many small changes to align with V1 of the schema
 - `resource` and `dataset` primary keys are now the UUID
 - Use postgres instead of sqlite for testing
 - Update GitHub Actions workflow to use postgres
 - Created tables which reflect the views
 - Programmatically obtain views
 
 ### Added
-- New tables: humanitarian\_needs, funding, refugees, conflict\_events, poverty_rate
-- New enums: Gender, DisabledMarker, EventType, PopulationGroup, PopulationStatus, IPCPhase, PovertyClassification
-  IPCType, and RiskClass
+- New tables: humanitarian\_needs, funding, refugees, conflict\_event, poverty\_rate
+- New enums: Gender, DisabledMarker, EventType, PopulationGroup, PopulationStatus, IPCPhase, PovertyClassification, IPCType, and RiskClass
 - Generalized constraints
 
 ### Removed
 
-- ipc_phase, ipc_type, age_range, and gender tables
+- ipc\_phase, ipc\_type, age\_range, and gender tables
 
 
 ## [0.7.3]
 
 ### Fixed
 
 - Incorrect constraint quotes in IPC type
```

### Comparing `hapi_schema-0.8.0/contributing.md` & `hapi_schema-0.8.2/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/requirements.txt` & `hapi_schema-0.8.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/.config/pre-commit-config.yaml` & `hapi_schema-0.8.2/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/.github/workflows/publish.yaml` & `hapi_schema-0.8.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.8.2/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.2/src/hapi_schema/db_admin1.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         nullable=False,
     )
     code: Mapped[str] = mapped_column(String(128), nullable=False, index=True)
     name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
     is_unspecified: Mapped[bool] = mapped_column(
         Boolean, server_default=text("FALSE"), nullable=False
     )
+    from_cods: Mapped[bool] = mapped_column(
+        Boolean, nullable=False, server_default=text("TRUE")
+    )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
 
@@ -60,24 +63,7 @@
         DBAdmin1.__table__.join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
     ),
 )
-
-
-class DBAdmin1VAT(Base):
-    __tablename__ = "admin1_vat"
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    location_ref: Mapped[int] = mapped_column(Integer)
-    code: Mapped[str] = mapped_column(String(128))
-    name: Mapped[str] = mapped_column(String(512))
-    is_unspecified: Mapped[bool] = mapped_column(Boolean)
-    reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, index=True
-    )
-    reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, index=True
-    )
-    location_code: Mapped[str] = mapped_column(String(128), index=True)
-    location_name: Mapped[str] = mapped_column(String(512), index=True)
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.2/src/hapi_schema/db_admin2.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         nullable=False,
     )
     code: Mapped[str] = mapped_column(String(128), nullable=False, index=True)
     name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
     is_unspecified: Mapped[bool] = mapped_column(
         Boolean, server_default=text("FALSE"), nullable=False
     )
+    from_cods: Mapped[bool] = mapped_column(
+        Boolean, nullable=False, server_default=text("TRUE")
+    )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
 
@@ -68,27 +71,7 @@
         ).join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         ),
     ),
 )
-
-
-class DBAdmin2VAT(Base):
-    __tablename__ = "admin2_vat"
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    admin1_ref: Mapped[int] = mapped_column(Integer)
-    code: Mapped[str] = mapped_column(String(128), index=True)
-    name: Mapped[str] = mapped_column(String(512), index=True)
-    is_unspecified: Mapped[bool] = mapped_column(Boolean)
-    reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, index=True
-    )
-    reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, index=True
-    )
-    admin1_code: Mapped[str] = mapped_column(String(128))
-    admin1_name: Mapped[str] = mapped_column(String(512))
-    admin1_is_unspecified: Mapped[bool] = mapped_column(Boolean)
-    location_code: Mapped[str] = mapped_column(String(128), index=True)
-    location_name: Mapped[str] = mapped_column(String(512), index=True)
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_conflict_event.py` & `hapi_schema-0.8.2/src/hapi_schema/db_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.2/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.2/src/hapi_schema/db_humanitarian_needs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,127 @@
-"""Food security table and view."""
+"""HumanitarianNeeds table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
-    Boolean,
     DateTime,
     Enum,
-    Float,
     ForeignKey,
     Integer,
     String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.db_location import DBLocation
-from hapi_schema.db_resource import DBResource
+from hapi_schema.db_sector import DBSector
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
+    max_age_constraint,
+    min_age_constraint,
     population_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import IPCPhase, IPCType
+from hapi_schema.utils.enums import (
+    DisabledMarker,
+    Gender,
+    PopulationGroup,
+    PopulationStatus,
+)
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBFoodSecurity(Base):
-    __tablename__ = "food_security"
+class DBHumanitarianNeeds(Base):
+    __tablename__ = "humanitarian_needs"
     __table_args__ = (
+        min_age_constraint(),
+        max_age_constraint(),
+        population_constraint(),
         reference_period_constraint(),
-        population_constraint(population_var_name="population_in_phase"),
     )
 
     resource_hdx_id: Mapped[str] = mapped_column(
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
-        ForeignKey("admin2.id", onupdate="CASCADE"), primary_key=True
+        ForeignKey("admin2.id", onupdate="CASCADE"),
+        primary_key=True,
     )
-    ipc_phase: Mapped[IPCPhase] = mapped_column(
-        Enum(IPCPhase), primary_key=True
+    gender: Mapped[Gender] = mapped_column(Enum(Gender), primary_key=True)
+    age_range: Mapped[str] = mapped_column(String(32), primary_key=True)
+    min_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
+    max_age: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
+    sector_code: Mapped[str] = mapped_column(
+        ForeignKey("sector.code", onupdate="CASCADE"),
+        primary_key=True,
     )
-    ipc_type: Mapped[IPCType] = mapped_column(Enum(IPCType), primary_key=True)
-    population_in_phase: Mapped[int] = mapped_column(
-        Integer, nullable=False, index=True
+    population_group: Mapped[PopulationGroup] = mapped_column(
+        Enum(PopulationGroup),
+        primary_key=True,
     )
-    population_fraction_in_phase: Mapped[float] = mapped_column(
-        Float, nullable=False, index=True
+
+    population_status: Mapped[PopulationStatus] = mapped_column(
+        Enum(PopulationStatus),
+        primary_key=True,
     )
+
+    disabled_marker: Mapped[DisabledMarker] = mapped_column(
+        Enum(DisabledMarker), primary_key=True
+    )
+    population: Mapped[int] = mapped_column(Integer, nullable=False)
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, primary_key=True
+        DateTime,
+        primary_key=True,
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
 
-    resource = relationship(DBResource)
-    admin2 = relationship(DBAdmin2)
+    resource = relationship("DBResource")
+    admin2 = relationship("DBAdmin2")
+    sector = relationship("DBSector")
 
 
-view_params_food_security = ViewParams(
-    name="food_security_view",
+view_params_humanitarian_needs = ViewParams(
+    name="humanitarian_needs_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBFoodSecurity.__table__.columns,
+        *DBHumanitarianNeeds.__table__.columns,
+        DBSector.name.label("sector_name"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
+        DBAdmin1.location_ref.label("location_ref"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
-        DBAdmin1.location_ref.label("location_ref"),
         DBAdmin2.code.label("admin2_code"),
         DBAdmin2.name.label("admin2_name"),
         DBAdmin2.is_unspecified.label("admin2_is_unspecified"),
         DBAdmin2.admin1_ref.label("admin1_ref"),
     ).select_from(
         # Join pop to admin2 to admin1 to loc
-        DBFoodSecurity.__table__.join(
+        DBHumanitarianNeeds.__table__.join(
             DBAdmin2.__table__,
-            DBFoodSecurity.admin2_ref == DBAdmin2.id,
+            DBHumanitarianNeeds.admin2_ref == DBAdmin2.id,
             isouter=True,
         )
         .join(
             DBAdmin1.__table__,
             DBAdmin2.admin1_ref == DBAdmin1.id,
             isouter=True,
         )
         .join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
+        # Join needs to sector
+        .join(
+            DBSector.__table__,
+            DBHumanitarianNeeds.sector_code == DBSector.code,
+            isouter=True,
+        )
     ),
 )
-
-
-class DBFoodSecurityVAT(Base):
-    __tablename__ = "food_security_vat"
-    resource_hdx_id: Mapped[str] = mapped_column(String(36))
-    admin2_ref: Mapped[int] = mapped_column(
-        Integer, index=True, primary_key=True
-    )
-    ipc_phase: Mapped[IPCPhase] = mapped_column(
-        Enum(IPCPhase), index=True, primary_key=True
-    )
-    ipc_type: Mapped[IPCType] = mapped_column(
-        Enum(IPCType), index=True, primary_key=True
-    )
-    population_in_phase: Mapped[int] = mapped_column(Integer, primary_key=True)
-    population_fraction_in_phase: Mapped[float] = mapped_column(
-        Float, index=True, primary_key=True
-    )
-    reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, index=True
-    )
-    reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, index=True
-    )
-    location_code: Mapped[str] = mapped_column(String(128))
-    location_name: Mapped[str] = mapped_column(String(512), index=True)
-    admin1_code: Mapped[str] = mapped_column(String(128))
-    admin1_name: Mapped[str] = mapped_column(String(512))
-    admin1_is_unspecified: Mapped[bool] = mapped_column(Boolean)
-    location_ref: Mapped[int] = mapped_column(Integer)
-    admin2_code: Mapped[str] = mapped_column(String(128), index=True)
-    admin2_name: Mapped[str] = mapped_column(String(512), index=True)
-    admin2_is_unspecified: Mapped[bool] = mapped_column(Boolean)
-    admin1_ref: Mapped[int] = mapped_column(Integer)
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_funding.py` & `hapi_schema-0.8.2/src/hapi_schema/db_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_location.py` & `hapi_schema-0.8.2/src/hapi_schema/db_location.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Location table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
+    Boolean,
     DateTime,
     Integer,
     String,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column
@@ -25,14 +26,17 @@
         reference_period_constraint(),
         code_and_reference_period_unique_constraint(admin_level="location"),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     code: Mapped[str] = mapped_column(String(128), nullable=False, index=True)
     name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
+    from_cods: Mapped[bool] = mapped_column(
+        Boolean, nullable=False, server_default=text("TRUE")
+    )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.8.2/src/hapi_schema/db_national_risk.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from sqlalchemy import (
     CheckConstraint,
     DateTime,
     Enum,
     Float,
     ForeignKey,
     Integer,
-    String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_location import DBLocation
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
@@ -89,29 +88,7 @@
         DBNationalRisk.__table__.join(
             DBLocation.__table__,
             DBNationalRisk.location_ref == DBLocation.id,
             isouter=True,
         )
     ),
 )
-
-
-class DBNationalRiskVAT(Base):
-    __tablename__ = "national_risk_vat"
-    resource_hdx_id: Mapped[str] = mapped_column(String(36))
-    location_ref: Mapped[int] = mapped_column(Integer, primary_key=True)
-    risk_class: Mapped[str] = mapped_column(String(9))
-    global_rank: Mapped[int] = mapped_column(Integer)
-    overall_risk: Mapped[float] = mapped_column(Float)
-    hazard_exposure_risk: Mapped[float] = mapped_column(Float)
-    vulnerability_risk: Mapped[float] = mapped_column(Float)
-    coping_capacity_risk: Mapped[float] = mapped_column(Float)
-    meta_missing_indicators_pct: Mapped[float] = mapped_column(Float)
-    meta_avg_recentness_years: Mapped[float] = mapped_column(Float)
-    reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, primary_key=True
-    )
-    reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, primary_key=True
-    )
-    location_code: Mapped[str] = mapped_column(String(128))
-    location_name: Mapped[str] = mapped_column(String(512))
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.2/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.2/src/hapi_schema/db_patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Patch table"""
 
 import enum
 from datetime import datetime
 
-from sqlalchemy import DateTime, Enum, Integer, String
+from sqlalchemy import DateTime, Enum, Integer, String, select
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
+from hapi_schema.utils.view_params import ViewParams
 
 
 class StateEnum(str, enum.Enum):
     discovered = 1  # -> it was found in the patch repo
     executed = 2  # -> the patch was executed successfully
     failed = 3  # -> HWA tried to execute the patch but it failed (either pre-conditions
     #                were not met OR the transaction failed and was rolled back)
@@ -20,27 +21,44 @@
 class DBPatch(Base):
     __tablename__ = "patch"
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     patch_sequence_number: Mapped[int] = mapped_column(
         Integer, nullable=False, index=True
     )
-    commit_hash: Mapped[str] = mapped_column(
-        String(48), unique=True, nullable=False
-    )
+    commit_hash: Mapped[str] = mapped_column(String(48), nullable=False)
     commit_date: Mapped[datetime] = mapped_column(DateTime, nullable=False)
     patch_path: Mapped[str] = mapped_column(
         String(512), nullable=False, index=True
     )
     patch_permalink_url: Mapped[str] = mapped_column(
         String(1024), nullable=False, unique=True
     )
     patch_target: Mapped[str] = mapped_column(String(128), nullable=False)
-    patch_hash: Mapped[str] = mapped_column(
-        String(48), unique=True, nullable=False
-    )
+    patch_hash: Mapped[str] = mapped_column(String(48), nullable=False)
     state: Mapped[StateEnum] = mapped_column(
         Enum(StateEnum), nullable=False, index=True
     )
     execution_date: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, index=True
     )
+
+
+view_params_patch = ViewParams(
+    name="patch_view",
+    metadata=Base.metadata,
+    selectable=select(*DBPatch.__table__.columns),
+)
+
+
+class DBPatchVAT(Base):
+    __tablename__ = "patch_vat"
+    id: Mapped[int] = mapped_column(Integer, primary_key=True)
+    patch_sequence_number: Mapped[int] = mapped_column(Integer, index=True)
+    commit_hash: Mapped[str] = mapped_column(String(48))
+    commit_date: Mapped[datetime] = mapped_column(DateTime)
+    patch_path: Mapped[str] = mapped_column(String(512), index=True)
+    patch_permalink_url: Mapped[str] = mapped_column(String(1024))
+    patch_target: Mapped[str] = mapped_column(String(128))
+    patch_hash: Mapped[str] = mapped_column(String(48))
+    state: Mapped[str] = mapped_column(String(10), index=True)
+    execution_date: Mapped[datetime] = mapped_column(DateTime, index=True)
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_poverty_rate.py` & `hapi_schema-0.8.2/src/hapi_schema/db_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_refugees.py` & `hapi_schema-0.8.2/src/hapi_schema/db_refugees.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,26 +60,27 @@
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
 
-    resource = relationship("DBResource")
+    # resource = relationship("DBResource")
     origin_country = relationship(
         "DBLocation", foreign_keys=(origin_location_ref)
     )
     asylum_country = relationship(
         "DBLocation", foreign_keys=(asylum_location_ref)
     )
 
 
 # Use aliases because we join to DBLocation twice
 origin_location = aliased(DBLocation)
 asylum_location = aliased(DBLocation)
+resource = relationship("DBResource")
 
 view_params_refugees = ViewParams(
     name="refugees_view",
     metadata=Base.metadata,
     selectable=select(
         *DBRefugees.__table__.columns,
         origin_location.code.label("origin_location_code"),
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.2/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/views.py` & `hapi_schema-0.8.2/src/hapi_schema/views.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/src/hapi_schema/utils/constraints.py` & `hapi_schema-0.8.2/src/hapi_schema/utils/constraints.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,22 @@
     population_var_name: str = "population",
 ) -> CheckConstraint:
     """Population must not be a negative number."""
     sqltext = f"{population_var_name} >= 0"
     return CheckConstraint(sqltext=sqltext, name=f"{population_var_name}")
 
 
+def non_negative_constraint(
+    var_name: str,
+) -> CheckConstraint:
+    """Require a column to be non-negative."""
+    sqltext = f"{var_name} >= 0"
+    return CheckConstraint(sqltext=sqltext, name=f"{var_name}")
+
+
 def reference_period_constraint() -> CheckConstraint:
     """reference_period_end should be greater than reference_period_start"""
     sqltext = "reference_period_end >= reference_period_start "
     return CheckConstraint(sqltext=sqltext, name="reference_period")
 
 
 def general_risk_constraint(risk_name: str) -> CheckConstraint:
@@ -50,7 +58,13 @@
     admin_level: str,
 ) -> UniqueConstraint:
     return UniqueConstraint(
         "code",
         "reference_period_start",
         name=f"{admin_level}_code_and_reference_period_unique",
     )
+
+
+def latlon_constraint() -> CheckConstraint:
+    """Latitude and longitude must be valid"""
+    sqltext = "lat <= 90.0 AND lat >= -90.0 AND lon <= 180.0 AND lon >= -180.0"
+    return CheckConstraint(sqltext=sqltext, name="latlon")
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/utils/enums.py` & `hapi_schema-0.8.2/src/hapi_schema/utils/enums.py`

 * *Files 25% similar despite different names*

```diff
@@ -47,14 +47,26 @@
     AFFECTED = "AFF"
     INNEED = "INN"
     TARGETED = "TGT"
     REACHED = "REA"
     ALL = "*"
 
 
+class PriceFlag(str, enum.Enum):
+    ACTUAL = "actual"
+    AGGREGATE = "aggregate"
+    ACTUAL_AGGREGATE = "actual,aggregate"
+
+
+class PriceType(str, enum.Enum):
+    FARM_GATE = "Farm Gate"
+    RETAIL = "Retail"
+    WHOLESALE = "Wholesale"
+
+
 class PovertyClassification(str, enum.Enum):
     POOR = "poor"
     VULNERABLE = "vulnerable"
     EXTREMELY_POOR = "extremely_poor"
     ALL = "*"
 
 
@@ -76,7 +88,18 @@
 
 class RiskClass(str, enum.Enum):
     VERY_LOW = "1"
     LOW = "2"
     MEDIUM = "3"
     HIGH = "4"
     VERY_HIGH = "5"
+
+
+class CommodityCategory(str, enum.Enum):
+    CEREALS_TUBORS = "cereals and tubors"
+    MEAT_FISH_EGGS = "meat, fish and eggs"
+    MILK_DAIRY = "milk and dairy"
+    MISCELLANEOUS_FOOD = "miscellaneous food"
+    NON_FOOD = "non-food"
+    OILS_FATS = "oils and fats"
+    PULSES_NUTS = "pulses and nuts"
+    VEGETABLES_FRUITS = "vegetables and fruits"
```

### Comparing `hapi_schema-0.8.0/src/hapi_schema/utils/view_as_table_code_generator.py` & `hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_code_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,150 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 This script is designed to print a sqlalchemy table class from a view.
-To use it the code needs to be edited appropriately before running it:
 
-1. Update the import of the view_params below to pick the right view
-2. Change the target_view string to provide the new table name - conventionally this ends "_vat"
-3. Fill in the expected_primary_keys and expected_indexes lists
-4. Run the script - the class definition is output to console
-5. Copy the class definition to the file from which the view_params were
-6. Create a test of the view following the style, of test_operational_presence.py/test_operational_presence_vat -
-   this requires the expected_primary_keys and expected_indexes created in step 3 and will check the "view_as_tables"
-   columns match the view columns as well as checking the primary_keys and indexes.
+The code is configured using the `view_as_table_definitions.toml` file and then with an invocation like:
+
+`./view_as_table_code_generator.py patch_view`
+
+This will pick up the appropriate section from the toml file
 
 Ian Hopkinson 2024-05-09
 """
 
+import os
+import sys
+from importlib import import_module
+
+import tomllib
 from hdx.database import Database
-from sqlalchemy import Table
 
 # Edit this to import the view parameters
-from hapi_schema.db_national_risk import (
-    view_params_national_risk,
-)
 from hapi_schema.utils.base import Base
 from hapi_schema.views import prepare_hapi_views
 
 
-def output_table_code_to_stdout():
-    # Change these the target_view, prepare_view, expected_primary_keys and expected_indexes
+def parse_toml():
     target_view = "national_risk_view"
-    _ = Database.prepare_view(view_params_national_risk.__dict__)
-    expected_primary_keys = [
-        "location_ref",
-        "reference_period_start",
-        "reference_period_end",
-    ]
+    if len(sys.argv) == 2:
+        target_view = sys.argv[1]
+
+    config_file_path = os.path.join(
+        os.path.dirname(__file__), "view_as_table_definitions.toml"
+    )
+    with open(config_file_path, "rb") as file_handle:
+        config = tomllib.load(file_handle)
+
+    parameters = None
+    for table in config["tables"]:
+        if table["target_view"] == target_view:
+            parameters = table
+            break
+
+    test_code = create_test_code(parameters)
+    for line in test_code:
+        print(line, flush=True)
+
+    table_code = create_table_code(parameters)
+    for line in table_code:
+        print(line, flush=True)
+
+
+def create_table_code(parameters: dict) -> list[str]:
+    # Change these the target_view, prepare_view, expected_primary_keys and expected_indexes
+    target_view = parameters["target_view"]
+    expected_primary_keys = parameters["expected_primary_keys"]
+    expected_indexes = parameters["expected_indexes"]
+    expected_nullables = parameters["expected_nullables"]
 
-    expected_indexes = []
+    view_params_dict = dynamically_load_view_params(
+        parameters["db_module"], parameters["view_params_name"]
+    )
+    _ = Database.prepare_view(view_params_dict)
     #
     session = make_session()
     target_table = target_view.replace("view", "vat")
     Base.metadata.create_all(session.get_bind())
     Base.metadata.reflect(bind=session.get_bind(), views=True)
     columns = Base.metadata.tables[target_view].columns
 
-    new_columns = make_table_template_from_view(
+    new_columns, table_code = make_table_template_from_view(
         target_table,
         columns,
-        expected_indexes,
-        primary_keys=expected_primary_keys,
+        expected_indexes=expected_indexes,
+        expected_nullables=expected_nullables,
+        expected_primary_keys=expected_primary_keys,
     )
 
-    _ = Table(target_table, Base.metadata, *new_columns)
+    return table_code
 
-    Base.metadata.create_all(session.get_bind())
 
-    assert target_table in Base.metadata.tables.keys()
+def create_test_code(parameters: dict) -> list[str]:
+    test_code = []
+
+    test_code.append(
+        f"from hapi_schema.{parameters['db_module']} import {parameters['view_params_name']}"
+    )
+
+    table_name = parameters["target_view"].replace("view", "vat")
+    test_code.append(
+        f""
+        f"def test_{table_name}(\n"
+        f"    run_indexes_test, run_columns_test, run_primary_keys_test\n"
+        f"):\n"
+        f"    '''Check that {table_name} is correct - columns match, expected indexes present'''\n"
+        f"    expected_primary_keys = {parameters['expected_primary_keys']}\n"
+        f"    expected_indexes = {parameters['expected_indexes']}\n"
+        f"    run_columns_test('{table_name}', '{parameters['target_view']}', {parameters['view_params_name']})\n"
+        f"    run_indexes_test('{table_name}', expected_indexes)\n"
+        f"    run_primary_keys_test('{table_name}', expected_primary_keys)\n"
+    )
+    return test_code
 
 
 def make_table_template_from_view(
-    target_table, columns, expected_indexes, primary_keys=["id"]
+    target_table,
+    columns,
+    expected_indexes=None,
+    expected_primary_keys=None,
+    expected_nullables=None,
 ):
+    if expected_primary_keys is None:
+        expected_primary_keys = ["id"]
+    if expected_indexes is None:
+        expected_indexes = []
+    if expected_nullables is None:
+        expected_nullables = []
+
     # Make a CamelCase name from the supplied table name
     class_name = (
         "DB"
         + target_table.replace("_vat", "")
         .replace("_", " ")
         .title()
         .replace(" ", "")
         + "VAT"
     )
-    print(f"class {class_name}(Base):", flush=True)
-    print(f"    __tablename__ = '{target_table}'", flush=True)
+    table_code = []
+    table_code.append(f"class {class_name}(Base):")
+    table_code.append(f"    __tablename__ = '{target_table}'")
 
     new_columns = []
     for column in columns:
         new_column = column._copy()
         primary_key_str = ""
         index_str = ""
-        if column.name in primary_keys:
+        nullable_str = ""
+        if column.name in expected_primary_keys:
             primary_key_str = ", primary_key=True"
         if column.name in expected_indexes:
             index_str = ", index=True"
+        if column.name in expected_nullables:
+            nullable_str = ", nullable=True"
         column_type = str(column.type)
         mapped_type_1 = column_type
         mapped_type_2 = column_type
         if column_type == "INTEGER":
             mapped_type_1 = "int"
             mapped_type_2 = "Integer"
         elif column_type.startswith("VARCHAR"):
@@ -100,26 +158,34 @@
             mapped_type_2 = "DateTime"
         elif column_type in ["FLOAT", "DOUBLE PRECISION"]:
             mapped_type_1 = "float"
             mapped_type_2 = "Float"
         elif column_type == "TEXT":
             mapped_type_1 = "str"
             mapped_type_2 = "Text"
-        print(
-            f"    {column.name}: Mapped[{mapped_type_1}] = mapped_column({mapped_type_2}{primary_key_str}{index_str})"
+        table_code.append(
+            f"    {column.name}: Mapped[{mapped_type_1}] = mapped_column({mapped_type_2}{primary_key_str}{nullable_str}{index_str})"
         )
 
         new_columns.append(new_column)
-    return new_columns
+    return new_columns, table_code
 
 
 def make_session():
     db_uri = "postgresql+psycopg://postgres:postgres@localhost:5432/hapitest"
     database = Database(
         db_uri=db_uri, recreate_schema=True, prepare_fn=prepare_hapi_views
     )
     session = database.get_session()
     return session
 
 
+def dynamically_load_view_params(db_module, view_name):
+    module = import_module(f"hapi_schema.{db_module}")
+    target_view_params = getattr(module, f"{view_name}")
+
+    return target_view_params.__dict__
+
+
 if __name__ == "__main__":
-    output_table_code_to_stdout()
+    parse_toml()
+    # output_table_code_to_stdout()
```

### Comparing `hapi_schema-0.8.0/tests/conftest.py` & `hapi_schema-0.8.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 )
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.declarative import DeclarativeMeta
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.db_conflict_event import DBConflictEvent
+from hapi_schema.db_currency import DBCurrency
 from hapi_schema.db_dataset import DBDataset
+from hapi_schema.db_food_price import (
+    DBFoodPrice,
+)
 from hapi_schema.db_food_security import (
     DBFoodSecurity,
 )
 from hapi_schema.db_funding import DBFunding
 from hapi_schema.db_humanitarian_needs import (
     DBHumanitarianNeeds,
 )
@@ -30,34 +34,40 @@
 from hapi_schema.db_org_type import DBOrgType
 from hapi_schema.db_patch import DBPatch
 from hapi_schema.db_population import DBPopulation
 from hapi_schema.db_poverty_rate import DBPovertyRate
 from hapi_schema.db_refugees import DBRefugees
 from hapi_schema.db_resource import DBResource
 from hapi_schema.db_sector import DBSector
+from hapi_schema.db_wfp_commodity import DBWFPCommodity
+from hapi_schema.db_wfp_market import DBWFPMarket
 from hapi_schema.utils.base import Base
 from hapi_schema.views import prepare_hapi_views
 from sample_data.data_admin1 import data_admin1
 from sample_data.data_admin2 import data_admin2
 from sample_data.data_conflict_event import data_conflict_event
+from sample_data.data_currency import data_currency
 from sample_data.data_dataset import data_dataset
+from sample_data.data_food_price import data_food_price
 from sample_data.data_food_security import data_food_security
 from sample_data.data_funding import data_funding
 from sample_data.data_humanitarian_needs import data_humanitarian_needs
 from sample_data.data_location import data_location
 from sample_data.data_national_risk import data_national_risk
 from sample_data.data_operational_presence import data_operational_presence
 from sample_data.data_org import data_org
 from sample_data.data_org_type import data_org_type
 from sample_data.data_patch import data_patch
 from sample_data.data_population import data_population
 from sample_data.data_poverty_rate import data_poverty_rate
 from sample_data.data_refugees import data_refugees
 from sample_data.data_resource import data_resource
 from sample_data.data_sector import data_sector
+from sample_data.data_wfp_commodity import data_wfp_commodity
+from sample_data.data_wfp_market import data_wfp_market
 
 
 @pytest.fixture(scope="session")
 def session():
     # Build the DB
     db_uri = "postgresql+psycopg://postgres:postgres@localhost:5432/hapitest"
     database = Database(
@@ -72,23 +82,27 @@
     session.execute(insert(DBLocation), data_location)
     session.execute(insert(DBAdmin1), data_admin1)
     session.execute(insert(DBAdmin2), data_admin2)
 
     session.execute(insert(DBOrgType), data_org_type)
     session.execute(insert(DBOrg), data_org)
     session.execute(insert(DBSector), data_sector)
+    session.execute(insert(DBWFPCommodity), data_wfp_commodity)
+    session.execute(insert(DBWFPMarket), data_wfp_market)
+    session.execute(insert(DBCurrency), data_currency)
 
     session.execute(insert(DBConflictEvent), data_conflict_event)
     session.execute(insert(DBFunding), data_funding)
     session.execute(insert(DBNationalRisk), data_national_risk)
     session.execute(insert(DBPopulation), data_population)
     session.execute(insert(DBOperationalPresence), data_operational_presence)
     session.execute(insert(DBPovertyRate), data_poverty_rate)
     session.execute(insert(DBRefugees), data_refugees)
     session.execute(insert(DBFoodSecurity), data_food_security)
+    session.execute(insert(DBFoodPrice), data_food_price)
     session.execute(insert(DBHumanitarianNeeds), data_humanitarian_needs)
 
     session.execute(insert(DBPatch), data_patch)
 
     session.commit()
     return session
```

### Comparing `hapi_schema-0.8.0/tests/test_admin1.py` & `hapi_schema-0.8.2/tests/test_admin1.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,24 @@
         whereclause=(
             view_admin1.c.id == 1,
             view_admin1.c.location_code == "FOO",
         ),
     )
 
 
-def test_admin1_vat(run_indexes_test, run_columns_test):
-    """Check that the admin1 view as table is correct - columns match, expected indexes present"""
-    expected_indexes = [
-        "location_code",
-        "location_name",
-        "reference_period_start",
-        "reference_period_end",
-    ]
-    run_columns_test("admin1_vat", "admin1_view", view_params_admin1)
-    run_indexes_test("admin1_vat", expected_indexes)
+def test_admin1_defaults(run_view_test):
+    """Check that default values are set properly."""
+    view_admin1 = Database.prepare_view(view_params_admin1.__dict__)
+    run_view_test(
+        view=view_admin1,
+        whereclause=(
+            view_admin1.c.id == 2,
+            view_admin1.c.from_cods,  # should be True
+        ),
+    )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBAdmin1(
```

### Comparing `hapi_schema-0.8.0/tests/test_admin2.py` & `hapi_schema-0.8.2/tests/sample_data/data_humanitarian_needs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,63 @@
 from datetime import datetime
 
-from hdx.database import Database
-
-from hapi_schema.db_admin2 import DBAdmin2, view_params_admin2
-
-
-def test_admin2_view(run_view_test):
-    """Check that admin2 view references admin1 and location."""
-    view_admin2 = Database.prepare_view(view_params_admin2.__dict__)
-    run_view_test(
-        view=view_admin2,
-        whereclause=(
-            view_admin2.c.id == 1,
-            view_admin2.c.admin1_code == "FOO-XXX",
-            view_admin2.c.location_code == "FOO",
-        ),
-    )
-
-
-def test_admin2_vat(run_indexes_test, run_columns_test):
-    """Check that the view as table is correct - columns match, expected indexes present"""
-    expected_indexes = [
-        "location_code",
-        "location_name",
-        "code",
-        "name",
-        "location_name",
-        "reference_period_start",
-        "reference_period_end",
-    ]
-    run_columns_test("admin2_vat", "admin2_view", view_params_admin2)
-    run_indexes_test("admin2_vat", expected_indexes)
-
-
-def test_reference_period_constraint(run_constraints_test):
-    """Check that reference_period_end cannot be less than start"""
-    run_constraints_test(
-        new_rows=[
-            DBAdmin2(
-                admin1_ref=3,
-                code="FOO-002-D",
-                name="District D",
-                is_unspecified=False,
-                reference_period_start=datetime(2023, 1, 2),
-                reference_period_end=datetime(2023, 1, 1),
-            )
-        ],
-        expected_constraint="reference_period",
-    )
-
-
-def test_code_date_unique(run_constraints_test):
-    """Check that reference_period_start and code must be unique together"""
-    run_constraints_test(
-        new_rows=[
-            DBAdmin2(
-                admin1_ref=3,
-                code="FOO-002-D",
-                name="District D",
-                is_unspecified=False,
-                reference_period_start=datetime(2023, 1, 1),
-            ),
-            DBAdmin2(
-                admin1_ref=3,
-                code="FOO-002-D",
-                name="District D",
-                is_unspecified=False,
-                reference_period_start=datetime(2023, 1, 1),
-            ),
-        ],
-        expected_constraint="admin2_code_and_reference_period_unique",
-    )
+data_humanitarian_needs = [
+    # total national
+    dict(
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=1,
+        gender="*",
+        age_range="*",
+        disabled_marker="*",
+        sector_code="*",
+        population_group="*",
+        population_status="AFF",
+        population=1_000_000,
+        reference_period_start=datetime(2023, 1, 1),
+        reference_period_end=datetime(2023, 6, 30),
+    ),
+    # national f, all ages, disabled, sector SHL
+    dict(
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=1,
+        gender="f",
+        age_range="*",
+        disabled_marker="n",
+        sector_code="SHL",
+        population_group="REF",
+        population_status="INN",
+        population=500_000,
+        reference_period_start=datetime(2023, 1, 1),
+        reference_period_end=datetime(2023, 6, 30),
+    ),
+    # admin1 f, age 0-4, not disabled, sector WSH
+    dict(
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=2,
+        gender="f",
+        age_range="0-4",
+        min_age=0,
+        max_age=4,
+        disabled_marker="y",
+        sector_code="WSH",
+        population_group="IDP",
+        population_status="INN",
+        population=5_000,
+        reference_period_start=datetime(2023, 1, 1),
+        reference_period_end=datetime(2023, 6, 30),
+    ),
+    # admin2 ages 80+, disabled, sector HEA
+    dict(
+        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        admin2_ref=4,
+        gender="*",
+        age_range="80+",
+        min_age=80,
+        disabled_marker="y",
+        sector_code="HEA",
+        population_group="IDP",
+        population_status="AFF",
+        population=500,
+        reference_period_start=datetime(2023, 1, 1),
+        reference_period_end=datetime(2023, 6, 30),
+    ),
+]
```

### Comparing `hapi_schema-0.8.0/tests/test_conflict_event.py` & `hapi_schema-0.8.2/tests/test_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/test_dataset.py` & `hapi_schema-0.8.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/test_food_security.py` & `hapi_schema-0.8.2/tests/test_food_security.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,33 +21,14 @@
             view_food_security.c.admin2_code == "FOO-001-A",
             view_food_security.c.admin1_code == "FOO-001",
             view_food_security.c.location_code == "FOO",
         ),
     )
 
 
-def test_food_security_vat(run_indexes_test, run_columns_test):
-    """Check that the food_security view as table is correct - columns match, expected indexes present"""
-    expected_indexes = [
-        "admin2_ref",
-        "population_fraction_in_phase",
-        "ipc_phase",
-        "ipc_type",
-        "admin2_code",
-        "admin2_name",
-        "location_name",
-        "reference_period_start",
-        "reference_period_end",
-    ]
-    run_columns_test(
-        "food_security_vat", "food_security_view", view_params_food_security
-    )
-    run_indexes_test("food_security_vat", expected_indexes)
-
-
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBFoodSecurity(
                 resource_hdx_id="62ad6e55-5f5d-4494-854c-4110687e9e25",
                 admin2_ref=4,
```

### Comparing `hapi_schema-0.8.0/tests/test_funding.py` & `hapi_schema-0.8.2/tests/test_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/test_humanitarian_needs.py` & `hapi_schema-0.8.2/tests/test_humanitarian_needs.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,33 +34,14 @@
             == "Water Sanitation Hygiene",
             view_humanitarian_needs.c.gender == "f",
             view_humanitarian_needs.c.disabled_marker == "y",  # noqa: E712
         ),
     )
 
 
-def test_humanitarian_needs_vat(run_indexes_test, run_columns_test):
-    """Check that the humanitarian_needs view as table is correct - columns match, expected indexes present"""
-    expected_indexes = [
-        "admin2_ref",
-        "admin2_code",
-        "admin2_name",
-        "location_name",
-        "min_age",
-        "max_age",
-        "reference_period_end",
-    ]
-    run_columns_test(
-        "humanitarian_needs_vat",
-        "humanitarian_needs_view",
-        view_params_humanitarian_needs,
-    )
-    run_indexes_test("humanitarian_needs_vat", expected_indexes)
-
-
 @pytest.fixture(scope="module")
 def base_parameters():
     return dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
         gender=Gender.ALL,
         age_range="-1-20",
```

### Comparing `hapi_schema-0.8.0/tests/test_location.py` & `hapi_schema-0.8.2/tests/test_location.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,26 @@
             view_location.c.id == 1,
             view_location.c.code == "FOO",
             view_location.c.name == "Foolandia",
         ),
     )
 
 
+def test_location_defaults(run_view_test):
+    """Check that default values are set properly."""
+    view_location = Database.prepare_view(view_params_location.__dict__)
+    run_view_test(
+        view=view_location,
+        whereclause=(
+            view_location.c.id == 1,
+            view_location.c.from_cods,  # should be True
+        ),
+    )
+
+
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBLocation(
                 code="BAR",
                 name="Barlandia",
```

### Comparing `hapi_schema-0.8.0/tests/test_national_risk.py` & `hapi_schema-0.8.2/tests/test_national_risk.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,32 +20,14 @@
             view_national_risk.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
             view_national_risk.c.location_name == "Foolandia",
         ),
     )
 
 
-def test_national_risk_vat(
-    run_indexes_test, run_columns_test, run_primary_keys_test
-):
-    """Check that the national_risk view as table is correct - columns match, expected indexes present"""
-    expected_primary_keys = [
-        "location_ref",
-        "reference_period_start",
-        "reference_period_end",
-    ]
-
-    expected_indexes = []
-    run_columns_test(
-        "national_risk_vat", "national_risk_view", view_params_national_risk
-    )
-    run_indexes_test("national_risk_vat", expected_indexes)
-    run_primary_keys_test("national_risk_vat", expected_primary_keys)
-
-
 @pytest.fixture
 def base_parameters():
     return dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         location_ref=1,
         risk_class="5",
         global_rank=4,
```

### Comparing `hapi_schema-0.8.0/tests/test_operational_presence.py` & `hapi_schema-0.8.2/tests/test_operational_presence.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,41 +25,14 @@
             view_operational_presence.c.org_type_code == "437",
             view_operational_presence.c.sector_name
             == "Water Sanitation Hygiene",
         ),
     )
 
 
-def test_operational_presence_vat(
-    run_indexes_test, run_columns_test, run_primary_keys_test
-):
-    """Check that the operational_presence view as table is correct - columns match, expected indexes present"""
-    expected_primary_keys = [
-        "admin2_ref",
-        "org_acronym",
-        "org_name",
-        "reference_period_start",
-    ]
-
-    expected_indexes = [
-        "admin2_ref",
-        "admin2_code",
-        "admin2_name",
-        "location_name",
-        "reference_period_end",
-    ]
-    run_columns_test(
-        "operational_presence_vat",
-        "operational_presence_view",
-        view_params_operational_presence,
-    )
-    run_indexes_test("operational_presence_vat", expected_indexes)
-    run_primary_keys_test("operational_presence_vat", expected_primary_keys)
-
-
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBOperationalPresence(
                 resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=2,
```

### Comparing `hapi_schema-0.8.0/tests/test_patch.py` & `hapi_schema-0.8.2/tests/test_patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,15 @@
         patch_path VARCHAR(512) NOT NULL,
         patch_permalink_url VARCHAR(1024) NOT NULL,
         patch_target VARCHAR(128) NOT NULL,
         patch_hash VARCHAR(48) NOT NULL,
         state VARCHAR(10) NOT NULL,
         execution_date DATETIME,
         PRIMARY KEY (id),
-        UNIQUE (commit_hash),
-        UNIQUE (patch_permalink_url),
-        UNIQUE (patch_hash)
+        UNIQUE (patch_permalink_url)
 )
 """
     sql_patch_sequence_number_index_creation = """
     CREATE INDEX ix_patch_patch_sequence_number ON patch (patch_sequence_number)
     """
     sql_state_index_creation = (
         """CREATE INDEX ix_patch_state ON patch (state)"""
```

### Comparing `hapi_schema-0.8.0/tests/test_population.py` & `hapi_schema-0.8.2/tests/test_population.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,39 +19,14 @@
             view_population.c.admin1_code == "FOO-001",
             view_population.c.location_code == "FOO",
             view_population.c.gender == "f",
         ),
     )
 
 
-def test_population_vat(
-    run_indexes_test, run_columns_test, run_primary_keys_test
-):
-    """Check that the population view as table is correct - columns match, expected indexes present"""
-    expected_primary_keys = [
-        "admin2_ref",
-        "gender",
-        "age_range",
-    ]
-
-    expected_indexes = [
-        "min_age",
-        "max_age",
-        "reference_period_start",
-        "reference_period_end",
-    ]
-    run_columns_test(
-        "population_vat",
-        "population_view",
-        view_params_population,
-    )
-    run_indexes_test("population_vat", expected_indexes)
-    run_primary_keys_test("population_vat", expected_primary_keys)
-
-
 @pytest.fixture
 def base_parameters():
     return dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
         gender=Gender.ALL,
         population=1_000_000,
```

### Comparing `hapi_schema-0.8.0/tests/test_poverty_rate.py` & `hapi_schema-0.8.2/tests/test_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/test_refugees.py` & `hapi_schema-0.8.2/tests/test_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_admin2.py` & `hapi_schema-0.8.2/tests/sample_data/data_admin2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 data_admin2 = [
     dict(
         admin1_ref=1,
         code="FOO-XXX-XXX",
         name="Unspecified",
         is_unspecified=True,
+        from_cods=False,
     ),
     dict(
         admin1_ref=2,
         code="FOO-001-XXX",
         name="Unspecified",
         is_unspecified=True,
+        from_cods=False,
     ),
     dict(
         admin1_ref=3,
         code="FOO-002-XXX",
         name="Unspecified",
         is_unspecified=True,
+        from_cods=False,
     ),
     dict(
         admin1_ref=2,
         code="FOO-001-A",
         name="District A",
         is_unspecified=False,
     ),
```

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_conflict_event.py` & `hapi_schema-0.8.2/tests/sample_data/data_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_food_security.py` & `hapi_schema-0.8.2/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.2/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.2/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_patch.py` & `hapi_schema-0.8.2/tests/sample_data/data_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_population.py` & `hapi_schema-0.8.2/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_refugees.py` & `hapi_schema-0.8.2/tests/sample_data/data_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/tests/sample_data/data_resource.py` & `hapi_schema-0.8.2/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/.gitignore` & `hapi_schema-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/LICENSE` & `hapi_schema-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/pyproject.toml` & `hapi_schema-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.0/PKG-INFO` & `hapi_schema-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.8.0
+Version: 0.8.2
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

