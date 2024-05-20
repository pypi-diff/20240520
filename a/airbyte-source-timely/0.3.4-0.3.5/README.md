# Comparing `tmp/airbyte_source_timely-0.3.4.tar.gz` & `tmp/airbyte_source_timely-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_timely-0.3.4.tar", max compression
+gzip compressed data, was "airbyte_source_timely-0.3.5.tar", max compression
```

## Comparing `airbyte_source_timely-0.3.4.tar` & `airbyte_source_timely-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4496 2024-05-01 19:04:45.049501 airbyte_source_timely-0.3.4/README.md
--rw-r--r--   0        0        0      743 2024-05-01 19:08:15.001426 airbyte_source_timely-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-01 19:04:45.053501 airbyte_source_timely-0.3.4/source_timely/__init__.py
--rw-r--r--   0        0        0    20519 2024-05-01 19:04:45.053501 airbyte_source_timely-0.3.4/source_timely/manifest.yaml
--rw-r--r--   0        0        0      230 2024-05-01 19:04:45.053501 airbyte_source_timely-0.3.4/source_timely/run.py
--rw-r--r--   0        0        0      475 2024-05-01 19:04:45.053501 airbyte_source_timely-0.3.4/source_timely/source.py
--rw-r--r--   0        0        0      662 2024-05-01 19:04:45.053501 airbyte_source_timely-0.3.4/source_timely/spec.yaml
--rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 airbyte_source_timely-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     4506 2024-05-20 03:35:59.001905 airbyte_source_timely-0.3.5/README.md
+-rw-r--r--   0        0        0      743 2024-05-20 03:39:29.780842 airbyte_source_timely-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-20 03:35:59.001905 airbyte_source_timely-0.3.5/source_timely/__init__.py
+-rw-r--r--   0        0        0    19108 2024-05-20 03:35:59.001905 airbyte_source_timely-0.3.5/source_timely/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-05-20 03:35:59.001905 airbyte_source_timely-0.3.5/source_timely/run.py
+-rw-r--r--   0        0        0      475 2024-05-20 03:35:59.001905 airbyte_source_timely-0.3.5/source_timely/source.py
+-rw-r--r--   0        0        0     5210 1970-01-01 00:00:00.000000 airbyte_source_timely-0.3.5/PKG-INFO
```

### Comparing `airbyte_source_timely-0.3.4/README.md` & `airbyte_source_timely-0.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Timely source connector
 
-
 This is the repository for the Timely source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/timely).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/timely)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_timely/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-timely spec
 poetry run source-timely check --config secrets/config.json
 poetry run source-timely discover --config secrets/config.json
 poetry run source-timely read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-timely build
 ```
 
 An image will be available on your host with the tag `airbyte/source-timely:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-timely:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-timely:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-timely:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-timely:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-timely test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-timely test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/timely.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_timely-0.3.4/pyproject.toml` & `airbyte_source_timely-0.3.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.4"
+version = "0.3.5"
 name = "airbyte-source-timely"
 description = "Source implementation for Timely."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_timely-0.3.4/source_timely/manifest.yaml` & `airbyte_source_timely-0.3.5/source_timely/manifest.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,646 +1,693 @@
-version: "0.29.0"
+version: 0.78.5
+
 type: DeclarativeSource
+
 check:
   type: CheckStream
   stream_names:
     - events
+
+definitions:
+  streams:
+    events:
+      type: DeclarativeStream
+      name: events
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: "{{ config.account_id }}/events"
+          http_method: GET
+          request_parameters:
+            account_id: "{{ config.account_id }}"
+            since: "{{ config.start_date }}"
+            upto: "{{ now_utc().strftime('%Y-%m-%d') }}"
+          request_headers:
+            Content-Type: application/json
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: per_page
+          pagination_strategy:
+            type: PageIncrement
+            start_from_page: 1
+            page_size: 1000
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/events"
+  base_requester:
+    type: HttpRequester
+    url_base: https://api.timelyapp.com/1.1/
+    authenticator:
+      type: BearerAuthenticator
+      api_token: "{{ config['bearer_token'] }}"
+
 streams:
-  - type: DeclarativeStream
-    name: events
-    primary_key:
-      - id
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://api.timelyapp.com/1.1/
-        path: "{{ config.account_id }}/events"
-        http_method: GET
-        request_parameters:
-          account_id: "{{ config.account_id }}"
-          since: "{{ config.start_date }}"
-          upto: "{{ now_utc().strftime('%Y-%m-%d') }}"
-        request_headers:
-          Content-Type: application/json
-        authenticator:
-          type: BearerAuthenticator
-          api_token: "{{ config['bearer_token'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: DefaultPaginator
-        page_token_option:
-          type: RequestOption
-          inject_into: request_parameter
-          field_name: page
-        page_size_option:
-          inject_into: request_parameter
-          field_name: per_page
-          type: RequestOption
-        pagination_strategy:
-          type: PageIncrement
-          start_from_page: 1
-          page_size: 1000
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
+  - $ref: "#/definitions/streams/events"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - account_id
+      - bearer_token
+      - start_date
+    properties:
+      account_id:
+        type: string
+        title: account_id
+        description: Timely account id
+        order: 0
+      bearer_token:
+        type: string
+        title: Bearer token
+        description: Timely bearer token
+        order: 1
+      start_date:
+        type: string
+        title: startDate
+        description: start date
+        pattern: ^[0-9]{4}-[0-9]{2}-[0-9]{2}$
+        example: "2022-05-06"
+        order: 2
+    additionalProperties: true
+
+metadata:
+  autoImportSchema:
+    events: false
+
+schemas:
+  events:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      billable:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event is billable or not
+      billed:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event has been billed or not
+      billed_at:
+        type:
+          - "null"
+          - string
+        airbyte_type: timestamp_with_timezone
+        description: Date and time when the event was billed
+        format: date-time
+      cost:
+        type:
+          - "null"
+          - object
         additionalProperties: true
+        description: The cost associated with the event
         properties:
-          invoice_id:
-            description: ID of the invoice associated with the event
+          amount:
+            type:
+              - "null"
+              - number
+            description: The amount of the cost
+          formatted:
             type:
               - "null"
               - string
-          suggestion_id:
-            description: ID of the suggestion associated with the event
+            description: The cost formatted as a string
+          fractional:
+            type:
+              - "null"
+              - integer
+            description: The fractional part of the cost
+      created_at:
+        type:
+          - "null"
+          - integer
+        description: Date and time when the event was created
+      created_from:
+        type:
+          - "null"
+          - string
+        description: Source from which the event was created
+      created_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the creator
+      creator_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the creator
+      day:
+        type:
+          - "null"
+          - string
+        description: Date of the event
+        format: date
+      deleted:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event has been deleted
+      draft:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event is in draft mode
+      duration:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: The duration of the event
+        properties:
+          correctedHours:
             type:
               - "null"
               - integer
-          locked:
-            description: Indicates whether the event is locked
+            description: Corrected hours of the event duration
+          formatted:
             type:
               - "null"
-              - boolean
-          creator_id:
-            description: ID of the creator
+              - string
+            description: Duration formatted as a string
+          hours:
             type:
               - "null"
               - integer
-          state:
-            description: State of the event
+            description: Hours component of the duration
+          minutes:
             type:
               - "null"
-              - object
-            additionalProperties: true
-          timestamps:
-            description: Timestamps related to the event
+              - integer
+            description: Minutes component of the duration
+          seconds:
             type:
               - "null"
-              - array
-            items:
-              description: Array of timestamps associated with the event
-              type:
-                - "null"
-                - string
-          created_id:
-            description: ID of the creator
+              - integer
+            description: Seconds component of the duration
+          total_hours:
+            type:
+              - "null"
+              - number
+            description: Total duration in hours
+          total_minutes:
             type:
               - "null"
               - integer
-          hour_rate_in_cents:
-            description: Hourly rate in cents for the event
+            description: Total duration in minutes
+          total_seconds:
+            type:
+              - "null"
+              - integer
+            description: Total duration in seconds
+      entry_ids:
+        type:
+          - "null"
+          - array
+        description: IDs related to the event entries
+        items:
+          type:
+            - "null"
+            - string
+          description: Array of entry IDs linked to the event
+      estimated:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event is estimated
+      estimated_cost:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: The estimated cost of the event
+        properties:
+          amount:
             type:
               - "null"
               - number
-          deleted:
-            description: Indicates whether the event has been deleted
+            description: The estimated amount of the cost
+          formatted:
             type:
               - "null"
-              - boolean
-          to:
-            description: End date and time of the event
+              - string
+            description: The estimated cost formatted as a string
+          fractional:
+            type:
+              - "null"
+              - integer
+            description: The fractional part of the estimated cost
+      estimated_duration:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: The estimated duration of the event
+        properties:
+          formatted:
             type:
               - "null"
               - string
-            format: date-time
-            airbyte_type: timestamp_with_timezone
-          estimated_cost:
-            description: The estimated cost of the event
+            description: Estimated duration formatted as a string
+          hours:
             type:
               - "null"
-              - object
-            additionalProperties: true
-            properties:
-              amount:
-                description: The estimated amount of the cost
-                type:
-                  - "null"
-                  - number
-              formatted:
-                description: The estimated cost formatted as a string
-                type:
-                  - "null"
-                  - string
-              fractional:
-                description: The fractional part of the estimated cost
-                type:
-                  - "null"
-                  - integer
-          billable:
-            description: Indicates whether the event is billable or not
+              - integer
+            description: Estimated hours component of the duration
+          minutes:
             type:
               - "null"
-              - boolean
-          updater_id:
-            description: ID of the user who last updated the event
+              - integer
+            description: Estimated minutes component of the duration
+          seconds:
             type:
               - "null"
               - integer
-          label_ids:
-            description: IDs related to event labels
+            description: Estimated seconds component of the duration
+          total_hours:
             type:
               - "null"
-              - array
-            items:
-              description: Array of label IDs associated with the event
-              type:
-                - "null"
-                - string
-          forecast_id:
-            description: ID of the forecast associated with the event
+              - number
+            description: Total estimated duration in hours
+          total_minutes:
             type:
               - "null"
-              - string
-          user_ids:
-            description: IDs related to users associated with the event
+              - integer
+            description: Total estimated duration in minutes
+          total_seconds:
             type:
               - "null"
-              - array
-            items:
-              description: Array of user IDs linked to the event
-              type:
-                - "null"
-                - string
-          timer_stopped_on:
-            description: Date and time when the timer was stopped
+              - integer
+            description: Total estimated duration in seconds
+      external_id:
+        type:
+          - "null"
+          - integer
+        description: External ID of the event
+      forecast_id:
+        type:
+          - "null"
+          - string
+        description: ID of the forecast associated with the event
+      from:
+        type:
+          - "null"
+          - string
+        airbyte_type: timestamp_with_timezone
+        description: Start date and time of the event
+        format: date-time
+      hour_rate:
+        type:
+          - "null"
+          - number
+        description: Hourly rate for the event
+      hour_rate_in_cents:
+        type:
+          - "null"
+          - number
+        description: Hourly rate in cents for the event
+      id:
+        type:
+          - "null"
+          - integer
+        description: ID of the event
+      invoice_id:
+        type:
+          - "null"
+          - string
+        description: ID of the invoice associated with the event
+      label_ids:
+        type:
+          - "null"
+          - array
+        description: IDs related to event labels
+        items:
+          type:
+            - "null"
+            - string
+          description: Array of label IDs associated with the event
+      locked:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event is locked
+      locked_reason:
+        type:
+          - "null"
+          - string
+        description: Reason for locking the event
+      manage:
+        type:
+          - "null"
+          - boolean
+        description: Indicates whether the event is managed
+      note:
+        type:
+          - "null"
+          - string
+        description: Additional notes for the event
+      project:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: Information related to the project for the event
+        properties:
+          account_id:
             type:
               - "null"
               - integer
-          day:
-            description: Date of the event
+            description: ID of the account associated with the project
+          active:
             type:
               - "null"
-              - string
-            format: date
-          external_id:
-            description: External ID of the event
+              - boolean
+            description: Indicates whether the project is active
+          billable:
+            type:
+              - "null"
+              - boolean
+            description: Indicates whether the project is billable
+          budget:
             type:
               - "null"
               - integer
-          cost:
-            description: The cost associated with the event
+            description: Budget allocated for the project
+          budget_calculation:
             type:
               - "null"
-              - object
-            additionalProperties: true
-            properties:
-              amount:
-                description: The amount of the cost
-                type:
-                  - "null"
-                  - number
-              formatted:
-                description: The cost formatted as a string
-                type:
-                  - "null"
-                  - string
-              fractional:
-                description: The fractional part of the cost
-                type:
-                  - "null"
-                  - integer
-          billed_at:
-            description: Date and time when the event was billed
+              - string
+            description: Calculation method for project budget
+          budget_expired_on:
             type:
               - "null"
               - string
-            format: date-time
-            airbyte_type: timestamp_with_timezone
-          sequence:
-            description: Sequence number of the event
+            description: Date on which the project budget expires
+          budget_percent:
             type:
               - "null"
-              - integer
-          created_at:
-            description: Date and time when the event was created
+              - number
+            description: Percentage of budget utilized
+          budget_progress:
             type:
               - "null"
-              - integer
-          project:
-            description: Information related to the project for the event
+              - number
+            description: Progress of budget utilization
+          budget_scope:
+            type:
+              - "null"
+              - string
+            description: Scope of the project budget
+          budget_type:
+            type:
+              - "null"
+              - string
+            description: Type of budget assigned to the project
+          client:
             type:
               - "null"
               - object
             additionalProperties: true
+            description: Information about the client associated with the project
             properties:
-              required_label_ids:
-                description: IDs of labels required for the project
-                type:
-                  - "null"
-                  - array
-                items:
-                  description: Array of required label IDs for the project
-                  type:
-                    - "null"
-                    - string
-              labels:
-                description: Labels associated with the project
-                type:
-                  - "null"
-                  - array
-                items:
-                  description: Array of labels associated with the project
-                  type:
-                    - "null"
-                    - string
-              invoice_by_budget:
-                description: Indicates whether invoicing is based on budget
-                type:
-                  - "null"
-                  - boolean
-              budget_percent:
-                description: Percentage of budget utilized
-                type:
-                  - "null"
-                  - number
-              name:
-                description: Name of the project
-                type:
-                  - "null"
-                  - string
-              budget:
-                description: Budget allocated for the project
-                type:
-                  - "null"
-                  - integer
-              hour_rate:
-                description: Hourly rate for the project
-                type:
-                  - "null"
-                  - number
-              budget_scope:
-                description: Scope of the project budget
-                type:
-                  - "null"
-                  - string
-              budget_calculation:
-                description: Calculation method for project budget
-                type:
-                  - "null"
-                  - string
-              has_recurrence:
-                description: Indicates whether the project has a recurrence
-                type:
-                  - "null"
-                  - boolean
-              label_ids:
-                description: IDs related to project labels
-                type:
-                  - "null"
-                  - array
-                items:
-                  description: Array of label IDs associated with the project
-                  type:
-                    - "null"
-                    - string
-              enable_labels:
-                description: Indicates whether project labels are enabled
-                type:
-                  - "null"
-                  - string
-              required_labels:
-                description: Indicates whether labels are required for the project
-                type:
-                  - "null"
-                  - boolean
-              required_notes:
-                description: Indicates whether notes are required for the project
-                type:
-                  - "null"
-                  - boolean
-              client:
-                description: Information about the client associated with the project
-                type:
-                  - "null"
-                  - object
-                additionalProperties: true
-                properties:
-                  external_id:
-                    description: External ID of the client
-                    type:
-                      - "null"
-                      - string
-                  active:
-                    description: Indicates whether the client is active
-                    type:
-                      - "null"
-                      - boolean
-                  name:
-                    description: Name of the client
-                    type:
-                      - "null"
-                      - string
-                  updated_at:
-                    description: Date and time of client update
-                    type:
-                      - "null"
-                      - string
-                    format: date-time
-                    airbyte_type: timestamp_with_timezone
-                  id:
-                    description: ID of the client
-                    type:
-                      - "null"
-                      - integer
-              account_id:
-                description: ID of the account associated with the project
-                type:
-                  - "null"
-                  - integer
-              updated_at:
-                description: Date and time of project update
-                type:
-                  - "null"
-                  - integer
-              budget_progress:
-                description: Progress of budget utilization
-                type:
-                  - "null"
-                  - number
-              budget_expired_on:
-                description: Date on which the project budget expires
-                type:
-                  - "null"
-                  - string
-              external_id:
-                description: External ID of the project
-                type:
-                  - "null"
-                  - string
-              hour_rate_in_cents:
-                description: Hourly rate in cents for the project
-                type:
-                  - "null"
-                  - number
               active:
-                description: Indicates whether the project is active
                 type:
                   - "null"
                   - boolean
-              rate_type:
-                description: Type of rate for the project
-                type:
-                  - "null"
-                  - string
-              color:
-                description: Color associated with the project
-                type:
-                  - "null"
-                  - string
-              budget_type:
-                description: Type of budget assigned to the project
+                description: Indicates whether the client is active
+              external_id:
                 type:
                   - "null"
                   - string
-              billable:
-                description: Indicates whether the project is billable
-                type:
-                  - "null"
-                  - boolean
+                description: External ID of the client
               id:
-                description: ID of the project
                 type:
                   - "null"
                   - integer
-          user:
-            description: Information about the user associated with the event
-            type:
-              - "null"
-              - object
-            additionalProperties: true
-            properties:
+                description: ID of the client
               name:
-                description: Name of the user
-                type:
-                  - "null"
-                  - string
-              email:
-                description: Email address of the user
                 type:
                   - "null"
                   - string
+                description: Name of the client
               updated_at:
-                description: Date and time of user update
                 type:
                   - "null"
                   - string
-                format: date-time
                 airbyte_type: timestamp_with_timezone
-              avatar:
-                description: User's avatar information
-                type:
-                  - "null"
-                  - object
-                additionalProperties: true
-                properties:
-                  medium:
-                    description: URL of the medium avatar image
-                    type:
-                      - "null"
-                      - string
-                  medium_retina:
-                    description: URL of the medium retina avatar image
-                    type:
-                      - "null"
-                      - string
-                  timeline:
-                    description: URL of the timeline avatar image
-                    type:
-                      - "null"
-                      - string
-                  large:
-                    description: URL of the large avatar image
-                    type:
-                      - "null"
-                      - string
-                  large_retina:
-                    description: URL of the large retina avatar image
-                    type:
-                      - "null"
-                      - string
-              id:
-                description: ID of the user
-                type:
-                  - "null"
-                  - integer
-          estimated:
-            description: Indicates whether the event is estimated
+                description: Date and time of client update
+                format: date-time
+          color:
             type:
               - "null"
-              - boolean
-          note:
-            description: Additional notes for the event
+              - string
+            description: Color associated with the project
+          enable_labels:
             type:
               - "null"
               - string
-          estimated_duration:
-            description: The estimated duration of the event
+            description: Indicates whether project labels are enabled
+          external_id:
             type:
               - "null"
-              - object
-            additionalProperties: true
-            properties:
-              total_minutes:
-                description: Total estimated duration in minutes
-                type:
-                  - "null"
-                  - integer
-              total_seconds:
-                description: Total estimated duration in seconds
-                type:
-                  - "null"
-                  - integer
-              formatted:
-                description: Estimated duration formatted as a string
-                type:
-                  - "null"
-                  - string
-              total_hours:
-                description: Total estimated duration in hours
-                type:
-                  - "null"
-                  - number
-              seconds:
-                description: Estimated seconds component of the duration
-                type:
-                  - "null"
-                  - integer
-              minutes:
-                description: Estimated minutes component of the duration
-                type:
-                  - "null"
-                  - integer
-              hours:
-                description: Estimated hours component of the duration
-                type:
-                  - "null"
-                  - integer
-          draft:
-            description: Indicates whether the event is in draft mode
+              - string
+            description: External ID of the project
+          has_recurrence:
             type:
               - "null"
               - boolean
-          from:
-            description: Start date and time of the event
+            description: Indicates whether the project has a recurrence
+          hour_rate:
             type:
               - "null"
-              - string
-            format: date-time
-            airbyte_type: timestamp_with_timezone
-          uid:
-            description: Unique identifier of the event
+              - number
+            description: Hourly rate for the project
+          hour_rate_in_cents:
+            type:
+              - "null"
+              - number
+            description: Hourly rate in cents for the project
+          id:
+            type:
+              - "null"
+              - integer
+            description: ID of the project
+          invoice_by_budget:
+            type:
+              - "null"
+              - boolean
+            description: Indicates whether invoicing is based on budget
+          label_ids:
+            type:
+              - "null"
+              - array
+            description: IDs related to project labels
+            items:
+              type:
+                - "null"
+                - string
+              description: Array of label IDs associated with the project
+          labels:
+            type:
+              - "null"
+              - array
+            description: Labels associated with the project
+            items:
+              type:
+                - "null"
+                - string
+              description: Array of labels associated with the project
+          name:
             type:
               - "null"
               - string
-          timer_state:
-            description: State of the timer for the event
+            description: Name of the project
+          rate_type:
             type:
               - "null"
               - string
-          manage:
-            description: Indicates whether the event is managed
+            description: Type of rate for the project
+          required_label_ids:
+            type:
+              - "null"
+              - array
+            description: IDs of labels required for the project
+            items:
+              type:
+                - "null"
+                - string
+              description: Array of required label IDs for the project
+          required_labels:
             type:
               - "null"
               - boolean
-          id:
-            description: ID of the event
+            description: Indicates whether labels are required for the project
+          required_notes:
+            type:
+              - "null"
+              - boolean
+            description: Indicates whether notes are required for the project
+          updated_at:
             type:
               - "null"
               - integer
-          duration:
-            description: The duration of the event
+            description: Date and time of project update
+      sequence:
+        type:
+          - "null"
+          - integer
+        description: Sequence number of the event
+      state:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: State of the event
+      suggestion_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the suggestion associated with the event
+      timer_started_on:
+        type:
+          - "null"
+          - integer
+        description: Date and time when the timer was started
+      timer_state:
+        type:
+          - "null"
+          - string
+        description: State of the timer for the event
+      timer_stopped_on:
+        type:
+          - "null"
+          - integer
+        description: Date and time when the timer was stopped
+      timestamps:
+        type:
+          - "null"
+          - array
+        description: Timestamps related to the event
+        items:
+          type:
+            - "null"
+            - string
+          description: Array of timestamps associated with the event
+      to:
+        type:
+          - "null"
+          - string
+        airbyte_type: timestamp_with_timezone
+        description: End date and time of the event
+        format: date-time
+      uid:
+        type:
+          - "null"
+          - string
+        description: Unique identifier of the event
+      updated_at:
+        type:
+          - "null"
+          - integer
+        description: Date and time when the event was last updated
+      updated_from:
+        type:
+          - "null"
+          - string
+        description: Source from which the event was last updated
+      updater_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the user who last updated the event
+      user:
+        type:
+          - "null"
+          - object
+        additionalProperties: true
+        description: Information about the user associated with the event
+        properties:
+          avatar:
             type:
               - "null"
               - object
             additionalProperties: true
+            description: User's avatar information
             properties:
-              total_minutes:
-                description: Total duration in minutes
-                type:
-                  - "null"
-                  - integer
-              total_seconds:
-                description: Total duration in seconds
-                type:
-                  - "null"
-                  - integer
-              formatted:
-                description: Duration formatted as a string
+              large:
                 type:
                   - "null"
                   - string
-              total_hours:
-                description: Total duration in hours
-                type:
-                  - "null"
-                  - number
-              correctedHours:
-                description: Corrected hours of the event duration
+                description: URL of the large avatar image
+              large_retina:
                 type:
                   - "null"
-                  - integer
-              seconds:
-                description: Seconds component of the duration
+                  - string
+                description: URL of the large retina avatar image
+              medium:
                 type:
                   - "null"
-                  - integer
-              minutes:
-                description: Minutes component of the duration
+                  - string
+                description: URL of the medium avatar image
+              medium_retina:
                 type:
                   - "null"
-                  - integer
-              hours:
-                description: Hours component of the duration
+                  - string
+                description: URL of the medium retina avatar image
+              timeline:
                 type:
                   - "null"
-                  - integer
-          billed:
-            description: Indicates whether the event has been billed or not
-            type:
-              - "null"
-              - boolean
-          locked_reason:
-            description: Reason for locking the event
+                  - string
+                description: URL of the timeline avatar image
+          email:
             type:
               - "null"
               - string
-          entry_ids:
-            description: IDs related to the event entries
-            type:
-              - "null"
-              - array
-            items:
-              description: Array of entry IDs linked to the event
-              type:
-                - "null"
-                - string
-          hour_rate:
-            description: Hourly rate for the event
-            type:
-              - "null"
-              - number
-          updated_from:
-            description: Source from which the event was last updated
+            description: Email address of the user
+          id:
             type:
               - "null"
-              - string
-          created_from:
-            description: Source from which the event was created
+              - integer
+            description: ID of the user
+          name:
             type:
               - "null"
               - string
-          timer_started_on:
-            description: Date and time when the timer was started
-            type:
-              - "null"
-              - integer
+            description: Name of the user
           updated_at:
-            description: Date and time when the event was last updated
             type:
               - "null"
-              - integer
+              - string
+            airbyte_type: timestamp_with_timezone
+            description: Date and time of user update
+            format: date-time
+      user_ids:
+        type:
+          - "null"
+          - array
+        description: IDs related to users associated with the event
+        items:
+          type:
+            - "null"
+            - string
+          description: Array of user IDs linked to the event
```

### Comparing `airbyte_source_timely-0.3.4/PKG-INFO` & `airbyte_source_timely-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-timely
-Version: 0.3.4
+Version: 0.3.5
 Summary: Source implementation for Timely.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/timely
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Timely source connector
 
-
 This is the repository for the Timely source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/timely).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/timely)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_timely/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-timely spec
 poetry run source-timely check --config secrets/config.json
 poetry run source-timely discover --config secrets/config.json
 poetry run source-timely read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-timely build
 ```
 
 An image will be available on your host with the tag `airbyte/source-timely:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-timely:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-timely:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-timely:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-timely:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-timely test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-timely test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/timely.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

