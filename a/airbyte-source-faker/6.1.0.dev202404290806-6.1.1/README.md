# Comparing `tmp/airbyte_source_faker-6.1.0.dev202404290806.tar.gz` & `tmp/airbyte_source_faker-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_faker-6.1.0.dev202404290806.tar", max compression
+gzip compressed data, was "airbyte_source_faker-6.1.1.tar", max compression
```

## Comparing `airbyte_source_faker-6.1.0.dev202404290806.tar` & `airbyte_source_faker-6.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4478 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/README.md
--rw-r--r--   0        0        0      800 2024-04-29 08:06:59.942747 airbyte_source_faker-6.1.0.dev202404290806/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/__init__.py
--rw-r--r--   0        0        0      727 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/airbyte_message_with_cached_json.py
--rw-r--r--   0        0        0     4590 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/purchase_generator.py
--rw-r--r--   0        0        0    15356 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/record_data/products.json
--rw-r--r--   0        0        0      266 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/run.py
--rw-r--r--   0        0        0      529 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/schemas/products.json
--rw-r--r--   0        0        0      892 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/schemas/purchases.json
--rw-r--r--   0        0        0     1259 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/schemas/users.json
--rw-r--r--   0        0        0     1395 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/source.py
--rw-r--r--   0        0        0     1849 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/spec.json
--rw-r--r--   0        0        0     6705 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/streams.py
--rw-r--r--   0        0        0     3325 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/user_generator.py
--rw-r--r--   0        0        0      937 2024-04-29 08:03:59.314373 airbyte_source_faker-6.1.0.dev202404290806/source_faker/utils.py
--rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 airbyte_source_faker-6.1.0.dev202404290806/PKG-INFO
+-rw-r--r--   0        0        0     4488 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/README.md
+-rw-r--r--   0        0        0      784 2024-05-20 18:16:25.752215 airbyte_source_faker-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/airbyte_message_with_cached_json.py
+-rw-r--r--   0        0        0     4590 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/purchase_generator.py
+-rw-r--r--   0        0        0    15356 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/record_data/products.json
+-rw-r--r--   0        0        0      266 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/run.py
+-rw-r--r--   0        0        0      529 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/schemas/products.json
+-rw-r--r--   0        0        0      892 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/schemas/purchases.json
+-rw-r--r--   0        0        0     1259 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/schemas/users.json
+-rw-r--r--   0        0        0     1366 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/source.py
+-rw-r--r--   0        0        0     1849 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/spec.json
+-rw-r--r--   0        0        0     6705 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/streams.py
+-rw-r--r--   0        0        0     3325 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/user_generator.py
+-rw-r--r--   0        0        0      937 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/utils.py
+-rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 airbyte_source_faker-6.1.1/PKG-INFO
```

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/README.md` & `airbyte_source_faker-6.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Faker source connector
 
-
 This is the repository for the Faker source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/faker).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/faker)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_faker/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-faker spec
 poetry run source-faker check --config secrets/config.json
 poetry run source-faker discover --config secrets/config.json
 poetry run source-faker read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-faker build
 ```
 
 An image will be available on your host with the tag `airbyte/source-faker:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-faker:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-faker:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-faker:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-faker:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-faker test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-faker test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/faker.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/pyproject.toml` & `airbyte_source_faker-6.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "6.1.0.dev202404290806"
+version = "6.1.1"
 name = "airbyte-source-faker"
 description = "Source implementation for fake but realistic looking data."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/airbyte_message_with_cached_json.py` & `airbyte_source_faker-6.1.1/source_faker/airbyte_message_with_cached_json.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/purchase_generator.py` & `airbyte_source_faker-6.1.1/source_faker/purchase_generator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/record_data/products.json` & `airbyte_source_faker-6.1.1/source_faker/record_data/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/schemas/products.json` & `airbyte_source_faker-6.1.1/source_faker/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/schemas/purchases.json` & `airbyte_source_faker-6.1.1/source_faker/schemas/purchases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/schemas/users.json` & `airbyte_source_faker-6.1.1/source_faker/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/source.py` & `airbyte_source_faker-6.1.1/source_faker/source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
+import logging
 from typing import Any, List, Mapping, Tuple
 
-from airbyte_cdk.logger import AirbyteLogger
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
 
 from .streams import Products, Purchases, Users
 
 DEFAULT_COUNT = 1_000
 
 
 class SourceFaker(AbstractSource):
-    def check_connection(self, logger: AirbyteLogger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
+    def check_connection(self, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
         if type(config["count"]) == int or type(config["count"]) == float:
             return True, None
         else:
             return False, "Count option is missing"
 
     def streams(self, config: Mapping[str, Any]) -> List[Stream]:
         count: int = config["count"] if "count" in config else DEFAULT_COUNT
```

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/spec.json` & `airbyte_source_faker-6.1.1/source_faker/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/streams.py` & `airbyte_source_faker-6.1.1/source_faker/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/user_generator.py` & `airbyte_source_faker-6.1.1/source_faker/user_generator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/source_faker/utils.py` & `airbyte_source_faker-6.1.1/source_faker/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.0.dev202404290806/PKG-INFO` & `airbyte_source_faker-6.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-faker
-Version: 6.1.0.dev202404290806
+Version: 6.1.1
 Summary: Source implementation for fake but realistic looking data.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -16,96 +16,110 @@
 Requires-Dist: mimesis (==6.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/faker
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Faker source connector
 
-
 This is the repository for the Faker source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/faker).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/faker)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_faker/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-faker spec
 poetry run source-faker check --config secrets/config.json
 poetry run source-faker discover --config secrets/config.json
 poetry run source-faker read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-faker build
 ```
 
 An image will be available on your host with the tag `airbyte/source-faker:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-faker:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-faker:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-faker:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-faker:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-faker test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-faker test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/faker.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```
