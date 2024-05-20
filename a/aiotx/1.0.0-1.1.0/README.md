# Comparing `tmp/aiotx-1.0.0.tar.gz` & `tmp/aiotx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-1.0.0.tar", last modified: Sun May 19 09:59:19 2024, max compression
+gzip compressed data, was "aiotx-1.1.0.tar", last modified: Sun May 19 13:16:13 2024, max compression
```

## Comparing `aiotx-1.0.0.tar` & `aiotx-1.1.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.495382 aiotx-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.435382 aiotx-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 09:59:13.000000 aiotx-1.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-19 09:59:13.000000 aiotx-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-19 09:59:13.000000 aiotx-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-19 09:59:13.000000 aiotx-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 09:59:13.000000 aiotx-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-19 09:59:13.000000 aiotx-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 09:59:19.495382 aiotx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-19 09:59:13.000000 aiotx-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.435382 aiotx-1.0.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18394 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/clients/_utxo_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/utils/bep20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-19 09:59:13.000000 aiotx-1.0.0/aiotx/utils/erc20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.495382 aiotx-1.0.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 09:59:19.000000 aiotx-1.0.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.439382 aiotx-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/docs/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/docs/clients/evm_client/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_contract_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_contract_decimals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_gas_price.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_last_block.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/get_transaction_count.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/send_token.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/evm_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/docs/clients/tron_client/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/tron_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/docs/clients/utxo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/estimate_smart_fee.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/from_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/get_last_block_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/import_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/send_bulk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/clients/utxo_client/to_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/monitoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-19 09:59:13.000000 aiotx-1.0.0/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 09:59:13.000000 aiotx-1.0.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-19 09:59:13.000000 aiotx-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 09:59:13.000000 aiotx-1.0.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-19 09:59:13.000000 aiotx-1.0.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 09:59:19.495382 aiotx-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-19 09:59:13.000000 aiotx-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.443382 aiotx-1.0.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.447382 aiotx-1.0.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.459382 aiotx-1.0.0/tests/fixtures/cassettes/btc/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-19 09:59:13.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 10849634 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 21956267 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.487382 aiotx-1.0.0/tests/fixtures/cassettes/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/fixtures/cassettes/ltc/
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    40578 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28458 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/fixtures/networks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/tests/test_evm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/test_evm/test_bsc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/test_evm/test_eth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/test_eth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/test_eth_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_evm/test_eth/test_eth_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.431383 aiotx-1.0.0/tests/test_utxo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.491382 aiotx-1.0.0/tests/test_utxo/test_btc/
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_btc/test_btc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_btc/test_btc_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:19.495382 aiotx-1.0.0/tests/test_utxo/test_ltc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_ltc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-19 09:59:14.000000 aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.443337 aiotx-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-19 13:16:02.000000 aiotx-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 13:16:02.000000 aiotx-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-19 13:16:02.000000 aiotx-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 13:16:02.000000 aiotx-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-19 13:16:02.000000 aiotx-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 13:16:13.443337 aiotx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-19 13:16:02.000000 aiotx-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/_utxo_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.387336 aiotx-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.387336 aiotx-1.1.0/docs/clients/evm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_contract_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_contract_decimals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/send_token.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.387336 aiotx-1.1.0/docs/clients/tron_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/docs/clients/utxo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/estimate_smart_fee.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/from_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_last_block_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/import_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/send_bulk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/to_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-19 13:16:02.000000 aiotx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 13:16:02.000000 aiotx-1.1.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-19 13:16:02.000000 aiotx-1.1.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 13:16:13.443337 aiotx-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-19 13:16:02.000000 aiotx-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.395336 aiotx-1.1.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.407336 aiotx-1.1.0/tests/fixtures/cassettes/btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 10849634 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 21956267 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.435337 aiotx-1.1.0/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/fixtures/cassettes/ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    40578 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    28458 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/networks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/tests/test_evm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_evm/test_bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_evm/test_eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/test_eth_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/tests/test_utxo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_utxo/test_btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_utxo/test_ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_ltc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
```

### Comparing `aiotx-1.0.0/.github/workflows/lint-check.yml` & `aiotx-1.1.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/.github/workflows/python-publish.yml` & `aiotx-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/.github/workflows/static.yml` & `aiotx-1.1.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/.github/workflows/test.yml` & `aiotx-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/.gitignore` & `aiotx-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/CHANGELOG.md` & `aiotx-1.1.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [1.1.0]
+- UTXO client hotfix - we should have keys for all used inputs and not just for all inputs
+
 ## [1.0.0]
 - LTC/BTC logic and tests added
 
 ## [0.6.0]
 - UTXO client block monitoring logic added and tested for LTC and BTC (both covered by tests)
 
 ## [0.5.1]
```

### Comparing `aiotx-1.0.0/CODE_OF_CONDUCT.md` & `aiotx-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/CONTRIBUTING.md` & `aiotx-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/LICENSE` & `aiotx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/PKG-INFO` & `aiotx-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.0.0
+Version: 1.1.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
```

### Comparing `aiotx-1.0.0/README.md` & `aiotx-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx/clients/__init__.py` & `aiotx-1.1.0/aiotx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx/clients/_base_client.py` & `aiotx-1.1.0/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx/clients/_evm_base_client.py` & `aiotx-1.1.0/aiotx/clients/_evm_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx/clients/_utxo_base_client.py` & `aiotx-1.1.0/aiotx/clients/_utxo_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             empty_fee_transaction.fee_per_kb = fee_per_kb
             empty_fee_transaction = self._sign_transaction(empty_fee_transaction, [private_key])
             empty_fee_transaction.estimate_size()
             total_fee = empty_fee_transaction.calculate_fee()
 
         transaction, inputs_used = await self._create_transaction(destinations, utxo_list, from_address, total_fee, deduct_fee)
 
-        signed_tx = self._sign_transaction(transaction, [private_key] * len(utxo_list))
+        signed_tx = self._sign_transaction(transaction, [private_key] * len(inputs_used))
         txid = await self._send_transaction(signed_tx.raw_hex())
         await self._mark_inputs_as_used(inputs_used)
         return txid
 
     async def send(
         self,
         private_key: str,
```

### Comparing `aiotx-1.0.0/aiotx/exceptions.py` & `aiotx-1.1.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx/utils/bep20_abi.json` & `aiotx-1.1.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx/utils/erc20_abi.json` & `aiotx-1.1.0/aiotx/utils/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/aiotx.egg-info/PKG-INFO` & `aiotx-1.1.0/aiotx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.0.0
+Version: 1.1.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
```

### Comparing `aiotx-1.0.0/aiotx.egg-info/SOURCES.txt` & `aiotx-1.1.0/aiotx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/Makefile` & `aiotx-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/get_balance.rst` & `aiotx-1.1.0/docs/clients/evm_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/get_block_by_number.rst` & `aiotx-1.1.0/docs/clients/evm_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/get_contract_balance.rst` & `aiotx-1.1.0/docs/clients/evm_client/get_contract_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/get_contract_decimals.rst` & `aiotx-1.1.0/docs/clients/evm_client/get_contract_decimals.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/get_transaction.rst` & `aiotx-1.1.0/docs/clients/evm_client/get_transaction.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/get_transaction_count.rst` & `aiotx-1.1.0/docs/clients/evm_client/get_transaction_count.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/index.rst` & `aiotx-1.1.0/docs/clients/evm_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/send.rst` & `aiotx-1.1.0/docs/clients/evm_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/evm_client/send_token.rst` & `aiotx-1.1.0/docs/clients/evm_client/send_token.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/estimate_smart_fee.rst` & `aiotx-1.1.0/docs/clients/utxo_client/estimate_smart_fee.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/generate_address.rst` & `aiotx-1.1.0/docs/clients/utxo_client/generate_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/get_address_from_private_key.rst` & `aiotx-1.1.0/docs/clients/utxo_client/get_address_from_private_key.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/get_balance.rst` & `aiotx-1.1.0/docs/clients/utxo_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/get_block_by_number.rst` & `aiotx-1.1.0/docs/clients/utxo_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/import_address.rst` & `aiotx-1.1.0/docs/clients/utxo_client/import_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/index.rst` & `aiotx-1.1.0/docs/clients/utxo_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/send.rst` & `aiotx-1.1.0/docs/clients/utxo_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/clients/utxo_client/send_bulk.rst` & `aiotx-1.1.0/docs/clients/utxo_client/send_bulk.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/conf.py` & `aiotx-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/index.rst` & `aiotx-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/make.bat` & `aiotx-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/monitoring.rst` & `aiotx-1.1.0/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/docs/testing.rst` & `aiotx-1.1.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/examples/aiogram_notificator_bot.png` & `aiotx-1.1.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/examples/aiogram_notificator_bot.py` & `aiotx-1.1.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/examples/block_and_transactions_parser.py` & `aiotx-1.1.0/examples/block_and_transactions_parser.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/examples/two_block_parsers.py` & `aiotx-1.1.0/examples/two_block_parsers.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/setup.py` & `aiotx-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/conftest.py` & `aiotx-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/btc/send_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/btc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_balance.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_gas_price.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_last_block.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_token_balance.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/get_last_block.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_bulk.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_bulk.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_transaction.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml` & `aiotx-1.1.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/fixtures/networks.json` & `aiotx-1.1.0/tests/fixtures/networks.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_client.py` & `aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py` & `aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_evm/test_bsc/test_bsc_monitoring.py` & `aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_evm/test_eth/test_eth_client.py` & `aiotx-1.1.0/tests/test_evm/test_eth/test_eth_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_evm/test_eth/test_eth_input_decoding.py` & `aiotx-1.1.0/tests/test_evm/test_eth/test_eth_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_evm/test_eth/test_eth_monitoring.py` & `aiotx-1.1.0/tests/test_evm/test_eth/test_eth_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_utxo/test_btc/test_btc_client.py` & `aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_utxo/test_btc/test_btc_monitor.py` & `aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_monitor.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_client.py` & `aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.0.0/tests/test_utxo/test_ltc/test_ltc_monitor.py` & `aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_monitor.py`

 * *Files identical despite different names*

