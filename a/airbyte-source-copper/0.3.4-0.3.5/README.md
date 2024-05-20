# Comparing `tmp/airbyte_source_copper-0.3.4.tar.gz` & `tmp/airbyte_source_copper-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_copper-0.3.4.tar", max compression
+gzip compressed data, was "airbyte_source_copper-0.3.5.tar", max compression
```

## Comparing `airbyte_source_copper-0.3.4.tar` & `airbyte_source_copper-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4496 2024-05-01 18:34:32.580011 airbyte_source_copper-0.3.4/README.md
--rw-r--r--   0        0        0      718 2024-05-01 18:38:11.562550 airbyte_source_copper-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-01 18:34:32.580011 airbyte_source_copper-0.3.4/source_copper/__init__.py
--rw-r--r--   0        0        0    20492 2024-05-01 18:34:32.580011 airbyte_source_copper-0.3.4/source_copper/manifest.yaml
--rw-r--r--   0        0        0      230 2024-05-01 18:34:32.580011 airbyte_source_copper-0.3.4/source_copper/run.py
--rw-r--r--   0        0        0      475 2024-05-01 18:34:32.580011 airbyte_source_copper-0.3.4/source_copper/source.py
--rw-r--r--   0        0        0      470 2024-05-01 18:34:32.580011 airbyte_source_copper-0.3.4/source_copper/spec.yaml
--rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 airbyte_source_copper-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     4506 2024-05-20 03:36:24.129421 airbyte_source_copper-0.3.5/README.md
+-rw-r--r--   0        0        0      718 2024-05-20 03:40:01.774551 airbyte_source_copper-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-20 03:36:24.129421 airbyte_source_copper-0.3.5/source_copper/__init__.py
+-rw-r--r--   0        0        0    21472 2024-05-20 03:36:24.129421 airbyte_source_copper-0.3.5/source_copper/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-05-20 03:36:24.129421 airbyte_source_copper-0.3.5/source_copper/run.py
+-rw-r--r--   0        0        0      475 2024-05-20 03:36:24.129421 airbyte_source_copper-0.3.5/source_copper/source.py
+-rw-r--r--   0        0        0     5210 1970-01-01 00:00:00.000000 airbyte_source_copper-0.3.5/PKG-INFO
```

### Comparing `airbyte_source_copper-0.3.4/README.md` & `airbyte_source_copper-0.3.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Copper source connector
 
-
 This is the repository for the Copper source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/copper).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/copper)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_copper/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-copper spec
 poetry run source-copper check --config secrets/config.json
 poetry run source-copper discover --config secrets/config.json
 poetry run source-copper read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-copper build
 ```
 
 An image will be available on your host with the tag `airbyte/source-copper:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-copper:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-copper:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-copper:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-copper:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-copper test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-copper test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/copper.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_copper-0.3.4/pyproject.toml` & `airbyte_source_copper-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

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
 name = "airbyte-source-copper"
 description = "Source implementation for Copper."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_copper-0.3.4/source_copper/manifest.yaml` & `airbyte_source_copper-0.3.5/source_copper/manifest.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,683 +1,788 @@
-version: "0.29.0"
+version: 0.78.5
+
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - people
 
 definitions:
-  selector:
-    type: RecordSelector
-    extractor:
-      type: DpathExtractor
-      field_path: []
-  requester:
+  streams:
+    people:
+      type: DeclarativeStream
+      name: people
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: people/search
+          http_method: POST
+          request_headers:
+            X-PW-UserEmail: "{{ config['user_email'] }}"
+            X-PW-Application: developer_api
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
+            field_name: page_number
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page_size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 200
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
+          path: projects/search
+          http_method: POST
+          request_headers:
+            X-PW-UserEmail: "{{ config['user_email'] }}"
+            X-PW-Application: developer_api
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
+            field_name: page_number
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page_size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 200
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/projects"
+    companies:
+      type: DeclarativeStream
+      name: companies
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: companies/search
+          http_method: POST
+          request_headers:
+            X-PW-UserEmail: "{{ config['user_email'] }}"
+            X-PW-Application: developer_api
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
+            field_name: page_number
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page_size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 200
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/companies"
+    opportunities:
+      type: DeclarativeStream
+      name: opportunities
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: opportunities/search
+          http_method: POST
+          request_headers:
+            X-PW-UserEmail: "{{ config['user_email'] }}"
+            X-PW-Application: developer_api
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
+            field_name: page_number
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page_size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 200
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/opportunities"
+  base_requester:
     type: HttpRequester
-    url_base: "https://api.copper.com/developer_api/v1/"
-    http_method: "POST"
+    url_base: https://api.copper.com/developer_api/v1/
     authenticator:
-      type: "ApiKeyAuthenticator"
-      header: "X-PW-AccessToken"
+      type: ApiKeyAuthenticator
       api_token: "{{ config['api_key'] }}"
-    request_headers:
-      X-PW-UserEmail: "{{ config['user_email'] }}"
-      X-PW-Application: "developer_api"
+      inject_into:
+        type: RequestOption
+        field_name: X-PW-AccessToken
+        inject_into: header
 
-  retriever:
-    type: SimpleRetriever
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: "DefaultPaginator"
-      page_size_option:
-        type: "RequestOption"
-        inject_into: "request_parameter"
-        field_name: "page_size"
-      pagination_strategy:
-        type: "PageIncrement"
-        page_size: 200
-      page_token_option:
-        type: "RequestOption"
-        inject_into: "request_parameter"
-        field_name: "page_number"
-    requester:
-      $ref: "#/definitions/requester"
+streams:
+  - $ref: "#/definitions/streams/people"
+  - $ref: "#/definitions/streams/projects"
+  - $ref: "#/definitions/streams/companies"
+  - $ref: "#/definitions/streams/opportunities"
 
-  base_stream:
-    type: DeclarativeStream
-    retriever:
-      $ref: "#/definitions/retriever"
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - api_key
+      - user_email
+    properties:
+      api_key:
+        type: string
+        title: API Key
+        airbyte_secret: true
+        description: Copper API key
+        order: 0
+      user_email:
+        type: string
+        title: User email
+        description: user email used to login in to Copper
+        order: 1
+    additionalProperties: true
 
-  people_stream:
-    $ref: "#/definitions/base_stream"
-    name: "people"
-    primary_key: "id"
-    $parameters:
-      path: "people/search"
+metadata:
+  autoImportSchema:
+    people: false
+    projects: false
+    companies: false
+    opportunities: false
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-04/schema#
-        type: object
-        additionalProperties: true
+schemas:
+  people:
+    type: object
+    $schema: http://json-schema.org/draft-04/schema#
+    additionalProperties: true
+    properties:
+      address:
+        type:
+          - "null"
+          - object
+        description: Physical address details of the person
         properties:
-          id:
-            description: Unique identifier for the person record.
-            type:
-              - "null"
-              - integer
-          name:
-            description: The full name of the person.
+          city:
             type:
-              - "null"
               - string
-          socials:
-            description: Social media profiles of the person
-            type:
-              - "null"
-              - array
-            properties:
-              note:
-                description:
-                  Notes or additional information about the person's social
-                  profiles.
-                type:
-                  - "null"
-                  - string
-          leads_converted_from:
-            description: Details of leads converted to the person
-            type:
-              - "null"
-              - array
-            properties:
-              leads:
-                description:
-                  Information about leads that were converted into this
-                  person record.
-                type:
-                  - "null"
-                  - string
-          tags:
-            description: Tags or labels assigned to the person
-            type:
-              - "null"
-              - array
-            properties:
-              sticker:
-                description:
-                  Tags or labels associated with the person for categorization
-                  or identification.
-                type:
-                  - "null"
-                  - string
-          custom_fields:
-            description: Additional custom fields related to the person
-            type:
               - "null"
-              - array
-            properties:
-              mprc:
-                description: Custom field for specific data related to the person.
-                type:
-                  - "null"
-                  - string
-          prefix:
-            description:
-              A title or honorific preceding the person's name (e.g., Mr.,
-              Dr., etc.).
+            description: The city where the person resides.
+          country:
             type:
-              - "null"
               - string
-          first_name:
-            description: The first name of the person.
-            type:
               - "null"
-              - string
-          middle_name:
-            description: The middle name of the person.
+            description: The country where the person resides.
+          postal_code:
             type:
-              - "null"
               - string
-          last_name:
-            description: The last name of the person.
-            type:
               - "null"
-              - string
-          suffix:
-            description:
-              A title or honorific following the person's name (e.g., Jr.,
-              III, etc.).
+            description: The postal code of the person's address.
+          state:
             type:
-              - "null"
               - string
-          address:
-            description: Physical address details of the person
-            type:
-              - "null"
-              - object
-            properties:
-              street:
-                description: The street address of the person.
-                type:
-                  - "null"
-                  - string
-              city:
-                description: The city where the person resides.
-                type:
-                  - string
-                  - "null"
-              state:
-                description: The state or region where the person resides.
-                type:
-                  - string
-                  - "null"
-              postal_code:
-                description: The postal code of the person's address.
-                type:
-                  - string
-                  - "null"
-              country:
-                description: The country where the person resides.
-                type:
-                  - string
-                  - "null"
-          assignee_id:
-            description: ID of the assigned user or team.
-            type:
-              - "null"
-              - integer
-          company_id:
-            description: ID of the company to which the person belongs.
-            type:
               - "null"
-              - integer
-          company_name:
-            description: The name of the company the person is associated with.
+            description: The state or region where the person resides.
+          street:
             type:
               - "null"
               - string
-          contact_type_id:
-            description: ID representing the type of contact (e.g., client, prospect).
-            type:
-              - "null"
-              - integer
-          details:
-            description: Additional details or notes about the person.
-            type: "null"
-          emails:
-            description: Email addresses associated with the person
+            description: The street address of the person.
+      assignee_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the assigned user or team.
+      company_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the company to which the person belongs.
+      company_name:
+        type:
+          - "null"
+          - string
+        description: The name of the company the person is associated with.
+      contact_type_id:
+        type:
+          - "null"
+          - integer
+        description: ID representing the type of contact (e.g., client, prospect).
+      custom_fields:
+        type:
+          - "null"
+          - array
+        description: Additional custom fields related to the person
+        properties:
+          mprc:
             type:
               - "null"
-              - array
-            items:
+              - string
+            description: Custom field for specific data related to the person.
+      date_created:
+        type:
+          - "null"
+          - integer
+        description: The date when the person record was created.
+      date_last_contacted:
+        type:
+          - "null"
+          - integer
+        description: The date of the last contact or interaction with the person.
+      date_lead_created:
+        type:
+          - "null"
+          - integer
+        description: The date when the person was identified as a lead.
+      date_modified:
+        type:
+          - "null"
+          - integer
+        description: The date when the person record was last updated.
+      details:
+        type: "null"
+        description: Additional details or notes about the person.
+      emails:
+        type:
+          - "null"
+          - array
+        description: Email addresses associated with the person
+        items:
+          type:
+            - "null"
+            - object
+          properties:
+            category:
               type:
                 - "null"
-                - object
-              properties:
-                category:
-                  description:
-                    The category or type of email address (e.g., work,
-                    personal, etc.).
-                  type:
-                    - "null"
-                    - string
-                email:
-                  description: The email address of the person.
-                  type:
-                    - "null"
-                    - string
-          phone_numbers:
-            description: Phone numbers associated with the person
-            type:
-              - "null"
-              - array
-            items:
+                - string
+              description: >-
+                The category or type of email address (e.g., work, personal,
+                etc.).
+            email:
               type:
                 - "null"
-                - object
-              properties:
-                number:
-                  description: The phone number of the person.
-                  type:
-                    - "null"
-                    - string
-                category:
-                  description:
-                    The category or type of phone number (e.g., mobile,
-                    office, etc.).
-                  type:
-                    - "null"
-                    - string
-          title:
-            description: The job title or role of the person.
+                - string
+              description: The email address of the person.
+      first_name:
+        type:
+          - "null"
+          - string
+        description: The first name of the person.
+      id:
+        type:
+          - "null"
+          - integer
+        description: Unique identifier for the person record.
+      interaction_count:
+        type:
+          - "null"
+          - integer
+        description: The total number of interactions with the person.
+      last_name:
+        type:
+          - "null"
+          - string
+        description: The last name of the person.
+      leads_converted_from:
+        type:
+          - "null"
+          - array
+        description: Details of leads converted to the person
+        properties:
+          leads:
             type:
               - "null"
               - string
-          websites:
-            description: Websites associated with the person
-            type:
-              - "null"
-              - array
-            items:
+            description: >-
+              Information about leads that were converted into this person
+              record.
+      middle_name:
+        type:
+          - "null"
+          - string
+        description: The middle name of the person.
+      name:
+        type:
+          - "null"
+          - string
+        description: The full name of the person.
+      phone_numbers:
+        type:
+          - "null"
+          - array
+        description: Phone numbers associated with the person
+        items:
+          type:
+            - "null"
+            - object
+          properties:
+            category:
               type:
                 - "null"
-                - object
-              properties:
-                url:
-                  description: The URL of a website associated with the person.
-                  type:
-                    - "null"
-                    - string
-                category:
-                  description:
-                    The category or type of website URL (e.g., personal,
-                    company, etc.).
-                  type:
-                    - "null"
-                    - string
-          date_created:
-            description: The date when the person record was created.
-            type:
-              - "null"
-              - integer
-          date_modified:
-            description: The date when the person record was last updated.
-            type:
-              - "null"
-              - integer
-          date_last_contacted:
-            description: The date of the last contact or interaction with the person.
-            type:
-              - "null"
-              - integer
-          interaction_count:
-            description: The total number of interactions with the person.
-            type:
-              - "null"
-              - integer
-          date_lead_created:
-            description: The date when the person was identified as a lead.
-            type:
-              - "null"
-              - integer
-        required:
-          - id
-  projects_stream:
-    $ref: "#/definitions/base_stream"
-    name: "projects"
-    primary_key: "id"
-    $parameters:
-      path: "projects/search"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-04/schema#
+                - string
+              description: >-
+                The category or type of phone number (e.g., mobile, office,
+                etc.).
+            number:
+              type:
+                - "null"
+                - string
+              description: The phone number of the person.
+      prefix:
         type:
           - "null"
-          - object
-        additionalProperties: true
+          - string
+        description: >-
+          A title or honorific preceding the person's name (e.g., Mr., Dr.,
+          etc.).
+      socials:
+        type:
+          - "null"
+          - array
+        description: Social media profiles of the person
         properties:
-          id:
-            description: The unique identifier of the project.
-            type:
-              - "null"
-              - integer
-          name:
-            description: The name or title of the project.
-            type:
-              - "null"
-              - string
-          tags:
-            description: Tags associated with the project for categorization.
-            type:
-              - "null"
-              - array
-            properties:
-              sticker:
-                description: Tag associated with the project (e.g., priority, category).
-                type:
-                  - "null"
-                  - string
-          custom_fields:
-            description: Custom fields specific to each project.
-            type:
-              - "null"
-              - array
-            properties:
-              mprc:
-                description:
-                  Custom field representing the main project requirement
-                  criteria.
-                type:
-                  - "null"
-                  - string
-          related_resource:
-            description: Reference to any related resource linked to the project.
+          note:
             type:
               - "null"
               - string
-          assignee_id:
-            description: The unique identifier of the user assigned to the project.
-            type:
-              - "null"
-              - integer
-          status:
-            description: The current status of the project.
-            type:
-              - "null"
-              - string
-          details:
-            description: Additional details or description of the project.
-            type:
-              - "null"
-              - string
-          date_created:
-            description: The date when the project was created.
-            type:
-              - "null"
-              - integer
-          date_modified:
-            description: The date when the project was last modified.
-            type:
-              - "null"
-              - integer
-  companies_stream:
-    $ref: "#/definitions/base_stream"
-    name: "companies"
-    primary_key: "id"
-    $parameters:
-      path: "companies/search"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-04/schema#
-        type: object
-        additionalProperties: true
+            description: >-
+              Notes or additional information about the person's social
+              profiles.
+      suffix:
+        type:
+          - "null"
+          - string
+        description: >-
+          A title or honorific following the person's name (e.g., Jr., III,
+          etc.).
+      tags:
+        type:
+          - "null"
+          - array
+        description: Tags or labels assigned to the person
         properties:
-          id:
-            description: Unique identifier for the company
-            type:
-              - "null"
-              - integer
-          phone_numbers:
-            description: Phone numbers associated with the company
-            type:
-              - "null"
-              - array
-            properties:
-              category:
-                description: Category of the phone number
-                type:
-                  - "null"
-                  - string
-              number:
-                description: Phone number
-                type:
-                  - "null"
-                  - string
-          custom_fields:
-            description: Custom fields associated with the company
-            type:
-              - "null"
-              - array
-            properties:
-              mpc:
-                description: Custom field for a specific attribute
-                type:
-                  - "null"
-                  - string
-          name:
-            description: Name of the company
-            type:
-              - "null"
-              - string
-          address:
-            description: Company address details
-            type: object
-            properties:
-              street:
-                description: Street address of the company
-                type:
-                  - "null"
-                  - string
-              city:
-                description: City of the company address
-                type:
-                  - "null"
-                  - string
-              state:
-                description: State of the company address
-                type:
-                  - "null"
-                  - string
-              postal_code:
-                description: Postal code of the company address
-                type:
-                  - "null"
-                  - string
-              country:
-                description: Country of the company address
-                type:
-                  - "null"
-                  - string
-          assignee_id:
-            description: ID of the assignee for the company
-            type:
-              - "null"
-              - integer
-          contact_type_id:
-            description: ID representing the contact type
-            type:
-              - "null"
-              - integer
-          details:
-            description: Additional details about the company
-            type:
-              - "null"
-              - string
-          email_domain:
-            description: Email domain associated with the company
-            type:
-              - "null"
-              - string
-          socials:
-            description: Social media profiles associated with the company
-            type:
-              - "null"
-              - array
-            items:
-              type: object
-              properties:
-                url:
-                  description: URL of the social media profile
-                  type:
-                    - "null"
-                    - string
-                category:
-                  description: Category of the social media profile
-                  type:
-                    - "null"
-                    - string
-          tags:
-            description: Tags associated with the company
-            type:
-              - "null"
-              - array
-            items:
-              description: Tag item
-          websites:
-            description: Websites associated with the company
+          sticker:
             type:
               - "null"
-              - array
-            items:
+              - string
+            description: >-
+              Tags or labels associated with the person for categorization or
+              identification.
+      title:
+        type:
+          - "null"
+          - string
+        description: The job title or role of the person.
+      websites:
+        type:
+          - "null"
+          - array
+        description: Websites associated with the person
+        items:
+          type:
+            - "null"
+            - object
+          properties:
+            category:
               type:
-                - object
                 - "null"
-              properties:
-                url:
-                  description: URL of the website
-                  type:
-                    - "null"
-                    - string
-                category:
-                  description: Category of the website
-                  type:
-                    - "null"
-                    - string
-          interaction_count:
-            description: Count of interactions with the company
-            type:
-              - "null"
-              - integer
-          date_created:
-            description: Date when the company record was created
-            type:
-              - "null"
-              - integer
-          date_modified:
-            description: Date when the company record was last modified
-            type:
-              - "null"
-              - integer
-  opportunities_stream:
-    $ref: "#/definitions/base_stream"
-    name: "opportunities"
-    primary_key: "id"
-    $parameters:
-      path: "opportunities/search"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
-        additionalProperties: true
+                - string
+              description: >-
+                The category or type of website URL (e.g., personal, company,
+                etc.).
+            url:
+              type:
+                - "null"
+                - string
+              description: The URL of a website associated with the person.
+    required:
+      - id
+  projects:
+    type:
+      - "null"
+      - object
+    $schema: http://json-schema.org/draft-04/schema#
+    additionalProperties: true
+    path: projects/search
+    properties:
+      assignee_id:
+        type:
+          - "null"
+          - integer
+        description: The unique identifier of the user assigned to the project.
+      custom_fields:
+        type:
+          - "null"
+          - array
+        description: Custom fields specific to each project.
         properties:
-          id:
-            description: The unique identifier of the opportunity.
-            type:
-              - "null"
-              - integer
-          name:
-            description: The name or title of the opportunity.
-            type:
-              - "null"
-              - string
-          assignee_id:
-            description: The unique identifier of the user assigned to this opportunity.
-            type:
-              - "null"
-              - number
-          close_date:
-            description: The expected or actual closing date of the opportunity.
-            type:
-              - "null"
-              - string
-          company_id:
-            description:
-              The unique identifier of the company associated with this
-              opportunity.
+          mprc:
             type:
               - "null"
               - string
-          company_name:
-            description: The name of the company associated with this opportunity.
+            description: Custom field representing the main project requirement criteria.
+      date_created:
+        type:
+          - "null"
+          - integer
+        description: The date when the project was created.
+      date_modified:
+        type:
+          - "null"
+          - integer
+        description: The date when the project was last modified.
+      details:
+        type:
+          - "null"
+          - string
+        description: Additional details or description of the project.
+      id:
+        type:
+          - "null"
+          - integer
+        description: The unique identifier of the project.
+      name:
+        type:
+          - "null"
+          - string
+        description: The name or title of the project.
+      related_resource:
+        type:
+          - "null"
+          - string
+        description: Reference to any related resource linked to the project.
+      status:
+        type:
+          - "null"
+          - string
+        description: The current status of the project.
+      tags:
+        type:
+          - "null"
+          - array
+        description: Tags associated with the project for categorization.
+        properties:
+          sticker:
             type:
               - "null"
               - string
-          customer_source_id:
-            description:
-              The unique identifier of the source through which the customer
-              was acquired.
+            description: Tag associated with the project (e.g., priority, category).
+  companies:
+    type: object
+    $schema: http://json-schema.org/draft-04/schema#
+    additionalProperties: true
+    properties:
+      address:
+        type:
+          - "null"
+          - object
+        description: Company address details
+        properties:
+          city:
             type:
               - "null"
               - string
-          details:
-            description: Additional details or notes related to the opportunity.
+            description: City of the company address
+          country:
             type:
               - "null"
               - string
-          loss_reason_id:
-            description: The unique identifier of the reason for losing the opportunity.
+            description: Country of the company address
+          postal_code:
             type:
               - "null"
               - string
-          monetary_value:
-            description:
-              The potential or actual monetary value associated with the
-              opportunity.
-            type:
-              - "null"
-              - integer
-          pipeline_id:
-            description:
-              The unique identifier of the pipeline to which the opportunity
-              belongs.
+            description: Postal code of the company address
+          state:
             type:
               - "null"
               - string
-          primary_contact_id:
-            description:
-              The unique identifier of the primary contact associated with
-              the opportunity.
+            description: State of the company address
+          street:
             type:
               - "null"
               - string
-          priority:
-            description: The priority level assigned to the opportunity.
+            description: Street address of the company
+      assignee_id:
+        type:
+          - "null"
+          - integer
+        description: ID of the assignee for the company
+      contact_type_id:
+        type:
+          - "null"
+          - integer
+        description: ID representing the contact type
+      custom_fields:
+        type:
+          - "null"
+          - array
+        description: Custom fields associated with the company
+        properties:
+          mpc:
             type:
               - "null"
               - string
-          pipeline_stage_id:
-            description:
-              The unique identifier of the stage of the pipeline the opportunity
-              is currently in.
+            description: Custom field for a specific attribute
+      date_created:
+        type:
+          - "null"
+          - integer
+        description: Date when the company record was created
+      date_modified:
+        type:
+          - "null"
+          - integer
+        description: Date when the company record was last modified
+      details:
+        type:
+          - "null"
+          - string
+        description: Additional details about the company
+      email_domain:
+        type:
+          - "null"
+          - string
+        description: Email domain associated with the company
+      id:
+        type:
+          - "null"
+          - integer
+        description: Unique identifier for the company
+      interaction_count:
+        type:
+          - "null"
+          - integer
+        description: Count of interactions with the company
+      name:
+        type:
+          - "null"
+          - string
+        description: Name of the company
+      phone_numbers:
+        type:
+          - "null"
+          - array
+        description: Phone numbers associated with the company
+        properties:
+          category:
             type:
               - "null"
               - string
-          status:
-            description:
-              The current status of the opportunity (e.g., open, closed-won,
-              closed-lost).
+            description: Category of the phone number
+          number:
             type:
               - "null"
               - string
-          tags:
-            description: An array of tags or labels associated with the opportunity.
-            type:
-              - "null"
-              - array
-            items:
-              description: A tag or label associated with the opportunity.
+            description: Phone number
+      socials:
+        type:
+          - "null"
+          - array
+        description: Social media profiles associated with the company
+        items:
+          type: object
+          properties:
+            category:
               type:
                 - "null"
                 - string
-          win_probability:
-            description:
-              The probability of winning the opportunity expressed as a
-              percentage.
-            type:
-              - "null"
-              - number
-          date_created:
-            description: The date and time when the opportunity was created.
-            type:
-              - "null"
-              - integer
-          date_modified:
-            description: The date and time when the opportunity was last modified.
-            type:
-              - "null"
-              - integer
-streams:
-  - "#/definitions/people_stream"
-  - "#/definitions/projects_stream"
-  - "#/definitions/companies_stream"
-  - "#/definitions/opportunities_stream"
-
-check:
-  type: CheckStream
-  stream_names:
-    - "people"
-    - "projects"
-    - "companies"
-    - "opportunities"
+              description: Category of the social media profile
+            url:
+              type:
+                - "null"
+                - string
+              description: URL of the social media profile
+      tags:
+        type:
+          - "null"
+          - array
+        description: Tags associated with the company
+        items:
+          description: Tag item
+      websites:
+        type:
+          - "null"
+          - array
+        description: Websites associated with the company
+        items:
+          type:
+            - object
+            - "null"
+          properties:
+            category:
+              type:
+                - "null"
+                - string
+              description: Category of the website
+            url:
+              type:
+                - "null"
+                - string
+              description: URL of the website
+  opportunities:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      assignee_id:
+        type:
+          - "null"
+          - number
+        description: The unique identifier of the user assigned to this opportunity.
+      close_date:
+        type:
+          - "null"
+          - string
+        description: The expected or actual closing date of the opportunity.
+      company_id:
+        type:
+          - "null"
+          - string
+        description: The unique identifier of the company associated with this opportunity.
+      company_name:
+        type:
+          - "null"
+          - string
+        description: The name of the company associated with this opportunity.
+      customer_source_id:
+        type:
+          - "null"
+          - string
+        description: >-
+          The unique identifier of the source through which the customer was
+          acquired.
+      date_created:
+        type:
+          - "null"
+          - integer
+        description: The date and time when the opportunity was created.
+      date_modified:
+        type:
+          - "null"
+          - integer
+        description: The date and time when the opportunity was last modified.
+      details:
+        type:
+          - "null"
+          - string
+        description: Additional details or notes related to the opportunity.
+      id:
+        type:
+          - "null"
+          - integer
+        description: The unique identifier of the opportunity.
+      loss_reason_id:
+        type:
+          - "null"
+          - string
+        description: The unique identifier of the reason for losing the opportunity.
+      monetary_value:
+        type:
+          - "null"
+          - integer
+        description: >-
+          The potential or actual monetary value associated with the
+          opportunity.
+      name:
+        type:
+          - "null"
+          - string
+        description: The name or title of the opportunity.
+      pipeline_id:
+        type:
+          - "null"
+          - string
+        description: >-
+          The unique identifier of the pipeline to which the opportunity
+          belongs.
+      pipeline_stage_id:
+        type:
+          - "null"
+          - string
+        description: >-
+          The unique identifier of the stage of the pipeline the opportunity is
+          currently in.
+      primary_contact_id:
+        type:
+          - "null"
+          - string
+        description: >-
+          The unique identifier of the primary contact associated with the
+          opportunity.
+      priority:
+        type:
+          - "null"
+          - string
+        description: The priority level assigned to the opportunity.
+      status:
+        type:
+          - "null"
+          - string
+        description: >-
+          The current status of the opportunity (e.g., open, closed-won,
+          closed-lost).
+      tags:
+        type:
+          - "null"
+          - array
+        description: An array of tags or labels associated with the opportunity.
+        items:
+          type:
+            - "null"
+            - string
+          description: A tag or label associated with the opportunity.
+      win_probability:
+        type:
+          - "null"
+          - number
+        description: The probability of winning the opportunity expressed as a percentage.
```

### Comparing `airbyte_source_copper-0.3.4/PKG-INFO` & `airbyte_source_copper-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-copper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Source implementation for Copper.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/copper
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Copper source connector
 
-
 This is the repository for the Copper source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/copper).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/copper)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_copper/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-copper spec
 poetry run source-copper check --config secrets/config.json
 poetry run source-copper discover --config secrets/config.json
 poetry run source-copper read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-copper build
 ```
 
 An image will be available on your host with the tag `airbyte/source-copper:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-copper:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-copper:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-copper:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-copper:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-copper test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-copper test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/copper.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

