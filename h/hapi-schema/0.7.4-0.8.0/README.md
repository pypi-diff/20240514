# Comparing `tmp/hapi_schema-0.7.4.tar.gz` & `tmp/hapi_schema-0.8.0.tar.gz`

## Comparing `hapi_schema-0.7.4.tar` & `hapi_schema-0.8.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/changelog.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/contributing.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/coveragerc
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.config/ruff.toml
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_age_range.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_gender.py
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_ipc_phase.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_ipc_type.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_population_group.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_population_status.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/conftest.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_admin1.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_admin2.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_age_range.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_dataset.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_food_security.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_gender.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_ipc_phase.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_ipc_type.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_location.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_national_risk.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_operational_presence.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_org.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_org_type.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_patch.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_population.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_population_group.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_population_status.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_resource.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/test_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_age_range.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_gender.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_ipc_phase.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_ipc_type.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_population_group.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_population_status.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/README.md
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_admin1.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_admin2.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_dataset.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_food_security.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_funding.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_location.py
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_national_risk.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_org_type.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_patch.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_population.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_refugees.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/test_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.0/PKG-INFO
```

### Comparing `hapi_schema-0.7.4/contributing.md` & `hapi_schema-0.8.0/contributing.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 
 To check if your changes pass pre-commit without committing, run:
 
     pre-commit run --all-files --config=.config/pre-commit-config.yaml
 
 ## Testing
 
+Testing is now done against a Postgres database which can be deployed from the Docker definition in the `docker` directory using:
+
+`docker-compose up -d`
+
 To run the tests and view coverage, execute:
 
     pytest -c .config/pytest.ini --cov hapi_schema --cov-config .config/coveragerc
 
 Follow the example set out already in ``documentation/main.md`` as you write the documentation.
 
 ## Packages
```

### Comparing `hapi_schema-0.7.4/requirements.txt` & `hapi_schema-0.8.0/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,44 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --all-extras --output-file=requirements.txt pyproject.toml
-#
+# This file was autogenerated by uv via the following command:
+#    uv pip compile pyproject.toml --resolver=backtracking --all-extras -o requirements.txt
 cfgv==3.4.0
     # via pre-commit
-colorama==0.4.6
-    # via pytest
-coverage[toml]==7.4.4
-    # via
-    #   coverage
-    #   pytest-cov
+coverage==7.5.1
+    # via pytest-cov
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.4
+filelock==3.14.0
     # via virtualenv
 greenlet==3.0.3
     # via sqlalchemy
-hdx-python-database==1.3.0
-    # via hapi-schema (pyproject.toml)
-identify==2.5.35
+hdx-python-database==1.3.1
+identify==2.5.36
     # via pre-commit
 iniconfig==2.0.0
     # via pytest
 nodeenv==1.8.0
     # via pre-commit
 packaging==24.0
     # via pytest
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 pre-commit==3.7.0
-    # via hapi-schema (pyproject.toml)
-pytest==8.1.1
-    # via
-    #   hapi-schema (pyproject.toml)
-    #   pytest-cov
+psycopg==3.1.18
+psycopg-binary==3.1.18
+    # via psycopg
+pytest==8.2.0
+    # via pytest-cov
 pytest-cov==5.0.0
-    # via hapi-schema (pyproject.toml)
 pyyaml==6.0.1
     # via pre-commit
-sqlalchemy==2.0.29
-    # via
-    #   hapi-schema (pyproject.toml)
-    #   hdx-python-database
+setuptools==69.5.1
+    # via nodeenv
+sqlalchemy==2.0.30
+    # via hdx-python-database
 typing-extensions==4.11.0
-    # via sqlalchemy
-virtualenv==20.25.3
+    # via
+    #   psycopg
+    #   sqlalchemy
+virtualenv==20.26.1
     # via pre-commit
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `hapi_schema-0.7.4/.github/workflows/publish.yaml` & `hapi_schema-0.8.0/.github/workflows/publish.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: '3.11'
+        python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install --upgrade hatch
     - name: Build with hatch
       run: |
         hatch build
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.0/src/hapi_schema/db_admin1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 """Admin1 table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
     Boolean,
-    CheckConstraint,
     DateTime,
     ForeignKey,
     Integer,
     String,
-    UniqueConstraint,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_location import DBLocation
 from hapi_schema.utils.base import Base
+from hapi_schema.utils.constraints import (
+    code_and_reference_period_unique_constraint,
+    reference_period_constraint,
+)
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBAdmin1(Base):
     __tablename__ = "admin1"
     __table_args__ = (
-        CheckConstraint(
-            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
-            name="reference_period",
-        ),
-        CheckConstraint(
-            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
-            name="hapi_dates",
-        ),
-        UniqueConstraint("code", "hapi_updated_date"),
+        reference_period_constraint(),
+        code_and_reference_period_unique_constraint(admin_level="admin1"),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     location_ref: Mapped[int] = mapped_column(
         ForeignKey("location.id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
-    code: Mapped[str] = mapped_column(String(128), nullable=False)
-    name: Mapped[str] = mapped_column(String(512), nullable=False)
+    code: Mapped[str] = mapped_column(String(128), nullable=False, index=True)
+    name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
     is_unspecified: Mapped[bool] = mapped_column(
-        Boolean, server_default=text("FALSE")
+        Boolean, server_default=text("FALSE"), nullable=False
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
-    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
-    hapi_replaced_date: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
-    )
 
     location = relationship("DBLocation")
 
 
 view_params_admin1 = ViewParams(
     name="admin1_view",
     metadata=Base.metadata,
     selectable=select(
         *DBAdmin1.__table__.columns,
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
-        DBLocation.reference_period_start.label(
-            "location_reference_period_start"
-        ),
-        DBLocation.reference_period_end.label("location_reference_period_end"),
     ).select_from(
         DBAdmin1.__table__.join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
     ),
 )
+
+
+class DBAdmin1VAT(Base):
+    __tablename__ = "admin1_vat"
+    id: Mapped[int] = mapped_column(Integer, primary_key=True)
+    location_ref: Mapped[int] = mapped_column(Integer)
+    code: Mapped[str] = mapped_column(String(128))
+    name: Mapped[str] = mapped_column(String(512))
+    is_unspecified: Mapped[bool] = mapped_column(Boolean)
+    reference_period_start: Mapped[datetime] = mapped_column(
+        DateTime, index=True
+    )
+    reference_period_end: Mapped[datetime] = mapped_column(
+        DateTime, index=True
+    )
+    location_code: Mapped[str] = mapped_column(String(128), index=True)
+    location_name: Mapped[str] = mapped_column(String(512), index=True)
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.0/src/hapi_schema/db_poverty_rate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,81 @@
-"""Admin2 table and view."""
+"""PovertyRate table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
-    Boolean,
-    CheckConstraint,
     DateTime,
+    Enum,
     ForeignKey,
     Integer,
-    String,
-    UniqueConstraint,
     select,
-    text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_location import DBLocation
+from hapi_schema.db_resource import DBResource
 from hapi_schema.utils.base import Base
+from hapi_schema.utils.constraints import (
+    population_constraint,
+    reference_period_constraint,
+)
+from hapi_schema.utils.enums import PovertyClassification
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBAdmin2(Base):
-    __tablename__ = "admin2"
+# normalised table
+class DBPovertyRate(Base):
+    __tablename__ = "poverty_rate"
     __table_args__ = (
-        CheckConstraint(
-            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
-            name="reference_period",
-        ),
-        CheckConstraint(
-            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
-            name="hapi_dates",
-        ),
-        UniqueConstraint("code", "hapi_updated_date"),
+        population_constraint(),
+        reference_period_constraint(),
     )
 
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
+    resource_hdx_id: Mapped[str] = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
+        nullable=False,
+    )
     admin1_ref: Mapped[int] = mapped_column(
-        ForeignKey("admin1.id", onupdate="CASCADE", ondelete="CASCADE"),
+        ForeignKey("admin1.id", onupdate="CASCADE"),
         nullable=False,
+        primary_key=True,
     )
-    code: Mapped[str] = mapped_column(String(128), nullable=False)
-    name: Mapped[str] = mapped_column(String(512), nullable=False)
-    is_unspecified: Mapped[bool] = mapped_column(
-        Boolean, server_default=text("FALSE")
+    classification: Mapped[PovertyClassification] = mapped_column(
+        Enum(PovertyClassification), nullable=False, primary_key=True
     )
+    population: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
+        DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
-    )
-
-    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
-    hapi_replaced_date: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
+        DateTime, nullable=False, index=True
     )
 
-    admin1 = relationship("DBAdmin1")
+    resource = relationship(DBResource)
+    admin1 = relationship(DBAdmin1)
 
 
-view_params_admin2 = ViewParams(
-    name="admin2_view",
+# view
+view_params_poverty_rate = ViewParams(
+    name="poverty_rate_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBAdmin2.__table__.columns,
+        *DBPovertyRate.__table__.columns,
+        DBLocation.code.label("location_code"),
+        DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
-        DBAdmin1.reference_period_start.label("admin1_reference_period_start"),
-        DBAdmin1.reference_period_end.label("admin1_reference_period_end"),
-        DBLocation.code.label("location_code"),
-        DBLocation.name.label("location_name"),
-        DBLocation.reference_period_start.label(
-            "location_reference_period_start"
-        ),
-        DBLocation.reference_period_end.label("location_reference_period_end"),
+        DBAdmin1.location_ref.label("location_ref"),
     ).select_from(
-        DBAdmin2.__table__.join(
+        DBPovertyRate.__table__.join(
             DBAdmin1.__table__,
-            DBAdmin2.admin1_ref == DBAdmin1.id,
+            DBPovertyRate.admin1_ref == DBAdmin1.id,
             isouter=True,
         ).join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
-        ),
+        )
     ),
 )
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.0/src/hapi_schema/db_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class DBDataset(Base):
     __tablename__ = "dataset"
 
     hdx_id: Mapped[str] = mapped_column(String(36), primary_key=True)
     hdx_stub: Mapped[str] = mapped_column(
-        String(128), unique=True, nullable=False
+        String(128), unique=True, nullable=False, index=True
     )
     title = mapped_column(String(1024), nullable=False)
     hdx_provider_stub: Mapped[str] = mapped_column(
         String(128), nullable=False, index=True
     )
     hdx_provider_name: Mapped[str] = mapped_column(
         String(512), nullable=False, index=True
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.0/src/hapi_schema/db_food_security.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,76 @@
-"""Population table and view."""
+"""Food security table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
-    CheckConstraint,
+    Boolean,
     DateTime,
+    Enum,
     Float,
     ForeignKey,
     Integer,
-    Text,
+    String,
     select,
-    text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_admin2 import DBAdmin2
-from hapi_schema.db_dataset import DBDataset
-from hapi_schema.db_ipc_phase import DBIpcPhase
-from hapi_schema.db_ipc_type import DBIpcType
 from hapi_schema.db_location import DBLocation
 from hapi_schema.db_resource import DBResource
 from hapi_schema.utils.base import Base
+from hapi_schema.utils.constraints import (
+    population_constraint,
+    reference_period_constraint,
+)
+from hapi_schema.utils.enums import IPCPhase, IPCType
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBFoodSecurity(Base):
     __tablename__ = "food_security"
     __table_args__ = (
-        CheckConstraint(
-            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
-            name="reference_period",
-        ),
+        reference_period_constraint(),
+        population_constraint(population_var_name="population_in_phase"),
     )
 
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    resource_hdx_id: Mapped[int] = mapped_column(
+    resource_hdx_id: Mapped[str] = mapped_column(
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
     admin2_ref: Mapped[int] = mapped_column(
-        ForeignKey("admin2.id", onupdate="CASCADE"), nullable=False
-    )
-    ipc_phase_code: Mapped[str] = mapped_column(
-        ForeignKey("ipc_phase.code", onupdate="CASCADE"), nullable=False
+        ForeignKey("admin2.id", onupdate="CASCADE"), primary_key=True
     )
-    ipc_type_code: Mapped[str] = mapped_column(
-        ForeignKey("ipc_type.code", onupdate="CASCADE"), nullable=False
+    ipc_phase: Mapped[IPCPhase] = mapped_column(
+        Enum(IPCPhase), primary_key=True
     )
+    ipc_type: Mapped[IPCType] = mapped_column(Enum(IPCType), primary_key=True)
     population_in_phase: Mapped[int] = mapped_column(
         Integer, nullable=False, index=True
     )
     population_fraction_in_phase: Mapped[float] = mapped_column(
         Float, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=False, index=True
+        DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
+        DateTime, nullable=False, index=True
     )
-    source_data: Mapped[str] = mapped_column(Text, nullable=True)
 
-    resource = relationship("DBResource")
-    admin2 = relationship("DBAdmin2")
-    ipc_phase = relationship("DBIpcPhase")
-    ipc_type = relationship("DBIpcType")
+    resource = relationship(DBResource)
+    admin2 = relationship(DBAdmin2)
 
 
 view_params_food_security = ViewParams(
     name="food_security_view",
     metadata=Base.metadata,
     selectable=select(
         *DBFoodSecurity.__table__.columns,
-        DBDataset.hdx_id.label("dataset_hdx_id"),
-        DBDataset.hdx_stub.label("dataset_hdx_stub"),
-        DBDataset.title.label("dataset_title"),
-        DBDataset.hdx_provider_stub.label("dataset_hdx_provider_stub"),
-        DBDataset.hdx_provider_name.label("dataset_hdx_provider_name"),
-        DBIpcPhase.name.label("ipc_phase_name"),
-        DBResource.name.label("resource_name"),
-        DBResource.update_date.label("resource_update_date"),
-        DBResource.hapi_updated_date.label("hapi_updated_date"),
-        DBResource.hapi_replaced_date.label("hapi_replaced_date"),
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
         DBAdmin1.code.label("admin1_code"),
         DBAdmin1.name.label("admin1_name"),
         DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
         DBAdmin1.location_ref.label("location_ref"),
         DBAdmin2.code.label("admin2_code"),
@@ -106,32 +90,43 @@
             isouter=True,
         )
         .join(
             DBLocation.__table__,
             DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
-        # Join pop to resource to dataset
-        .join(
-            DBResource.__table__,
-            DBFoodSecurity.resource_hdx_id == DBResource.hdx_id,
-            isouter=True,
-        )
-        .join(
-            DBDataset.__table__,
-            DBResource.dataset_hdx_id == DBDataset.hdx_id,
-            isouter=True,
-        )
-        # Join to ipc phase
-        .join(
-            DBIpcPhase.__table__,
-            DBFoodSecurity.ipc_phase_code == DBIpcPhase.code,
-            isouter=True,
-        )
-        # Join to ipc type
-        .join(
-            DBIpcType.__table__,
-            DBFoodSecurity.ipc_type_code == DBIpcType.code,
-            isouter=True,
-        )
     ),
 )
+
+
+class DBFoodSecurityVAT(Base):
+    __tablename__ = "food_security_vat"
+    resource_hdx_id: Mapped[str] = mapped_column(String(36))
+    admin2_ref: Mapped[int] = mapped_column(
+        Integer, index=True, primary_key=True
+    )
+    ipc_phase: Mapped[IPCPhase] = mapped_column(
+        Enum(IPCPhase), index=True, primary_key=True
+    )
+    ipc_type: Mapped[IPCType] = mapped_column(
+        Enum(IPCType), index=True, primary_key=True
+    )
+    population_in_phase: Mapped[int] = mapped_column(Integer, primary_key=True)
+    population_fraction_in_phase: Mapped[float] = mapped_column(
+        Float, index=True, primary_key=True
+    )
+    reference_period_start: Mapped[datetime] = mapped_column(
+        DateTime, index=True
+    )
+    reference_period_end: Mapped[datetime] = mapped_column(
+        DateTime, index=True
+    )
+    location_code: Mapped[str] = mapped_column(String(128))
+    location_name: Mapped[str] = mapped_column(String(512), index=True)
+    admin1_code: Mapped[str] = mapped_column(String(128))
+    admin1_name: Mapped[str] = mapped_column(String(512))
+    admin1_is_unspecified: Mapped[bool] = mapped_column(Boolean)
+    location_ref: Mapped[int] = mapped_column(Integer)
+    admin2_code: Mapped[str] = mapped_column(String(128), index=True)
+    admin2_name: Mapped[str] = mapped_column(String(512), index=True)
+    admin2_is_unspecified: Mapped[bool] = mapped_column(Boolean)
+    admin1_ref: Mapped[int] = mapped_column(Integer)
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_location.py` & `hapi_schema-0.8.0/src/hapi_schema/db_location.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 """Location table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
-    CheckConstraint,
     DateTime,
     Integer,
     String,
-    UniqueConstraint,
     select,
     text,
 )
 from sqlalchemy.orm import Mapped, mapped_column
 
 from hapi_schema.utils.base import Base
+from hapi_schema.utils.constraints import (
+    code_and_reference_period_unique_constraint,
+    reference_period_constraint,
+)
 from hapi_schema.utils.view_params import ViewParams
 
 
 class DBLocation(Base):
     __tablename__ = "location"
     __table_args__ = (
-        CheckConstraint(
-            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
-            name="reference_period",
-        ),
-        CheckConstraint(
-            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
-            name="hapi_dates",
-        ),
-        UniqueConstraint("code", "hapi_updated_date"),
+        reference_period_constraint(),
+        code_and_reference_period_unique_constraint(admin_level="location"),
     )
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    code: Mapped[str] = mapped_column(String(128), nullable=False)
-    name: Mapped[str] = mapped_column(String(512), nullable=False)
+    code: Mapped[str] = mapped_column(String(128), nullable=False, index=True)
+    name: Mapped[str] = mapped_column(String(512), nullable=False, index=True)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=True, server_default=text("NULL"), index=True
     )
-    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
-    hapi_replaced_date: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
-    )
 
 
 view_params_location = ViewParams(
     name="location_view",
     metadata=Base.metadata,
     selectable=select(*DBLocation.__table__.columns),
 )
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_org.py` & `hapi_schema-0.8.0/src/hapi_schema/db_conflict_event.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,95 @@
-"""Org table and view."""
+"""ConflictEvent table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
-    CheckConstraint,
     DateTime,
+    Enum,
     ForeignKey,
     Integer,
-    String,
     select,
-    text,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
-from hapi_schema.db_org_type import DBOrgType
+from hapi_schema.db_admin1 import DBAdmin1, DBLocation
+from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.utils.base import Base
+from hapi_schema.utils.constraints import (
+    population_constraint,
+    reference_period_constraint,
+)
+from hapi_schema.utils.enums import EventType
 from hapi_schema.utils.view_params import ViewParams
 
 
-class DBOrg(Base):
-    __tablename__ = "org"
+# normalised table
+class DBConflictEvent(Base):
+    __tablename__ = "conflict_event"
     __table_args__ = (
-        CheckConstraint(
-            "(reference_period_end >= reference_period_start) OR (reference_period_start IS NULL)",
-            name="reference_period",
-        ),
-        CheckConstraint(
-            "(hapi_replaced_date IS NULL) OR (hapi_replaced_date >= hapi_updated_date)",
-            name="hapi_dates",
-        ),
-    )
-
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    acronym = mapped_column(String(32), nullable=False, index=True)
-    name: Mapped[str] = mapped_column(String(512), nullable=False)
-    org_type_code: Mapped[str] = mapped_column(
-        ForeignKey("org_type.code", onupdate="CASCADE", ondelete="CASCADE"),
-        nullable=True,
+        population_constraint(
+            population_var_name="events"
+        ),  # not really a population
+        population_constraint(population_var_name="fatalities"),
+        reference_period_constraint(),
+    )
+
+    resource_hdx_id: Mapped[str] = mapped_column(
+        ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
+        nullable=False,
+    )
+    admin2_ref: Mapped[int] = mapped_column(
+        ForeignKey("admin2.id", onupdate="CASCADE"),
+        nullable=False,
+        primary_key=True,
+    )
+    event_type: Mapped[EventType] = mapped_column(
+        Enum(EventType), nullable=False, primary_key=True
     )
+    events: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
+    fatalities: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     reference_period_start: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
+        DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
-    )
-    hapi_updated_date = mapped_column(DateTime, nullable=False, index=True)
-    hapi_replaced_date: Mapped[datetime] = mapped_column(
-        DateTime, nullable=True, server_default=text("NULL"), index=True
+        DateTime, nullable=False, index=True
     )
 
-    org_type = relationship("DBOrgType")
+    resource = relationship("DBResource")
+    admin2 = relationship("DBAdmin2")
 
 
-view_params_org = ViewParams(
-    name="org_view",
+# view
+view_params_conflict_event = ViewParams(
+    name="conflict_event_view",
     metadata=Base.metadata,
     selectable=select(
-        *DBOrg.__table__.columns,
-        DBOrgType.description.label("org_type_description"),
+        *DBConflictEvent.__table__.columns,
+        DBLocation.code.label("location_code"),
+        DBLocation.name.label("location_name"),
+        DBAdmin1.code.label("admin1_code"),
+        DBAdmin1.name.label("admin1_name"),
+        DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
+        DBAdmin1.location_ref.label("location_ref"),
+        DBAdmin2.code.label("admin2_code"),
+        DBAdmin2.name.label("admin2_name"),
+        DBAdmin2.is_unspecified.label("admin2_is_unspecified"),
+        DBAdmin2.admin1_ref.label("admin1_ref"),
     ).select_from(
-        DBOrg.__table__.join(
-            DBOrgType.__table__,
-            DBOrg.org_type_code == DBOrgType.code,
+        # Join risk to admin2
+        DBConflictEvent.__table__.join(
+            DBAdmin2.__table__,
+            DBConflictEvent.admin2_ref == DBAdmin2.id,
+            isouter=True,
+        )
+        .join(
+            DBAdmin1.__table__,
+            DBAdmin2.admin1_ref == DBAdmin1.id,
+            isouter=True,
+        )
+        .join(
+            DBLocation.__table__,
+            DBAdmin1.location_ref == DBLocation.id,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.0/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.0/src/hapi_schema/db_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.4/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.0/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.4/tests/test_admin1.py` & `hapi_schema-0.8.0/tests/test_admin2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,73 @@
 from datetime import datetime
 
-from hdx.database.views import build_view
+from hdx.database import Database
 
-from hapi_schema.db_admin1 import DBAdmin1, view_params_admin1
+from hapi_schema.db_admin2 import DBAdmin2, view_params_admin2
 
 
-def test_admin1_view(run_view_test):
-    """Check that admin1 view references location."""
-    view_admin1 = build_view(view_params_admin1.__dict__)
+def test_admin2_view(run_view_test):
+    """Check that admin2 view references admin1 and location."""
+    view_admin2 = Database.prepare_view(view_params_admin2.__dict__)
     run_view_test(
-        view=view_admin1,
+        view=view_admin2,
         whereclause=(
-            view_admin1.c.id == 1,
-            view_admin1.c.location_code == "FOO",
+            view_admin2.c.id == 1,
+            view_admin2.c.admin1_code == "FOO-XXX",
+            view_admin2.c.location_code == "FOO",
         ),
     )
 
 
+def test_admin2_vat(run_indexes_test, run_columns_test):
+    """Check that the view as table is correct - columns match, expected indexes present"""
+    expected_indexes = [
+        "location_code",
+        "location_name",
+        "code",
+        "name",
+        "location_name",
+        "reference_period_start",
+        "reference_period_end",
+    ]
+    run_columns_test("admin2_vat", "admin2_view", view_params_admin2)
+    run_indexes_test("admin2_vat", expected_indexes)
+
+
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
-            DBAdmin1(
-                location_ref=1,
-                code="FOO-003",
-                name="Province 3",
+            DBAdmin2(
+                admin1_ref=3,
+                code="FOO-002-D",
+                name="District D",
                 is_unspecified=False,
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
             )
         ],
         expected_constraint="reference_period",
     )
 
 
-def test_hapi_date_constraint(run_constraints_test):
-    """Check that hapi_replaced_date cannot be less than hapi_updated_date"""
-    run_constraints_test(
-        new_rows=[
-            DBAdmin1(
-                location_ref=1,
-                code="FOO-003",
-                name="Province 3",
-                is_unspecified=False,
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 2),
-                hapi_replaced_date=datetime(2023, 1, 1),
-            )
-        ],
-        expected_constraint="hapi_dates",
-    )
-
-
 def test_code_date_unique(run_constraints_test):
-    """Check that hapi_updated_date and code must be unique together"""
+    """Check that reference_period_start and code must be unique together"""
     run_constraints_test(
         new_rows=[
-            DBAdmin1(
-                location_ref=1,
-                code="FOO-003",
-                name="Province 3",
+            DBAdmin2(
+                admin1_ref=3,
+                code="FOO-002-D",
+                name="District D",
                 is_unspecified=False,
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
+                reference_period_start=datetime(2023, 1, 1),
             ),
-            DBAdmin1(
-                location_ref=1,
-                code="FOO-003",
-                name="Province 3",
+            DBAdmin2(
+                admin1_ref=3,
+                code="FOO-002-D",
+                name="District D",
                 is_unspecified=False,
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
+                reference_period_start=datetime(2023, 1, 1),
             ),
         ],
-        expected_constraint="UNIQUE constraint failed",
+        expected_constraint="admin2_code_and_reference_period_unique",
     )
```

### Comparing `hapi_schema-0.7.4/tests/test_dataset.py` & `hapi_schema-0.8.0/tests/test_dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from hdx.database.views import build_view
+from hdx.database import Database
 
 from hapi_schema.db_dataset import view_params_dataset
 
 
 def test_dataset_view(run_view_test):
     """Check that dataset view has most columns."""
-    view_dataset = build_view(view_params_dataset.__dict__)
+    view_dataset = Database.prepare_view(view_params_dataset.__dict__)
     run_view_test(
         view=view_dataset,
         whereclause=(
             view_dataset.c.hdx_id == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_dataset.c.hdx_stub == "dataset01",
             view_dataset.c.title == "Dataset #1",
             view_dataset.c.hdx_provider_stub == "provider01",
```

### Comparing `hapi_schema-0.7.4/tests/test_location.py` & `hapi_schema-0.8.0/tests/test_location.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 
-from hdx.database.views import build_view
+from hdx.database import Database
 
 from hapi_schema.db_location import DBLocation, view_params_location
 
 
 def test_location_view(run_view_test):
     """Check that location view has some columns."""
-    view_location = build_view(view_params_location.__dict__)
+    view_location = Database.prepare_view(view_params_location.__dict__)
     run_view_test(
         view=view_location,
         whereclause=(
             view_location.c.id == 1,
             view_location.c.code == "FOO",
             view_location.c.name == "Foolandia",
         ),
@@ -23,55 +23,30 @@
     run_constraints_test(
         new_rows=[
             DBLocation(
                 code="BAR",
                 name="Barlandia",
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
             )
         ],
         expected_constraint="reference_period",
     )
 
 
-def test_hapi_date_constraint(run_constraints_test):
-    """Check that hapi_replaced_date cannot be less than hapi_udpated_date"""
-    run_constraints_test(
-        new_rows=[
-            DBLocation(
-                code="BAR",
-                name="Barlandia",
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 2),
-                hapi_replaced_date=datetime(2023, 1, 1),
-            )
-        ],
-        expected_constraint="hapi_dates",
-    )
-
-
 def test_code_date_unique(run_constraints_test):
-    """Check that hapi_updated_date and code must be unique together"""
+    """Check that reference_period_start and code must be unique together"""
     run_constraints_test(
         new_rows=[
             DBLocation(
                 code="BAR",
                 name="Barlandia",
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
+                reference_period_start=datetime(2023, 1, 1),
             ),
             DBLocation(
                 code="BAR",
                 name="Barlandia",
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
+                reference_period_start=datetime(2023, 1, 1),
             ),
         ],
-        expected_constraint="UNIQUE constraint failed",
+        expected_constraint="location_code_and_reference_period_unique",
     )
```

### Comparing `hapi_schema-0.7.4/tests/test_operational_presence.py` & `hapi_schema-0.8.0/tests/test_operational_presence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,74 @@
 from datetime import datetime
 
-from hdx.database.views import build_view
+from hdx.database import Database
 
 from hapi_schema.db_operational_presence import (
     DBOperationalPresence,
     view_params_operational_presence,
 )
 
 
 def test_operational_presence_view(run_view_test):
     """Check that OP view has all references."""
-    view_operational_presence = build_view(
+    view_operational_presence = Database.prepare_view(
         view_params_operational_presence.__dict__
     )
     run_view_test(
         view=view_operational_presence,
         whereclause=(
-            view_operational_presence.c.id == 5,
-            view_operational_presence.c.dataset_hdx_id
-            == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
             view_operational_presence.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
-            view_operational_presence.c.resource_name == "resource-01.csv",
             view_operational_presence.c.admin2_code == "FOO-XXX-XXX",
             view_operational_presence.c.admin1_code == "FOO-XXX",
             view_operational_presence.c.location_code == "FOO",
-            view_operational_presence.c.org_type_description
-            == "International NGO",
             view_operational_presence.c.org_acronym == "ORG02",
+            view_operational_presence.c.org_type_code == "437",
             view_operational_presence.c.sector_name
             == "Water Sanitation Hygiene",
         ),
     )
 
 
+def test_operational_presence_vat(
+    run_indexes_test, run_columns_test, run_primary_keys_test
+):
+    """Check that the operational_presence view as table is correct - columns match, expected indexes present"""
+    expected_primary_keys = [
+        "admin2_ref",
+        "org_acronym",
+        "org_name",
+        "reference_period_start",
+    ]
+
+    expected_indexes = [
+        "admin2_ref",
+        "admin2_code",
+        "admin2_name",
+        "location_name",
+        "reference_period_end",
+    ]
+    run_columns_test(
+        "operational_presence_vat",
+        "operational_presence_view",
+        view_params_operational_presence,
+    )
+    run_indexes_test("operational_presence_vat", expected_indexes)
+    run_primary_keys_test("operational_presence_vat", expected_primary_keys)
+
+
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
             DBOperationalPresence(
                 resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
                 admin2_ref=2,
-                org_ref=1,
+                org_acronym="ORG01",
+                org_name="Organisation 1",
                 sector_code="SHL",
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
-                source_data="DATA,DATA,DATA",
             )
         ],
         expected_constraint="reference_period",
     )
```

### Comparing `hapi_schema-0.7.4/tests/test_org.py` & `hapi_schema-0.8.0/tests/test_admin1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 from datetime import datetime
 
-from hdx.database.views import build_view
+from hdx.database import Database
 
-from hapi_schema.db_org import DBOrg, view_params_org
+from hapi_schema.db_admin1 import DBAdmin1, view_params_admin1
 
 
-def test_org_view(run_view_test):
-    """Check that org view references org type."""
-    view_org = build_view(view_params_org.__dict__)
+def test_admin1_view(run_view_test):
+    """Check that admin1 view references location."""
+    view_admin1 = Database.prepare_view(view_params_admin1.__dict__)
     run_view_test(
-        view=view_org,
+        view=view_admin1,
         whereclause=(
-            view_org.c.id == 1,
-            view_org.c.org_type_code == "433",
-            view_org.c.org_type_description == "Donor",
+            view_admin1.c.id == 1,
+            view_admin1.c.location_code == "FOO",
         ),
     )
 
 
+def test_admin1_vat(run_indexes_test, run_columns_test):
+    """Check that the admin1 view as table is correct - columns match, expected indexes present"""
+    expected_indexes = [
+        "location_code",
+        "location_name",
+        "reference_period_start",
+        "reference_period_end",
+    ]
+    run_columns_test("admin1_vat", "admin1_view", view_params_admin1)
+    run_indexes_test("admin1_vat", expected_indexes)
+
+
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
-            DBOrg(
-                acronym="ORG04",
-                name="Organisation 4",
-                org_type_code="433",
+            DBAdmin1(
+                location_ref=1,
+                code="FOO-003",
+                name="Province 3",
+                is_unspecified=False,
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
-                hapi_updated_date=datetime(2023, 1, 1),
-                hapi_replaced_date=None,
-            ),
+            )
         ],
         expected_constraint="reference_period",
     )
 
 
-def test_hapi_date_constraint(run_constraints_test):
-    """Check that hapi_replaced_date cannot be less than hapi_udpated_date"""
+def test_code_date_unique(run_constraints_test):
+    """Check that reference_period_start and code must be unique together"""
     run_constraints_test(
         new_rows=[
-            DBOrg(
-                acronym="ORG04",
-                name="Organisation 4",
-                org_type_code="433",
-                reference_period_start=None,
-                reference_period_end=None,
-                hapi_updated_date=datetime(2023, 1, 2),
-                hapi_replaced_date=datetime(2023, 1, 1),
+            DBAdmin1(
+                location_ref=1,
+                code="FOO-003",
+                name="Province 3",
+                is_unspecified=False,
+                reference_period_start=datetime(2023, 1, 1),
+            ),
+            DBAdmin1(
+                location_ref=1,
+                code="FOO-003",
+                name="Province 3",
+                is_unspecified=False,
+                reference_period_start=datetime(2023, 1, 1),
             ),
         ],
-        expected_constraint="hapi_dates",
+        expected_constraint="admin1_code_and_reference_period_unique",
     )
```

### Comparing `hapi_schema-0.7.4/tests/test_patch.py` & `hapi_schema-0.8.0/tests/test_patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sqlalchemy import create_engine
 
 from hapi_schema.utils.base import Base
 
 
 def test_db_patch(capfd):
     engine = create_engine("sqlite://", echo=True)
-    Base.metadata.create_all(engine)
+    Base.metadata.create_all(engine, tables=[Base.metadata.tables["patch"]])
 
     sql_table_creation_code = """CREATE TABLE patch (
         id INTEGER NOT NULL,
         patch_sequence_number INTEGER NOT NULL,
         commit_hash VARCHAR(48) NOT NULL,
         commit_date DATETIME NOT NULL,
         patch_path VARCHAR(512) NOT NULL,
```

### Comparing `hapi_schema-0.7.4/tests/test_population.py` & `hapi_schema-0.8.0/tests/sample_data/data_humanitarian_needs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from datetime import datetime
 
-from hdx.database.views import build_view
-
-from hapi_schema.db_population import DBPopulation, view_params_population
-
-
-def test_population_view(run_view_test):
-    """Check that population references other tables."""
-    view_population = build_view(view_params_population.__dict__)
-    run_view_test(
-        view=view_population,
-        whereclause=(
-            view_population.c.id == 3,
-            view_population.c.dataset_hdx_id
-            == "c3f001fa-b45b-464c-9460-1ca79fd39b40",
-            view_population.c.resource_hdx_id
-            == "90deb235-1bf5-4bae-b231-3393222c2d01",
-            view_population.c.resource_name == "resource-01.csv",
-            view_population.c.admin2_code == "FOO-001-XXX",
-            view_population.c.admin1_code == "FOO-001",
-            view_population.c.location_code == "FOO",
-            view_population.c.gender_code == "f",
-        ),
-    )
-
-
-def test_reference_period_constraint(run_constraints_test):
-    """Check that reference_period_end cannot be less than start"""
-    run_constraints_test(
-        new_rows=[
-            DBPopulation(
-                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-                admin2_ref=1,
-                gender_code=None,
-                age_range_code=None,
-                population=1_000_000,
-                reference_period_start=datetime(2023, 1, 2),
-                reference_period_end=datetime(2023, 1, 1),
-                source_data="DATA,DATA,DATA",
-            )
-        ],
-        expected_constraint="reference_period",
-    )
-
-
-def test_population_positive(run_constraints_test):
-    """Check that the population value is positive"""
-    run_constraints_test(
-        new_rows=[
-            DBPopulation(
-                resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-                admin2_ref=1,
-                gender_code=None,
-                age_range_code=None,
-                population=-1,
-                reference_period_start=None,
-                reference_period_end=None,
-                source_data="DATA,DATA,DATA",
-            ),
-        ],
-        expected_constraint="population",
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

### Comparing `hapi_schema-0.7.4/tests/test_resource.py` & `hapi_schema-0.8.0/tests/sample_data/data_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,37 @@
 from datetime import datetime
 
-from hdx.database.views import build_view
-
-from hapi_schema.db_resource import DBResource, view_params_resource
-
-
-def test_resource_view(run_view_test):
-    """Check that resource references dataset."""
-    view_resource = build_view(view_params_resource.__dict__)
-    run_view_test(
-        view=view_resource,
-        whereclause=(
-            view_resource.c.hdx_id == "90deb235-1bf5-4bae-b231-3393222c2d01",
-            view_resource.c.dataset_hdx_stub == "dataset01",
-        ),
-    )
-
-
-def test_hapi_date_constraint(run_constraints_test):
-    """Check that hapi_replaced_date cannot be less than hapi_updated_date"""
-    run_constraints_test(
-        new_rows=[
-            DBResource(
-                hdx_id="9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f",
-                dataset_hdx_id="7cf3cec8-dbbc-4c96-9762-1464cd0bff75",
-                name="resource-04.csv",
-                format="csv",
-                update_date=datetime(2023, 1, 1),
-                download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f/download/resource-04.csv",
-                is_hxl=True,
-                hapi_updated_date=datetime(2023, 1, 2),
-                hapi_replaced_date=datetime(2023, 1, 1),
-            )
-        ],
-        expected_constraint="hapi_dates",
-    )
-
-    (
-        dict(
-            hdx_id="9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f",
-            dataset_hdx_id="7cf3cec8-dbbc-4c96-9762-1464cd0bff75",
-            name="resource-04.csv",
-            format="csv",
-            update_date=datetime(2023, 1, 1),
-            download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/9d9e07c9-a758-43bd-87dc-5cdd3b3f7e9f/download/resource-04.csv",
-            is_hxl=True,
-            hapi_updated_date=datetime(2023, 8, 1),
-            hapi_replaced_date=None,
-        ),
-    )
+data_resource = [
+    dict(
+        hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
+        dataset_hdx_id="c3f001fa-b45b-464c-9460-1ca79fd39b40",
+        name="resource-01.csv",
+        format="csv",
+        update_date=datetime(2023, 6, 1),
+        download_url="https://data.humdata.org/dataset/c3f001fa-b45b-464c-9460-1ca79fd39b40/resource/90deb235-1bf5-4bae-b231-3393222c2d01/download/resource-01.csv",
+        is_hxl=True,
+        hapi_updated_date=datetime(2023, 6, 1),
+        hapi_replaced_date=None,
+    ),
+    dict(
+        hdx_id="b9e438e0-b68a-49f9-b9a9-68c0f3e93604",
+        dataset_hdx_id="c3f001fa-b45b-464c-9460-1ca79fd39b40",
+        name="resource-02.xlsx",
+        format="xlsx",
+        update_date=datetime(2023, 7, 1),
+        download_url="https://fdw.fews.net/api/tradeflowquantityvaluefacts/?dataset=1845&country=TZ&fields=simple&format=xlsx",
+        is_hxl=True,
+        hapi_updated_date=datetime(2023, 7, 1),
+        hapi_replaced_date=None,
+    ),
+    dict(
+        hdx_id="62ad6e55-5f5d-4494-854c-4110687e9e25",
+        dataset_hdx_id="7cf3cec8-dbbc-4c96-9762-1464cd0bff75",
+        name="resource-03.csv",
+        format="csv",
+        update_date=datetime(2023, 8, 1),
+        download_url="https://data.humdata.org/dataset/7cf3cec8-dbbc-4c96-9762-1464cd0bff75/resource/62ad6e55-5f5d-4494-854c-4110687e9e25/download/resource-03.csv",
+        is_hxl=True,
+        hapi_updated_date=datetime(2023, 8, 1),
+        hapi_replaced_date=None,
+    ),
+]
```

### Comparing `hapi_schema-0.7.4/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.0/tests/sample_data/data_national_risk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from datetime import datetime
 
 data_national_risk = [
     dict(
-        id=1,
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin2_ref=1,
-        risk_class=5,
+        location_ref=1,
+        risk_class="5",
         global_rank=4,
         overall_risk=8.1,
         hazard_exposure_risk=8.7,
         vulnerability_risk=8.5,
         coping_capacity_risk=7.1,
         meta_missing_indicators_pct=8,
         meta_avg_recentness_years=0.26,
         reference_period_start=datetime(2024, 1, 1),
         reference_period_end=datetime(2024, 12, 31),
-        source_data="DATA,DATA,DATA",
     ),
 ]
```

### Comparing `hapi_schema-0.7.4/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.0/tests/sample_data/data_population.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 from datetime import datetime
 
-data_operational_presence = [
+data_population = [
+    # total national
     dict(
-        id=1,
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin2_ref=2,
-        org_ref=1,
-        sector_code="SHL",
-        reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-        source_data="DATA,DATA,DATA",
-    ),
-    dict(
-        id=2,
-        resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin2_ref=4,
-        org_ref=2,
-        sector_code="FSC",
+        admin2_ref=1,
+        gender="*",
+        age_range="*",
+        population=1_000_000,
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-        source_data="DATA,DATA,DATA",
+        reference_period_end=datetime(2023, 6, 30),
     ),
+    # national f, all ages
     dict(
-        id=3,
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin2_ref=4,
-        org_ref=3,
-        sector_code="WSH",
+        admin2_ref=1,
+        gender="f",
+        age_range="*",
+        population=500_000,
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-        source_data="DATA,DATA,DATA",
+        reference_period_end=datetime(2023, 6, 30),
     ),
+    # admin1 f, age 0-4
     dict(
-        id=4,
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin2_ref=6,
-        org_ref=3,
-        sector_code="HEA",
+        admin2_ref=2,
+        gender="f",
+        age_range="0-4",
+        min_age=0,
+        max_age=4,
+        population=5_000,
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-        source_data="DATA,DATA,DATA",
+        reference_period_end=datetime(2023, 6, 30),
     ),
+    # admin2 ages 80+
     dict(
-        id=5,
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin2_ref=1,
-        org_ref=2,
-        sector_code="WSH",
+        admin2_ref=4,
+        gender="*",
+        age_range="80+",
+        min_age=80,
+        population=500,
         reference_period_start=datetime(2023, 1, 1),
-        reference_period_end=None,
-        source_data="DATA,DATA,DATA",
+        reference_period_end=datetime(2023, 6, 30),
     ),
 ]
```

### Comparing `hapi_schema-0.7.4/tests/sample_data/data_patch.py` & `hapi_schema-0.8.0/tests/sample_data/data_patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from datetime import datetime
 
 data_patch = [
     dict(
-        id=1,
         patch_sequence_number=1,
         commit_hash="66e7e589a1224a1832ba7360817dda7a7d9313cf",
         commit_date=datetime(2023, 1, 1),
         patch_path="/2024/01/hapi_patch_1_hno.json",
         patch_target="humanitarian_needs",
         patch_hash="66e7e589a1224a1832ba7360817dda7a7d9313dg",
         patch_permalink_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/66e7e589a1224a1832ba7360817dda7a7d9313cf/2024/01/hapi_patch_1_hno.json",
         state="executed",
         execution_date=datetime(2023, 1, 2),
     ),
     dict(
-        id=2,
         patch_sequence_number=2,
         commit_hash="554f18a92cf6a23a14e0f29356a6dec150f651ff",
         commit_date=datetime(2023, 1, 2),
         patch_path="2024/01/hapi_patch_2_hno.json",
         patch_target="humanitarian_needs",
         patch_hash="554f18a92cf6a23a14e0f29356a6dec150f651gg",
         patch_permalink_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/554f18a92cf6a23a14e0f29356a6dec150f651ff/2024/01/hapi_patch_2_hno.json",
         state="failed",
         execution_date=datetime(2023, 1, 3),
     ),
     dict(
-        id=3,
         patch_sequence_number=3,
         commit_hash="35ea27da009e5add8d8d227e02fd2c4bbcc84b76",
         commit_date=datetime(2023, 1, 3),
         patch_path="2024/01/hapi_patch_3_hno.json",
         patch_target="humanitarian_needs",
         patch_hash="554f18a92cf6a23a14e0f29356a6dec150f65187",
         patch_permalink_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/35ea27da009e5add8d8d227e02fd2c4bbcc84b76/2024/01/hapi_patch_3_hno.json",
```

### Comparing `hapi_schema-0.7.4/.gitignore` & `hapi_schema-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.4/LICENSE` & `hapi_schema-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.4/pyproject.toml` & `hapi_schema-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/OCHA-DAP/hapi-schemas"
 
 [project.optional-dependencies]
-database = ["hdx-python-database>=1.3.0"]
+database = ["hdx-python-database>=1.3.1"]
 dev = ["pre-commit"]
-test = ["hdx-python-database>=1.3.0", "pytest", "pytest-cov"]
+test = ["hdx-python-database>=1.3.1", "psycopg[binary]", "pytest", "pytest-cov"]
 
 #########
 # Hatch #
 #########
 
 # Build
```

### Comparing `hapi_schema-0.7.4/PKG-INFO` & `hapi_schema-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.7.4
+Version: 0.8.0
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
@@ -22,18 +22,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: sqlalchemy
 Provides-Extra: database
-Requires-Dist: hdx-python-database>=1.3.0; extra == 'database'
+Requires-Dist: hdx-python-database>=1.3.1; extra == 'database'
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: hdx-python-database>=1.3.0; extra == 'test'
+Requires-Dist: hdx-python-database>=1.3.1; extra == 'test'
+Requires-Dist: psycopg[binary]; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # hapi-sqlalchemy-schema
 Schema for HAPI database in SQLAlchemy
```

