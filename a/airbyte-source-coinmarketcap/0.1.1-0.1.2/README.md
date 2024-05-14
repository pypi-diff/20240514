# Comparing `tmp/airbyte-source-coinmarketcap-0.1.1.tar.gz` & `tmp/airbyte_source_coinmarketcap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-coinmarketcap-0.1.1.tar", last modified: Tue Jan 30 14:33:03 2024, max compression
+gzip compressed data, was "airbyte_source_coinmarketcap-0.1.2.tar", max compression
```

## Comparing `airbyte-source-coinmarketcap-0.1.1.tar` & `airbyte_source_coinmarketcap-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:33:03.730812 airbyte-source-coinmarketcap-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     4294 2024-01-30 14:33:03.730812 airbyte-source-coinmarketcap-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4105 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:33:03.730812 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4294 2024-01-30 14:33:03.000000 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      889 2024-01-30 14:33:03.000000 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 14:33:03.000000 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-01-30 14:33:03.000000 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-30 14:33:03.000000 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-01-30 14:33:03.000000 airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:33:03.730812 airbyte-source-coinmarketcap-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       59 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      111 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     4151 2024-01-30 14:33:03.734812 airbyte-source-coinmarketcap-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      942 2024-01-30 14:33:01.000000 airbyte-source-coinmarketcap-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:33:03.730812 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2190 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      251 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:33:03.730812 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/schemas/
--rw-r--r--   0 root         (0) root         (0)      758 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/schemas/categories.json
--rw-r--r--   0 root         (0) root         (0)      463 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/schemas/exchange.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/schemas/fiat.json
--rw-r--r--   0 root         (0) root         (0)     1188 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/schemas/listing.json
--rw-r--r--   0 root         (0) root         (0)       99 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/schemas/quotes.json
--rw-r--r--   0 root         (0) root         (0)      482 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/source.py
--rw-r--r--   0 root         (0) root         (0)     1206 2024-01-30 14:29:13.000000 airbyte-source-coinmarketcap-0.1.1/source_coinmarketcap/spec.yaml
+-rw-r--r--   0        0        0     4639 2024-05-14 00:02:41.000000 airbyte_source_coinmarketcap-0.1.2/README.md
+-rw-r--r--   0        0        0      141 2024-05-14 00:02:41.000000 airbyte_source_coinmarketcap-0.1.2/main.py
+-rw-r--r--   0        0        0      797 2024-05-14 00:53:34.912860 airbyte_source_coinmarketcap-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-14 00:02:41.000000 airbyte_source_coinmarketcap-0.1.2/source_coinmarketcap/__init__.py
+-rw-r--r--   0        0        0     9860 2024-05-14 00:02:41.000000 airbyte_source_coinmarketcap-0.1.2/source_coinmarketcap/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-14 00:02:41.000000 airbyte_source_coinmarketcap-0.1.2/source_coinmarketcap/run.py
+-rw-r--r--   0        0        0      482 2024-05-14 00:02:41.000000 airbyte_source_coinmarketcap-0.1.2/source_coinmarketcap/source.py
+-rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 airbyte_source_coinmarketcap-0.1.2/PKG-INFO
```

### Comparing `airbyte-source-coinmarketcap-0.1.1/PKG-INFO` & `airbyte_source_coinmarketcap-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,103 @@
-Metadata-Version: 2.1
-Name: airbyte-source-coinmarketcap
-Version: 0.1.1
-Summary: Source implementation for Coinmarketcap.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-
 # Coinmarketcap Source
 
 This is the repository for the Coinmarketcap configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/coinmarketcap).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/coinmarketcap).
+
+## Local development
+
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/coinmarketcap)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_coinmarketcap/spec.yaml` file.
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/coinmarketcap)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `src/source_coinmarketcap/manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source coinmarketcap test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 
+```
+poetry run source-coinmarketcap spec
+poetry run source-coinmarketcap check --config secrets/config.json
+poetry run source-coinmarketcap discover --config secrets/config.json
+poetry run source-coinmarketcap read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-coinmarketcap build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-coinmarketcap:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-coinmarketcap:dev .
+airbyte-ci connectors --name=source-coinmarketcap build
 ```
 
+An image will be available on your host with the tag `airbyte/source-coinmarketcap:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-coinmarketcap:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coinmarketcap:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coinmarketcap:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-coinmarketcap:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-coinmarketcap test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-coinmarketcap test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/coinmarketcap.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/coinmarketcap.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-coinmarketcap-0.1.1/airbyte_source_coinmarketcap.egg-info/PKG-INFO` & `airbyte_source_coinmarketcap-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-coinmarketcap
-Version: 0.1.1
-Summary: Source implementation for Coinmarketcap.
+Version: 0.1.2
+Summary: Source implementation for coinmarketcap.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/coinmarketcap
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Coinmarketcap Source
 
 This is the repository for the Coinmarketcap configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/coinmarketcap).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/coinmarketcap).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/coinmarketcap)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_coinmarketcap/spec.yaml` file.
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/coinmarketcap)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `src/source_coinmarketcap/manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source coinmarketcap test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 
+```
+poetry run source-coinmarketcap spec
+poetry run source-coinmarketcap check --config secrets/config.json
+poetry run source-coinmarketcap discover --config secrets/config.json
+poetry run source-coinmarketcap read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-coinmarketcap build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-coinmarketcap:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-coinmarketcap:dev .
+airbyte-ci connectors --name=source-coinmarketcap build
 ```
 
+An image will be available on your host with the tag `airbyte/source-coinmarketcap:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-coinmarketcap:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coinmarketcap:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coinmarketcap:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-coinmarketcap:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-coinmarketcap test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-coinmarketcap test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/coinmarketcap.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/coinmarketcap.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

