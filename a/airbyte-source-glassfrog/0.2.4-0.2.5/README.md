# Comparing `tmp/airbyte_source_glassfrog-0.2.4.tar.gz` & `tmp/airbyte_source_glassfrog-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_glassfrog-0.2.4.tar", max compression
+gzip compressed data, was "airbyte_source_glassfrog-0.2.5.tar", max compression
```

## Comparing `airbyte_source_glassfrog-0.2.4.tar` & `airbyte_source_glassfrog-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4550 2024-05-01 18:44:14.558985 airbyte_source_glassfrog-0.2.4/README.md
--rw-r--r--   0        0        0      761 2024-05-01 18:47:25.862284 airbyte_source_glassfrog-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-01 18:44:14.558985 airbyte_source_glassfrog-0.2.4/source_glassfrog/__init__.py
--rw-r--r--   0        0        0    17607 2024-05-01 18:44:14.558985 airbyte_source_glassfrog-0.2.4/source_glassfrog/manifest.yaml
--rw-r--r--   0        0        0      239 2024-05-01 18:44:14.558985 airbyte_source_glassfrog-0.2.4/source_glassfrog/run.py
--rw-r--r--   0        0        0      478 2024-05-01 18:44:14.558985 airbyte_source_glassfrog-0.2.4/source_glassfrog/source.py
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 airbyte_source_glassfrog-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4560 2024-05-20 03:34:48.881964 airbyte_source_glassfrog-0.2.5/README.md
+-rw-r--r--   0        0        0      761 2024-05-20 03:38:23.670793 airbyte_source_glassfrog-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-20 03:34:48.881964 airbyte_source_glassfrog-0.2.5/source_glassfrog/__init__.py
+-rw-r--r--   0        0        0    18115 2024-05-20 03:34:48.881964 airbyte_source_glassfrog-0.2.5/source_glassfrog/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-20 03:34:48.881964 airbyte_source_glassfrog-0.2.5/source_glassfrog/run.py
+-rw-r--r--   0        0        0      478 2024-05-20 03:34:48.881964 airbyte_source_glassfrog-0.2.5/source_glassfrog/source.py
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 airbyte_source_glassfrog-0.2.5/PKG-INFO
```

### Comparing `airbyte_source_glassfrog-0.2.4/README.md` & `airbyte_source_glassfrog-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Glassfrog source connector
 
-
 This is the repository for the Glassfrog source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/glassfrog).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/glassfrog)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_glassfrog/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-glassfrog spec
 poetry run source-glassfrog check --config secrets/config.json
 poetry run source-glassfrog discover --config secrets/config.json
 poetry run source-glassfrog read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-glassfrog build
 ```
 
 An image will be available on your host with the tag `airbyte/source-glassfrog:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-glassfrog:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-glassfrog:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-glassfrog:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-glassfrog:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-glassfrog test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-glassfrog test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/glassfrog.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_glassfrog-0.2.4/pyproject.toml` & `airbyte_source_glassfrog-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.4"
+version = "0.2.5"
 name = "airbyte-source-glassfrog"
 description = "Source implementation for Glassfrog."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_glassfrog-0.2.4/source_glassfrog/manifest.yaml` & `airbyte_source_glassfrog-0.2.5/source_glassfrog/manifest.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,591 +1,667 @@
-version: "0.29.0"
+version: 0.78.5
+
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - assignments
 
 definitions:
-  selector:
-    type: RecordSelector
-    extractor:
-      type: DpathExtractor
-      field_path: ["{{ parameters.path}}"]
-  requester:
+  streams:
+    assignments:
+      type: DeclarativeStream
+      name: assignments
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: assignments
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - assignments
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/assignments"
+    checklist_items:
+      type: DeclarativeStream
+      name: checklist_items
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: checklist_items
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - checklist_items
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/checklist_items"
+    circles:
+      type: DeclarativeStream
+      name: circles
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: circles
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - circles
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/circles"
+    custom_fields:
+      type: DeclarativeStream
+      name: custom_fields
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: custom_fields
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - custom_fields
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/custom_fields"
+    metrics:
+      type: DeclarativeStream
+      name: metrics
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: metrics
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - metrics
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/metrics"
+    people:
+      type: DeclarativeStream
+      name: people
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: people
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - people
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/people"
+    projects:
+      type: DeclarativeStream
+      name: projects
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: projects
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - projects
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/projects"
+    roles:
+      type: DeclarativeStream
+      name: roles
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: roles
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - roles
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/roles"
+  base_requester:
     type: HttpRequester
-    url_base: "https://api.glassfrog.com/api/v3/"
-    http_method: "GET"
+    url_base: https://api.glassfrog.com/api/v3/
     authenticator:
       type: ApiKeyAuthenticator
-      header: "X-Auth-Token"
       api_token: "{{ config['api_key'] }}"
-  retriever:
-    type: SimpleRetriever
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: NoPagination
-    requester:
-      $ref: "#/definitions/requester"
-  base_stream:
-    type: DeclarativeStream
-    retriever:
-      $ref: "#/definitions/retriever"
+      inject_into:
+        type: RequestOption
+        field_name: X-Auth-Token
+        inject_into: header
+
+streams:
+  - $ref: "#/definitions/streams/assignments"
+  - $ref: "#/definitions/streams/checklist_items"
+  - $ref: "#/definitions/streams/circles"
+  - $ref: "#/definitions/streams/custom_fields"
+  - $ref: "#/definitions/streams/metrics"
+  - $ref: "#/definitions/streams/people"
+  - $ref: "#/definitions/streams/projects"
+  - $ref: "#/definitions/streams/roles"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - api_key
+    properties:
+      api_key:
+        type: string
+        title: API Key
+        airbyte_secret: true
+        description: API key provided by Glassfrog
+        order: 0
+    additionalProperties: true
 
-  assignments_stream:
-    $ref: "#/definitions/base_stream"
-    name: "assignments"
-    primary_key: "id"
-    $parameters:
-      path: "assignments"
+metadata:
+  autoImportSchema:
+    assignments: false
+    checklist_items: false
+    circles: false
+    custom_fields: false
+    metrics: false
+    people: false
+    projects: false
+    roles: false
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+schemas:
+  assignments:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      election:
+        type:
+          - "null"
+          - string
+        default: null
+        description: The election status of the assignment.
+      exclude_from_meetings:
+        type: boolean
+        default: false
+        description: Specifies if the assignment should be excluded from meetings.
+      focus:
+        type:
+          - "null"
+          - string
+        description: The focus of the assignment.
+      id:
+        type: integer
+        default: 0
+        description: The unique identifier of the assignment.
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: The related links associated with the assignment.
         properties:
-          id:
-            description: The unique identifier of the assignment.
-            type: integer
-            default: 0
-          election:
-            description: The election status of the assignment.
+          person:
             type:
               - "null"
-              - string
-            default:
-          exclude_from_meetings:
-            description: Specifies if the assignment should be excluded from meetings.
-            type: boolean
-            default: false
-          focus:
-            description: The focus of the assignment.
-            type:
-              - "null"
-              - string
-            default: ""
-          links:
-            description: The related links associated with the assignment.
-            type: object
-            default: {}
-            properties:
-              person:
-                description: Link to the person assigned to the role.
-                type:
-                  - "null"
-                  - integer
-                default:
-              role:
-                description: Link to the role assigned as part of the assignment.
-                type:
-                  - "null"
-                  - integer
-                default:
-  checklist_items_stream:
-    $ref: "#/definitions/base_stream"
-    name: "checklist_items"
-    primary_key: "id"
-    $parameters:
-      path: "checklist_items"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
-        type: object
-        additionalProperties: true
-        properties:
-          id:
-            description: The unique identifier of the checklist item.
-            type: integer
-            default: 0
-          description:
-            description: The description of the checklist item.
-            type: string
-            default: ""
-          frequency:
-            description: The frequency at which the checklist item needs to be completed.
-            type: string
-            default: ""
-          link:
-            description: A link related to the checklist item.
-            type: string
-            default: ""
-          global:
-            description: Indicates if the checklist item is global across all circles.
-            type: boolean
-            default: false
-          links:
-            description: Additional links related to the checklist item.
-            type: object
-            default: {}
-            properties:
-              circle:
-                description: The circle associated with the checklist item.
-                type:
-                  - "null"
-                  - integer
-                default:
-              role:
-                description: The role associated with the checklist item.
-                type:
-                  - "null"
-                  - integer
-                default:
-  circles_stream:
-    $ref: "#/definitions/base_stream"
-    name: "circles"
-    primary_key: "id"
-    $parameters:
-      path: "circles"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+              - integer
+            default: null
+            description: Link to the person assigned to the role.
+          role:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: Link to the role assigned as part of the assignment.
+  checklist_items:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      description:
+        type: string
+        description: The description of the checklist item.
+      frequency:
+        type: string
+        description: The frequency at which the checklist item needs to be completed.
+      global:
+        type: boolean
+        default: false
+        description: Indicates if the checklist item is global across all circles.
+      id:
+        type: integer
+        default: 0
+        description: The unique identifier of the checklist item.
+      link:
+        type: string
+        description: A link related to the checklist item.
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: Additional links related to the checklist item.
         properties:
-          id:
-            description: The unique identifier of the circle
-            type: integer
-            default: 0
-          name:
-            description: The name of the circle
-            type: string
-            default: ""
-          short_name:
-            description: The short name or abbreviation of the circle
-            type: string
-            default: ""
-          strategy:
-            description: The strategy or purpose behind the formation of the circle
-            type:
-              - "null"
-              - string
-            default:
-          organization_id:
-            description: The identifier of the organization to which the circle belongs
-            type: integer
-            default: 0
-          links:
-            description: Various links associated with the circle
-            type: object
-            default: {}
-            properties:
-              roles:
-                description: Link to the roles within the circle
-                type: array
-                default: []
-                items:
-                  type: integer
-              policies:
-                description: Link to the policies related to the circle
-                type: array
-                default: []
-                items:
-                  type: integer
-                  default: 0
-              domain:
-                description: Link to the domain associated with the circle
-                type: array
-                default: []
-                items:
-                  type: integer
-                  default: 0
-              supported_role:
-                description: Supporting role within the circle
-                type: integer
-                default: 0
-  custom_fields_stream:
-    $ref: "#/definitions/base_stream"
-    name: "custom_fields"
-    primary_key: "id"
-    $parameters:
-      path: "custom_fields"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+          circle:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: The circle associated with the checklist item.
+          role:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: The role associated with the checklist item.
+  circles:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      id:
+        type: integer
+        default: 0
+        description: The unique identifier of the circle
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: Various links associated with the circle
         properties:
-          id:
-            description: The unique identifier for the custom field entry.
+          domain:
+            type: array
+            default: []
+            description: Link to the domain associated with the circle
+            items:
+              type: integer
+              default: 0
+          policies:
+            type: array
+            default: []
+            description: Link to the policies related to the circle
+            items:
+              type: integer
+              default: 0
+          roles:
+            type: array
+            default: []
+            description: Link to the roles within the circle
+            items:
+              type: integer
+          supported_role:
             type: integer
             default: 0
-          field_name:
-            description: The name of the custom field.
-            type: string
-            default: ""
-          field_value:
-            description: The value associated with the custom field.
-            type: string
-            default: ""
-          links:
-            description: Additional links associated with the custom field entry.
-            type: object
-            default: {}
-            properties:
-              role:
-                description: The role associated with the custom field entry.
-                type:
-                  - "null"
-                  - integer
-                default:
-  metrics_stream:
-    $ref: "#/definitions/base_stream"
-    name: "metrics"
-    primary_key: "id"
-    $parameters:
-      path: "metrics"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+            description: Supporting role within the circle
+      name:
+        type: string
+        description: The name of the circle
+      organization_id:
+        type: integer
+        default: 0
+        description: The identifier of the organization to which the circle belongs
+      short_name:
+        type: string
+        description: The short name or abbreviation of the circle
+      strategy:
+        type:
+          - "null"
+          - string
+        default: null
+        description: The strategy or purpose behind the formation of the circle
+  custom_fields:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      field_name:
+        type: string
+        description: The name of the custom field.
+      field_value:
+        type: string
+        description: The value associated with the custom field.
+      id:
+        type: integer
+        default: 0
+        description: The unique identifier for the custom field entry.
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: Additional links associated with the custom field entry.
         properties:
-          id:
-            description: Unique identifier for the metric data
-            type: integer
-            default: 0
-          description:
-            description: Description of the metric data
-            type: string
-            default: ""
-          frequency:
-            description:
-              The frequency at which the metric is recorded (e.g., daily,
-              weekly)
-            type: string
-            default: ""
-          link:
-            description: Related link for more information about the metric
-            type: string
-            default: ""
-          global:
-            description:
-              Indicates whether the metric data is global or specific to
-              a particular entity
-            type: boolean
-            default: false
-          links:
-            description: Additional related links
-            type: object
-            default: {}
-            properties:
-              role:
-                description: Link to the role associated with the metric
-                type:
-                  - "null"
-                  - integer
-                default:
-              circle:
-                description: Link to the circle associated with the metric
-                type:
-                  - "null"
-                  - integer
-                default:
-  people_stream:
-    $ref: "#/definitions/base_stream"
-    name: "people"
-    primary_key: "id"
-    $parameters:
-      path: "people"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+          role:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: The role associated with the custom field entry.
+  metrics:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      description:
+        type: string
+        description: Description of the metric data
+      frequency:
+        type: string
+        description: The frequency at which the metric is recorded (e.g., daily, weekly)
+      global:
+        type: boolean
+        default: false
+        description: >-
+          Indicates whether the metric data is global or specific to a
+          particular entity
+      id:
+        type: integer
+        default: 0
+        description: Unique identifier for the metric data
+      link:
+        type: string
+        description: Related link for more information about the metric
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: Additional related links
         properties:
-          id:
-            description: The unique identifier of the person.
+          circle:
             type:
               - "null"
               - integer
-          tag_names:
-            description: List of tag names associated with the person.
+            default: null
+            description: Link to the circle associated with the metric
+          role:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: Link to the role associated with the metric
+  people:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      email:
+        type:
+          - "null"
+          - string
+        description: The email address of the person.
+      external_id:
+        type:
+          - "null"
+          - integer
+        description: The unique external identifier of the person.
+      id:
+        type:
+          - "null"
+          - integer
+        description: The unique identifier of the person.
+      links:
+        type:
+          - "null"
+          - object
+        description: Links related to the person.
+        properties:
+          circles:
             type:
               - "null"
               - array
+            description: List of circles the person is part of.
             items:
               type:
                 - "null"
-                - string
-          name:
-            description: The name of the person.
-            type:
-              - "null"
-              - string
-          settings:
-            description: Settings or preferences of the person.
-            type:
-              - "null"
-              - object
-          email:
-            description: The email address of the person.
-            type:
-              - "null"
-              - string
-          external_id:
-            description: The unique external identifier of the person.
+                - integer
+          organization_ids:
             type:
               - "null"
-              - integer
-          links:
-            description: Links related to the person.
-            type:
-              - "null"
-              - object
-            properties:
-              circles:
-                description: List of circles the person is part of.
-                type:
-                  - "null"
-                  - array
-                items:
-                  type:
-                    - "null"
-                    - integer
-              organization_ids:
-                description: List of organization IDs associated with the person.
-                type:
-                  - "null"
-                  - array
-                items:
-                  type:
-                    - "null"
-                    - integer
-  projects_stream:
-    $ref: "#/definitions/base_stream"
-    name: "projects"
-    primary_key: "id"
-    $parameters:
-      path: "projects"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+              - array
+            description: List of organization IDs associated with the person.
+            items:
+              type:
+                - "null"
+                - integer
+      name:
+        type:
+          - "null"
+          - string
+        description: The name of the person.
+      settings:
+        type:
+          - "null"
+          - object
+        description: Settings or preferences of the person.
+      tag_names:
+        type:
+          - "null"
+          - array
+        description: List of tag names associated with the person.
+        items:
+          type:
+            - "null"
+            - string
+  projects:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      type:
+        type: string
+        description: The type or category of the project.
+      archived_at:
+        type:
+          - "null"
+          - string
+        default: null
+        description: The date and time when the project was archived.
+        format: date-time
+      created_at:
+        type: string
+        description: The date and time when the project was created.
+        format: date-time
+      description:
+        type: string
+        description: A brief description of the project.
+      effort:
+        type:
+          - "null"
+          - integer
+        default: null
+        description: The effort or resources required for the project.
+      id:
+        type: integer
+        default: 0
+        description: The unique identifier of the project.
+      link:
+        type:
+          - "null"
+          - string
+        default: null
+        description: A link associated with the project.
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: Links to other related entities.
         properties:
-          id:
-            description: The unique identifier of the project.
-            type: integer
-            default: 0
-          description:
-            description: A brief description of the project.
-            type: string
-            default: ""
-          status:
-            description: The current status of the project.
-            type: string
-            default: ""
-          waiting_on_who:
-            description: Specifies who the project is waiting on.
-            type:
-              - "null"
-              - string
-            default:
-          waiting_on_what:
-            description: Specifies what the project is waiting on.
-            type:
-              - "null"
-              - string
-            default:
-          link:
-            description: A link associated with the project.
-            type:
-              - "null"
-              - string
-            default:
-          value:
-            description: The estimated value or impact of the project.
+          circle:
             type:
               - "null"
               - integer
-            default:
-          effort:
-            description: The effort or resources required for the project.
+            default: null
+            description: Link to the circle associated with the project.
+          person:
             type:
               - "null"
               - integer
-            default:
-          roi:
-            description: Return on investment (ROI) for the project.
+            default: null
+            description: Link to the person associated with the project.
+          role:
             type:
               - "null"
-              - number
-            default:
-          private_to_circle:
-            description: Indicates if the project is private to the circle.
-            type: boolean
-            default: false
-          created_at:
-            description: The date and time when the project was created.
-            type: string
-            format: date-time
-            default: ""
-          archived_at:
-            description: The date and time when the project was archived.
-            type:
-              - "null"
-              - string
-            format: date-time
-            default:
-          type:
-            description: The type or category of the project.
-            type: string
-            default: ""
-          links:
-            description: Links to other related entities.
-            type: object
-            default: {}
-            properties:
-              role:
-                description: Link to the role associated with the project.
-                type:
-                  - "null"
-                  - integer
-                default:
-              person:
-                description: Link to the person associated with the project.
-                type:
-                  - "null"
-                  - integer
-                default:
-              circle:
-                description: Link to the circle associated with the project.
-                type:
-                  - "null"
-                  - integer
-                default:
-  roles_stream:
-    $ref: "#/definitions/base_stream"
-    name: "roles"
-    primary_key: "id"
-    $parameters:
-      path: "roles"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: https://json-schema.org/draft-07/schema
+              - integer
+            default: null
+            description: Link to the role associated with the project.
+      private_to_circle:
+        type: boolean
+        default: false
+        description: Indicates if the project is private to the circle.
+      roi:
+        type:
+          - "null"
+          - number
+        default: null
+        description: Return on investment (ROI) for the project.
+      status:
+        type: string
+        description: The current status of the project.
+      value:
+        type:
+          - "null"
+          - integer
+        default: null
+        description: The estimated value or impact of the project.
+      waiting_on_what:
+        type:
+          - "null"
+          - string
+        default: null
+        description: Specifies what the project is waiting on.
+      waiting_on_who:
+        type:
+          - "null"
+          - string
+        default: null
+        description: Specifies who the project is waiting on.
+  roles:
+    type: object
+    $schema: https://json-schema.org/draft-07/schema
+    additionalProperties: true
+    properties:
+      elected_until:
+        type:
+          - "null"
+          - string
+        default: null
+        description: Date until the role is elected for
+        format: date
+      id:
+        type: integer
+        default: 0
+        description: Unique identifier for the role
+      is_core:
+        type: boolean
+        default: false
+        description: Flag indicating if the role is a core role within the circle
+      links:
         type: object
-        additionalProperties: true
+        default: {}
+        description: Related links for the role
         properties:
-          id:
-            description: Unique identifier for the role
-            type: integer
-            default: 0
-          tag_names:
-            description: List of tags associated with the role
+          accountabilities:
             type: array
             default: []
+            description: List of accountabilities associated with the role
             items:
-              type: string
-              default: ""
-          name:
-            description: Name of the role
-            type: string
-            default: ""
-          is_core:
-            description: Flag indicating if the role is a core role within the circle
-            type: boolean
-            default: false
-          name_with_circle_for_core_roles:
-            description: Combination of role name and circle name for core roles
-            type: string
-            default: ""
-          purpose:
-            description: Purpose or objective of the role
-            type: string
-            default: ""
-          elected_until:
-            description: Date until the role is elected for
-            type:
-              - "null"
-              - string
-            format: date
-            default:
-          organization_id:
-            description: Unique identifier for the organization
-            type: integer
-            default: 0
-          links:
-            description: Related links for the role
-            type: object
-            default: {}
-            properties:
-              circle:
-                description: Circle to which the role belongs
-                type:
-                  - "null"
-                  - integer
-                default:
-              supporting_circle:
-                description: Supporting circle for the role if applicable
-                type:
-                  - "null"
-                  - integer
-                default:
-              domains:
-                description: List of domains in which the role operates
-                type: array
-                default: []
-                items:
-                  type:
-                    - "null"
-                    - integer
-                  default:
-              accountabilities:
-                description: List of accountabilities associated with the role
-                type: array
-                default: []
-                items:
-                  type:
-                    - "null"
-                    - integer
-                  default:
-              people:
-                description: List of people assigned to the role
-                type: array
-                default: []
-                items:
-                  type:
-                    - "null"
-                    - integer
-                  default:
-streams:
-  - "#/definitions/assignments_stream"
-  - "#/definitions/checklist_items_stream"
-  - "#/definitions/circles_stream"
-  - "#/definitions/custom_fields_stream"
-  - "#/definitions/metrics_stream"
-  - "#/definitions/people_stream"
-  - "#/definitions/projects_stream"
-  - "#/definitions/roles_stream"
-
-check:
-  type: CheckStream
-  stream_names:
-    - "assignments"
-
-spec:
-  type: Spec
-  documentationUrl: https://docs.airbyte.com/integrations/sources/glassfrog
-  connection_specification:
-    $schema: http://json-schema.org/draft-07/schema#
-    title: Glassfrog Spec
-    type: object
-    required:
-      - api_key
-    additionalProperties: true
-    properties:
-      api_key:
+              type:
+                - "null"
+                - integer
+              default: null
+          circle:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: Circle to which the role belongs
+          domains:
+            type: array
+            default: []
+            description: List of domains in which the role operates
+            items:
+              type:
+                - "null"
+                - integer
+              default: null
+          people:
+            type: array
+            default: []
+            description: List of people assigned to the role
+            items:
+              type:
+                - "null"
+                - integer
+              default: null
+          supporting_circle:
+            type:
+              - "null"
+              - integer
+            default: null
+            description: Supporting circle for the role if applicable
+      name:
         type: string
-        description: API key provided by Glassfrog
-        airbyte_secret: true
+        description: Name of the role
+      name_with_circle_for_core_roles:
+        type: string
+        description: Combination of role name and circle name for core roles
+      organization_id:
+        type: integer
+        default: 0
+        description: Unique identifier for the organization
+      purpose:
+        type: string
+        description: Purpose or objective of the role
+      tag_names:
+        type: array
+        default: []
+        description: List of tags associated with the role
+        items:
+          type: string
```

### Comparing `airbyte_source_glassfrog-0.2.4/PKG-INFO` & `airbyte_source_glassfrog-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-glassfrog
-Version: 0.2.4
+Version: 0.2.5
 Summary: Source implementation for Glassfrog.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/glassfrog
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Glassfrog source connector
 
-
 This is the repository for the Glassfrog source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/glassfrog).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/glassfrog)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_glassfrog/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-glassfrog spec
 poetry run source-glassfrog check --config secrets/config.json
 poetry run source-glassfrog discover --config secrets/config.json
 poetry run source-glassfrog read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-glassfrog build
 ```
 
 An image will be available on your host with the tag `airbyte/source-glassfrog:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-glassfrog:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-glassfrog:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-glassfrog:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-glassfrog:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-glassfrog test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-glassfrog test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/glassfrog.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

