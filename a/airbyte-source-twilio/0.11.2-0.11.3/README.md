# Comparing `tmp/airbyte_source_twilio-0.11.2.tar.gz` & `tmp/airbyte_source_twilio-0.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_twilio-0.11.2.tar", max compression
+gzip compressed data, was "airbyte_source_twilio-0.11.3.tar", max compression
```

## Comparing `airbyte_source_twilio-0.11.2.tar` & `airbyte_source_twilio-0.11.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     4507 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/README.md
--rw-r--r--   0        0        0      809 2024-05-07 13:32:53.178253 airbyte_source_twilio-0.11.2/pyproject.toml
--rw-r--r--   0        0        0     1134 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/__init__.py
--rw-r--r--   0        0        0      514 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/auth.py
--rw-r--r--   0        0        0      230 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/run.py
--rw-r--r--   0        0        0     2914 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/accounts.json
--rw-r--r--   0        0        0     2215 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/addresses.json
--rw-r--r--   0        0        0     2209 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/alerts.json
--rw-r--r--   0        0        0     3370 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/applications.json
--rw-r--r--   0        0        0     1318 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_number_countries.json
--rw-r--r--   0        0        0     2403 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_numbers_local.json
--rw-r--r--   0        0        0     2430 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_numbers_mobile.json
--rw-r--r--   0        0        0     2682 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_numbers_toll_free.json
--rw-r--r--   0        0        0     5398 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/calls.json
--rw-r--r--   0        0        0     2222 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/conference_participants.json
--rw-r--r--   0        0        0     2173 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/conferences.json
--rw-r--r--   0        0        0     4172 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/conversation_messages.json
--rw-r--r--   0        0        0     2447 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/conversation_participants.json
--rw-r--r--   0        0        0     2057 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/conversations.json
--rw-r--r--   0        0        0     4312 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/dependent_phone_numbers.json
--rw-r--r--   0        0        0     2161 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/executions.json
--rw-r--r--   0        0        0     1531 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/flows.json
--rw-r--r--   0        0        0     6035 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/incoming_phone_numbers.json
--rw-r--r--   0        0        0      659 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/keys.json
--rw-r--r--   0        0        0     1118 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/message_media.json
--rw-r--r--   0        0        0     3338 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/messages.json
--rw-r--r--   0        0        0     1165 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/outgoing_caller_ids.json
--rw-r--r--   0        0        0     1715 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/queues.json
--rw-r--r--   0        0        0     3762 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/recordings.json
--rw-r--r--   0        0        0     1453 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/roles.json
--rw-r--r--   0        0        0     4633 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/services.json
--rw-r--r--   0        0        0     2118 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/step.json
--rw-r--r--   0        0        0     2030 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/transcriptions.json
--rw-r--r--   0        0        0     3766 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/trunks.json
--rw-r--r--   0        0        0     3732 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/usage_records.json
--rw-r--r--   0        0        0     2294 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/usage_triggers.json
--rw-r--r--   0        0        0     3351 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/user_conversations.json
--rw-r--r--   0        0        0     2088 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/users.json
--rw-r--r--   0        0        0     5496 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/schemas/verify_services.json
--rw-r--r--   0        0        0     5040 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/source.py
--rw-r--r--   0        0        0     1497 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/spec.json
--rw-r--r--   0        0        0    25186 2024-05-07 11:13:23.000000 airbyte_source_twilio-0.11.2/source_twilio/streams.py
--rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 airbyte_source_twilio-0.11.2/PKG-INFO
+-rw-r--r--   0        0        0     4517 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/README.md
+-rw-r--r--   0        0        0      809 2024-05-20 18:16:31.552923 airbyte_source_twilio-0.11.3/pyproject.toml
+-rw-r--r--   0        0        0     1134 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/__init__.py
+-rw-r--r--   0        0        0      514 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/auth.py
+-rw-r--r--   0        0        0      230 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/run.py
+-rw-r--r--   0        0        0     2914 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/accounts.json
+-rw-r--r--   0        0        0     2215 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/addresses.json
+-rw-r--r--   0        0        0     2209 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/alerts.json
+-rw-r--r--   0        0        0     3370 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/applications.json
+-rw-r--r--   0        0        0     1318 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_number_countries.json
+-rw-r--r--   0        0        0     2403 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_numbers_local.json
+-rw-r--r--   0        0        0     2430 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_numbers_mobile.json
+-rw-r--r--   0        0        0     2682 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_numbers_toll_free.json
+-rw-r--r--   0        0        0     5398 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/calls.json
+-rw-r--r--   0        0        0     2222 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/conference_participants.json
+-rw-r--r--   0        0        0     2173 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/conferences.json
+-rw-r--r--   0        0        0     4172 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/conversation_messages.json
+-rw-r--r--   0        0        0     2447 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/conversation_participants.json
+-rw-r--r--   0        0        0     2057 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/conversations.json
+-rw-r--r--   0        0        0     4312 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/dependent_phone_numbers.json
+-rw-r--r--   0        0        0     2161 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/executions.json
+-rw-r--r--   0        0        0     1531 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/flows.json
+-rw-r--r--   0        0        0     6035 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/incoming_phone_numbers.json
+-rw-r--r--   0        0        0      659 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/keys.json
+-rw-r--r--   0        0        0     1118 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/message_media.json
+-rw-r--r--   0        0        0     3338 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/messages.json
+-rw-r--r--   0        0        0     1165 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/outgoing_caller_ids.json
+-rw-r--r--   0        0        0     1715 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/queues.json
+-rw-r--r--   0        0        0     3762 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/recordings.json
+-rw-r--r--   0        0        0     1453 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/roles.json
+-rw-r--r--   0        0        0     4633 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/services.json
+-rw-r--r--   0        0        0     2118 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/step.json
+-rw-r--r--   0        0        0     2030 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/transcriptions.json
+-rw-r--r--   0        0        0     3766 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/trunks.json
+-rw-r--r--   0        0        0     3732 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/usage_records.json
+-rw-r--r--   0        0        0     2294 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/usage_triggers.json
+-rw-r--r--   0        0        0     3351 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/user_conversations.json
+-rw-r--r--   0        0        0     2088 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/users.json
+-rw-r--r--   0        0        0     5496 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/schemas/verify_services.json
+-rw-r--r--   0        0        0     5011 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/source.py
+-rw-r--r--   0        0        0     1497 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/spec.json
+-rw-r--r--   0        0        0    25186 2024-05-20 04:10:43.000000 airbyte_source_twilio-0.11.3/source_twilio/streams.py
+-rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 airbyte_source_twilio-0.11.3/PKG-INFO
```

### Comparing `airbyte_source_twilio-0.11.2/README.md` & `airbyte_source_twilio-0.11.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Twilio source connector
 
-
 This is the repository for the Twilio source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/twilio).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/twilio)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_twilio/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-twilio spec
 poetry run source-twilio check --config secrets/config.json
 poetry run source-twilio discover --config secrets/config.json
 poetry run source-twilio read --config secrets/config.json --catalog integration_tests/constant_records_catalog.json
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
 airbyte-ci connectors --name=source-twilio build
 ```
 
 An image will be available on your host with the tag `airbyte/source-twilio:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-twilio:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-twilio:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-twilio:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-twilio:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-twilio test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-twilio test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/twilio.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_twilio-0.11.2/pyproject.toml` & `airbyte_source_twilio-0.11.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.11.2"
+version = "0.11.3"
 name = "airbyte-source-twilio"
 description = "Source implementation for Twilio."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/__init__.py` & `airbyte_source_twilio-0.11.3/source_twilio/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/auth.py` & `airbyte_source_twilio-0.11.3/source_twilio/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/accounts.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/addresses.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/addresses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/alerts.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/alerts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/applications.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/applications.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_number_countries.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_number_countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_numbers_local.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_numbers_local.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_numbers_mobile.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_numbers_mobile.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/available_phone_numbers_toll_free.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/available_phone_numbers_toll_free.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/calls.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/calls.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/conference_participants.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/conference_participants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/conferences.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/conferences.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/conversation_messages.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/conversation_messages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/conversation_participants.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/conversation_participants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/conversations.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/conversations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/dependent_phone_numbers.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/dependent_phone_numbers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/executions.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/executions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/flows.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/flows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/incoming_phone_numbers.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/incoming_phone_numbers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/keys.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/keys.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/message_media.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/message_media.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/messages.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/messages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/outgoing_caller_ids.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/outgoing_caller_ids.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/queues.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/queues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/recordings.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/recordings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/roles.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/services.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/services.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/step.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/step.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/transcriptions.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/transcriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/trunks.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/trunks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/usage_records.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/usage_records.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/usage_triggers.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/usage_triggers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/user_conversations.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/user_conversations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/users.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/schemas/verify_services.json` & `airbyte_source_twilio-0.11.3/source_twilio/schemas/verify_services.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/source.py` & `airbyte_source_twilio-0.11.3/source_twilio/source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import datetime
+import logging
 from typing import Any, List, Mapping, Tuple
 
 import pendulum
-from airbyte_cdk.logger import AirbyteLogger
 from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
 from source_twilio.auth import HttpBasicAuthenticator
 from source_twilio.streams import (
     Accounts,
     Addresses,
@@ -48,15 +48,15 @@
     VerifyServices,
 )
 
 RETENTION_WINDOW_LIMIT = 400
 
 
 class SourceTwilio(AbstractSource):
-    def check_connection(self, logger: AirbyteLogger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
+    def check_connection(self, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, Any]:
         try:
             auth = HttpBasicAuthenticator(
                 (
                     config["account_sid"],
                     config["auth_token"],
                 ),
             )
```

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/spec.json` & `airbyte_source_twilio-0.11.3/source_twilio/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/source_twilio/streams.py` & `airbyte_source_twilio-0.11.3/source_twilio/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_twilio-0.11.2/PKG-INFO` & `airbyte_source_twilio-0.11.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-twilio
-Version: 0.11.2
+Version: 0.11.3
 Summary: Source implementation for Twilio.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -17,96 +17,110 @@
 Requires-Dist: requests (==2.31.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/twilio
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Twilio source connector
 
-
 This is the repository for the Twilio source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/twilio).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/twilio)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_twilio/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-twilio spec
 poetry run source-twilio check --config secrets/config.json
 poetry run source-twilio discover --config secrets/config.json
 poetry run source-twilio read --config secrets/config.json --catalog integration_tests/constant_records_catalog.json
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
 airbyte-ci connectors --name=source-twilio build
 ```
 
 An image will be available on your host with the tag `airbyte/source-twilio:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-twilio:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-twilio:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-twilio:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-twilio:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-twilio test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-twilio test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/twilio.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

