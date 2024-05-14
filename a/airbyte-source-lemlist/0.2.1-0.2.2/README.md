# Comparing `tmp/airbyte_source_lemlist-0.2.1.tar.gz` & `tmp/airbyte_source_lemlist-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_lemlist-0.2.1.tar", max compression
+gzip compressed data, was "airbyte_source_lemlist-0.2.2.tar", max compression
```

## Comparing `airbyte_source_lemlist-0.2.1.tar` & `airbyte_source_lemlist-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,7 @@
--rw-r--r--   0        0        0     4011 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/README.md
--rw-r--r--   0        0        0      745 2024-04-30 18:31:50.402150 airbyte_source_lemlist-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      126 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/__init__.py
--rw-r--r--   0        0        0     2048 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/manifest.yaml
--rw-r--r--   0        0        0      233 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/run.py
--rw-r--r--   0        0        0     2085 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/schemas/activities.json
--rw-r--r--   0        0        0      304 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/schemas/campaigns.json
--rw-r--r--   0        0        0     3272 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/schemas/team.json
--rw-r--r--   0        0        0      199 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/schemas/unsubscribes.json
--rw-r--r--   0        0        0      476 2024-04-30 18:06:06.000000 airbyte_source_lemlist-0.2.1/source_lemlist/source.py
--rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 airbyte_source_lemlist-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4022 2024-05-14 00:02:29.000000 airbyte_source_lemlist-0.2.2/README.md
+-rw-r--r--   0        0        0      745 2024-05-14 00:52:32.668008 airbyte_source_lemlist-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-14 00:02:29.000000 airbyte_source_lemlist-0.2.2/source_lemlist/__init__.py
+-rw-r--r--   0        0        0     9162 2024-05-14 00:02:29.000000 airbyte_source_lemlist-0.2.2/source_lemlist/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-14 00:02:29.000000 airbyte_source_lemlist-0.2.2/source_lemlist/run.py
+-rw-r--r--   0        0        0      476 2024-05-14 00:02:29.000000 airbyte_source_lemlist-0.2.2/source_lemlist/source.py
+-rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 airbyte_source_lemlist-0.2.2/PKG-INFO
```

### Comparing `airbyte_source_lemlist-0.2.1/README.md` & `airbyte_source_lemlist-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,66 +2,77 @@
 
 This is the repository for the Lemlist configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/lemlist).
 
 ## Local development
 
 #### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/lemlist)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_lemlist/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
 **If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source lemlist test creds`
 and place them into `secrets/config.json`.
 
 ### Locally running the connector docker image
 
-
 #### Build
+
 **Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+
 ```bash
 airbyte-ci connectors --name=source-lemlist build
 ```
 
 An image will be built with the tag `airbyte/source-lemlist:dev`.
 
 **Via `docker build`:**
+
 ```bash
 docker build -t airbyte/source-lemlist:dev .
 ```
 
 #### Run
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-lemlist:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-lemlist:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-lemlist:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-lemlist:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ## Testing
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-lemlist test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ## Dependency Management
+
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+
+- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
+- required for the testing need to go to `TEST_REQUIREMENTS` list
 
 ### Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-lemlist test`
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/lemlist.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
```

### Comparing `airbyte_source_lemlist-0.2.1/pyproject.toml` & `airbyte_source_lemlist-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.1"
+version = "0.2.2"
 name = "airbyte-source-lemlist"
 description = "Source implementation for Lemlist."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_lemlist-0.2.1/PKG-INFO` & `airbyte_source_lemlist-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-lemlist
-Version: 0.2.1
+Version: 0.2.2
 Summary: Source implementation for Lemlist.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -21,67 +21,78 @@
 
 This is the repository for the Lemlist configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/lemlist).
 
 ## Local development
 
 #### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/lemlist)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_lemlist/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
 **If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source lemlist test creds`
 and place them into `secrets/config.json`.
 
 ### Locally running the connector docker image
 
-
 #### Build
+
 **Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+
 ```bash
 airbyte-ci connectors --name=source-lemlist build
 ```
 
 An image will be built with the tag `airbyte/source-lemlist:dev`.
 
 **Via `docker build`:**
+
 ```bash
 docker build -t airbyte/source-lemlist:dev .
 ```
 
 #### Run
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-lemlist:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-lemlist:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-lemlist:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-lemlist:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ## Testing
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-lemlist test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ## Dependency Management
+
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+
+- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
+- required for the testing need to go to `TEST_REQUIREMENTS` list
 
 ### Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-lemlist test`
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/lemlist.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 
-
```

