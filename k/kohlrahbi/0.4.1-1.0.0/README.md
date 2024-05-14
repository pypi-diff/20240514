# Comparing `tmp/kohlrahbi-0.4.1.tar.gz` & `tmp/kohlrahbi-1.0.0.tar.gz`

## Comparing `kohlrahbi-0.4.1.tar` & `kohlrahbi-1.0.0.tar`

### file list

```diff
@@ -1,66 +1,75 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/README.md
--rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/kohlrahbi-image.png
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/requirements.in
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/requirements.txt
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/docxfilefinder.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/table_header.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/changehistory/changehistorytable.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
--rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
--rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
--rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
--rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/scrape_pruefis/collect_pruefis.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    21329 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/LICENSE
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8800 2020-02-02 00:00:00.000000 kohlrahbi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.gitattributes
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/README.md
+-rw-r--r--   0        0        0   202926 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/kohlrahbi-image.png
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/requirements.txt
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/tox.ini
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/wip.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxfilefinder.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0    11369 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/table_header.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/version.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahb/command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/__init__.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbcondtions.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbpackagetable.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbsubtable.py
+-rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtable.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtablerow.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/changehistory/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/changehistory/changehistorytable.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/changehistory/command.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/conditions/__init__.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/conditions/command.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/ahbexportfileformat.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2104_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2110_all_known_pruefis.toml
+-rw-r--r--   0        0        0    50700 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml
+-rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml
+-rw-r--r--   0        0        0    65727 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml
+-rw-r--r--   0        0        0    36218 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2410_all_known_pruefis.toml
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    19261 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 kohlrahbi-1.0.0/PKG-INFO
```

### Comparing `kohlrahbi-0.4.1/.pre-commit-config.yaml` & `kohlrahbi-1.0.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+exclude: '.*\.csv$'
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
```

### Comparing `kohlrahbi-0.4.1/kohlrahbi-image.png` & `kohlrahbi-1.0.0/kohlrahbi-image.png`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/requirements.txt` & `kohlrahbi-1.0.0/dev_requirements/requirements-type_check.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,49 @@
+# SHA1:192c47d357926822155fd77ec6f38ea760b815d3
 #
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
+# This file is autogenerated by pip-compile-multi
+# To update, run:
 #
-#    pip-compile requirements.in
+#    pip-compile-multi
 #
-attrs==23.2.0
-    # via
-    #   -r requirements.in
-    #   maus
-click==8.1.7
-    # via -r requirements.in
-colorama==0.4.6
-    # via
-    #   click
-    #   colorlog
-colorlog==6.8.2
-    # via -r requirements.in
-et-xmlfile==1.1.0
-    # via openpyxl
-lxml==5.1.0
-    # via python-docx
-marshmallow==3.21.1
-    # via maus
-maus==0.4.2
-    # via -r requirements.in
-more-itertools==10.2.0
-    # via maus
+iniconfig==2.0.0
+    # via pytest
+mypy==1.10.0
+    # via -r dev_requirements/requirements-type_check.in
+mypy-extensions==1.0.0
+    # via mypy
+networkx==3.3
+    # via networkx-stubs
+networkx-stubs==0.0.1
+    # via -r dev_requirements/requirements-type_check.in
 numpy==1.26.4
-    # via pandas
-openpyxl==3.1.2
-    # via -r requirements.in
+    # via
+    #   pandas
+    #   pandas-stubs
 packaging==24.0
-    # via marshmallow
-pandas==2.2.1
-    # via -r requirements.in
+    # via pytest
+pandas==2.2.2
+    # via -r dev_requirements/requirements-type_check.in
+pandas-stubs==2.2.1.240316
+    # via -r dev_requirements/requirements-type_check.in
+pluggy==1.5.0
+    # via pytest
+pytest==8.2.0
+    # via -r dev_requirements/requirements-type_check.in
 python-dateutil==2.9.0.post0
     # via pandas
-python-docx==1.1.0
-    # via -r requirements.in
 pytz==2024.1
     # via pandas
 six==1.16.0
     # via python-dateutil
-tomlkit==0.12.4
-    # via -r requirements.in
-typing-extensions==4.10.0
-    # via python-docx
+types-freezegun==1.1.10
+    # via -r dev_requirements/requirements-type_check.in
+types-pytz==2024.1.0.20240417
+    # via pandas-stubs
+types-requests==2.31.0.20240406
+    # via -r dev_requirements/requirements-type_check.in
+typing-extensions==4.11.0
+    # via mypy
 tzdata==2024.1
     # via pandas
-xlsxwriter==3.2.0
-    # via -r requirements.in
+urllib3==2.2.1
+    # via types-requests
```

### Comparing `kohlrahbi-0.4.1/tox.ini` & `kohlrahbi-1.0.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # the linting environment is called by the Github Action that runs the linter
 deps =
     -rrequirements.txt
     -r dev_requirements/requirements-linting.txt
 setenv = PYTHONPATH = {toxinidir}/src
 # add your fixtures like e.g. pytest_datafiles here
 commands =
-    pylint kohlrahbi
+    pylint kohlrahbi --ignore=version.py
 
 [testenv:type_check]
 # the type_check environment checks the type hints using mypy
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
     -rrequirements.txt
      -r dev_requirements/requirements-type_check.txt
@@ -60,17 +60,17 @@
     {[testenv:linting]deps}
     {[testenv:coverage]deps}
     -r dev_requirements/requirements-formatting.txt
     pip-tools
     pre-commit
 commands =
     python -m pip install --upgrade pip
-    # pip-compile requirements.in
+    pip-compile pyproject.toml
     pip install -r requirements.txt
-    # pre-commit install
+    pre-commit install
 
 [testenv:test_packaging]
 skip_install = true
 deps =
     -r dev_requirements/requirements-test_packaging.txt
 commands =
     python -m build
```

### Comparing `kohlrahbi-0.4.1/.github/dependabot.yml` & `kohlrahbi-1.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/coverage.yml` & `kohlrahbi-1.0.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/dependabot_automerge.yml` & `kohlrahbi-1.0.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/formatting.yml` & `kohlrahbi-1.0.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/packaging_test.yml` & `kohlrahbi-1.0.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/python-publish.yml` & `kohlrahbi-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/pythonlint.yml` & `kohlrahbi-1.0.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/.github/workflows/unittests.yml` & `kohlrahbi-1.0.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/dev_requirements/requirements-test_packaging.txt` & `kohlrahbi-1.0.0/dev_requirements/requirements-test_packaging.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # SHA1:93e4fbf2b6cce1574fe3d5315360512fa9927699
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-build==1.1.1
-    # via -r dev_requirements\requirements-test_packaging.in
+backports-tarfile==1.1.0
+    # via jaraco-context
+build==1.2.1
+    # via -r dev_requirements/requirements-test_packaging.in
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-colorama==0.4.6
-    # via build
-docutils==0.20.1
+docutils==0.21.1
     # via readme-renderer
-idna==3.6
+idna==3.7
     # via requests
 importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
     # via keyring
-jaraco-context==4.3.0
+jaraco-context==5.3.0
     # via keyring
-jaraco-functools==4.0.0
+jaraco-functools==4.0.1
     # via keyring
-keyring==25.0.0
+keyring==25.1.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
     # via
@@ -45,29 +45,27 @@
     # via twine
 pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-pywin32-ctypes==0.2.2
-    # via keyring
 readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
     # via twine
 twine==5.0.0
-    # via -r dev_requirements\requirements-test_packaging.in
+    # via -r dev_requirements/requirements-test_packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/docxfilefinder.py` & `kohlrahbi-1.0.0/src/kohlrahbi/docxfilefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 This module contains the DocxFileFinder class.
 """
 
 from itertools import groupby
 from pathlib import Path
 
-import attrs
 from maus.edifact import EdifactFormat, get_format_of_pruefidentifikator
+from pydantic import BaseModel
 
 from kohlrahbi.logger import logger
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class DocxFileFinder:
+class DocxFileFinder(BaseModel):
     """
     This class is responsible for finding the docx files in the input directory.
     It can find MIG and AHB docx files.
     """
 
     paths_to_docx_files: list[Path]
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-1.0.0/src/kohlrahbi/row_type_checker.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/seed.py` & `kohlrahbi-1.0.0/src/kohlrahbi/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 This module provides a class to collect information which of need for all parsing functions
 """
 
-from attrs import define
 from docx.table import Table  # type:ignore[import]
+from pydantic import BaseModel
 
 from kohlrahbi.enums import RowType
 from kohlrahbi.table_header import PruefiMetaData, TableHeader, get_tabstop_positions
 
 
 # pylint: disable=too-few-public-methods
-@define
-class Seed:
+class Seed(BaseModel):
     """
     helper class to store all values to extract the AHB and the final AHB as dataframe
     """
 
     pruefidentifikatoren: list[str] = []
     column_headers: list[str] = []
     edifact_struktur_left_indent_position: int = 0
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/table_header.py` & `kohlrahbi-1.0.0/src/kohlrahbi/table_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This module contains the TableHeader class.
 """
 
 from enum import StrEnum
 from typing import Dict, List, Mapping, cast
 
-from attrs import define
 from docx.table import _Cell  # type:ignore[import]
 from docx.text.paragraph import Paragraph  # type:ignore[import]
 from more_itertools import first, last
+from pydantic import BaseModel
 
 
 class HeaderSection(StrEnum):
     """
     Enum for the different sections of the table header
     """
 
@@ -71,27 +71,27 @@
 
         mapping[current_tabstop_positions[i]] = initial_tabstop_positions[min_j]
 
     return mapping
 
 
 # pylint: disable=too-few-public-methods
-@define
-class PruefiMetaData:
+
+
+class PruefiMetaData(BaseModel):
     """
     This class contains the information about the Prüfidentifikatoren
     """
 
     pruefidentifikator: str
     name: str
     communication_direction: str
 
 
-@define
-class TableHeader:
+class TableHeader(BaseModel):
     """
     Class for the table header.
     It contains the information about the Prüfidentifikatoren.
     """
 
     pruefi_meta_data: List[PruefiMetaData] = []
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbsubtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 This module contains the AhbSubTable class.
 """
 
 from typing import Generator
 
-import attrs
 import pandas as pd
 from docx.table import Table as DocxTable  # type:ignore[import]
 from docx.table import _Cell  # type:ignore[import]
+from pydantic import BaseModel, ConfigDict
 
-from kohlrahbi.ahb.ahbtablerow import AhbTableRow
+from kohlrahbi.ahbtable.ahbtablerow import AhbTableRow
 from kohlrahbi.row_type_checker import RowType, get_row_type
 from kohlrahbi.seed import Seed
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class AhbSubTable:
+class AhbSubTable(BaseModel):
     """
     The AHB table for one Pruefidentifikator is separated into small sub tables.
     This class contains the information from such a sub table.
     """
 
     table_meta_data: Seed
     table: pd.DataFrame
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     @staticmethod
     def _parse_docx_table(
         table_meta_data: Seed, ahb_table_dataframe: pd.DataFrame, docx_table: DocxTable
     ) -> pd.DataFrame:
         for row in docx_table.rows:
-            sanitized_cells = list(AhbSubTable._iter_visible_cells(row=row))
+            sanitized_cells = list(AhbSubTable.iter_visible_cells(row=row))
 
             current_edifact_struktur_cell = sanitized_cells[0]
 
             # check for row type
             current_row_type = get_row_type(
                 edifact_struktur_cell=current_edifact_struktur_cell,
                 left_indent_position=table_meta_data.edifact_struktur_left_indent_position,
@@ -117,15 +118,15 @@
             ahb_table_dataframe=ahb_table_dataframe,
             docx_table=docx_table,
         )
 
         return cls(table_meta_data=tmd, table=ahb_table_dataframe)
 
     @staticmethod
-    def _iter_visible_cells(row) -> Generator[_Cell, None, None]:
+    def iter_visible_cells(row) -> Generator[_Cell, None, None]:
         """
         This function makes sure that you will iterate over the cells you see in the word document.
         For more information go to https://github.com/python-openxml/python-docx/issues/970#issuecomment-877386927
         """
         table_row = row._tr  # pylint:disable=protected-access
         for table_column in table_row.tc_lst:
             yield _Cell(table_column, row.table)
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 This module provides the AhbTable class
 """
 
 from pathlib import Path
 from typing import Union
 
-import attrs
 import pandas as pd
 from maus.edifact import get_format_of_pruefidentifikator
 from more_itertools import peekable
+from pydantic import BaseModel, ConfigDict
 
-from kohlrahbi.ahb.ahbsubtable import AhbSubTable
+from kohlrahbi.ahbtable.ahbsubtable import AhbSubTable
 from kohlrahbi.logger import logger
 from kohlrahbi.table_header import PruefiMetaData
 
 _column_letter_width_mapping: dict[str, Union[float, int]] = {
     "A": 3.5,
     "B": 47,
     "C": 9,
@@ -22,23 +22,24 @@
     "E": 39,
     "F": 33,
     "G": 18,
     "H": 102,
 }
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class AhbTable:
+class AhbTable(BaseModel):
     """
     This class contains the AHB table as you see it in the AHB documents, but in a machine readable format.
     """
 
     table: pd.DataFrame
     metadata: list[PruefiMetaData] = []
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def fill_segment_gruppe_segment_dataelement(self) -> None:
         """
         For easier readability this functions adds the segment
 
         before
         ======
 
@@ -166,15 +167,15 @@
 
         self.fill_segment_gruppe_segment_dataelement()
 
         columns_to_export = list(self.table.columns)[:5] + [pruefi]
         columns_to_export.append("Bedingung")
         df_to_export = self.table[columns_to_export]
 
-        df_to_export.to_csv(csv_output_directory_path / f"{pruefi}.csv")
+        df_to_export.to_csv(csv_output_directory_path / f"{pruefi}.csv", encoding="utf-8")
         logger.info("The csv file for %s is saved at %s", pruefi, csv_output_directory_path / f"{pruefi}.csv")
 
     # pylint: disable=too-many-locals
     def to_xlsx(self, pruefi: str, path_to_output_directory: Path) -> None:
         """
         Dump a AHB table of a given pruefi into an excel file.
         The excel file will be saved in the following directory structure:
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-1.0.0/src/kohlrahbi/ahbtable/ahbtablerow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 This module contains the class AhbTableRow
 """
 
 from typing import Optional
 
 import pandas as pd
-from attrs import define, field, validators
 from docx.table import _Cell  # type:ignore[import]
+from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.docxtablecells import BedingungCell, BodyCell, EdifactStrukturCell
 from kohlrahbi.row_type_checker import RowType
 from kohlrahbi.seed import Seed
 
 
 # pylint:disable=too-few-public-methods
-@define(auto_attribs=True, kw_only=True)
-class AhbTableRow:
+class AhbTableRow(BaseModel):
     """
     A AhbTableRow is a single row from an AHB table.
     It contains a seed and the three cells (columns).
     """
 
-    seed: Seed = field(validator=validators.instance_of(Seed))
-    edifact_struktur_cell: _Cell = field(validator=validators.instance_of(_Cell))
-    middle_cell: _Cell = field(validator=validators.instance_of(_Cell))
-    bedingung_cell: _Cell = field(validator=validators.instance_of(_Cell))
+    seed: Seed
+    edifact_struktur_cell: _Cell
+    middle_cell: _Cell
+    bedingung_cell: _Cell
+
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def parse(
         self,
         row_type: RowType,
     ) -> Optional[pd.DataFrame]:
         """
         Writes the current row of the current table into the DataFrame depending on the type of the row.
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/changehistory/changehistorytable.py` & `kohlrahbi-1.0.0/src/kohlrahbi/changehistory/changehistorytable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 This module provides the ChangeHistoryTable class
 """
 
-import attrs
 import pandas as pd
 from docx.table import Table  # type:ignore[import]
+from pydantic import BaseModel, ConfigDict
 
-from kohlrahbi.ahb.ahbsubtable import AhbSubTable
+from kohlrahbi.ahbtable.ahbsubtable import AhbSubTable
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class ChangeHistoryTable:
+class ChangeHistoryTable(BaseModel):
     """
     This class  contains the change history table.
     """
 
     table: pd.DataFrame
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     @classmethod
     def from_docx_change_history_table(cls, docx_table: Table) -> "ChangeHistoryTable":
         """
         Create a ChangeHistorySubTable object from a change history table.
         """
 
         change_history_rows: list[list[str]] = []
 
         for row in docx_table.rows:
-            sanitized_cells = list(AhbSubTable._iter_visible_cells(row=row))
+            sanitized_cells = list(AhbSubTable.iter_visible_cells(row=row))
 
             is_header_row = sanitized_cells[0].text == "Änd-ID" or sanitized_cells[2].text == "Bisher"
             if is_header_row:
                 continue
-            else:
-                change_history_rows.append([cell.text for cell in sanitized_cells])
+            change_history_rows.append([cell.text for cell in sanitized_cells])
 
         headers = ["Änd-ID", "Ort", "Änderungen Bisher", "Änderungen Neu", "Grund der Anpassung", "Status"]
 
         df = pd.DataFrame(change_history_rows, columns=headers)
 
         return cls(table=df)
 
@@ -73,9 +73,7 @@
                             str(self.table.iloc[i - 1, col]) + " " + str(self.table.iloc[i, col]).strip()
                         )
                 # Drop the current row since it has been merged
                 self.table.drop(i, inplace=True)
 
         # Reset index after dropping rows
         self.table.reset_index(drop=True, inplace=True)
-
-        return None
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 This module contains the class BedingungCell
 """
 
 import re
 
-import attrs
 import pandas as pd
 from docx.table import _Cell  # type:ignore[import]
+from pydantic import BaseModel, ConfigDict
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class BedingungCell:
+class BedingungCell(BaseModel):
     """
     BedingungCell contains all information and a method
     to extract the Bedingungen of an AHB Bedingung cell.
     """
 
     table_cell: _Cell
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def parse(self, ahb_row_dataframe: pd.DataFrame) -> pd.DataFrame:
         """
         Parses a cell in the Bedingung column and puts the information into the appropriate column of the dataframe.
         """
 
         bedingung = self.beautify_bedingungen()
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 This module contains the class BodyCell
 """
 
-import attrs
 import pandas as pd
 from docx.table import _Cell  # type:ignore[import]
 from maus.reader.flat_ahb_reader import FlatAhbCsvReader
+from pydantic import BaseModel, ConfigDict
 
 from kohlrahbi.table_header import get_tabstop_positions
 
 INDEX_OF_CODES_AND_QUALIFIER_COLUMN = 3
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class BodyCell:
+class BodyCell(BaseModel):
     """
     BodyCell contains all information and a method
     to extract dataelement/qualifier, the name of the dataelement
     as well as the conditions for each Prüfidentifikator.
     """
 
     table_cell: _Cell
     left_indent_position: int
     indicator_tabstop_positions: list[int]
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     # I see why pylint is not happy about this many branches, but at the moment I have no clue how to avoid them.
     # pylint: disable=too-many-branches
     def parse(self, ahb_row_dataframe: pd.DataFrame) -> pd.DataFrame:
         """Parses a paragraph in the middle column and puts the information into the appropriate columns
 
         Args:
             paragraph (Paragraph): Current paragraph in the edifact struktur cell
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-1.0.0/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 This module contains the class EdifactStrukturCell
 """
 
 import re
 
-import attrs
 import pandas as pd
 from docx.table import _Cell  # type:ignore[import]
+from pydantic import BaseModel, ConfigDict
 
 _segment_group_pattern = re.compile(r"^SG\d+$")
 _segment_pattern = re.compile(r"^[A-Z]{3}$")
 
 
 # pylint: disable=too-few-public-methods
-@attrs.define(auto_attribs=True, kw_only=True)
-class EdifactStrukturCell:
+class EdifactStrukturCell(BaseModel):
     """
     EdifactStrukturCell contains all information and a method
     to extract the segment name, segment group, segment and data element.
     """
 
     table_cell: _Cell
     edifact_struktur_cell_left_indent_position: int
 
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     def parse(self, ahb_row_dataframe: pd.DataFrame) -> pd.DataFrame:
         """Parses a paragraph in the edifact struktur column and puts the information into the appropriate columns
 
         Args:
             table_cell (Cell): edifact struktur cell
             dataframe (pd.DataFrame): Contains all infos
             row_index (int): Current index of the DataFrame
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-1.0.0/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml` & `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2210_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml` & `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2304_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml` & `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2310_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml` & `kohlrahbi-1.0.0/src/kohlrahbi/format_versions/FV2404_all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 This module contains the UnfoldedAhbLine class.
 """
 
-from attrs import define
+from pydantic import BaseModel
 
 
 # pylint: disable=too-few-public-methods
-@define(auto_attribs=True, kw_only=True)
-class UnfoldedAhbLine:
+class UnfoldedAhbLine(BaseModel):
     """
     This class represents one unfolded line of the AHB.
     Unfolded means that we separate segment_name and segment_gruppe as well as code and qualifier
 
     Example:
 
     AhbLine(
```

### Comparing `kohlrahbi-0.4.1/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-1.0.0/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 import copy
 import json
 import re
 from pathlib import Path
 from uuid import uuid4
 
-import attrs
 import pandas as pd
 from maus.edifact import get_format_of_pruefidentifikator
 from maus.models.anwendungshandbuch import (
     AhbLine,
     AhbMetaInformation,
     FlatAnwendungshandbuch,
     FlatAnwendungshandbuchSchema,
 )
 from maus.reader.flat_ahb_reader import FlatAhbCsvReader
 from more_itertools import first_true, peekable
+from pydantic import BaseModel
 
-from kohlrahbi.ahb.ahbtable import AhbTable, _column_letter_width_mapping
+from kohlrahbi.ahbtable.ahbtable import AhbTable, _column_letter_width_mapping
 from kohlrahbi.logger import logger
 from kohlrahbi.unfoldedahb.unfoldedahbline import UnfoldedAhbLine
 from kohlrahbi.unfoldedahb.unfoldedahbtablemetadata import UnfoldedAhbTableMetaData
 
 _segment_group_pattern = re.compile(r"^SG\d+$")
 
 
@@ -56,26 +56,23 @@
                 ),
             ):
                 updated_ahb.lines[update_index].guid = existing_line_match.guid
                 # if we found a line match, we can start the next search at the next line in the next loop iteration
                 existing_ahb_search_start_index = existing_ahb.lines.index(existing_line_match) + 1
 
 
-@attrs.define(auto_attribs=True, kw_only=True)
-class UnfoldedAhb:
+class UnfoldedAhb(BaseModel):
     """
     The UnfoldedAhb contains one Prüfidentifikator.
     Some columns in the AHB documents contain multiple information in one column e.g. Segmentname and Segmentgruppe.
     The unfolded classes add new columns/attribues to avoid the duplication of information in one column.
     """
 
     meta_data: UnfoldedAhbTableMetaData
-    unfolded_ahb_lines: list[UnfoldedAhbLine] = attrs.field(
-        validator=attrs.validators.deep_iterable(member_validator=attrs.validators.instance_of(UnfoldedAhbLine))
-    )
+    unfolded_ahb_lines: list[UnfoldedAhbLine]
 
     @classmethod
     def from_ahb_table(cls, ahb_table: AhbTable, pruefi: str):
         """
         This function creates an UnfoldedAhb from an AhbTable.
         """
         unfolded_ahb_lines: list[UnfoldedAhbLine] = []
@@ -412,15 +409,15 @@
         if edifact_format is None:
             logger.warning("'%s' is not a pruefidentifikator", self.meta_data.pruefidentifikator)
             return
 
         csv_output_directory_path = path_to_output_directory / str(edifact_format) / "csv"
         csv_output_directory_path.mkdir(parents=True, exist_ok=True)
 
-        df.to_csv(csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv")
+        df.to_csv(csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv", encoding="utf-8")
         logger.info(
             "The csv file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv",
         )
         del df
 
@@ -455,45 +452,7 @@
             logger.error("The Excel file %s is open. Please close this file and try again.", excel_file_name)
 
         logger.info(
             "The xlsx file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             xlsx_output_directory_path / f"{self.meta_data.pruefidentifikator}.json",
         )
-
-    def collect_condition(self, already_known_conditions: dict) -> None:
-        """
-        Collect conditions of UnfoldedAHB in dict if they are not known yet.
-        """
-        df = self.convert_to_dataframe()
-
-        edifact_format = get_format_of_pruefidentifikator(self.meta_data.pruefidentifikator)
-        if edifact_format is None:
-            logger.warning("'%s' is not a pruefidentifikator", self.meta_data.pruefidentifikator)
-            return
-        if already_known_conditions.get(edifact_format) is None:
-            already_known_conditions[edifact_format] = {}
-        # check if there are conditions:
-        there_are_conditions = (df["Bedingung"] != "").any()
-        if there_are_conditions:
-            for conditions_text in df["Bedingung"][df["Bedingung"] != ""]:
-                # Split the input into parts enclosed in square brackets and other parts
-                matches = re.findall(
-                    r"\[(\d+)](.*?)(?=\[\d+]|$)",
-                    conditions_text,
-                    re.DOTALL,
-                )
-                for match in matches:
-                    # make text prettier:
-                    text = match[1].strip()
-                    text = re.sub(r"\s+", " ", text)
-                    # check whether condition was already collected:
-                    condition_key_not_collected_yet = already_known_conditions[edifact_format].get(match[0]) is None
-                    if not condition_key_not_collected_yet:
-                        key_exits_but_shorter_text = len(text) > len(
-                            already_known_conditions[edifact_format].get(match[0])
-                        )
-                    if condition_key_not_collected_yet or key_exits_but_shorter_text:
-                        already_known_conditions[edifact_format][match[0]] = text
-
-        logger.info("The conditions for %s were collected", self.meta_data.pruefidentifikator)
-        del df
```

### Comparing `kohlrahbi-0.4.1/.gitignore` & `kohlrahbi-1.0.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -164,21 +164,28 @@
 .vscode/
 
 # document folders
 documents/
 backup_documents/
 
 # output files
+output/
+src/kohlrahbi/cache/
 *.xlsx
 *.csv
 *.json
 *.7z
 
+#however include
+!unittests/test-edi-energy-mirror-repo/edi_energy_de/*/expected-output/**/*.xlsx
+!unittests/test-edi-energy-mirror-repo/edi_energy_de/*/expected-output/**/*.csv
+!unittests/test-edi-energy-mirror-repo/edi_energy_de/*/expected-output/**/*.json
+
 # Word temporary
 ~$*.doc*
 
 # Word Auto Backup File
 Backup of *.doc*
 
 # version number for kohlrahbi; gets auto-generated during the command
 # python -m build
-_kohlrahbi_version.py
+src/kohlrahbi/version.py
```

### Comparing `kohlrahbi-0.4.1/LICENSE` & `kohlrahbi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.4.1/pyproject.toml` & `kohlrahbi-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,26 @@
 # Build system information and other project-specific configuration below.
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
+dependencies = [
+  "click>=8.0.0",
+  "colorlog>=6.7.0",
+  "maus>=0.3.43",
+  "openpyxl>=3.1.1",
+  "pandas>=1.5.3",
+  "python-docx>=1.0.0",
+  "pytz>=2022.7.1",
+  "pydantic>=2.6.0",
+  "tomlkit>=0.11.6",
+  "xlsxwriter>=3.0.8",
+]
 name = "kohlrahbi"
 description = "Tool to generate machine readable files from AHB documents"
 license = { text = "GPL" }
 requires-python = ">=3.11"
 authors = [{ name = "Kevin Krechan", email = "kevin.krechan@hochfrequenz.de" }]
 keywords = ["automation", "ahb", "bdew", "edi@energy"]
 classifiers = [
@@ -23,48 +35,33 @@
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-dependencies = [
-  "attrs>=22.2.0",
-  "click>=8.0.0",
-  "colorlog>=6.7.0",
-  "maus>=0.3.43",
-  "openpyxl>=3.1.1",
-  "pandas>=1.5.3",
-  "python-docx>=1.0.0",
-  "pytz>=2022.7.1",
-  "tomlkit>=0.11.6",
-  "xlsxwriter>=3.0.8",
-]
 dynamic = ["readme", "version"]
 
 [project.scripts]
-kohlrahbi = "kohlrahbi:main"
+kohlrahbi = "kohlrahbi:cli"
 
 
 [project.urls]
 Changelog = "https://github.com/Hochfrequenz/kohlrahbi/releases"
 Homepage = "https://github.com/Hochfrequenz/kohlrahbi"
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 fragments = [{ path = "README.md" }]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
-version-file = "src/_kohlrahbi_version.py"
-template = '''
-version = "{version}"
-'''
+version-file = "src/kohlrahbi/version.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/unittests"]
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src"]
 sources = ["src"]
```

