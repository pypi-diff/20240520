# Comparing `tmp/airbyte_source_surveymonkey-0.3.1.tar.gz` & `tmp/airbyte_source_surveymonkey-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_surveymonkey-0.3.1.tar", max compression
+gzip compressed data, was "airbyte_source_surveymonkey-0.3.2.tar", max compression
```

## Comparing `airbyte_source_surveymonkey-0.3.1.tar` & `airbyte_source_surveymonkey-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4609 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/README.md
--rw-r--r--   0        0        0      822 2024-05-07 12:32:06.325868 airbyte_source_surveymonkey-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1244 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/components.py
--rw-r--r--   0        0        0     2620 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/config_migrations.py
--rw-r--r--   0        0        0    15740 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/manifest.yaml
--rw-r--r--   0        0        0      347 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/run.py
--rw-r--r--   0        0        0     3791 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/collectors.json
--rw-r--r--   0        0        0      660 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_collectors.json
--rw-r--r--   0        0        0      588 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_ids.json
--rw-r--r--   0        0        0      815 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_pages.json
--rw-r--r--   0        0        0     4871 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_questions.json
--rw-r--r--   0        0        0     4641 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_responses.json
--rw-r--r--   0        0        0     3390 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/surveys.json
--rw-r--r--   0        0        0     2344 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/source.py
--rw-r--r--   0        0        0     8428 2024-05-07 11:00:36.000000 airbyte_source_surveymonkey-0.3.1/source_surveymonkey/streams.py
--rw-r--r--   0        0        0     5397 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4619 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/README.md
+-rw-r--r--   0        0        0      822 2024-05-20 18:14:42.339942 airbyte_source_surveymonkey-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1244 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/components.py
+-rw-r--r--   0        0        0     2620 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/config_migrations.py
+-rw-r--r--   0        0        0    15740 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/manifest.yaml
+-rw-r--r--   0        0        0      347 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/run.py
+-rw-r--r--   0        0        0     3791 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/collectors.json
+-rw-r--r--   0        0        0      660 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_collectors.json
+-rw-r--r--   0        0        0      588 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_ids.json
+-rw-r--r--   0        0        0      815 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_pages.json
+-rw-r--r--   0        0        0     4871 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_questions.json
+-rw-r--r--   0        0        0     4641 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_responses.json
+-rw-r--r--   0        0        0     3390 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/surveys.json
+-rw-r--r--   0        0        0     2315 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/source.py
+-rw-r--r--   0        0        0     8428 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/streams.py
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.2/PKG-INFO
```

### Comparing `airbyte_source_surveymonkey-0.3.1/README.md` & `airbyte_source_surveymonkey-0.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Surveymonkey source connector
 
-
 This is the repository for the Surveymonkey source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/surveymonkey).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/surveymonkey)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_surveymonkey/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-surveymonkey spec
 poetry run source-surveymonkey check --config secrets/config.json
 poetry run source-surveymonkey discover --config secrets/config.json
 poetry run source-surveymonkey read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-surveymonkey build
 ```
 
 An image will be available on your host with the tag `airbyte/source-surveymonkey:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-surveymonkey:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-surveymonkey:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-surveymonkey:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-surveymonkey:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-surveymonkey test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-surveymonkey test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/surveymonkey.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_surveymonkey-0.3.1/pyproject.toml` & `airbyte_source_surveymonkey-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.1"
+version = "0.3.2"
 name = "airbyte-source-surveymonkey"
 description = "Source implementation for Surveymonkey."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/__init__.py` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/components.py` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/config_migrations.py` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/manifest.yaml` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/collectors.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/collectors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_collectors.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_collectors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_ids.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_ids.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_pages.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_questions.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_questions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/survey_responses.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_responses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/schemas/surveys.json` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/surveys.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/source.py` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
+import logging
 from typing import Any, List, Mapping, Tuple
 
 import pendulum
 import requests
-from airbyte_cdk.logger import AirbyteLogger
 from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.http.auth import TokenAuthenticator
 
 from .streams import Surveys
 
 """
@@ -38,15 +38,15 @@
     @staticmethod
     def get_authenticator(config: Mapping[str, Any]):
         token = config.get("credentials", {}).get("access_token")
         if not token:
             token = config["access_token"]
         return TokenAuthenticator(token=token)
 
-    def check_connection(self, logger: AirbyteLogger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
+    def check_connection(self, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
         # Check scopes
         try:
             authenticator = self.get_authenticator(config)
             response = requests.get(url="https://api.surveymonkey.com/v3/users/me", headers=authenticator.get_auth_header())
             response.raise_for_status()
             return self._check_scopes(response.json())
         except Exception as e:
```

### Comparing `airbyte_source_surveymonkey-0.3.1/source_surveymonkey/streams.py` & `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.1/PKG-INFO` & `airbyte_source_surveymonkey-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-surveymonkey
-Version: 0.3.1
+Version: 0.3.2
 Summary: Source implementation for Surveymonkey.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -17,96 +17,110 @@
 Requires-Dist: vcrpy (==4.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/surveymonkey
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Surveymonkey source connector
 
-
 This is the repository for the Surveymonkey source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/surveymonkey).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/surveymonkey)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_surveymonkey/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-surveymonkey spec
 poetry run source-surveymonkey check --config secrets/config.json
 poetry run source-surveymonkey discover --config secrets/config.json
 poetry run source-surveymonkey read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-surveymonkey build
 ```
 
 An image will be available on your host with the tag `airbyte/source-surveymonkey:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-surveymonkey:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-surveymonkey:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-surveymonkey:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-surveymonkey:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-surveymonkey test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-surveymonkey test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/surveymonkey.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

