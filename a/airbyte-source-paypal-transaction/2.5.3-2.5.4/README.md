# Comparing `tmp/airbyte_source_paypal_transaction-2.5.3.tar.gz` & `tmp/airbyte_source_paypal_transaction-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_paypal_transaction-2.5.3.tar", max compression
+gzip compressed data, was "airbyte_source_paypal_transaction-2.5.4.tar", max compression
```

## Comparing `airbyte_source_paypal_transaction-2.5.3.tar` & `airbyte_source_paypal_transaction-2.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11632 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/README.md
--rw-r--r--   0        0        0      836 2024-05-07 13:36:53.356879 airbyte_source_paypal_transaction-2.5.3/pyproject.toml
--rw-r--r--   0        0        0      146 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/__init__.py
--rw-r--r--   0        0        0     3072 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/components.py
--rw-r--r--   0        0        0   101426 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/manifest.yaml
--rw-r--r--   0        0        0      264 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/run.py
--rw-r--r--   0        0        0      523 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/source.py
--rw-r--r--   0        0        0     3021 2024-05-07 10:51:28.000000 airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/spec.yaml
--rw-r--r--   0        0        0    12372 1970-01-01 00:00:00.000000 airbyte_source_paypal_transaction-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11572 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/README.md
+-rw-r--r--   0        0        0      836 2024-05-20 20:23:23.669932 airbyte_source_paypal_transaction-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/__init__.py
+-rw-r--r--   0        0        0     3072 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/components.py
+-rw-r--r--   0        0        0   101426 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/manifest.yaml
+-rw-r--r--   0        0        0      264 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/run.py
+-rw-r--r--   0        0        0      501 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/source.py
+-rw-r--r--   0        0        0     3021 2024-05-20 04:00:42.000000 airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/spec.yaml
+-rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 airbyte_source_paypal_transaction-2.5.4/PKG-INFO
```

### Comparing `airbyte_source_paypal_transaction-2.5.3/README.md` & `airbyte_source_paypal_transaction-2.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,103 +1,106 @@
 # Paypal-Transaction source connector
 
 This is the repository for the Paypal-Transaction source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/paypal-transaction).
 
 ## Local development
 
-
 #### Prerequisites
-  * Python (~=3.9)
-  * Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
-  * Paypal Client ID and Client Secret
-  * If you are going to use the data generator scripts you need to setup yourPaypal Sandbox and a Buyer user in your sandbox, to simulate the data. YOu cna get that information in the [Apps & Credentials page](https://developer.paypal.com/dashboard/applications/live).
-     * Buyer Username
-     * Buyer Password
-     * Payer ID (Account ID)
+
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+- Paypal Client ID and Client Secret
+- If you are going to use the data generator scripts you need to setup yourPaypal Sandbox and a Buyer user in your sandbox, to simulate the data. YOu cna get that information in the [Apps & Credentials page](https://developer.paypal.com/dashboard/applications/live).
+  - Buyer Username
+  - Buyer Password
+  - Payer ID (Account ID)
 
 ### Installing the connector
 
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
 ### Create credentials
 
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/paypal-transaction)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_paypal_transaction/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-* You must have created your credentials under the `secrets/` folder
-* For the read command, you can create separate catalogs to test the streams individually. All catalogs are under the folder `integration_tests`. Select the one you want to test with the read command.
-
+- You must have created your credentials under the `secrets/` folder
+- For the read command, you can create separate catalogs to test the streams individually. All catalogs are under the folder `integration_tests`. Select the one you want to test with the read command.
 
 ### Locally running the connector
 
 ```
 poetry run source-paypal-transaction spec
 poetry run source-paypal-transaction check --config secrets/config.json
 poetry run source-paypal-transaction discover --config secrets/config.json
 # Example with list_payments catalog and the debug flag
 poetry run source-paypal-transaction read --config secrets/config.json --catalog integration_tests/configured_catalog_list_payments.json --debug
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
 
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
 
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 
-
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
 ##### Customizing our build process
+
 When contributing on our connector you might need to customize the build process to add a system dependency or set an env var.
 You can customize our build process by adding a `build_customization.py` module to your connector.
 This module should contain a `pre_connector_install` and `post_connector_install` async function that will mutate the base image and the connector container respectively.
 It will be imported at runtime by our build process and the functions will be called if they exist.
 
 Here is an example of a `build_customization.py` module:
+
 ```python
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     # Feel free to check the dagger documentation for more information on the Container object and its methods.
     # https://dagger-io.readthedocs.io/en/sdk-python-v0.6.4/
     from dagger import Container
 ```
 
 An image will be available on your host with the tag `airbyte/source-paypal-transaction:dev`.
 
-
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-paypal-transaction:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-paypal-transaction:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-paypal-transaction:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-paypal-transaction:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-
 ### Running our CI test suite
 
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 
 ```bash
 airbyte-ci connectors --name=source-paypal-transaction test
 ```
@@ -105,18 +108,18 @@
 If you are testing locally, you can use your local credentials (config.json file) by using `--use-local-secrets`
 
 ```bash
 airbyte-ci connectors --name source-paypal-transaction --use-local-secrets test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-
 ## Running Unit tests locally
 
 To run unit tests locally, form the root `source_paypal_transaction` directory run:
 
 ```bash
 python -m pytest unit_test
 ```
@@ -124,90 +127,100 @@
 ## Test changes in the sandbox
 
 If you have a [Paypal Sandbox](https://developer.paypal.com/tools/sandbox/accounts/) you will be able to use some APIs to create new data and test how data is being created in your destinaiton and choose the best syn strategy that suits better your use case.
 Some endpoints will require special permissions on the sandbox to update and change some values.
 
 In the `bin` folder you will find several data generator scripts:
 
-* **disputes_generator.py:** 
-   * Update dispute: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}` endpoint. You need the ID and create a payload to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_patch).
+- **disputes_generator.py:**
+
+  - Update dispute: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}` endpoint. You need the ID and create a payload to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_patch).
+
+  ```bash
+  python disputes_generator.py update DISPUTE_ID ''[{"op": "replace", "path": "/reason", "value": "The new reason"}]'
+  ```
+
+  - Update Evidence status: Uses the _POST_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}/require-evidence` endpoint. You need the ID and select an option to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_require-evidence)
+
+  ```bash
+  python update_dispute.py require-evidence DISPUTE_ID SELLER_EVIDENCE
+  ```
 
-   ```bash
-   python disputes_generator.py update DISPUTE_ID ''[{"op": "replace", "path": "/reason", "value": "The new reason"}]'
-   ```
-   
-   * Update Evidence status: Uses the _POST_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}/require-evidence` endpoint. You need the ID and select an option to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_require-evidence)
-   ```bash
-   python update_dispute.py require-evidence DISPUTE_ID SELLER_EVIDENCE
-   ```
-
-* **invoices.py:** 
-   * Create draft invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices` endpoint. It will automatically generate an invoice (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
-
-   ```bash
-   python invoices.py create_draft
-   ```
-   
-   * Send a Draft Invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices/{invoice_id}/send` endpoint. You need the Invoice ID, a subject and a note (just to have something to update) and an email as an argument. See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_send)
-   ```bash
-   python invoices.py send_draft --invoice_id "INV2-XXXX-XXXX-XXXX-XXXX" --subject "Your Invoice Subject" --note "Your custom note" --additional_recipients example@email.com
-   ```
-
-* **payments_generator.py:** 
-   * Partially update payment: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/payments/payment/{payment_id}` endpoint. You need the payment ID and a payload with new values. (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
-
-   ```bash
-    python script_name.py update PAYMENT_ID '[{"op": "replace", "path": "/transactions/0/amount", "value": {"total": "50.00", "currency": "USD"}}]'
-   ```
-   
-* **paypal_transaction_generator.py:** 
-   Make sure you have the `buyer_username`, `buyer_password` and `payer_id` in your config file. You can get the sample configuratin in the `sample_config.json`. 
-
-   * Generate transactions: This uses Selenium, so you will be prompted to your account to simulate the complete transaction flow. You can add a number at the end of the command to do more than one transaction. By default the script runs 3 transactions.
-
-   **NOTE: Be midnfu of the number of transactions, as it will be interacting with your machine, and you may not be able to use it while creating the transactions** 
-
-   ```bash
-    python paypal_transaction_generator.py [NUMBER_OF_DESIRED_TRANSACTIONS]
-   ```
-
-* **product_catalog.py:** 
-   * Create a product: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v1/catalogs/products` endpoint. You need to add the description and the category in the command line. For the proper category see more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_create).
-
-   ```bash
-   python product_catalog.py --action create --description "YOUR DESCRIPTION" --category PAYPAL_CATEGORY
-   ```
-   
-   * Update a product: Uses the _PATCH_ method of the `https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch` endpoint. You need the product ID, a description and the Category as an argument. See more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch)
-   ```bash
-   python product_catalog.py --action update --product_id PRODUCT_ID --update_payload '[{"op": "replace", "path": "/description", "value": "My Update. Does it changes it?"}]'
-   ```
+- **invoices.py:**
+
+  - Create draft invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices` endpoint. It will automatically generate an invoice (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
+
+  ```bash
+  python invoices.py create_draft
+  ```
+
+  - Send a Draft Invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices/{invoice_id}/send` endpoint. You need the Invoice ID, a subject and a note (just to have something to update) and an email as an argument. See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_send)
+
+  ```bash
+  python invoices.py send_draft --invoice_id "INV2-XXXX-XXXX-XXXX-XXXX" --subject "Your Invoice Subject" --note "Your custom note" --additional_recipients example@email.com
+  ```
+
+- **payments_generator.py:**
+
+  - Partially update payment: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/payments/payment/{payment_id}` endpoint. You need the payment ID and a payload with new values. (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
+
+  ```bash
+   python script_name.py update PAYMENT_ID '[{"op": "replace", "path": "/transactions/0/amount", "value": {"total": "50.00", "currency": "USD"}}]'
+  ```
+
+- **paypal_transaction_generator.py:**
+  Make sure you have the `buyer_username`, `buyer_password` and `payer_id` in your config file. You can get the sample configuratin in the `sample_config.json`.
+
+  - Generate transactions: This uses Selenium, so you will be prompted to your account to simulate the complete transaction flow. You can add a number at the end of the command to do more than one transaction. By default the script runs 3 transactions.
+
+  **NOTE: Be midnfu of the number of transactions, as it will be interacting with your machine, and you may not be able to use it while creating the transactions**
+
+  ```bash
+   python paypal_transaction_generator.py [NUMBER_OF_DESIRED_TRANSACTIONS]
+  ```
+
+- **product_catalog.py:**
+
+  - Create a product: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v1/catalogs/products` endpoint. You need to add the description and the category in the command line. For the proper category see more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_create).
+
+  ```bash
+  python product_catalog.py --action create --description "YOUR DESCRIPTION" --category PAYPAL_CATEGORY
+  ```
+
+  - Update a product: Uses the _PATCH_ method of the `https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch` endpoint. You need the product ID, a description and the Category as an argument. See more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch)
+
+  ```bash
+  python product_catalog.py --action update --product_id PRODUCT_ID --update_payload '[{"op": "replace", "path": "/description", "value": "My Update. Does it changes it?"}]'
+  ```
 
 ## Dependency Management
+
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
 
+- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
+- required for the testing need to go to `TEST_REQUIREMENTS` list
 
-All of your dependencies should be managed via Poetry. 
+All of your dependencies should be managed via Poetry.
 
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
-
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-paypal-transaction test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/paypal-transaction.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_paypal_transaction-2.5.3/pyproject.toml` & `airbyte_source_paypal_transaction-2.5.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.3"
+version = "2.5.4"
 name = "airbyte-source-paypal-transaction"
 description = "Source implementation for Paypal Transaction."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/components.py` & `airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/manifest.yaml` & `airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.3/source_paypal_transaction/spec.yaml` & `airbyte_source_paypal_transaction-2.5.4/source_paypal_transaction/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.3/PKG-INFO` & `airbyte_source_paypal_transaction-2.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-paypal-transaction
-Version: 2.5.3
+Version: 2.5.4
 Summary: Source implementation for Paypal Transaction.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -20,103 +20,106 @@
 # Paypal-Transaction source connector
 
 This is the repository for the Paypal-Transaction source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/paypal-transaction).
 
 ## Local development
 
-
 #### Prerequisites
-  * Python (~=3.9)
-  * Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
-  * Paypal Client ID and Client Secret
-  * If you are going to use the data generator scripts you need to setup yourPaypal Sandbox and a Buyer user in your sandbox, to simulate the data. YOu cna get that information in the [Apps & Credentials page](https://developer.paypal.com/dashboard/applications/live).
-     * Buyer Username
-     * Buyer Password
-     * Payer ID (Account ID)
+
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+- Paypal Client ID and Client Secret
+- If you are going to use the data generator scripts you need to setup yourPaypal Sandbox and a Buyer user in your sandbox, to simulate the data. YOu cna get that information in the [Apps & Credentials page](https://developer.paypal.com/dashboard/applications/live).
+  - Buyer Username
+  - Buyer Password
+  - Payer ID (Account ID)
 
 ### Installing the connector
 
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
 ### Create credentials
 
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/paypal-transaction)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_paypal_transaction/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-* You must have created your credentials under the `secrets/` folder
-* For the read command, you can create separate catalogs to test the streams individually. All catalogs are under the folder `integration_tests`. Select the one you want to test with the read command.
-
+- You must have created your credentials under the `secrets/` folder
+- For the read command, you can create separate catalogs to test the streams individually. All catalogs are under the folder `integration_tests`. Select the one you want to test with the read command.
 
 ### Locally running the connector
 
 ```
 poetry run source-paypal-transaction spec
 poetry run source-paypal-transaction check --config secrets/config.json
 poetry run source-paypal-transaction discover --config secrets/config.json
 # Example with list_payments catalog and the debug flag
 poetry run source-paypal-transaction read --config secrets/config.json --catalog integration_tests/configured_catalog_list_payments.json --debug
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
 
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
 
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
 
-
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
 ##### Customizing our build process
+
 When contributing on our connector you might need to customize the build process to add a system dependency or set an env var.
 You can customize our build process by adding a `build_customization.py` module to your connector.
 This module should contain a `pre_connector_install` and `post_connector_install` async function that will mutate the base image and the connector container respectively.
 It will be imported at runtime by our build process and the functions will be called if they exist.
 
 Here is an example of a `build_customization.py` module:
+
 ```python
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     # Feel free to check the dagger documentation for more information on the Container object and its methods.
     # https://dagger-io.readthedocs.io/en/sdk-python-v0.6.4/
     from dagger import Container
 ```
 
 An image will be available on your host with the tag `airbyte/source-paypal-transaction:dev`.
 
-
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-paypal-transaction:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-paypal-transaction:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-paypal-transaction:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-paypal-transaction:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-
 ### Running our CI test suite
 
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 
 ```bash
 airbyte-ci connectors --name=source-paypal-transaction test
 ```
@@ -124,18 +127,18 @@
 If you are testing locally, you can use your local credentials (config.json file) by using `--use-local-secrets`
 
 ```bash
 airbyte-ci connectors --name source-paypal-transaction --use-local-secrets test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-
 ## Running Unit tests locally
 
 To run unit tests locally, form the root `source_paypal_transaction` directory run:
 
 ```bash
 python -m pytest unit_test
 ```
@@ -143,90 +146,101 @@
 ## Test changes in the sandbox
 
 If you have a [Paypal Sandbox](https://developer.paypal.com/tools/sandbox/accounts/) you will be able to use some APIs to create new data and test how data is being created in your destinaiton and choose the best syn strategy that suits better your use case.
 Some endpoints will require special permissions on the sandbox to update and change some values.
 
 In the `bin` folder you will find several data generator scripts:
 
-* **disputes_generator.py:** 
-   * Update dispute: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}` endpoint. You need the ID and create a payload to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_patch).
+- **disputes_generator.py:**
+
+  - Update dispute: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}` endpoint. You need the ID and create a payload to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_patch).
+
+  ```bash
+  python disputes_generator.py update DISPUTE_ID ''[{"op": "replace", "path": "/reason", "value": "The new reason"}]'
+  ```
+
+  - Update Evidence status: Uses the _POST_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}/require-evidence` endpoint. You need the ID and select an option to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_require-evidence)
+
+  ```bash
+  python update_dispute.py require-evidence DISPUTE_ID SELLER_EVIDENCE
+  ```
+
+- **invoices.py:**
 
-   ```bash
-   python disputes_generator.py update DISPUTE_ID ''[{"op": "replace", "path": "/reason", "value": "The new reason"}]'
-   ```
-   
-   * Update Evidence status: Uses the _POST_ method of the `https://api-m.paypal.com/v1/customer/disputes/{dispute_id}/require-evidence` endpoint. You need the ID and select an option to pass it as an argument. See more information [here](https://developer.paypal.com/docs/api/customer-disputes/v1/#disputes_require-evidence)
-   ```bash
-   python update_dispute.py require-evidence DISPUTE_ID SELLER_EVIDENCE
-   ```
-
-* **invoices.py:** 
-   * Create draft invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices` endpoint. It will automatically generate an invoice (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
-
-   ```bash
-   python invoices.py create_draft
-   ```
-   
-   * Send a Draft Invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices/{invoice_id}/send` endpoint. You need the Invoice ID, a subject and a note (just to have something to update) and an email as an argument. See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_send)
-   ```bash
-   python invoices.py send_draft --invoice_id "INV2-XXXX-XXXX-XXXX-XXXX" --subject "Your Invoice Subject" --note "Your custom note" --additional_recipients example@email.com
-   ```
-
-* **payments_generator.py:** 
-   * Partially update payment: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/payments/payment/{payment_id}` endpoint. You need the payment ID and a payload with new values. (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
-
-   ```bash
-    python script_name.py update PAYMENT_ID '[{"op": "replace", "path": "/transactions/0/amount", "value": {"total": "50.00", "currency": "USD"}}]'
-   ```
-   
-* **paypal_transaction_generator.py:** 
-   Make sure you have the `buyer_username`, `buyer_password` and `payer_id` in your config file. You can get the sample configuratin in the `sample_config.json`. 
-
-   * Generate transactions: This uses Selenium, so you will be prompted to your account to simulate the complete transaction flow. You can add a number at the end of the command to do more than one transaction. By default the script runs 3 transactions.
-
-   **NOTE: Be midnfu of the number of transactions, as it will be interacting with your machine, and you may not be able to use it while creating the transactions** 
-
-   ```bash
-    python paypal_transaction_generator.py [NUMBER_OF_DESIRED_TRANSACTIONS]
-   ```
-
-* **product_catalog.py:** 
-   * Create a product: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v1/catalogs/products` endpoint. You need to add the description and the category in the command line. For the proper category see more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_create).
-
-   ```bash
-   python product_catalog.py --action create --description "YOUR DESCRIPTION" --category PAYPAL_CATEGORY
-   ```
-   
-   * Update a product: Uses the _PATCH_ method of the `https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch` endpoint. You need the product ID, a description and the Category as an argument. See more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch)
-   ```bash
-   python product_catalog.py --action update --product_id PRODUCT_ID --update_payload '[{"op": "replace", "path": "/description", "value": "My Update. Does it changes it?"}]'
-   ```
+  - Create draft invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices` endpoint. It will automatically generate an invoice (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
+
+  ```bash
+  python invoices.py create_draft
+  ```
+
+  - Send a Draft Invoice: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v2/invoicing/invoices/{invoice_id}/send` endpoint. You need the Invoice ID, a subject and a note (just to have something to update) and an email as an argument. See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_send)
+
+  ```bash
+  python invoices.py send_draft --invoice_id "INV2-XXXX-XXXX-XXXX-XXXX" --subject "Your Invoice Subject" --note "Your custom note" --additional_recipients example@email.com
+  ```
+
+- **payments_generator.py:**
+
+  - Partially update payment: Uses the _PATCH_ method of the `https://api-m.paypal.com/v1/payments/payment/{payment_id}` endpoint. You need the payment ID and a payload with new values. (no need to pass any parameters). See more information [here](https://developer.paypal.com/docs/api/invoicing/v2/#invoices_create).
+
+  ```bash
+   python script_name.py update PAYMENT_ID '[{"op": "replace", "path": "/transactions/0/amount", "value": {"total": "50.00", "currency": "USD"}}]'
+  ```
+
+- **paypal_transaction_generator.py:**
+  Make sure you have the `buyer_username`, `buyer_password` and `payer_id` in your config file. You can get the sample configuratin in the `sample_config.json`.
+
+  - Generate transactions: This uses Selenium, so you will be prompted to your account to simulate the complete transaction flow. You can add a number at the end of the command to do more than one transaction. By default the script runs 3 transactions.
+
+  **NOTE: Be midnfu of the number of transactions, as it will be interacting with your machine, and you may not be able to use it while creating the transactions**
+
+  ```bash
+   python paypal_transaction_generator.py [NUMBER_OF_DESIRED_TRANSACTIONS]
+  ```
+
+- **product_catalog.py:**
+
+  - Create a product: Uses the _POST_ method of the `https://api-m.sandbox.paypal.com/v1/catalogs/products` endpoint. You need to add the description and the category in the command line. For the proper category see more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_create).
+
+  ```bash
+  python product_catalog.py --action create --description "YOUR DESCRIPTION" --category PAYPAL_CATEGORY
+  ```
+
+  - Update a product: Uses the _PATCH_ method of the `https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch` endpoint. You need the product ID, a description and the Category as an argument. See more information [here](https://developer.paypal.com/docs/api/catalog-products/v1/#products_patch)
+
+  ```bash
+  python product_catalog.py --action update --product_id PRODUCT_ID --update_payload '[{"op": "replace", "path": "/description", "value": "My Update. Does it changes it?"}]'
+  ```
 
 ## Dependency Management
+
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
 
+- required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
+- required for the testing need to go to `TEST_REQUIREMENTS` list
 
-All of your dependencies should be managed via Poetry. 
+All of your dependencies should be managed via Poetry.
 
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
-
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-paypal-transaction test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/paypal-transaction.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

