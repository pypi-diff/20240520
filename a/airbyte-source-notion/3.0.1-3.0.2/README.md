# Comparing `tmp/airbyte_source_notion-3.0.1.tar.gz` & `tmp/airbyte_source_notion-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_notion-3.0.1.tar", max compression
+gzip compressed data, was "airbyte_source_notion-3.0.2.tar", max compression
```

## Comparing `airbyte_source_notion-3.0.1.tar` & `airbyte_source_notion-3.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     4501 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/README.md
--rw-r--r--   0        0        0      765 2024-05-07 12:29:16.900764 airbyte_source_notion-3.0.1/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/__init__.py
--rw-r--r--   0        0        0     5943 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/components.py
--rw-r--r--   0        0        0    14612 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/manifest.yaml
--rw-r--r--   0        0        0      230 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/run.py
--rw-r--r--   0        0        0    12049 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/blocks.json
--rw-r--r--   0        0        0     3535 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/comments.json
--rw-r--r--   0        0        0    16786 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/databases.json
--rw-r--r--   0        0        0    13980 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/pages.json
--rw-r--r--   0        0        0      168 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/child.json
--rw-r--r--   0        0        0      280 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/date.json
--rw-r--r--   0        0        0      232 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/emoji.json
--rw-r--r--   0        0        0      764 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/file.json
--rw-r--r--   0        0        0      299 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/heading.json
--rw-r--r--   0        0        0      123 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/icon.json
--rw-r--r--   0        0        0      444 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/options.json
--rw-r--r--   0        0        0      416 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/parent.json
--rw-r--r--   0        0        0     1936 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/rich_text.json
--rw-r--r--   0        0        0      313 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/text_element.json
--rw-r--r--   0        0        0     1401 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/title.json
--rw-r--r--   0        0        0     1726 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/shared/user.json
--rw-r--r--   0        0        0       82 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/schemas/users.json
--rw-r--r--   0        0        0     1941 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/source.py
--rw-r--r--   0        0        0     4638 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/spec.json
--rw-r--r--   0        0        0    13631 2024-05-07 10:46:02.000000 airbyte_source_notion-3.0.1/source_notion/streams.py
--rw-r--r--   0        0        0     5205 1970-01-01 00:00:00.000000 airbyte_source_notion-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4511 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/README.md
+-rw-r--r--   0        0        0      765 2024-05-20 20:03:05.020650 airbyte_source_notion-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/__init__.py
+-rw-r--r--   0        0        0     5943 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/components.py
+-rw-r--r--   0        0        0    14612 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/run.py
+-rw-r--r--   0        0        0    12049 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/blocks.json
+-rw-r--r--   0        0        0     3535 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/comments.json
+-rw-r--r--   0        0        0    16786 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/databases.json
+-rw-r--r--   0        0        0    13980 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/pages.json
+-rw-r--r--   0        0        0      168 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/child.json
+-rw-r--r--   0        0        0      280 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/date.json
+-rw-r--r--   0        0        0      232 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/emoji.json
+-rw-r--r--   0        0        0      764 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/file.json
+-rw-r--r--   0        0        0      299 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/heading.json
+-rw-r--r--   0        0        0      123 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/icon.json
+-rw-r--r--   0        0        0      444 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/options.json
+-rw-r--r--   0        0        0      416 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/parent.json
+-rw-r--r--   0        0        0     1936 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/rich_text.json
+-rw-r--r--   0        0        0      313 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/text_element.json
+-rw-r--r--   0        0        0     1401 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/title.json
+-rw-r--r--   0        0        0     1726 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/shared/user.json
+-rw-r--r--   0        0        0       82 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/schemas/users.json
+-rw-r--r--   0        0        0     1941 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/source.py
+-rw-r--r--   0        0        0     4638 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/spec.json
+-rw-r--r--   0        0        0    13601 2024-05-20 03:57:02.000000 airbyte_source_notion-3.0.2/source_notion/streams.py
+-rw-r--r--   0        0        0     5215 1970-01-01 00:00:00.000000 airbyte_source_notion-3.0.2/PKG-INFO
```

### Comparing `airbyte_source_notion-3.0.1/README.md` & `airbyte_source_notion-3.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Notion source connector
 
-
 This is the repository for the Notion source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/notion).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/notion)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_notion/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-notion spec
 poetry run source-notion check --config secrets/config.json
 poetry run source-notion discover --config secrets/config.json
 poetry run source-notion read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-notion build
 ```
 
 An image will be available on your host with the tag `airbyte/source-notion:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-notion:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-notion:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-notion:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-notion:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-notion test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-notion test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/notion.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_notion-3.0.1/pyproject.toml` & `airbyte_source_notion-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.1"
+version = "3.0.2"
 name = "airbyte-source-notion"
 description = "Source implementation for Notion."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_notion-3.0.1/source_notion/components.py` & `airbyte_source_notion-3.0.2/source_notion/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/manifest.yaml` & `airbyte_source_notion-3.0.2/source_notion/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/blocks.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/blocks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/comments.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/databases.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/databases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/pages.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/shared/file.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/shared/file.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/shared/rich_text.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/shared/rich_text.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/shared/title.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/shared/title.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/schemas/shared/user.json` & `airbyte_source_notion-3.0.2/source_notion/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/source.py` & `airbyte_source_notion-3.0.2/source_notion/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/spec.json` & `airbyte_source_notion-3.0.2/source_notion/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_notion-3.0.1/source_notion/streams.py` & `airbyte_source_notion-3.0.2/source_notion/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
+import logging as Logger
 from abc import ABC
 from typing import Any, Dict, Iterable, List, Mapping, MutableMapping, Optional, TypeVar
 
 import pendulum
 import pydantic
 import requests
-from airbyte_cdk.logger import AirbyteLogger as Logger
 from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources import Source
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.http import HttpStream, HttpSubStream
 from airbyte_cdk.sources.streams.http.availability_strategy import HttpAvailabilityStrategy
 from airbyte_cdk.sources.streams.http.exceptions import UserDefinedBackoffException
 from requests import HTTPError
```

### Comparing `airbyte_source_notion-3.0.1/PKG-INFO` & `airbyte_source_notion-3.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-notion
-Version: 3.0.1
+Version: 3.0.2
 Summary: Source implementation for Notion.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/notion
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Notion source connector
 
-
 This is the repository for the Notion source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/notion).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/notion)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_notion/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-notion spec
 poetry run source-notion check --config secrets/config.json
 poetry run source-notion discover --config secrets/config.json
 poetry run source-notion read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-notion build
 ```
 
 An image will be available on your host with the tag `airbyte/source-notion:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-notion:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-notion:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-notion:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-notion:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-notion test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-notion test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/notion.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

