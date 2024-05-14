# Comparing `tmp/airbyte-source-aha-0.3.1.tar.gz` & `tmp/airbyte_source_aha-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-aha-0.3.1.tar", last modified: Tue Jan 30 13:24:02 2024, max compression
+gzip compressed data, was "airbyte_source_aha-0.3.2.tar", max compression
```

## Comparing `airbyte-source-aha-0.3.1.tar` & `airbyte_source_aha-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:24:02.879607 airbyte-source-aha-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     4109 2024-01-30 13:24:02.879607 airbyte-source-aha-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3945 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:24:02.875607 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4109 2024-01-30 13:24:02.000000 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      883 2024-01-30 13:24:02.000000 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 13:24:02.000000 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-01-30 13:24:02.000000 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-30 13:24:02.000000 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-30 13:24:02.000000 airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:24:02.871607 airbyte-source-aha-0.3.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      106 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     3981 2024-01-30 13:24:02.879607 airbyte-source-aha-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      907 2024-01-30 13:24:00.000000 airbyte-source-aha-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:24:02.875607 airbyte-source-aha-0.3.1/source_aha/
--rw-r--r--   0 root         (0) root         (0)      118 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3263 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      221 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:24:02.875607 airbyte-source-aha-0.3.1/source_aha/schemas/
--rw-r--r--   0 root         (0) root         (0)      533 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/features.json
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/goals.json
--rw-r--r--   0 root         (0) root         (0)      326 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/idea_categories.json
--rw-r--r--   0 root         (0) root         (0)     2512 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/idea_comments.json
--rw-r--r--   0 root         (0) root         (0)     2081 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/idea_endorsements.json
--rw-r--r--   0 root         (0) root         (0)     1332 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/ideas.json
--rw-r--r--   0 root         (0) root         (0)      492 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/products.json
--rw-r--r--   0 root         (0) root         (0)      855 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/source.py
--rw-r--r--   0 root         (0) root         (0)      453 2024-01-30 13:02:18.000000 airbyte-source-aha-0.3.1/source_aha/spec.yaml
+-rw-r--r--   0        0        0     4441 2024-05-14 20:00:56.000000 airbyte_source_aha-0.3.2/README.md
+-rw-r--r--   0        0        0      131 2024-05-14 20:00:56.000000 airbyte_source_aha-0.3.2/main.py
+-rw-r--r--   0        0        0      737 2024-05-14 20:29:42.869483 airbyte_source_aha-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-14 20:00:56.000000 airbyte_source_aha-0.3.2/source_aha/__init__.py
+-rw-r--r--   0        0        0    21648 2024-05-14 20:00:56.000000 airbyte_source_aha-0.3.2/source_aha/manifest.yaml
+-rw-r--r--   0        0        0      219 2024-05-14 20:00:56.000000 airbyte_source_aha-0.3.2/source_aha/run.py
+-rw-r--r--   0        0        0      472 2024-05-14 20:00:56.000000 airbyte_source_aha-0.3.2/source_aha/source.py
+-rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 airbyte_source_aha-0.3.2/PKG-INFO
```

### Comparing `airbyte-source-aha-0.3.1/PKG-INFO` & `airbyte_source_aha-0.3.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,103 @@
-Metadata-Version: 2.1
-Name: airbyte-source-aha
-Version: 0.3.1
-Summary: Source implementation for Aha.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-
 # Aha Source
 
 This is the repository for the Aha configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/aha).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/aha).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/aha)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_aha/spec.yaml` file.
-Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Prerequisites
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source aha test creds`
-and place them into `secrets/config.json`.
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Installing the connector
+
+From this connector directory, run:
 ```bash
-airbyte-ci connectors --name=source-aha build
+poetry install --with dev
 ```
 
-An image will be built with the tag `airbyte/source-aha:dev`.
 
-**Via `docker build`:**
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/aha)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_aha/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+
+```
+poetry run source-aha spec
+poetry run source-aha check --config secrets/config.json
+poetry run source-aha discover --config secrets/config.json
+poetry run source-aha read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
+
+```
+poetry run pytest tests
+```
+
+### Building the docker image
+
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-aha:dev .
+airbyte-ci connectors --name=source-aha build
 ```
 
+An image will be available on your host with the tag `airbyte/source-aha:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-aha:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-aha:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-aha:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-aha:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-aha test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-aha test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/aha.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/aha.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-aha-0.3.1/airbyte_source_aha.egg-info/PKG-INFO` & `airbyte_source_aha-0.3.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-aha
-Version: 0.3.1
-Summary: Source implementation for Aha.
+Version: 0.3.2
+Summary: Source implementation for aha.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/aha
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Aha Source
 
 This is the repository for the Aha configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/aha).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/aha).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/aha)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_aha/spec.yaml` file.
-Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source aha test creds`
-and place them into `secrets/config.json`.
 
 
+### Installing the connector
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+From this connector directory, run:
 ```bash
-airbyte-ci connectors --name=source-aha build
+poetry install --with dev
+```
+
+
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/aha)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `src/source_aha/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+
+```
+poetry run source-aha spec
+poetry run source-aha check --config secrets/config.json
+poetry run source-aha discover --config secrets/config.json
+poetry run source-aha read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
+
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-aha:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-aha:dev .
+airbyte-ci connectors --name=source-aha build
 ```
 
+An image will be available on your host with the tag `airbyte/source-aha:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-aha:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-aha:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-aha:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-aha:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-aha test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-aha test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/aha.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/aha.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

