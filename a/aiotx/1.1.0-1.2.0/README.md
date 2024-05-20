# Comparing `tmp/aiotx-1.1.0.tar.gz` & `tmp/aiotx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-1.1.0.tar", last modified: Sun May 19 13:16:13 2024, max compression
+gzip compressed data, was "aiotx-1.2.0.tar", last modified: Mon May 20 05:49:24 2024, max compression
```

## Comparing `aiotx-1.1.0.tar` & `aiotx-1.2.0.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.443337 aiotx-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 13:16:02.000000 aiotx-1.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-19 13:16:02.000000 aiotx-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-19 13:16:02.000000 aiotx-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-19 13:16:02.000000 aiotx-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 13:16:02.000000 aiotx-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-19 13:16:02.000000 aiotx-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 13:16:13.443337 aiotx-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-19 13:16:02.000000 aiotx-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/clients/_utxo_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.383336 aiotx-1.1.0/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/utils/bep20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-19 13:16:02.000000 aiotx-1.1.0/aiotx/utils/erc20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 13:16:13.000000 aiotx-1.1.0/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.387336 aiotx-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/docs/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.387336 aiotx-1.1.0/docs/clients/evm_client/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_contract_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_contract_decimals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_gas_price.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_last_block.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/get_transaction_count.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/send_token.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/evm_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.387336 aiotx-1.1.0/docs/clients/tron_client/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/tron_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/docs/clients/utxo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/estimate_smart_fee.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/from_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/get_last_block_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/import_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/send_bulk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/clients/utxo_client/to_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/monitoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-19 13:16:02.000000 aiotx-1.1.0/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-19 13:16:02.000000 aiotx-1.1.0/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-19 13:16:02.000000 aiotx-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 13:16:02.000000 aiotx-1.1.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-19 13:16:02.000000 aiotx-1.1.0/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 13:16:13.443337 aiotx-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-19 13:16:02.000000 aiotx-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.391336 aiotx-1.1.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.395336 aiotx-1.1.0/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.407336 aiotx-1.1.0/tests/fixtures/cassettes/btc/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 10849634 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 21956267 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.435337 aiotx-1.1.0/tests/fixtures/cassettes/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/fixtures/cassettes/ltc/
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    40578 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28458 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/fixtures/networks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/tests/test_evm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_evm/test_bsc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_evm/test_eth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/test_eth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/test_eth_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_evm/test_eth/test_eth_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.379336 aiotx-1.1.0/tests/test_utxo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_utxo/test_btc/
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:13.439337 aiotx-1.1.0/tests/test_utxo/test_ltc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_ltc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-19 13:16:02.000000 aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.402900 aiotx-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.406900 aiotx-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-20 05:49:18.000000 aiotx-1.2.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-20 05:49:18.000000 aiotx-1.2.0/.github/workflows/mysql_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 05:49:18.000000 aiotx-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-20 05:49:18.000000 aiotx-1.2.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 05:49:18.000000 aiotx-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-20 05:49:18.000000 aiotx-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-20 05:49:18.000000 aiotx-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-20 05:49:18.000000 aiotx-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-20 05:49:18.000000 aiotx-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-20 05:49:18.000000 aiotx-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-20 05:49:24.462900 aiotx-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-20 05:49:18.000000 aiotx-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.406900 aiotx-1.2.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.406900 aiotx-1.2.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18874 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/clients/_utxo_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.406900 aiotx-1.2.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.406900 aiotx-1.2.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-20 05:49:18.000000 aiotx-1.2.0/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-20 05:49:24.000000 aiotx-1.2.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-20 05:49:24.000000 aiotx-1.2.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:49:24.000000 aiotx-1.2.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 05:49:24.000000 aiotx-1.2.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 05:49:24.000000 aiotx-1.2.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.410900 aiotx-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.402900 aiotx-1.2.0/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.410900 aiotx-1.2.0/docs/clients/evm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_contract_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_contract_decimals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/send_token.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/evm_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.410900 aiotx-1.2.0/docs/clients/tron_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/tron_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/tron_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/tron_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/tron_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.414900 aiotx-1.2.0/docs/clients/utxo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/estimate_smart_fee.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/from_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/get_last_block_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/import_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/send_bulk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/clients/utxo_client/to_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-20 05:49:18.000000 aiotx-1.2.0/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.414900 aiotx-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-20 05:49:18.000000 aiotx-1.2.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 05:49:18.000000 aiotx-1.2.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-20 05:49:18.000000 aiotx-1.2.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 05:49:18.000000 aiotx-1.2.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-20 05:49:18.000000 aiotx-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 05:49:18.000000 aiotx-1.2.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.414900 aiotx-1.2.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-20 05:49:18.000000 aiotx-1.2.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-20 05:49:24.466900 aiotx-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-20 05:49:18.000000 aiotx-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.414900 aiotx-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.414900 aiotx-1.2.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.402900 aiotx-1.2.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.418900 aiotx-1.2.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.430900 aiotx-1.2.0/tests/fixtures/cassettes/btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/btc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 10849634 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 21956267 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.458900 aiotx-1.2.0/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/tests/fixtures/cassettes/ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    40578 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    28458 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/fixtures/networks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.402900 aiotx-1.2.0/tests/test_evm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/tests/test_evm/test_bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_bsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_bsc/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/tests/test_evm/test_eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_eth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_eth/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_eth/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_evm/test_eth/test_eth_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.402900 aiotx-1.2.0/tests/test_utxo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/tests/test_utxo/test_btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_utxo/test_btc/test_btc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_utxo/test_btc/test_btc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:24.462900 aiotx-1.2.0/tests/test_utxo/test_ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_utxo/test_ltc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_utxo/test_ltc/test_ltc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-20 05:49:18.000000 aiotx-1.2.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
```

### Comparing `aiotx-1.1.0/.github/workflows/lint-check.yml` & `aiotx-1.2.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/.github/workflows/python-publish.yml` & `aiotx-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/.github/workflows/static.yml` & `aiotx-1.2.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/.github/workflows/test.yml` & `aiotx-1.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/.gitignore` & `aiotx-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/CHANGELOG.md` & `aiotx-1.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [1.2.0]
+- UTXO client - adding UTXOs after send, so we will able to send few transactions in same block
+    without waiting for new one to get our UTXOs
+
 ## [1.1.0]
 - UTXO client hotfix - we should have keys for all used inputs and not just for all inputs
 
 ## [1.0.0]
 - LTC/BTC logic and tests added
 
 ## [0.6.0]
```

### Comparing `aiotx-1.1.0/CODE_OF_CONDUCT.md` & `aiotx-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/CONTRIBUTING.md` & `aiotx-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/LICENSE` & `aiotx-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/PKG-INFO` & `aiotx-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.1.0
+Version: 1.2.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
```

### Comparing `aiotx-1.1.0/README.md` & `aiotx-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx/clients/__init__.py` & `aiotx-1.2.0/aiotx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx/clients/_base_client.py` & `aiotx-1.2.0/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx/clients/_evm_base_client.py` & `aiotx-1.2.0/aiotx/clients/_evm_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx/clients/_utxo_base_client.py` & `aiotx-1.2.0/aiotx/clients/_utxo_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         return result["result"]
 
     async def get_balance(self, address: str) -> int:
         utxo_data = await self.monitor._get_utxo_data(address)
         if len(utxo_data) == 0:
             return 0
         return sum(utxo.amount_satoshi for utxo in utxo_data)
-
+    
     async def _build_and_send_transaction(
         self,
         private_key: str,
         destinations: dict[str, int],
         conf_target: int,
         estimate_mode: FeeEstimate,
         total_fee: Optional[int],
@@ -127,30 +127,40 @@
         deduct_fee: bool
     ) -> str:
         from_wallet = self.get_address_from_private_key(private_key)
         from_address = from_wallet["address"]
         utxo_list = await self.monitor._get_utxo_data(from_address)
 
         if total_fee is None:
-            empty_fee_transaction, _ = await self._create_transaction(destinations, utxo_list, from_address, 0, deduct_fee)
+            empty_fee_transaction, _, _ = await self._create_transaction(destinations, utxo_list, from_address, 0, deduct_fee)
             if fee_per_byte is None:
                 fee_per_kb = await self.estimate_smart_fee(conf_target, estimate_mode)
             else:
                 fee_per_kb = fee_per_byte * 1024
             empty_fee_transaction.fee_per_kb = fee_per_kb
             empty_fee_transaction = self._sign_transaction(empty_fee_transaction, [private_key])
             empty_fee_transaction.estimate_size()
             total_fee = empty_fee_transaction.calculate_fee()
 
-        transaction, inputs_used = await self._create_transaction(destinations, utxo_list, from_address, total_fee, deduct_fee)
+        transaction, inputs_used, outputs_used = await self._create_transaction(destinations, utxo_list, from_address, total_fee, deduct_fee)
 
         signed_tx = self._sign_transaction(transaction, [private_key] * len(inputs_used))
         txid = await self._send_transaction(signed_tx.raw_hex())
         await self._mark_inputs_as_used(inputs_used)
+        await self._save_pending_outputs(outputs_used, from_address, txid)
         return txid
+    
+
+    async def _save_pending_outputs(self, outputs_used, from_address: str, tx_id: str):
+        for i, output in enumerate(outputs_used):
+            destination_address = output[0]
+            if from_address != destination_address:
+                continue
+            amount = output[1]
+            await self.monitor._add_new_utxo(from_address, tx_id, amount, i)
 
     async def send(
         self,
         private_key: str,
         to_address: str,
         amount: int,
         total_fee: int = None,
@@ -211,15 +221,15 @@
             prev_tx_id, prev_out_index, value = input_data
             transaction.add_input(prev_txid=prev_tx_id, output_n=prev_out_index, value=value, witness_type="segwit")
 
         for output_data in outputs:
             address, value = output_data
             transaction.add_output(value=value, address=address)
 
-        return transaction, inputs
+        return transaction, inputs, outputs
 
     def _sign_transaction(self, transaction: Transaction, private_keys: list[str]) -> Transaction:
         for i, private_key in enumerate(private_keys):
             key = Key(private_key)
             transaction.sign(key, i)
         return transaction
```

### Comparing `aiotx-1.1.0/aiotx/exceptions.py` & `aiotx-1.2.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx/utils/bep20_abi.json` & `aiotx-1.2.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx/utils/erc20_abi.json` & `aiotx-1.2.0/aiotx/utils/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/aiotx.egg-info/PKG-INFO` & `aiotx-1.2.0/aiotx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.1.0
+Version: 1.2.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
```

### Comparing `aiotx-1.1.0/aiotx.egg-info/SOURCES.txt` & `aiotx-1.2.0/aiotx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 LICENSE
 README.md
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 .github/workflows/lint-check.yml
+.github/workflows/mysql_test.yml
 .github/workflows/python-publish.yml
 .github/workflows/static.yml
 .github/workflows/test.yml
 aiotx/__init__.py
 aiotx/exceptions.py
 aiotx.egg-info/PKG-INFO
 aiotx.egg-info/SOURCES.txt
```

### Comparing `aiotx-1.1.0/docs/Makefile` & `aiotx-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/get_balance.rst` & `aiotx-1.2.0/docs/clients/evm_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/get_block_by_number.rst` & `aiotx-1.2.0/docs/clients/evm_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/get_contract_balance.rst` & `aiotx-1.2.0/docs/clients/evm_client/get_contract_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/get_contract_decimals.rst` & `aiotx-1.2.0/docs/clients/evm_client/get_contract_decimals.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/get_transaction.rst` & `aiotx-1.2.0/docs/clients/evm_client/get_transaction.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/get_transaction_count.rst` & `aiotx-1.2.0/docs/clients/evm_client/get_transaction_count.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/index.rst` & `aiotx-1.2.0/docs/clients/evm_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/send.rst` & `aiotx-1.2.0/docs/clients/evm_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/evm_client/send_token.rst` & `aiotx-1.2.0/docs/clients/evm_client/send_token.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/estimate_smart_fee.rst` & `aiotx-1.2.0/docs/clients/utxo_client/estimate_smart_fee.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/generate_address.rst` & `aiotx-1.2.0/docs/clients/utxo_client/generate_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/get_address_from_private_key.rst` & `aiotx-1.2.0/docs/clients/utxo_client/get_address_from_private_key.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/get_balance.rst` & `aiotx-1.2.0/docs/clients/utxo_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/get_block_by_number.rst` & `aiotx-1.2.0/docs/clients/utxo_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/import_address.rst` & `aiotx-1.2.0/docs/clients/utxo_client/import_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/index.rst` & `aiotx-1.2.0/docs/clients/utxo_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/send.rst` & `aiotx-1.2.0/docs/clients/utxo_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/clients/utxo_client/send_bulk.rst` & `aiotx-1.2.0/docs/clients/utxo_client/send_bulk.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/conf.py` & `aiotx-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/index.rst` & `aiotx-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/make.bat` & `aiotx-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/monitoring.rst` & `aiotx-1.2.0/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/docs/testing.rst` & `aiotx-1.2.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/examples/aiogram_notificator_bot.png` & `aiotx-1.2.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/examples/aiogram_notificator_bot.py` & `aiotx-1.2.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/examples/block_and_transactions_parser.py` & `aiotx-1.2.0/examples/block_and_transactions_parser.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/examples/two_block_parsers.py` & `aiotx-1.2.0/examples/two_block_parsers.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/setup.py` & `aiotx-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/conftest.py` & `aiotx-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/btc/send_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/btc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_balance.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_gas_price.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_last_block.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_token_balance.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/get_last_block.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_bulk.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_bulk.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_transaction.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml` & `aiotx-1.2.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/fixtures/networks.json` & `aiotx-1.2.0/tests/fixtures/networks.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_client.py` & `aiotx-1.2.0/tests/test_evm/test_bsc/test_bsc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py` & `aiotx-1.2.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_evm/test_bsc/test_bsc_monitoring.py` & `aiotx-1.2.0/tests/test_evm/test_bsc/test_bsc_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_evm/test_eth/test_eth_client.py` & `aiotx-1.2.0/tests/test_evm/test_eth/test_eth_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_evm/test_eth/test_eth_input_decoding.py` & `aiotx-1.2.0/tests/test_evm/test_eth/test_eth_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_evm/test_eth/test_eth_monitoring.py` & `aiotx-1.2.0/tests/test_evm/test_eth/test_eth_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_client.py` & `aiotx-1.2.0/tests/test_utxo/test_btc/test_btc_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 
     amount = 1000
     fee = btc_client.to_satoshi(0.00001)
     tx_id = await btc_client.send(
         TEST_BTC_WALLET_PRIVATE_KEY, "tb1q4tf08gc2vf8dgfqtd3jen3s5tddz6uu0mnyf90", amount, fee
     )
     utxo_list = await btc_client.monitor._get_utxo_data(TEST_BTC_ADDRESS)
-    assert len(utxo_list) == 0
+    utxo_list = await btc_client.monitor._get_utxo_data(TEST_BTC_ADDRESS)
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "4f9a64d28ae22134379f7da50282d7ca2ead8a1f8378b20e25defcaaa5c59228"
+    assert utxo_list[0][2] == 14263
     assert tx_id == "4f9a64d28ae22134379f7da50282d7ca2ead8a1f8378b20e25defcaaa5c59228"
     await btc_client.monitor._delete_utxo("25d56f693d5c4d00d3f98e58c8bd66e8db930e38c8a556bd67737b66cbf31ab9", 0)
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
@@ -53,15 +56,17 @@
             "2NDYhjHKdPLYjD5kVZVgeo8JxDrDUcRC14Q": amount,  # P2SH address
             "tb1qq4ay9zw2mygwucz47v6hsda04a9l2yajyynh00": amount,  # Bech32 address
             "tb1pwgjc67568cu6vncgve60t6eaht0rwr4pwdymnrpezrpepg3q5t8sp5250h": amount,  # Bech32M address
         },
         fee,
     )
     utxo_list = await btc_client.monitor._get_utxo_data(TEST_BTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "35158b7a8b6057bc67f6d904c64b5986adea8260f0bc96cbd755b530878e3cc2"
+    assert utxo_list[0][2] == 6263
     assert tx_id == "35158b7a8b6057bc67f6d904c64b5986adea8260f0bc96cbd755b530878e3cc2"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -75,17 +80,21 @@
     amount = 1000
     tx_id = await btc_client.send_bulk(
         TEST_BTC_WALLET_PRIVATE_KEY,
         {"mtkbaiLiUH3fvGJeSzuN3kUgmJzqinLejJ": amount},
         conf_target=1,
         estimate_mode=FeeEstimate.CONSERVATIVE,
     )
+    
+    assert tx_id == "77cb20c4b0325242b9e5f45f4850e5387dc585d6b72bb36ba65a126534436973"
+
     utxo_list = await btc_client.monitor._get_utxo_data(TEST_BTC_ADDRESS)
+    print("utxo_list", utxo_list)
     assert len(utxo_list) == 0
-    assert tx_id == "77cb20c4b0325242b9e5f45f4850e5387dc585d6b72bb36ba65a126534436973"
+
 
 
 
 async def test_get_balance(btc_client: AioTxBTCClient):
     await btc_client.monitor._add_new_address(TEST_BTC_ADDRESS)
     await btc_client.monitor._add_new_utxo(
         TEST_BTC_ADDRESS, "35158b7a8b6057bc67f6d904c64b5986adea8260f0bc96cbd755b530878e3cc2 ", 6263, 0
```

### Comparing `aiotx-1.1.0/tests/test_utxo/test_btc/test_btc_monitor.py` & `aiotx-1.2.0/tests/test_utxo/test_btc/test_btc_monitor.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_client.py` & `aiotx-1.2.0/tests/test_utxo/test_ltc/test_ltc_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,17 @@
     amount = ltc_public_client.to_satoshi(0.1)
     fee = ltc_public_client.to_satoshi(0.005)
     tx_id = await ltc_public_client.send(
         TEST_LTC_WALLET_PRIVATE_KEY, "tltc1q24gng65qj3wr55878324w2eeeta4k2plfwaf54", amount, fee
     )
     assert tx_id == "a006aedf3a08f423434aa781988997a0526f9365fe228fb8934ea64bbbb9d055"
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "a006aedf3a08f423434aa781988997a0526f9365fe228fb8934ea64bbbb9d055"
+    assert utxo_list[0][2] == 28500000
     await ltc_public_client.monitor._delete_utxo("55863cc61de0c6c1c87282d3d6fb03650c0fc90ed3282191c618069cbde1d525", 0)
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -71,15 +73,17 @@
         {
             "tltc1q24gng65qj3wr55878324w2eeeta4k2plfwaf54": amount,
             "tltc1qshy0jeejm4pw3ep4cedc5vlmxyz348epnk7etf": amount,
         },
         fee,
     )
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "64a89e7e269469c126e96d1de7b553850716c71d9081b153429ff781758a59a1"
+    assert utxo_list[0][2] == 20000000
     assert tx_id == "64a89e7e269469c126e96d1de7b553850716c71d9081b153429ff781758a59a1"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -92,15 +96,17 @@
     )
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "64a89e7e269469c126e96d1de7b553850716c71d9081b153429ff781758a59a1", 20000000, 0
     )
     amount = 28500000 + 20000000 - fee
     tx_id = await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, TEST_LTC_ADDRESS, amount, fee)
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "3fcd11698664ffea5fe00adef6bd2c1c35de66c3fafb50f9076c74ff13fea139"
+    assert utxo_list[0][2] == 48000000
     assert tx_id == "3fcd11698664ffea5fe00adef6bd2c1c35de66c3fafb50f9076c74ff13fea139"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -110,15 +116,17 @@
     await ltc_public_client.monitor._add_new_address(TEST_LTC_ADDRESS)
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "3fcd11698664ffea5fe00adef6bd2c1c35de66c3fafb50f9076c74ff13fea139", 48000000, 0
     )
     amount = ltc_public_client.to_satoshi(0.005)
     tx_id = await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, "mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX", amount, fee)
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "141c30ea6326ab447423465d2a7f4c3067812f06ef1e505c0443e85c06ed684a"
+    assert utxo_list[0][2] == 47000000
     assert tx_id == "141c30ea6326ab447423465d2a7f4c3067812f06ef1e505c0443e85c06ed684a"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -132,15 +140,17 @@
     amount = ltc_public_client.to_satoshi(0.005)
     tx_id = await ltc_public_client.send_bulk(
         TEST_LTC_WALLET_PRIVATE_KEY,
         {"mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX": amount, "tltc1q24gng65qj3wr55878324w2eeeta4k2plfwaf54": amount},
         fee,
     )
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "33f67e7ac0dde523598f416f8efa5928d9e8a4a681db48f7df7d174701225dd0"
+    assert utxo_list[0][2] == 45500000
     assert tx_id == "33f67e7ac0dde523598f416f8efa5928d9e8a4a681db48f7df7d174701225dd0"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -149,15 +159,17 @@
     await ltc_public_client.monitor._add_new_address(TEST_LTC_ADDRESS)
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "33f67e7ac0dde523598f416f8efa5928d9e8a4a681db48f7df7d174701225dd0", 45500000, 0
     )
     amount = ltc_public_client.to_satoshi(0.005)
     tx_id = await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, "mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX", amount)
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "ac3c62cb37887a41235fecbc8dd22c8a8b5b74e1d2695dbc78e6d05a0cbdf2e9"
+    assert utxo_list[0][2] == 44999715
     assert tx_id == "ac3c62cb37887a41235fecbc8dd22c8a8b5b74e1d2695dbc78e6d05a0cbdf2e9"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
@@ -167,15 +179,17 @@
     utxo_amount = ltc_public_client.to_satoshi(0.44448584)
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "487933e5f8028e9235f76dacb368efd64bb6f038989ff92b217661c192f0055f", utxo_amount, 0
     )
     amount = ltc_public_client.to_satoshi(0.0055)
     tx_id = await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, "mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX", amount, deduct_fee=True)
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "3ed6c7a8e3b263679c47223f3e9c65721f865378e1b6799182f0607e1ebf9179"
+    assert utxo_list[0][2] == 43898584
     assert tx_id == "3ed6c7a8e3b263679c47223f3e9c65721f865378e1b6799182f0607e1ebf9179"
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
 @vcr_c.use_cassette("ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml")
@@ -187,15 +201,17 @@
     )
     amount = ltc_public_client.to_satoshi(0.005)
     tx_id = await ltc_public_client.send_bulk(TEST_LTC_WALLET_PRIVATE_KEY, {"mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX": amount,
                                                                             "tltc1qshy0jeejm4pw3ep4cedc5vlmxyz348epnk7etf": amount},
                                                                             deduct_fee=True)
     
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "e328d42e61f6b022c1534cd2e7e184180574172c988bea359f0b8e8734f178c6"
+    assert utxo_list[0][2] == 42397453
     assert tx_id == "e328d42e61f6b022c1534cd2e7e184180574172c988bea359f0b8e8734f178c6"
 
 
 async def test_zero_balance_error(ltc_public_client: AioTxLTCClient):
     await ltc_public_client.monitor._add_new_address(TEST_LTC_ADDRESS)
     amount = ltc_public_client.to_satoshi(0.005)
     with pytest.raises(InsufficientFunds) as excinfo:  
@@ -234,17 +250,21 @@
 
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "c2f8e76c9537e5defa921b31edeb269603b8adec025c04d8e8b0e5764b80b861", utxo_amount, 2
     )
     
     tx_id = await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, TEST_LTC_ADDRESS, amount, deduct_fee=True)
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 1
+    assert utxo_list[0][0] == "477ff66cdf3c97661c66d38a05cfae018d0358fec300a8b85bde65808e6cf8f9"
+    assert utxo_list[0][2] == 997636
     assert tx_id == "477ff66cdf3c97661c66d38a05cfae018d0358fec300a8b85bde65808e6cf8f9"
 
+    await ltc_public_client.monitor._mark_utxo_used("477ff66cdf3c97661c66d38a05cfae018d0358fec300a8b85bde65808e6cf8f9", 0)
+
     with pytest.raises(InsufficientFunds) as excinfo:  
         await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, TEST_LTC_ADDRESS, amount)
     assert str(excinfo.value) == "We have only 0 satoshi and it's 1000000 at least needed to cover that transaction!"
 
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "8117d7261873ab0bb49e195043d70693362cebe3275333678da5f738932bb3a7", utxo_amount, 2
     )
@@ -255,15 +275,17 @@
 
     await ltc_public_client.monitor._add_new_utxo(
         TEST_LTC_ADDRESS, "a51a47a487ab537dbf263d70a4ffd4535b57f479ba792c1549c4a4e9a44fcfb2", utxo_amount, 2
     )
     second_tx_amount = ltc_public_client.to_satoshi(0.012)
     tx_id = await ltc_public_client.send(TEST_LTC_WALLET_PRIVATE_KEY, TEST_LTC_ADDRESS, second_tx_amount)
     utxo_list = await ltc_public_client.monitor._get_utxo_data(TEST_LTC_ADDRESS)
-    assert len(utxo_list) == 0
+    assert len(utxo_list) == 2
+    balance = await ltc_public_client.get_balance(TEST_LTC_ADDRESS)
+    assert balance == 296321 + 1200000
     assert tx_id == "09dac3c34ce8013a074890cdc34f90e264fda192b995350b7ad6d283f7d9276d"
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Skipping transaction signing tests on Windows because we are not using RFC6979 from fastecdsa by default",
 )
```

### Comparing `aiotx-1.1.0/tests/test_utxo/test_ltc/test_ltc_monitor.py` & `aiotx-1.2.0/tests/test_utxo/test_ltc/test_ltc_monitor.py`

 * *Files identical despite different names*

