# Comparing `tmp/airbyte-source-xero-0.2.5.tar.gz` & `tmp/airbyte_source_xero-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-xero-0.2.5.tar", last modified: Thu Feb  1 13:46:28 2024, max compression
+gzip compressed data, was "airbyte_source_xero-0.2.6.tar", max compression
```

## Comparing `airbyte-source-xero-0.2.5.tar` & `airbyte_source_xero-0.2.6.tar`

### file list

```diff
@@ -1,91 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.589239 airbyte-source-xero-0.2.5/
--rw-r--r--   0 root         (0) root         (0)     5331 2024-02-01 13:46:28.589239 airbyte-source-xero-0.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5331 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.589239 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5331 2024-02-01 13:46:28.000000 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3029 2024-02-01 13:46:28.000000 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 13:46:28.000000 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-02-01 13:46:28.000000 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 13:46:28.000000 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-02-01 13:46:28.000000 airbyte-source-xero-0.2.5/airbyte_source_xero.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.573239 airbyte-source-xero-0.2.5/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2894 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     8880 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      214 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      623 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      720 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5231 2024-02-01 13:46:28.589239 airbyte-source-xero-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      910 2024-02-01 13:46:26.000000 airbyte-source-xero-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.577239 airbyte-source-xero-0.2.5/source_xero/
--rw-r--r--   0 root         (0) root         (0)      120 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/oauth.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.581239 airbyte-source-xero-0.2.5/source_xero/schemas/
--rw-r--r--   0 root         (0) root         (0)     1218 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/accounts.json
--rw-r--r--   0 root         (0) root         (0)      684 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/addresses.json
--rw-r--r--   0 root         (0) root         (0)      286 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/allocations.json
--rw-r--r--   0 root         (0) root         (0)      137 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/attachments.json
--rw-r--r--   0 root         (0) root         (0)     1550 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/bank_transactions.json
--rw-r--r--   0 root         (0) root         (0)      952 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/bank_transfers.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/branding_themes.json
--rw-r--r--   0 root         (0) root         (0)      323 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/contact_groups.json
--rw-r--r--   0 root         (0) root         (0)     4460 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/contacts.json
--rw-r--r--   0 root         (0) root         (0)     1940 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/credit_notes.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/currencies.json
--rw-r--r--   0 root         (0) root         (0)      297 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/customers.json
--rw-r--r--   0 root         (0) root         (0)      467 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/employees.json
--rw-r--r--   0 root         (0) root         (0)      929 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/expense_claims.json
--rw-r--r--   0 root         (0) root         (0)     2938 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/invoices.json
--rw-r--r--   0 root         (0) root         (0)     1620 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/items.json
--rw-r--r--   0 root         (0) root         (0)     1785 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/journals.json
--rw-r--r--   0 root         (0) root         (0)      801 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/line_items.json
--rw-r--r--   0 root         (0) root         (0)      755 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/linked_transactions.json
--rw-r--r--   0 root         (0) root         (0)     1588 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/manual_journals.json
--rw-r--r--   0 root         (0) root         (0)     2250 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/nested_invoice.json
--rw-r--r--   0 root         (0) root         (0)     2447 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/organisations.json
--rw-r--r--   0 root         (0) root         (0)     1589 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/overpayments.json
--rw-r--r--   0 root         (0) root         (0)      593 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/payment_terms.json
--rw-r--r--   0 root         (0) root         (0)     1767 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/payments.json
--rw-r--r--   0 root         (0) root         (0)      336 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/phones.json
--rw-r--r--   0 root         (0) root         (0)     1588 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/prepayments.json
--rw-r--r--   0 root         (0) root         (0)     2204 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/purchase_orders.json
--rw-r--r--   0 root         (0) root         (0)     1546 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/quotes.json
--rw-r--r--   0 root         (0) root         (0)     1252 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/receipts.json
--rw-r--r--   0 root         (0) root         (0)     1718 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/repeating_invoices.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.585239 airbyte-source-xero-0.2.5/source_xero/schemas/shared/
--rw-r--r--   0 root         (0) root         (0)     1218 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/accounts.json
--rw-r--r--   0 root         (0) root         (0)      684 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/addresses.json
--rw-r--r--   0 root         (0) root         (0)      286 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/allocations.json
--rw-r--r--   0 root         (0) root         (0)      137 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/attachments.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/branding_themes.json
--rw-r--r--   0 root         (0) root         (0)      323 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/contact_groups.json
--rw-r--r--   0 root         (0) root         (0)     4460 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/contacts.json
--rw-r--r--   0 root         (0) root         (0)     1940 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/credit_notes.json
--rw-r--r--   0 root         (0) root         (0)      801 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/line_items.json
--rw-r--r--   0 root         (0) root         (0)     2250 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/nested_invoice.json
--rw-r--r--   0 root         (0) root         (0)     1589 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/overpayments.json
--rw-r--r--   0 root         (0) root         (0)      593 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/payment_terms.json
--rw-r--r--   0 root         (0) root         (0)     1767 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/payments.json
--rw-r--r--   0 root         (0) root         (0)      336 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/phones.json
--rw-r--r--   0 root         (0) root         (0)     1588 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/prepayments.json
--rw-r--r--   0 root         (0) root         (0)     1252 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/receipts.json
--rw-r--r--   0 root         (0) root         (0)     1718 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/repeating_invoices.json
--rw-r--r--   0 root         (0) root         (0)     1258 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/tracking_categories.json
--rw-r--r--   0 root         (0) root         (0)      608 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/users.json
--rw-r--r--   0 root         (0) root         (0)      204 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/shared/validation_errors.json
--rw-r--r--   0 root         (0) root         (0)     1282 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/tax_rates.json
--rw-r--r--   0 root         (0) root         (0)     1258 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/tracking_categories.json
--rw-r--r--   0 root         (0) root         (0)      608 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      204 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/schemas/validation_errors.json
--rw-r--r--   0 root         (0) root         (0)     3844 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/source.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/spec.yaml
--rw-r--r--   0 root         (0) root         (0)     7358 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/source_xero/streams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:46:28.589239 airbyte-source-xero-0.2.5/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/unit_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4047 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)     1346 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/unit_tests/test_streams.py
--rw-r--r--   0 root         (0) root         (0)      704 2024-02-01 13:41:32.000000 airbyte-source-xero-0.2.5/unit_tests/utils.py
+-rw-r--r--   0        0        0     4460 2024-05-19 23:00:37.135106 airbyte_source_xero-0.2.6/README.md
+-rw-r--r--   0        0        0      731 2024-05-19 23:04:53.203544 airbyte_source_xero-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      120 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/bootstrap.md
+-rw-r--r--   0        0        0     2151 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/oauth.py
+-rw-r--r--   0        0        0      224 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/run.py
+-rw-r--r--   0        0        0     1218 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/accounts.json
+-rw-r--r--   0        0        0      684 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/addresses.json
+-rw-r--r--   0        0        0      286 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/allocations.json
+-rw-r--r--   0        0        0      137 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/attachments.json
+-rw-r--r--   0        0        0     1550 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/bank_transactions.json
+-rw-r--r--   0        0        0      952 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/bank_transfers.json
+-rw-r--r--   0        0        0      351 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/branding_themes.json
+-rw-r--r--   0        0        0      323 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/contact_groups.json
+-rw-r--r--   0        0        0     4460 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/contacts.json
+-rw-r--r--   0        0        0     1940 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/credit_notes.json
+-rw-r--r--   0        0        0      194 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/currencies.json
+-rw-r--r--   0        0        0      297 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/customers.json
+-rw-r--r--   0        0        0      467 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/employees.json
+-rw-r--r--   0        0        0      929 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/expense_claims.json
+-rw-r--r--   0        0        0     2938 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/invoices.json
+-rw-r--r--   0        0        0     1620 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/items.json
+-rw-r--r--   0        0        0     1785 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/journals.json
+-rw-r--r--   0        0        0      801 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/line_items.json
+-rw-r--r--   0        0        0      755 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/linked_transactions.json
+-rw-r--r--   0        0        0     1588 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/manual_journals.json
+-rw-r--r--   0        0        0     2250 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/nested_invoice.json
+-rw-r--r--   0        0        0     2447 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/organisations.json
+-rw-r--r--   0        0        0     1589 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/overpayments.json
+-rw-r--r--   0        0        0      593 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/payment_terms.json
+-rw-r--r--   0        0        0     1767 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/payments.json
+-rw-r--r--   0        0        0      336 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/phones.json
+-rw-r--r--   0        0        0     1588 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/prepayments.json
+-rw-r--r--   0        0        0     2204 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/purchase_orders.json
+-rw-r--r--   0        0        0     1546 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/quotes.json
+-rw-r--r--   0        0        0     1252 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/receipts.json
+-rw-r--r--   0        0        0     1718 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/repeating_invoices.json
+-rw-r--r--   0        0        0     1218 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/accounts.json
+-rw-r--r--   0        0        0      684 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/addresses.json
+-rw-r--r--   0        0        0      286 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/allocations.json
+-rw-r--r--   0        0        0      137 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/attachments.json
+-rw-r--r--   0        0        0      351 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/branding_themes.json
+-rw-r--r--   0        0        0      323 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/contact_groups.json
+-rw-r--r--   0        0        0     4460 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/contacts.json
+-rw-r--r--   0        0        0     1940 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/credit_notes.json
+-rw-r--r--   0        0        0      801 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/line_items.json
+-rw-r--r--   0        0        0     2250 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/nested_invoice.json
+-rw-r--r--   0        0        0     1589 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/overpayments.json
+-rw-r--r--   0        0        0      593 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/payment_terms.json
+-rw-r--r--   0        0        0     1767 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/payments.json
+-rw-r--r--   0        0        0      336 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/phones.json
+-rw-r--r--   0        0        0     1588 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/prepayments.json
+-rw-r--r--   0        0        0     1252 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/receipts.json
+-rw-r--r--   0        0        0     1718 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/repeating_invoices.json
+-rw-r--r--   0        0        0     1258 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/tracking_categories.json
+-rw-r--r--   0        0        0      608 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/users.json
+-rw-r--r--   0        0        0      204 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/shared/validation_errors.json
+-rw-r--r--   0        0        0     1282 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/tax_rates.json
+-rw-r--r--   0        0        0     1258 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/tracking_categories.json
+-rw-r--r--   0        0        0      608 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/users.json
+-rw-r--r--   0        0        0      204 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/schemas/validation_errors.json
+-rw-r--r--   0        0        0     3844 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/source.py
+-rw-r--r--   0        0        0     3085 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/spec.yaml
+-rw-r--r--   0        0        0     7358 2024-05-19 23:00:37.139106 airbyte_source_xero-0.2.6/source_xero/streams.py
+-rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 airbyte_source_xero-0.2.6/PKG-INFO
```

### Comparing `airbyte-source-xero-0.2.5/PKG-INFO` & `airbyte_source_xero-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-xero
-Version: 0.2.5
+Version: 0.2.6
 Summary: Source implementation for Xero.
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
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/xero
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Xero Source
+# Xero source connector
 
-This is the repository for the Xero source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/xero).
 
+This is the repository for the Xero source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/xero).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/xero)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/xero)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_xero/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source xero test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-xero spec
+poetry run source-xero check --config secrets/config.json
+poetry run source-xero discover --config secrets/config.json
+poetry run source-xero read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-xero build
 ```
 
-An image will be built with the tag `airbyte/source-xero:dev`.
+An image will be available on your host with the tag `airbyte/source-xero:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-xero:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-xero:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-xero:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-xero test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-xero test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-xero-0.2.5/README.md` & `airbyte_source_xero-0.2.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-# Xero Source
+# Xero source connector
+
 
 This is the repository for the Xero source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/xero).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/xero).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
-
-#### Minimum Python version required `= 3.9.0`
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/xero)
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/xero)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_xero/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source xero test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-xero spec
+poetry run source-xero check --config secrets/config.json
+poetry run source-xero discover --config secrets/config.json
+poetry run source-xero read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
-
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-xero build
 ```
 
-An image will be built with the tag `airbyte/source-xero:dev`.
+An image will be available on your host with the tag `airbyte/source-xero:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-xero:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-xero:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-xero:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-xero:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-xero test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
-### Publishing a new version of the connector
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-xero test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/xero.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-xero-0.2.5/source_xero/oauth.py` & `airbyte_source_xero-0.2.6/source_xero/oauth.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/accounts.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/addresses.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/addresses.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/bank_transactions.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/bank_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/bank_transfers.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/bank_transfers.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/contacts.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/credit_notes.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/credit_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/expense_claims.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/expense_claims.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/invoices.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/items.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/items.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/journals.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/journals.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/line_items.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/linked_transactions.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/linked_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/manual_journals.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/manual_journals.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/nested_invoice.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/nested_invoice.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/organisations.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/organisations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/overpayments.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/overpayments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/payment_terms.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/payment_terms.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/payments.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/payments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/prepayments.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/prepayments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/purchase_orders.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/purchase_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/quotes.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/quotes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/receipts.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/receipts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/repeating_invoices.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/repeating_invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/accounts.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/addresses.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/addresses.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/contacts.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/credit_notes.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/credit_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/line_items.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/nested_invoice.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/nested_invoice.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/overpayments.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/overpayments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/payment_terms.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/payment_terms.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/payments.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/payments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/prepayments.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/prepayments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/receipts.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/receipts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/repeating_invoices.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/repeating_invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/tracking_categories.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/tracking_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/shared/users.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/shared/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/tax_rates.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/tax_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/tracking_categories.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/tracking_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/schemas/users.json` & `airbyte_source_xero-0.2.6/source_xero/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/source.py` & `airbyte_source_xero-0.2.6/source_xero/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/spec.yaml` & `airbyte_source_xero-0.2.6/source_xero/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-xero-0.2.5/source_xero/streams.py` & `airbyte_source_xero-0.2.6/source_xero/streams.py`

 * *Files identical despite different names*

