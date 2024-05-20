# Comparing `tmp/bitpay-6.0.2.tar.gz` & `tmp/bitpay-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitpay-6.0.2.tar", last modified: Mon May  6 16:53:20 2024, max compression
+gzip compressed data, was "bitpay-6.0.3.tar", last modified: Mon May 20 00:54:34 2024, max compression
```

## Comparing `bitpay-6.0.2.tar` & `bitpay-6.0.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.027037 bitpay-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 16:53:16.000000 bitpay-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 16:53:20.027037 bitpay-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-06 16:53:16.000000 bitpay-6.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-06 16:53:16.000000 bitpay-6.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:53:20.027037 bitpay-6.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.007037 bitpay-6.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.011037 bitpay-6.0.2/src/bitpay/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/bitpay_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    36869 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/bill_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/bitpay_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/currency_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/invoice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/ledger_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/payout_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/payout_recipient_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/rate_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/refund_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/settlement_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/clients/wallet_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_exception_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/exceptions/bitpay_validation_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/bitpay_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/logger_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/logger/logging_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.015037 bitpay-6.0.2/src/bitpay/models/bill/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/bill_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bill/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/bitpay_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.019037 bitpay-6.0.2/src/bitpay/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/buyer.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/buyer_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/buyer_provided_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_event_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_refund_addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/invoice_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/itemized_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/miner_fees.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/miner_fees_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/refund_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/shopper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/supported_transaction_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/supported_transaction_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/invoice/universal_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.019037 bitpay-6.0.2/src/bitpay/models/ledger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/buyer.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/ledger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/ledger/ledger_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/payout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_group_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_recipients.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/payout_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/payout/recipient_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/rate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/rate/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/rate/rates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/settlement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/invoice_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/payout_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/refund_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/settlement.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/settlement_ledger_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/settlement/with_holdings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.023037 bitpay-6.0.2/src/bitpay/models/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/currency_qr.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/models/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.027037 bitpay-6.0.2/src/bitpay/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/guid_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/model_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 16:53:16.000000 bitpay-6.0.2/src/bitpay/utils/token_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:53:20.027037 bitpay-6.0.2/src/bitpay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-06 16:53:20.000000 bitpay-6.0.2/src/bitpay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 16:53:19.000000 bitpay-6.0.2/src/bitpay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.728747 bitpay-6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-20 00:54:30.000000 bitpay-6.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-20 00:54:34.728747 bitpay-6.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 00:54:30.000000 bitpay-6.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-20 00:54:30.000000 bitpay-6.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:54:34.728747 bitpay-6.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.708747 bitpay-6.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.712747 bitpay-6.0.3/src/bitpay/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/bitpay_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36869 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.716747 bitpay-6.0.3/src/bitpay/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/bill_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/bitpay_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/currency_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/invoice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/ledger_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/payout_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/payout_recipient_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/rate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9970 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/refund_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/settlement_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/clients/wallet_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.716747 bitpay-6.0.3/src/bitpay/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/exceptions/bitpay_api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/exceptions/bitpay_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/exceptions/bitpay_exception_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/exceptions/bitpay_generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/exceptions/bitpay_validation_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.716747 bitpay-6.0.3/src/bitpay/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/logger/bitpay_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/logger/logger_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/logger/logging_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.716747 bitpay-6.0.3/src/bitpay/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.720747 bitpay-6.0.3/src/bitpay/models/bill/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/bill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/bill/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/bill/bill_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/bill/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/bitpay_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.724748 bitpay-6.0.3/src/bitpay/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/buyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/buyer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/buyer_provided_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/invoice_event_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/invoice_refund_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/invoice_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/itemized_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/miner_fees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/miner_fees_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/refund_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/refund_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/refund_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/shopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/supported_transaction_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/supported_transaction_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/invoice/universal_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.724748 bitpay-6.0.3/src/bitpay/models/ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/ledger/buyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/ledger/ledger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/ledger/ledger_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.724748 bitpay-6.0.3/src/bitpay/models/payout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_group_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_recipients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/payout_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/payout/recipient_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.724748 bitpay-6.0.3/src/bitpay/models/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/rate/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/rate/rates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.728747 bitpay-6.0.3/src/bitpay/models/settlement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/invoice_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/payout_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/refund_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/settlement_ledger_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/settlement/with_holdings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.728747 bitpay-6.0.3/src/bitpay/models/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/wallet/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/wallet/currency_qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/models/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.728747 bitpay-6.0.3/src/bitpay/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/utils/guid_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/utils/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 00:54:30.000000 bitpay-6.0.3/src/bitpay/utils/token_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:54:34.728747 bitpay-6.0.3/src/bitpay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-20 00:54:34.000000 bitpay-6.0.3/src/bitpay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-20 00:54:34.000000 bitpay-6.0.3/src/bitpay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:54:34.000000 bitpay-6.0.3/src/bitpay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 00:54:34.000000 bitpay-6.0.3/src/bitpay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 00:54:34.000000 bitpay-6.0.3/src/bitpay.egg-info/top_level.txt
```

### Comparing `bitpay-6.0.2/LICENSE` & `bitpay-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/PKG-INFO` & `bitpay-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpay
-Version: 6.0.2
+Version: 6.0.3
 Summary: Accept bitcoin with BitPay
 Author-email: Antonio Buedo <sales-engineering@bitpay.com>
 Project-URL: Homepage, https://github.com/bitpay/python-bitpay-client
 Project-URL: Bug Tracker, https://github.com/bitpay/python-bitpay-client/issues
 Keywords: bitcoin,payments,crypto,cash,ethereum,online payments
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `bitpay-6.0.2/README.md` & `bitpay-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/pyproject.toml` & `bitpay-6.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitpay"
-version = "6.0.2"
+version = "6.0.3"
 authors = [
   { name="Antonio Buedo", email="sales-engineering@bitpay.com" },
 ]
 requires-python = ">=3.8"
 dependencies = [
     "ecdsa >= 0.18.0",
     "requests >= 2.31.0",
```

### Comparing `bitpay-6.0.2/src/bitpay/bitpay_setup.py` & `bitpay-6.0.3/src/bitpay/bitpay_setup.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/client.py` & `bitpay-6.0.3/src/bitpay/client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/bill_client.py` & `bitpay-6.0.3/src/bitpay/clients/bill_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/bitpay_client.py` & `bitpay-6.0.3/src/bitpay/clients/bitpay_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/currency_client.py` & `bitpay-6.0.3/src/bitpay/clients/currency_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/invoice_client.py` & `bitpay-6.0.3/src/bitpay/clients/invoice_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/ledger_client.py` & `bitpay-6.0.3/src/bitpay/clients/ledger_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/payout_client.py` & `bitpay-6.0.3/src/bitpay/clients/payout_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/payout_recipient_client.py` & `bitpay-6.0.3/src/bitpay/clients/payout_recipient_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/rate_client.py` & `bitpay-6.0.3/src/bitpay/clients/rate_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/refund_client.py` & `bitpay-6.0.3/src/bitpay/clients/refund_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/response_parser.py` & `bitpay-6.0.3/src/bitpay/clients/response_parser.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/settlement_client.py` & `bitpay-6.0.3/src/bitpay/clients/settlement_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/clients/wallet_client.py` & `bitpay-6.0.3/src/bitpay/clients/wallet_client.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/exceptions/bitpay_api_exception.py` & `bitpay-6.0.3/src/bitpay/exceptions/bitpay_api_exception.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/exceptions/bitpay_exception_provider.py` & `bitpay-6.0.3/src/bitpay/exceptions/bitpay_exception_provider.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/logger/logger_provider.py` & `bitpay-6.0.3/src/bitpay/logger/logger_provider.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/logger/logging_logger.py` & `bitpay-6.0.3/src/bitpay/logger/logging_logger.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/bill/bill.py` & `bitpay-6.0.3/src/bitpay/models/bill/bill.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/bitpay_model.py` & `bitpay-6.0.3/src/bitpay/models/bitpay_model.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/currency.py` & `bitpay-6.0.3/src/bitpay/models/currency.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/buyer.py` & `bitpay-6.0.3/src/bitpay/models/invoice/buyer.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/buyer_fields.py` & `bitpay-6.0.3/src/bitpay/models/invoice/buyer_fields.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/buyer_provided_info.py` & `bitpay-6.0.3/src/bitpay/models/invoice/buyer_provided_info.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/invoice.py` & `bitpay-6.0.3/src/bitpay/models/invoice/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Invoice
 """
 
+from decimal import *
 from typing import List, Union, Dict
 from pydantic import Field
 from .buyer import Buyer
 from .buyer_provided_info import BuyerProvidedInfo
 from .invoice_refund_addresses import InvoiceRefundAddress
 from .miner_fees import MinerFees
 from .refund_info import RefundInfo
@@ -37,16 +38,16 @@
     notification_email: Union[str, None] = None
     redirect_url: Union[str, None] = Field(alias="redirectURL", default=None)
     order_id: Union[str, None] = None
     item_desc: Union[str, None] = None
     item_code: Union[str, None] = None
     physical: Union[bool, None] = False
     payment_currencies: Union[List[str], None] = None
-    payment_subtotals: Union[Dict[str, int], None] = None
-    payment_totals: Union[Dict[str, int], None] = None
+    payment_subtotals: Union[Dict[str, Decimal], None] = None
+    payment_totals: Union[Dict[str, Decimal], None] = None
     payment_display_totals: Union[Dict[str, str], None] = None
     payment_display_subtotals: Union[Dict[str, str], None] = None
     payment_codes: Union[Dict[str, Dict[str, str]], None] = None
     acceptance_window: Union[int, None] = None
     buyer: Union[Buyer, None] = None
     refund_addresses: Union[List[Dict[str, InvoiceRefundAddress]], None] = None
     close_url: Union[str, None] = Field(alias="closeURL", default=None)
```

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/invoice_webhook.py` & `bitpay-6.0.3/src/bitpay/models/invoice/invoice_webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from decimal import *
 from typing import Union, Dict
 
 from bitpay.models.bitpay_model import BitPayModel
 from bitpay.models.invoice.buyer_fields import BuyerFields
 
 
 class InvoiceWebhook(BitPayModel):
@@ -10,16 +11,16 @@
     currency: Union[str, None] = None
     currency_time: Union[str, None] = None
     exception_status: Union[str, None] = None
     exchange_rates: Union[Dict[str, Dict[str, float]], None] = None
     id: Union[str, None] = None
     invoice_time: Union[str, None] = None
     order_id: Union[str, None] = None
-    payment_subtotals: Union[Dict[str, int], None] = None
-    payment_totals: Union[Dict[str, int], None] = None
+    payment_subtotals: Union[Dict[str, Decimal], None] = None
+    payment_totals: Union[Dict[str, Decimal], None] = None
     pos_data: Union[str, None] = None
     price: Union[float, None] = None
     status: Union[str, None] = None
     transaction_currency: Union[str, None] = None
     url: Union[str, None] = None
     in_invoice_id: Union[str, None] = None
     in_payment_request: Union[str, None] = None
```

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/miner_fees.py` & `bitpay-6.0.3/src/bitpay/models/invoice/miner_fees.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/miner_fees_item.py` & `bitpay-6.0.3/src/bitpay/models/invoice/miner_fees_item.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/refund.py` & `bitpay-6.0.3/src/bitpay/models/invoice/refund.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/refund_webhook.py` & `bitpay-6.0.3/src/bitpay/models/invoice/refund_webhook.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/supported_transaction_currencies.py` & `bitpay-6.0.3/src/bitpay/models/invoice/supported_transaction_currencies.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/invoice/transaction.py` & `bitpay-6.0.3/src/bitpay/models/invoice/transaction.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/ledger/buyer.py` & `bitpay-6.0.3/src/bitpay/models/ledger/buyer.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/ledger/ledger_entry.py` & `bitpay-6.0.3/src/bitpay/models/ledger/ledger_entry.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/payout/payout.py` & `bitpay-6.0.3/src/bitpay/models/payout/payout.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/payout/payout_recipient.py` & `bitpay-6.0.3/src/bitpay/models/payout/payout_recipient.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/payout/payout_transaction.py` & `bitpay-6.0.3/src/bitpay/models/payout/payout_transaction.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/payout/payout_webhook.py` & `bitpay-6.0.3/src/bitpay/models/payout/payout_webhook.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/rate/rates.py` & `bitpay-6.0.3/src/bitpay/models/rate/rates.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/settlement/invoice_data.py` & `bitpay-6.0.3/src/bitpay/models/settlement/invoice_data.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/settlement/payout_info.py` & `bitpay-6.0.3/src/bitpay/models/settlement/payout_info.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/settlement/settlement.py` & `bitpay-6.0.3/src/bitpay/models/settlement/settlement.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/settlement/settlement_ledger_entry.py` & `bitpay-6.0.3/src/bitpay/models/settlement/settlement_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/wallet/currencies.py` & `bitpay-6.0.3/src/bitpay/models/wallet/currencies.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/models/wallet/wallet.py` & `bitpay-6.0.3/src/bitpay/models/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/utils/key_utils.py` & `bitpay-6.0.3/src/bitpay/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/utils/model_util.py` & `bitpay-6.0.3/src/bitpay/utils/model_util.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay/utils/token_container.py` & `bitpay-6.0.3/src/bitpay/utils/token_container.py`

 * *Files identical despite different names*

### Comparing `bitpay-6.0.2/src/bitpay.egg-info/PKG-INFO` & `bitpay-6.0.3/src/bitpay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitpay
-Version: 6.0.2
+Version: 6.0.3
 Summary: Accept bitcoin with BitPay
 Author-email: Antonio Buedo <sales-engineering@bitpay.com>
 Project-URL: Homepage, https://github.com/bitpay/python-bitpay-client
 Project-URL: Bug Tracker, https://github.com/bitpay/python-bitpay-client/issues
 Keywords: bitcoin,payments,crypto,cash,ethereum,online payments
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `bitpay-6.0.2/src/bitpay.egg-info/SOURCES.txt` & `bitpay-6.0.3/src/bitpay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

