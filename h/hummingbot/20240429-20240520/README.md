# Comparing `tmp/hummingbot-20240429.tar.gz` & `tmp/hummingbot-20240520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hummingbot-20240429.tar", last modified: Mon May 13 02:15:01 2024, max compression
+gzip compressed data, was "hummingbot-20240520.tar", last modified: Mon May 20 21:30:08 2024, max compression
```

## Comparing `hummingbot-20240429.tar` & `hummingbot-20240520.tar`

### file list

```diff
@@ -1,964 +1,966 @@
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.577706 hummingbot-20240429/
--rw-r--r--   0 madcatz    (501) staff       (20)    11352 2024-05-13 01:39:58.000000 hummingbot-20240429/LICENSE
--rw-r--r--   0 madcatz    (501) staff       (20)     1748 2024-05-13 02:15:01.577592 hummingbot-20240429/PKG-INFO
--rw-r--r--   0 madcatz    (501) staff       (20)     9669 2024-05-13 01:39:58.000000 hummingbot-20240429/README.md
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.110349 hummingbot-20240429/bin/
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6821 2024-05-13 01:39:58.000000 hummingbot-20240429/bin/hummingbot_quickstart.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.111509 hummingbot-20240429/hummingbot/
--rw-r--r--   0 madcatz    (501) staff       (20)       11 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/VERSION
--rw-r--r--   0 madcatz    (501) staff       (20)     5811 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.114291 hummingbot-20240429/hummingbot/client/
--rw-r--r--   0 madcatz    (501) staff       (20)      655 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.124170 hummingbot-20240429/hummingbot/client/command/
--rw-r--r--   0 madcatz    (501) staff       (20)     1249 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9967 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/balance_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    22563 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/config_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6908 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/connect_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16234 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/create_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1458 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/exit_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4844 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/export_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6371 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/gateway_api_manager.py
--rw-r--r--   0 madcatz    (501) staff       (20)    41186 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/gateway_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)      916 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/help_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12319 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/history_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3698 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/import_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4566 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/mqtt_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3001 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/order_book_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)      344 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/pmm_script_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2571 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/previous_strategy_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2697 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/rate_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9686 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/silly_commands.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15078 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/start_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10502 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/status_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2552 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/stop_command.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2996 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/command/ticker_command.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.131082 hummingbot-20240429/hummingbot/client/config/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42100 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/client_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18418 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/conf_migration.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4553 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/config_crypt.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2726 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/config_data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    38116 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/config_helpers.py
--rw-r--r--   0 madcatz    (501) staff       (20)      633 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/config_methods.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7452 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/config_validators.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3189 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/config_var.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1404 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/fee_overrides_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)      364 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/gateway_ssl_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/global_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3858 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/security.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6288 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/strategy_config_data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3003 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/config/trade_fee_schema_loader.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.131590 hummingbot-20240429/hummingbot/client/data_type/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/data_type/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      426 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/data_type/currency_amount.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15273 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/hummingbot_application.py
--rw-r--r--   0 madcatz    (501) staff       (20)    13787 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/performance.py
--rw-r--r--   0 madcatz    (501) staff       (20)      516 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/platform.py
--rw-r--r--   0 madcatz    (501) staff       (20)    27252 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/settings.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.133078 hummingbot-20240429/hummingbot/client/tab/
--rw-r--r--   0 madcatz    (501) staff       (20)      135 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/tab/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      872 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/tab/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3140 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/tab/order_book_tab.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1723 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/tab/tab_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)      774 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/tab/tab_example_tab.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.138290 hummingbot-20240429/hummingbot/client/ui/
--rw-r--r--   0 madcatz    (501) staff       (20)     8435 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    24695 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/completer.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9614 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/custom_widgets.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11623 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/hummingbot_cli.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4952 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/interface_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3593 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/keybindings.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11632 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/layout.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11856 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/parser.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1710 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/scroll_handlers.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2524 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/stdout_redirection.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11314 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/client/ui/style.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.161829 hummingbot-20240429/hummingbot/connector/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7400 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/budget_checker.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18938 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/client_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1403631 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/connector_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     6375 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/connector_metrics_collector.py
--rw-r--r--   0 madcatz    (501) staff       (20)      215 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/constants.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.163522 hummingbot-20240429/hummingbot/connector/derivative/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.167575 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9683 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1944 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6016 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    38371 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6334 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2428 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4013 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.171599 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10413 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3497 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4597 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    35998 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5494 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2420 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2670 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.176222 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12125 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2898 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5025 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40405 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5830 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2002 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.180166 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15468 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3238 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5848 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    38897 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6821 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4168 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)    19340 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341067 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.183510 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12544 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4454 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3774 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40418 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2566 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2154 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2663 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.188901 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    10758 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3135 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5254 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    34398 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4492 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1634 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1851 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.194314 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341751 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    10842 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7056 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3695 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    35513 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5656 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4106 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5119 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.196685 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      466 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4840 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    48511 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3981 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.200800 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341181 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    14498 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8026 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6301 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6066 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    45173 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2117 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6479 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.203648 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    20796 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5462 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5960 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    39008 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6527 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2707 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12961 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1421 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/perpetual_budget_checker.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.206901 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12075 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5017 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2335 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6113 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    32650 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2679 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3838 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2238 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/position.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.210659 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    14929 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3977 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9352 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1466 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py
--rw-r--r--   0 madcatz    (501) staff       (20)    66373 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6581 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2481 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6529 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2528 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/derivative_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.211052 hummingbot-20240429/hummingbot/connector/exchange/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.213592 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7240 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3627 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2478 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5036 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26170 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2084 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2719 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.216324 hummingbot-20240429/hummingbot/connector/exchange/binance/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6402 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6081 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2413 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4688 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_constants.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    25993 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3224 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2972 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3154 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/binance_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/binance/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.237748 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/
--rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   785958 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    22384 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2224 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1580 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)  3066951 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   554137 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   576798 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1273 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10355 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1057 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5028 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.241403 hummingbot-20240429/hummingbot/connector/exchange/bitmart/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10154 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     4787 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2913 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2473 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    19821 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2451 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2538 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/bitmart/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.244704 hummingbot-20240429/hummingbot/connector/exchange/bitrue/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     8798 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2385 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6008 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_constants.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    30434 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3211 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_order_book.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     8058 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1604 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3128 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.247776 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9564 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4055 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4543 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3114 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25469 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4545 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1662 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2831 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.250729 hummingbot-20240429/hummingbot/connector/exchange/bybit/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12169 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5372 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3308 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    21562 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4246 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2581 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5170 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339537 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/bybit/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.255685 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11069 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    13923 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12512 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5500 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    50376 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7810 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2030 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7161 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341676 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.275178 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   928124 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp
--rwxr-xr-x   0 madcatz    (501) staff       (20)    14517 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     5006 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2753 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)      493 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2596840 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   499653 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   535675 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1816 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8848 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1041 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2361 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2530 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.278996 hummingbot-20240429/hummingbot/connector/exchange/cube/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    11507 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3570 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3643 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3062 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    50864 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4473 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4390 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.281765 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10219 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15363 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/py.typed
--rw-r--r--   0 madcatz    (501) staff       (20)    15992 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py
--rw-r--r--   0 madcatz    (501) staff       (20)    29121 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi
--rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/cube/dummy.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.285812 hummingbot-20240429/hummingbot/connector/exchange/foxbit/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10078 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5190 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3912 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)   345010 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     5253 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    44815 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7671 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5090 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4155 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.288791 hummingbot-20240429/hummingbot/connector/exchange/gate_io/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7620 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4310 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3166 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3528 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    22712 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1255 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   341880 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/gate_io/placeholder.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.296313 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   754683 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    11733 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3224 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2451 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1847 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42970 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3162 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2397 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5637 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)      945 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2346 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5706 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4686 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.298707 hummingbot-20240429/hummingbot/connector/exchange/htx/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8241 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5047 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3477 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2958 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18960 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1589 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2553 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/htx/htx_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.302327 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4257 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/account_delegation_script.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.304311 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    71837 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    23529 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12854 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    24074 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5962 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)       90 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_events.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4376 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_market.py
--rw-r--r--   0 madcatz    (501) staff       (20)    14999 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_query_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3669 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42627 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15808 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.307066 hummingbot-20240429/hummingbot/connector/exchange/kraken/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     7715 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3909 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2929 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4146 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    27389 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2903 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8041 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.311018 hummingbot-20240429/hummingbot/connector/exchange/kucoin/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339651 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     8742 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4879 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3663 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3297 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    24398 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2132 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3049 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3215 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.315991 hummingbot-20240429/hummingbot/connector/exchange/mexc/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/dummy.cpp
--rwxr-xr-x   0 madcatz    (501) staff       (20)     6556 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     8131 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2480 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4344 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_constants.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    26610 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3481 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1705 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.321918 hummingbot-20240429/hummingbot/connector/exchange/ndax/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    15461 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5670 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2103 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5426 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    49594 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2421 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3556 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3561 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5934 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2369 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4179 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.324302 hummingbot-20240429/hummingbot/connector/exchange/okx/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9214 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4432 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3330 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2735 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18614 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1761 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2723 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/okx/okx_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.328860 hummingbot-20240429/hummingbot/connector/exchange/paper_trade/
--rw-r--r--   0 madcatz    (501) staff       (20)     1293 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/paper_trade/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      910 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/paper_trade/market_config.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2193726 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/paper_trade/trading_pair.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.336341 hummingbot-20240429/hummingbot/connector/exchange/polkadex/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4527 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4110 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25723 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18241 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16866 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2076 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)      405 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_web_utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.341876 hummingbot-20240429/hummingbot/connector/exchange/vertex/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   343537 2024-05-13 02:14:57.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     7949 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5123 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3400 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10086 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)      959 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40072 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4655 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_order_book.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7773 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1774 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1444726 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/connector/exchange_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    45930 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/exchange_py_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.343366 hummingbot-20240429/hummingbot/connector/gateway/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.344971 hummingbot-20240429/hummingbot/connector/gateway/amm/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10973 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_algorand_amm.py
--rw-r--r--   0 madcatz    (501) staff       (20)    46320 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_evm_amm.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9794 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_near_amm.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5794 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_tezos_amm.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.346960 hummingbot-20240429/hummingbot/connector/gateway/amm_lp/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm_lp/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    58500 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4735 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)    56750 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.347773 hummingbot-20240429/hummingbot/connector/gateway/amm_perpetual/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm_perpetual/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26154 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.348952 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.349408 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/data_sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/data_sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1425 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    21799 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4144 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.350797 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.352098 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7967 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.353838 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    29847 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1779 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1296 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18003 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.355363 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    40889 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)      315 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1952 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.356222 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    17880 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2560 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3244 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)    31044 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py
--rw-r--r--   0 madcatz    (501) staff       (20)      944 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/common_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10185 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/gateway_in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2230 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/gateway_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6890 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/gateway/gateway_price_shim.py
--rw-r--r--   0 madcatz    (501) staff       (20)   857765 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/connector/in_flight_order_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    29014 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/markets_recorder.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.356525 hummingbot-20240429/hummingbot/connector/other/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/other/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6037 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/parrot.py
--rw-r--r--   0 madcatz    (501) staff       (20)    17636 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/perpetual_derivative_py_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7622 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/perpetual_trading.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.368605 hummingbot-20240429/hummingbot/connector/test_support/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    86233 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/exchange_connector_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42837 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1411 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/mock_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)   814209 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/connector/test_support/mock_paper_exchange.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      227 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/mock_pure_python_paper_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8740 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/network_mocking_assistant.py
--rw-r--r--   0 madcatz    (501) staff       (20)    44545 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/oms_exchange_connector_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)    33536 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/test_support/perpetual_derivative_test.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3607 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/time_synchronizer.py
--rw-r--r--   0 madcatz    (501) staff       (20)   531657 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/connector/trading_rule.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.369177 hummingbot-20240429/hummingbot/connector/utilities/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.371883 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8912 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3929 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2849 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5724 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25851 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py
--rw-r--r--   0 madcatz    (501) staff       (20)      641 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2789 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4992 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/connector/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.378379 hummingbot-20240429/hummingbot/core/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.380752 hummingbot-20240429/hummingbot/core/api_throttler/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/api_throttler/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3565 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/api_throttler/async_request_context_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3888 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/api_throttler/async_throttler.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3875 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/api_throttler/async_throttler_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1789 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/api_throttler/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   699724 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/clock.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      104 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/clock_mode.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.384301 hummingbot-20240429/hummingbot/core/cpp/
--rw-r--r--   0 madcatz    (501) staff       (20)     4793 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/LimitOrder.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1832 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/LimitOrder.h
--rw-r--r--   0 madcatz    (501) staff       (20)     3183 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/OrderBookEntry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      991 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/OrderBookEntry.h
--rw-r--r--   0 madcatz    (501) staff       (20)     1825 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/OrderExpirationEntry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      868 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/OrderExpirationEntry.h
--rw-r--r--   0 madcatz    (501) staff       (20)      684 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/PyRef.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      503 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/PyRef.h
--rw-r--r--   0 madcatz    (501) staff       (20)     3086 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/TestOrderBookEntry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)       19 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/Utils.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      246 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/Utils.h
--rwxr-xr-x   0 madcatz    (501) staff       (20)      139 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/cpp/compile.sh
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.402482 hummingbot-20240429/hummingbot/core/data_type/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/cancellation_result.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1067 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/common.py
--rw-r--r--   0 madcatz    (501) staff       (20)   707386 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/data_type/composite_order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/funding_info.py
--rw-r--r--   0 madcatz    (501) staff       (20)    14142 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/in_flight_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)   664173 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/data_type/limit_order.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1836 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/market_order.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1140943 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2989 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book_message.py
--rw-r--r--   0 madcatz    (501) staff       (20)   390625 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book_query_result.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)      587 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book_row.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15929 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book_tracker.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    11594 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book_tracker_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)      776 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_book_tracker_entry.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15612 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_candidate.py
--rw-r--r--   0 madcatz    (501) staff       (20)   408361 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/data_type/order_expiration_entry.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/perpetual_api_order_book_data_source.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     5496 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/remote_api_order_book_data_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1843 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/trade.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12881 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/trade_fee.py
--rw-r--r--   0 madcatz    (501) staff       (20)   371702 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/data_type/transaction_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1310 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/user_stream_tracker.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)     3994 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/data_type/user_stream_tracker_data_source.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.406490 hummingbot-20240429/hummingbot/core/event/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/event/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      754 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/event/event_forwarder.py
--rw-r--r--   0 madcatz    (501) staff       (20)   402941 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/event/event_listener.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   604746 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/event/event_logger.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   448102 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/event/event_reporter.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     8411 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/event/events.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.408877 hummingbot-20240429/hummingbot/core/gateway/
--rw-r--r--   0 madcatz    (501) staff       (20)     5198 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/gateway/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    42014 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/gateway/gateway_http_client.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5292 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/gateway/gateway_status_monitor.py
--rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/gateway/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.409930 hummingbot-20240429/hummingbot/core/management/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/management/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2632 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/management/console.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1325 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/management/diagnosis.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.411115 hummingbot-20240429/hummingbot/core/mock_api/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/mock_api/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2827 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/mock_api/mock_mqtt_server.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9206 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/mock_api/mock_web_server.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8409 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/mock_api/mock_web_socket_server.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4386 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/network_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)   680641 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/network_iterator.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   498964 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/core/pubsub.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   331173 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/py_time_iterator.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.412016 hummingbot-20240429/hummingbot/core/rate_oracle/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8190 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/rate_oracle.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.415447 hummingbot-20240429/hummingbot/core/rate_oracle/sources/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2207 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3589 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/binance_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3624 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1386 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7211 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3578 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3871 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/cube_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2800 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2349 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)      605 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/sources/rate_source_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1678 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/rate_oracle/utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)   394085 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/core/time_iterator.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.419743 hummingbot-20240429/hummingbot/core/utils/
--rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4470 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/async_call_scheduler.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2486 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/async_retry.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2031 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/async_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3613 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/estimate_fee.py
--rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/fixed_rate_source.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5970 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/gateway_config_utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2821 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/kill_switch.py
--rw-r--r--   0 madcatz    (501) staff       (20)      940 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/market_price.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7907 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/ssl_cert.py
--rw-r--r--   0 madcatz    (501) staff       (20)      675 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/ssl_client_request.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2203 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/tracking_nonce.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4187 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/utils/trading_pair_fetcher.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.422206 hummingbot-20240429/hummingbot/core/web_assistant/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      696 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/auth.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.423469 hummingbot-20240429/hummingbot/core/web_assistant/connections/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/connections/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/connections/connections_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4371 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/connections/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)      797 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/connections/rest_connection.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4767 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/connections/ws_connection.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5116 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/rest_assistant.py
--rw-r--r--   0 madcatz    (501) staff       (20)      467 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/rest_post_processors.py
--rw-r--r--   0 madcatz    (501) staff       (20)      460 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/rest_pre_processors.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2883 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/web_assistants_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3740 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/ws_assistant.py
--rw-r--r--   0 madcatz    (501) staff       (20)      457 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/ws_post_processors.py
--rw-r--r--   0 madcatz    (501) staff       (20)      450 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/core/web_assistant/ws_pre_processors.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.425147 hummingbot-20240429/hummingbot/data_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5140 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/amm_gateway_data_feed.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.426467 hummingbot-20240429/hummingbot/data_feed/candles_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.427294 hummingbot-20240429/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      147 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8002 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1086 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.428049 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_perpetual_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      170 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_perpetual_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7298 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py
--rw-r--r--   0 madcatz    (501) staff       (20)      897 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.428878 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      141 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7267 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py
--rw-r--r--   0 madcatz    (501) staff       (20)      900 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8895 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/candles_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2620 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/candles_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)      539 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/data_types.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.429662 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      159 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1187 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9004 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.430673 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      985 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7884 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.431470 hummingbot-20240429/hummingbot/data_feed/candles_feed/kraken_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/kraken_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1046 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10243 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.432354 hummingbot-20240429/hummingbot/data_feed/candles_feed/kucoin_spot_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/kucoin_spot_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      816 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9224 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.433384 hummingbot-20240429/hummingbot/data_feed/candles_feed/okx_perpetual_candles/
--rw-r--r--   0 madcatz    (501) staff       (20)      145 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/okx_perpetual_candles/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6917 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.434256 hummingbot-20240429/hummingbot/data_feed/coin_cap_data_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)      118 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/coin_cap_data_feed/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1075 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6923 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.435155 hummingbot-20240429/hummingbot/data_feed/coin_gecko_data_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/coin_gecko_data_feed/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      602 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5803 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3226 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/custom_api_data_feed.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2466 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/data_feed_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.435835 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.436697 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/binance/
--rw-r--r--   0 madcatz    (501) staff       (20)      153 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/binance/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7294 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py
--rw-r--r--   0 madcatz    (501) staff       (20)      567 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/binance/constants.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8546 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/liquidations_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2550 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/liquidations_feed/liquidations_factory.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9688 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/market_data_provider.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3909 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/data_feed/wallet_tracker_data_feed.py
--rw-r--r--   0 madcatz    (501) staff       (20)      766 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/exceptions.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.438431 hummingbot-20240429/hummingbot/logger/
--rw-r--r--   0 madcatz    (501) staff       (20)      755 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/logger/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      586 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/logger/application_warning.py
--rw-r--r--   0 madcatz    (501) staff       (20)      668 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/logger/cli_handler.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4260 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/logger/log_server_client.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3785 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/logger/logger.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1234 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/logger/struct_logger.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.442371 hummingbot-20240429/hummingbot/model/
--rw-r--r--   0 madcatz    (501) staff       (20)      566 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      487 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/controllers.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.443244 hummingbot-20240429/hummingbot/model/db_migration/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/db_migration/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1877 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/db_migration/base_transformation.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2992 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/db_migration/migrator.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6482 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/db_migration/transformations.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1267 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/decimal_type_decorator.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2377 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/executors.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2961 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/funding_payment.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2005 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/inventory_cost.py
--rw-r--r--   0 madcatz    (501) staff       (20)      888 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/market_data.py
--rw-r--r--   0 madcatz    (501) staff       (20)      821 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/market_state.py
--rw-r--r--   0 madcatz    (501) staff       (20)      365 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/metadata.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3109 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/order.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1203 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/order_status.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1148 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/range_position_collected_fees.py
--rw-r--r--   0 madcatz    (501) staff       (20)      967 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/range_position_update.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5796 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/sql_connection_manager.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7084 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/trade_fill.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1100 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/model/transaction_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.443900 hummingbot-20240429/hummingbot/notifier/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/notifier/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      262 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/notifier/notifier_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7780 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/notifier/telegram_notifier.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.446640 hummingbot-20240429/hummingbot/pmm_script/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/pmm_script/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10849 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/pmm_script/pmm_script_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5675 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/pmm_script/pmm_script_interface.py
--rw-r--r--   0 madcatz    (501) staff       (20)   724923 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/pmm_script/pmm_script_iterator.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     1441 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/pmm_script/pmm_script_process.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.448368 hummingbot-20240429/hummingbot/remote_iface/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/remote_iface/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3855 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/remote_iface/messages.py
--rw-r--r--   0 madcatz    (501) staff       (20)    45513 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/remote_iface/mqtt.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.474466 hummingbot-20240429/hummingbot/strategy/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.475114 hummingbot-20240429/hummingbot/strategy/__utils__/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__utils__/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1261659 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/__utils__/ring_buffer.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.484354 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2136 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py
--rw-r--r--   0 madcatz    (501) staff       (20)      717 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py
--rw-r--r--   0 madcatz    (501) staff       (20)      734 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1141 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py
--rw-r--r--   0 madcatz    (501) staff       (20)   816500 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.490326 hummingbot-20240429/hummingbot/strategy/amm_arb/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    26897 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/amm_arb.py
--rw-r--r--   0 madcatz    (501) staff       (20)     6279 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/amm_arb_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7350 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   338533 2024-05-13 02:14:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     4476 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2327 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_arb/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.491618 hummingbot-20240429/hummingbot/strategy/amm_v3_lp/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_v3_lp/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     9882 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3293 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1052 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/amm_v3_lp/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)   550211 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/api_asset_price_delegate.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   381512 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/asset_price_delegate.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.504511 hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      142 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2721883 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    17210 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1767 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5368 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/conditional_execution_state.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.509055 hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      234 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/__init__.py
--rwxr-xr-x   0 madcatz    (501) staff       (20)    90840 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py
--rw-r--r--   0 madcatz    (501) staff       (20)    20395 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)   593721 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     3149 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/start.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.518782 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/
--rw-r--r--   0 madcatz    (501) staff       (20)      204 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)  1449647 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     5145 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)      548 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py
--rw-r--r--   0 madcatz    (501) staff       (20)   528526 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2547 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2166 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15084 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/directional_strategy_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    17966 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/hanging_orders_tracker.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.521042 hummingbot-20240429/hummingbot/strategy/hedge/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/hedge/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    29916 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/hedge/hedge.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10953 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/hedge/hedge_config_map_pydantic.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1772 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/hedge/start.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.524983 hummingbot-20240429/hummingbot/strategy/liquidity_mining/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/liquidity_mining/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      948 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/liquidity_mining/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   339646 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/liquidity_mining/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    28111 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/liquidity_mining/liquidity_mining.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7282 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2671 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/liquidity_mining/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)      524 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/maker_taker_market_pair.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2033 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/market_trading_pair_tuple.py
--rw-r--r--   0 madcatz    (501) staff       (20)   551075 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/order_book_asset_price_delegate.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   846938 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/order_tracker.cpp
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.529214 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)   340444 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    48666 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15708 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1452 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5933 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/perpetual_market_making/start.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.544242 hummingbot-20240429/hummingbot/strategy/pure_market_making/
--rw-r--r--   0 madcatz    (501) staff       (20)      226 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3288 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py
--rw-r--r--   0 madcatz    (501) staff       (20)   331772 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     2801 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/moving_price_band.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2526655 2024-05-13 02:15:00.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/pure_market_making.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    22271 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)   414399 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     8774 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/pure_market_making/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10449 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/script_strategy_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.548842 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2620 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py
--rw-r--r--   0 madcatz    (501) staff       (20)   340558 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    26556 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5762 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2592 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1942 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/utils.py
--rw-r--r--   0 madcatz    (501) staff       (20)  2398768 2024-05-13 02:15:00.000000 hummingbot-20240429/hummingbot/strategy/strategy_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)   620855 2024-05-13 02:15:00.000000 hummingbot-20240429/hummingbot/strategy/strategy_py_base.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)    20411 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/strategy_v2_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.553186 hummingbot-20240429/hummingbot/strategy/twap/
--rw-r--r--   0 madcatz    (501) staff       (20)       97 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/twap/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)   338167 2024-05-13 02:14:59.000000 hummingbot-20240429/hummingbot/strategy/twap/dummy.cpp
--rw-r--r--   0 madcatz    (501) staff       (20)     3468 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/twap/start.py
--rw-r--r--   0 madcatz    (501) staff       (20)    18542 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/twap/twap.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7079 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/twap/twap_config_map.py
--rw-r--r--   0 madcatz    (501) staff       (20)      700 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy/utils.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.553901 hummingbot-20240429/hummingbot/strategy_v2/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.555797 hummingbot-20240429/hummingbot/strategy_v2/backtesting/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2904 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16276 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.556736 hummingbot-20240429/hummingbot/strategy_v2/backtesting/controllers_backtesting/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/controllers_backtesting/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      294 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/controllers_backtesting/directional_trading_backtesting.py
--rw-r--r--   0 madcatz    (501) staff       (20)      440 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/controllers_backtesting/market_making_backtesting.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3591 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/executor_simulator_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.557609 hummingbot-20240429/hummingbot/strategy_v2/backtesting/executors_simulator/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/executors_simulator/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     7008 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3758 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.560049 hummingbot-20240429/hummingbot/strategy_v2/controllers/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/controllers/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8401 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/controllers/controller_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10241 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15922 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/controllers/market_making_controller_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.561770 hummingbot-20240429/hummingbot/strategy_v2/executors/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/__init__.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.562981 hummingbot-20240429/hummingbot/strategy_v2/executors/arbitrage_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/arbitrage_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)    12599 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)      492 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/arbitrage_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)      834 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/data_types.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.563974 hummingbot-20240429/hummingbot/strategy_v2/executors/dca_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/dca_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      876 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/dca_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    25744 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py
--rw-r--r--   0 madcatz    (501) staff       (20)    15360 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/executor_base.py
--rw-r--r--   0 madcatz    (501) staff       (20)    10331 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/executor_orchestrator.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.565944 hummingbot-20240429/hummingbot/strategy_v2/executors/position_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/position_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2172 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/position_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    30954 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/position_executor/position_executor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.567011 hummingbot-20240429/hummingbot/strategy_v2/executors/twap_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/twap_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1460 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/twap_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    13720 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.568482 hummingbot-20240429/hummingbot/strategy_v2/executors/xemm_executor/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/xemm_executor/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      464 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/xemm_executor/data_types.py
--rw-r--r--   0 madcatz    (501) staff       (20)    16859 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.570128 hummingbot-20240429/hummingbot/strategy_v2/models/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/models/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/models/base.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1113 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/models/executor_actions.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1504 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/models/executors.py
--rw-r--r--   0 madcatz    (501) staff       (20)     2639 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/models/executors_info.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.571098 hummingbot-20240429/hummingbot/strategy_v2/order_level_distributions/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/order_level_distributions/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4419 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/order_level_distributions/distributions.py
--rw-r--r--   0 madcatz    (501) staff       (20)     4758 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/order_level_distributions/order_level_builder.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3099 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/runnable_base.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.571934 hummingbot-20240429/hummingbot/strategy_v2/utils/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/utils/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)      312 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/utils/common.py
--rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/strategy_v2/utils/config_encoder_decoder.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.574677 hummingbot-20240429/hummingbot/templates/
--rw-r--r--   0 madcatz    (501) staff       (20)     1898 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)      536 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     5439 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     2001 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     4032 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     5161 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     1569 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml
--rw-r--r--   0 madcatz    (501) staff       (20)     1344 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml
--rwxr-xr-x   0 madcatz    (501) staff       (20)     2159 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/templates/hummingbot_logs_TEMPLATE.yml
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.575085 hummingbot-20240429/hummingbot/user/
--rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/user/__init__.py
--rw-r--r--   0 madcatz    (501) staff       (20)     8061 2024-05-13 01:39:58.000000 hummingbot-20240429/hummingbot/user/user_balances.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.576935 hummingbot-20240429/hummingbot.egg-info/
--rw-r--r--   0 madcatz    (501) staff       (20)     1748 2024-05-13 02:15:01.000000 hummingbot-20240429/hummingbot.egg-info/PKG-INFO
--rw-r--r--   0 madcatz    (501) staff       (20)    48054 2024-05-13 02:15:01.000000 hummingbot-20240429/hummingbot.egg-info/SOURCES.txt
--rw-r--r--   0 madcatz    (501) staff       (20)        1 2024-05-13 02:15:01.000000 hummingbot-20240429/hummingbot.egg-info/dependency_links.txt
--rw-r--r--   0 madcatz    (501) staff       (20)      614 2024-05-13 02:15:01.000000 hummingbot-20240429/hummingbot.egg-info/requires.txt
--rw-r--r--   0 madcatz    (501) staff       (20)       11 2024-05-13 02:15:01.000000 hummingbot-20240429/hummingbot.egg-info/top_level.txt
--rw-r--r--   0 madcatz    (501) staff       (20)      491 2024-05-13 01:39:58.000000 hummingbot-20240429/pyproject.toml
--rw-r--r--   0 madcatz    (501) staff       (20)       85 2024-05-13 02:15:01.578095 hummingbot-20240429/setup.cfg
--rw-r--r--   0 madcatz    (501) staff       (20)     4337 2024-05-13 01:39:58.000000 hummingbot-20240429/setup.py
-drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-13 02:15:01.576510 hummingbot-20240429/test/
--rw-r--r--   0 madcatz    (501) staff       (20)     6190 2024-05-13 01:39:59.000000 hummingbot-20240429/test/test_isolated_asyncio_wrapper_test_case.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3267 2024-05-13 01:39:59.000000 hummingbot-20240429/test/test_local_class_event_loop_wrapper_test_case.py
--rw-r--r--   0 madcatz    (501) staff       (20)     3504 2024-05-13 01:39:59.000000 hummingbot-20240429/test/test_local_test_event_loop_wrapper_test_case.py
--rw-r--r--   0 madcatz    (501) staff       (20)     5466 2024-05-13 01:39:59.000000 hummingbot-20240429/test/test_logger_mixin_for_test.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.360698 hummingbot-20240520/
+-rw-r--r--   0 madcatz    (501) staff       (20)    11352 2024-05-20 21:20:06.000000 hummingbot-20240520/LICENSE
+-rw-r--r--   0 madcatz    (501) staff       (20)     1771 2024-05-20 21:30:08.360598 hummingbot-20240520/PKG-INFO
+-rw-r--r--   0 madcatz    (501) staff       (20)     9670 2024-05-20 21:20:06.000000 hummingbot-20240520/README.md
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.815659 hummingbot-20240520/bin/
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6821 2024-05-20 21:20:06.000000 hummingbot-20240520/bin/hummingbot_quickstart.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.817081 hummingbot-20240520/hummingbot/
+-rw-r--r--   0 madcatz    (501) staff       (20)       10 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/VERSION
+-rw-r--r--   0 madcatz    (501) staff       (20)     5811 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.820297 hummingbot-20240520/hummingbot/client/
+-rw-r--r--   0 madcatz    (501) staff       (20)      655 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.831905 hummingbot-20240520/hummingbot/client/command/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1249 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9967 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/balance_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    22563 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/config_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6908 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/connect_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    16234 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/create_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1458 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/exit_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4844 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/export_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6371 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/gateway_api_manager.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    41186 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/gateway_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      916 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/help_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12319 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/history_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3698 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/import_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4566 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/mqtt_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3001 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/order_book_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      344 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/pmm_script_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2571 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/previous_strategy_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2697 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/rate_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9686 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/silly_commands.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15078 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/start_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10502 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/status_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2552 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/stop_command.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2996 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/command/ticker_command.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.839421 hummingbot-20240520/hummingbot/client/config/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    41900 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/client_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18418 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/conf_migration.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4553 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/config_crypt.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2608 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/config_data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    38116 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/config_helpers.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      633 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/config_methods.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7452 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/config_validators.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3189 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/config_var.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1404 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/fee_overrides_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      364 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/gateway_ssl_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/global_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3858 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/security.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6288 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/strategy_config_data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3003 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/config/trade_fee_schema_loader.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.839890 hummingbot-20240520/hummingbot/client/data_type/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/data_type/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      426 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/data_type/currency_amount.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15273 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/hummingbot_application.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    13787 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/performance.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      516 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/platform.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    27252 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/settings.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.841269 hummingbot-20240520/hummingbot/client/tab/
+-rw-r--r--   0 madcatz    (501) staff       (20)      135 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/tab/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      872 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/tab/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3140 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/tab/order_book_tab.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1723 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/tab/tab_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      774 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/tab/tab_example_tab.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.846159 hummingbot-20240520/hummingbot/client/ui/
+-rw-r--r--   0 madcatz    (501) staff       (20)     8435 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    24695 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/completer.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9614 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/custom_widgets.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11623 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/hummingbot_cli.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4952 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/interface_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3593 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/keybindings.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11632 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/layout.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11856 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/parser.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1710 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/scroll_handlers.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2524 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/stdout_redirection.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11314 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/client/ui/style.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.877245 hummingbot-20240520/hummingbot/connector/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7400 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/budget_checker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18938 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/client_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1403631 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/connector_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     6375 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/connector_metrics_collector.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      215 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/constants.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.880161 hummingbot-20240520/hummingbot/connector/derivative/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.884939 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9683 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1944 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6016 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    38371 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6334 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2428 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4013 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.889391 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10413 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3497 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4597 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    35998 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5494 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2420 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2670 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.896387 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12125 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2898 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5025 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40405 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5830 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2002 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.900806 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15468 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3238 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5848 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    38897 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6821 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4168 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    19340 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341067 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.911298 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12544 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4454 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3774 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40418 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2566 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2154 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2663 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.916997 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341295 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    10758 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3135 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5254 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    34398 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4492 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1634 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1851 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.922560 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341751 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    10842 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6022 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3695 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    36109 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5656 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4106 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5213 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.925284 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      466 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4840 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    48511 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3981 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.932375 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341181 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    14498 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8026 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6301 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6066 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    45173 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2117 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6479 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.935471 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    20796 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5462 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6000 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    39008 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6527 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2707 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12961 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1421 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/perpetual_budget_checker.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.938405 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12075 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5017 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2335 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6113 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    32650 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2679 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3838 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2238 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/position.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.944002 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    14929 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3977 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9352 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1466 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    66373 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6581 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2481 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6529 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2528 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/derivative_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.944373 hummingbot-20240520/hummingbot/connector/exchange/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.947196 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7240 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3627 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2478 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5036 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26170 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2084 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2719 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.951014 hummingbot-20240520/hummingbot/connector/exchange/binance/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6402 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6081 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2413 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4688 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_constants.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    25993 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3224 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2972 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3154 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/binance_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/binance/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.992394 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   785958 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    22384 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2224 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1580 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  3066951 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   554137 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   576798 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1273 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10355 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1057 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5028 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:07.996070 hummingbot-20240520/hummingbot/connector/exchange/bitmart/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10154 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     4787 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2913 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2473 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    19821 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2451 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2538 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339765 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/bitmart/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.000714 hummingbot-20240520/hummingbot/connector/exchange/bitrue/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     8798 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2385 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6008 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_constants.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    30434 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3211 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_order_book.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     8058 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1604 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3128 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.004306 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9564 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4055 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4543 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3114 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    25469 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4545 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1662 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2831 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.008283 hummingbot-20240520/hummingbot/connector/exchange/bybit/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12169 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5372 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3308 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    21562 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4246 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2581 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5170 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339537 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/bybit/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.014634 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11069 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    13923 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12512 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5500 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    50376 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7810 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2030 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7161 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341676 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.052957 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   928124 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    14517 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     5006 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2753 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      493 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2596840 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   499653 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   535675 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1816 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8848 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1041 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2361 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2530 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.057506 hummingbot-20240520/hummingbot/connector/exchange/cube/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    11507 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3570 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3643 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3062 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    51297 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4473 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4390 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.061032 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10219 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15363 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/py.typed
+-rw-r--r--   0 madcatz    (501) staff       (20)    15992 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    29121 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi
+-rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/cube/dummy.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.068843 hummingbot-20240520/hummingbot/connector/exchange/foxbit/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10078 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5190 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3912 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   345010 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     5253 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    44815 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7671 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5090 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4155 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.071963 hummingbot-20240520/hummingbot/connector/exchange/gate_io/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7620 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4310 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3166 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3528 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    22712 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1255 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   341880 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/gate_io/placeholder.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.089760 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   754683 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    11733 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3224 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2451 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1847 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42970 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3162 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2397 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5637 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      945 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2346 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5706 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4686 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.092913 hummingbot-20240520/hummingbot/connector/exchange/htx/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8241 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5047 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3477 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2958 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18960 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1589 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2553 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/htx/htx_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.097488 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4257 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/account_delegation_script.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.100991 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    71837 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    23529 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12854 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    24074 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5962 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)       90 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_events.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4376 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_market.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    14999 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_query_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3669 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42627 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15808 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      410 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.104494 hummingbot-20240520/hummingbot/connector/exchange/kraken/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     7715 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3909 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2929 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4146 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    27389 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2903 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8041 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1660 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.109543 hummingbot-20240520/hummingbot/connector/exchange/kucoin/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339651 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     8742 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4879 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3663 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3297 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    24398 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2132 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3049 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3215 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.114526 hummingbot-20240520/hummingbot/connector/exchange/mexc/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/dummy.cpp
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     6556 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     8131 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2480 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4344 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_constants.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    26610 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3481 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1705 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3142 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.119643 hummingbot-20240520/hummingbot/connector/exchange/ndax/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339423 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    15461 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5670 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2103 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5426 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    49594 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2421 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3556 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3561 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5934 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2369 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4179 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3928 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.122473 hummingbot-20240520/hummingbot/connector/exchange/okx/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9214 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4432 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3330 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2775 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18614 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1761 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2723 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/okx/okx_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.128582 hummingbot-20240520/hummingbot/connector/exchange/paper_trade/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1293 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/paper_trade/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      910 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/paper_trade/market_config.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2193726 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/paper_trade/trading_pair.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.132814 hummingbot-20240520/hummingbot/connector/exchange/polkadex/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4527 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4188 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26470 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18334 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    19864 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2076 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      405 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_web_utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.137293 hummingbot-20240520/hummingbot/connector/exchange/vertex/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   343537 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     7949 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5123 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3400 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10086 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      959 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40072 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4655 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_order_book.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7773 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1774 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1444726 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/connector/exchange_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    45930 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/exchange_py_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.138827 hummingbot-20240520/hummingbot/connector/gateway/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.141032 hummingbot-20240520/hummingbot/connector/gateway/amm/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10973 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_algorand_amm.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    46320 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_evm_amm.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9794 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_near_amm.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5794 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_tezos_amm.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.142824 hummingbot-20240520/hummingbot/connector/gateway/amm_lp/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm_lp/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    58500 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4735 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    56750 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.143871 hummingbot-20240520/hummingbot/connector/gateway/amm_perpetual/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm_perpetual/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26154 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.145156 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.145715 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/data_sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/data_sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1425 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    21799 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4144 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.146516 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.147678 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7967 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.149890 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    29847 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1779 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3455 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1296 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18003 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.152329 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    40889 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      315 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1952 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4659 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.153602 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    17880 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2560 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3244 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    31044 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      944 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/common_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10185 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/gateway_in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2230 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/gateway_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6890 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/gateway/gateway_price_shim.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   857765 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/in_flight_order_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    29014 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/markets_recorder.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.154022 hummingbot-20240520/hummingbot/connector/other/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/other/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6037 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/parrot.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    17636 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/perpetual_derivative_py_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7622 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/perpetual_trading.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.160890 hummingbot-20240520/hummingbot/connector/test_support/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    86233 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/exchange_connector_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42837 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1411 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/mock_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   814209 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/connector/test_support/mock_paper_exchange.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      227 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/mock_pure_python_paper_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8740 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/network_mocking_assistant.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    44545 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/oms_exchange_connector_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    33536 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/test_support/perpetual_derivative_test.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3607 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/time_synchronizer.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   531657 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/connector/trading_rule.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.161468 hummingbot-20240520/hummingbot/connector/utilities/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.164122 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8912 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3929 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2849 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5724 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    25851 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      641 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2789 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4992 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/connector/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.169740 hummingbot-20240520/hummingbot/core/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.176895 hummingbot-20240520/hummingbot/core/api_throttler/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/api_throttler/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3565 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/api_throttler/async_request_context_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3888 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/api_throttler/async_throttler.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3875 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/api_throttler/async_throttler_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1789 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/api_throttler/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   699724 2024-05-20 21:30:04.000000 hummingbot-20240520/hummingbot/core/clock.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      104 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/clock_mode.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.180324 hummingbot-20240520/hummingbot/core/cpp/
+-rw-r--r--   0 madcatz    (501) staff       (20)     4793 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/LimitOrder.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1832 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/LimitOrder.h
+-rw-r--r--   0 madcatz    (501) staff       (20)     3183 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/OrderBookEntry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      991 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/OrderBookEntry.h
+-rw-r--r--   0 madcatz    (501) staff       (20)     1825 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/OrderExpirationEntry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      868 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/OrderExpirationEntry.h
+-rw-r--r--   0 madcatz    (501) staff       (20)      684 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/PyRef.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      503 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/PyRef.h
+-rw-r--r--   0 madcatz    (501) staff       (20)     3086 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/TestOrderBookEntry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)       19 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/Utils.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      246 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/Utils.h
+-rwxr-xr-x   0 madcatz    (501) staff       (20)      139 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/cpp/compile.sh
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.199620 hummingbot-20240520/hummingbot/core/data_type/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/cancellation_result.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1067 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/common.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   707386 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/data_type/composite_order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2052 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/funding_info.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    14142 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/in_flight_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   664173 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/data_type/limit_order.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1836 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/market_order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1140943 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/data_type/order_book.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2989 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/order_book_message.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   390625 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/data_type/order_book_query_result.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)      587 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/order_book_row.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15929 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/order_book_tracker.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    11594 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/order_book_tracker_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      776 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/order_book_tracker_entry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15612 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/order_candidate.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   408361 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/data_type/order_expiration_entry.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/perpetual_api_order_book_data_source.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     5496 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/remote_api_order_book_data_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1843 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/trade.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12881 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/trade_fee.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   371702 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/data_type/transaction_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1310 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/user_stream_tracker.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     3994 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/data_type/user_stream_tracker_data_source.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.202660 hummingbot-20240520/hummingbot/core/event/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/event/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      754 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/event/event_forwarder.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   402941 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/event/event_listener.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   604746 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/event/event_logger.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   448102 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/event/event_reporter.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     8411 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/event/events.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.205217 hummingbot-20240520/hummingbot/core/gateway/
+-rw-r--r--   0 madcatz    (501) staff       (20)     5198 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/gateway/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    42014 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/gateway/gateway_http_client.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5292 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/gateway/gateway_status_monitor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/gateway/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.206159 hummingbot-20240520/hummingbot/core/management/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/management/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2632 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/management/console.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1325 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/management/diagnosis.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.207388 hummingbot-20240520/hummingbot/core/mock_api/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/mock_api/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2827 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/mock_api/mock_mqtt_server.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9206 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/mock_api/mock_web_server.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8409 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/mock_api/mock_web_socket_server.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4386 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/network_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   680641 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/network_iterator.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   498964 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/pubsub.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   331173 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/py_time_iterator.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.208353 hummingbot-20240520/hummingbot/core/rate_oracle/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8190 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/rate_oracle.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.211346 hummingbot-20240520/hummingbot/core/rate_oracle/sources/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2207 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3589 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/binance_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3624 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1386 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7211 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3578 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3871 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/cube_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2800 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2349 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      605 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/sources/rate_source_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1678 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/rate_oracle/utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   394085 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/core/time_iterator.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.215545 hummingbot-20240520/hummingbot/core/utils/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1257 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4470 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/async_call_scheduler.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2486 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/async_retry.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2031 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/async_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3613 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/estimate_fee.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      892 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/fixed_rate_source.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5970 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/gateway_config_utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2821 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/kill_switch.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      940 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/market_price.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7907 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/ssl_cert.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      675 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/ssl_client_request.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2203 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/tracking_nonce.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4187 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/utils/trading_pair_fetcher.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.217745 hummingbot-20240520/hummingbot/core/web_assistant/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      696 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/auth.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.219136 hummingbot-20240520/hummingbot/core/web_assistant/connections/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/connections/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1834 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/connections/connections_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4371 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/connections/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      797 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/connections/rest_connection.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4767 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/connections/ws_connection.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5116 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/rest_assistant.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      467 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/rest_post_processors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      460 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/rest_pre_processors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2883 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/web_assistants_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3740 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/ws_assistant.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      457 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/ws_post_processors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      450 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/core/web_assistant/ws_pre_processors.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.221043 hummingbot-20240520/hummingbot/data_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5140 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/amm_gateway_data_feed.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.222334 hummingbot-20240520/hummingbot/data_feed/candles_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.223236 hummingbot-20240520/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      147 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8002 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1086 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.224233 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_perpetual_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      170 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_perpetual_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7298 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      897 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.225325 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      141 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7262 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      900 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8895 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/candles_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2746 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/candles_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      539 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/data_types.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.226482 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      159 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1187 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9004 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.227414 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      985 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7884 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.228191 hummingbot-20240520/hummingbot/data_feed/candles_feed/kraken_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/kraken_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1046 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10243 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.229175 hummingbot-20240520/hummingbot/data_feed/candles_feed/kucoin_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      137 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/kucoin_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      816 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9411 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.230064 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_perpetual_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      145 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_perpetual_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8700 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.231311 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_spot_candles/
+-rw-r--r--   0 madcatz    (501) staff       (20)      125 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_spot_candles/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1387 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_spot_candles/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8670 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_spot_candles/okx_spot_candles.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.232565 hummingbot-20240520/hummingbot/data_feed/coin_cap_data_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)      118 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/coin_cap_data_feed/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1075 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6923 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.233524 hummingbot-20240520/hummingbot/data_feed/coin_gecko_data_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)      126 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/coin_gecko_data_feed/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      602 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5803 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3226 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/custom_api_data_feed.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2466 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/data_feed_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.234361 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.235246 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/binance/
+-rw-r--r--   0 madcatz    (501) staff       (20)      153 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/binance/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7604 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      567 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/binance/constants.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8828 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/liquidations_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2550 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/liquidations_feed/liquidations_factory.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9688 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/market_data_provider.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3909 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/data_feed/wallet_tracker_data_feed.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      766 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/exceptions.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.236913 hummingbot-20240520/hummingbot/logger/
+-rw-r--r--   0 madcatz    (501) staff       (20)      755 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/logger/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      586 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/logger/application_warning.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      668 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/logger/cli_handler.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4260 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/logger/log_server_client.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3785 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/logger/logger.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1234 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/logger/struct_logger.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.241817 hummingbot-20240520/hummingbot/model/
+-rw-r--r--   0 madcatz    (501) staff       (20)      566 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      487 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/controllers.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.242856 hummingbot-20240520/hummingbot/model/db_migration/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/db_migration/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1877 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/db_migration/base_transformation.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2992 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/db_migration/migrator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6482 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/db_migration/transformations.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1267 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/decimal_type_decorator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2377 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/executors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2961 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/funding_payment.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2005 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/inventory_cost.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      888 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/market_data.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      821 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/market_state.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      365 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/metadata.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3109 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/order.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1203 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/order_status.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1148 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/range_position_collected_fees.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      967 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/range_position_update.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5796 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/sql_connection_manager.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7084 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/trade_fill.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1100 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/model/transaction_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.243695 hummingbot-20240520/hummingbot/notifier/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/notifier/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      262 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/notifier/notifier_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7780 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/notifier/telegram_notifier.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.246102 hummingbot-20240520/hummingbot/pmm_script/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/pmm_script/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10849 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/pmm_script/pmm_script_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5675 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/pmm_script/pmm_script_interface.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   724923 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/pmm_script/pmm_script_iterator.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     1441 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/pmm_script/pmm_script_process.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.248012 hummingbot-20240520/hummingbot/remote_iface/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/remote_iface/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3855 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/remote_iface/messages.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    45513 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/remote_iface/mqtt.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.268228 hummingbot-20240520/hummingbot/strategy/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.268826 hummingbot-20240520/hummingbot/strategy/__utils__/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1261659 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/ring_buffer.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.277655 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2136 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      717 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      734 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1141 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   816500 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.282018 hummingbot-20240520/hummingbot/strategy/amm_arb/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    26897 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/amm_arb.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     6279 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/amm_arb_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7350 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   338533 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     4476 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2327 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_arb/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.283176 hummingbot-20240520/hummingbot/strategy/amm_v3_lp/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_v3_lp/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     9882 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3293 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1052 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/amm_v3_lp/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   550211 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/api_asset_price_delegate.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   381512 2024-05-20 21:30:05.000000 hummingbot-20240520/hummingbot/strategy/asset_price_delegate.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.294975 hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      142 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2721883 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    17210 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1767 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5368 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/conditional_execution_state.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.298000 hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      234 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/__init__.py
+-rwxr-xr-x   0 madcatz    (501) staff       (20)    90840 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    20395 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   593721 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     3149 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/start.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.308812 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/
+-rw-r--r--   0 madcatz    (501) staff       (20)      204 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  1449647 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     5145 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      548 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   528526 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2547 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2166 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15084 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/directional_strategy_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    17966 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/hanging_orders_tracker.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.311894 hummingbot-20240520/hummingbot/strategy/hedge/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/hedge/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    29916 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/hedge/hedge.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10953 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/hedge/hedge_config_map_pydantic.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1772 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/hedge/start.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.315562 hummingbot-20240520/hummingbot/strategy/liquidity_mining/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/liquidity_mining/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      948 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/liquidity_mining/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   339646 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/liquidity_mining/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    28111 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/liquidity_mining/liquidity_mining.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7282 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2671 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/liquidity_mining/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      524 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/maker_taker_market_pair.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2033 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/market_trading_pair_tuple.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   551075 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/order_book_asset_price_delegate.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   846938 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/order_tracker.cpp
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.319352 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      139 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   340444 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    48666 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15708 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1452 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5933 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/perpetual_market_making/start.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.331169 hummingbot-20240520/hummingbot/strategy/pure_market_making/
+-rw-r--r--   0 madcatz    (501) staff       (20)      226 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1407 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3288 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   331772 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     2801 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/moving_price_band.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2526655 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/pure_market_making.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    22271 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   414399 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     8774 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/pure_market_making/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10449 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/script_strategy_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.335600 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2620 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   340558 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    26556 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5762 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2592 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1942 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/utils.py
+-rw-r--r--   0 madcatz    (501) staff       (20)  2398768 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot/strategy/strategy_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)   620855 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/strategy_py_base.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)    20411 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/strategy_v2_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.338081 hummingbot-20240520/hummingbot/strategy/twap/
+-rw-r--r--   0 madcatz    (501) staff       (20)       97 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/twap/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)   338167 2024-05-20 21:30:06.000000 hummingbot-20240520/hummingbot/strategy/twap/dummy.cpp
+-rw-r--r--   0 madcatz    (501) staff       (20)     3468 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/twap/start.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    18542 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/twap/twap.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7079 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/twap/twap_config_map.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      700 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy/utils.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.338719 hummingbot-20240520/hummingbot/strategy_v2/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.340092 hummingbot-20240520/hummingbot/strategy_v2/backtesting/
+-rw-r--r--   0 madcatz    (501) staff       (20)      474 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3378 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    16829 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.340967 hummingbot-20240520/hummingbot/strategy_v2/backtesting/controllers_backtesting/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/controllers_backtesting/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      294 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/controllers_backtesting/directional_trading_backtesting.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      440 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/controllers_backtesting/market_making_backtesting.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3591 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/executor_simulator_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.342147 hummingbot-20240520/hummingbot/strategy_v2/backtesting/executors_simulator/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/executors_simulator/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     7060 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3758 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.343604 hummingbot-20240520/hummingbot/strategy_v2/controllers/
+-rw-r--r--   0 madcatz    (501) staff       (20)      645 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/controllers/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8401 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/controllers/controller_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10241 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15922 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/controllers/market_making_controller_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.344977 hummingbot-20240520/hummingbot/strategy_v2/executors/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/__init__.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.346062 hummingbot-20240520/hummingbot/strategy_v2/executors/arbitrage_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/arbitrage_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    12599 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      492 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/arbitrage_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      834 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/data_types.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.346799 hummingbot-20240520/hummingbot/strategy_v2/executors/dca_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/dca_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      876 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/dca_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    25744 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    15360 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/executor_base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    10331 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/executor_orchestrator.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.347834 hummingbot-20240520/hummingbot/strategy_v2/executors/position_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/position_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2172 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/position_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    30954 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/position_executor/position_executor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.348648 hummingbot-20240520/hummingbot/strategy_v2/executors/twap_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/twap_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1460 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/twap_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    13720 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.349582 hummingbot-20240520/hummingbot/strategy_v2/executors/xemm_executor/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/xemm_executor/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      464 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/xemm_executor/data_types.py
+-rw-r--r--   0 madcatz    (501) staff       (20)    16859 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.351416 hummingbot-20240520/hummingbot/strategy_v2/models/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/models/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      129 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/models/base.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1113 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/models/executor_actions.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1504 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/models/executors.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     2639 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/models/executors_info.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3099 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/runnable_base.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.353401 hummingbot-20240520/hummingbot/strategy_v2/utils/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/utils/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)      312 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/utils/common.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     1809 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/utils/config_encoder_decoder.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4419 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/utils/distributions.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     4738 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/strategy_v2/utils/order_level_builder.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.357164 hummingbot-20240520/hummingbot/templates/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1898 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)      536 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     5439 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     2001 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     4032 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     5161 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     1569 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml
+-rw-r--r--   0 madcatz    (501) staff       (20)     1344 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml
+-rwxr-xr-x   0 madcatz    (501) staff       (20)     2159 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/templates/hummingbot_logs_TEMPLATE.yml
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.357705 hummingbot-20240520/hummingbot/user/
+-rw-r--r--   0 madcatz    (501) staff       (20)        0 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/user/__init__.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     8061 2024-05-20 21:20:06.000000 hummingbot-20240520/hummingbot/user/user_balances.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.359941 hummingbot-20240520/hummingbot.egg-info/
+-rw-r--r--   0 madcatz    (501) staff       (20)     1771 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot.egg-info/PKG-INFO
+-rw-r--r--   0 madcatz    (501) staff       (20)    48151 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot.egg-info/SOURCES.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)        1 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot.egg-info/dependency_links.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)      622 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot.egg-info/requires.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)       11 2024-05-20 21:30:07.000000 hummingbot-20240520/hummingbot.egg-info/top_level.txt
+-rw-r--r--   0 madcatz    (501) staff       (20)      491 2024-05-20 21:20:06.000000 hummingbot-20240520/pyproject.toml
+-rw-r--r--   0 madcatz    (501) staff       (20)       85 2024-05-20 21:30:08.361099 hummingbot-20240520/setup.cfg
+-rw-r--r--   0 madcatz    (501) staff       (20)     4356 2024-05-20 21:28:45.000000 hummingbot-20240520/setup.py
+drwxr-xr-x   0 madcatz    (501) staff       (20)        0 2024-05-20 21:30:08.359502 hummingbot-20240520/test/
+-rw-r--r--   0 madcatz    (501) staff       (20)     6190 2024-05-20 21:20:06.000000 hummingbot-20240520/test/test_isolated_asyncio_wrapper_test_case.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3267 2024-05-20 21:20:06.000000 hummingbot-20240520/test/test_local_class_event_loop_wrapper_test_case.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     3504 2024-05-20 21:20:06.000000 hummingbot-20240520/test/test_local_test_event_loop_wrapper_test_case.py
+-rw-r--r--   0 madcatz    (501) staff       (20)     5466 2024-05-20 21:20:06.000000 hummingbot-20240520/test/test_logger_mixin_for_test.py
```

### Comparing `hummingbot-20240429/LICENSE` & `hummingbot-20240520/LICENSE`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/PKG-INFO` & `hummingbot-20240520/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummingbot
-Version: 20240429
+Version: 20240520
 Summary: Hummingbot
 Home-page: https://github.com/hummingbot/hummingbot
 Author: Hummingbot Foundation
 Author-email: dev@hummingbot.org
 License: Apache 2.0
 License-File: LICENSE
 Requires-Dist: bidict
@@ -33,14 +33,15 @@
 Requires-Dist: eth-typing
 Requires-Dist: eth-utils
 Requires-Dist: flake8
 Requires-Dist: hexbytes
 Requires-Dist: importlib-metadata
 Requires-Dist: injective-py
 Requires-Dist: mypy-extensions
+Requires-Dist: msgpack
 Requires-Dist: nose
 Requires-Dist: nose-exclude
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pip
 Requires-Dist: pre-commit
 Requires-Dist: prompt-toolkit
```

### Comparing `hummingbot-20240429/README.md` & `hummingbot-20240520/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 ## Getting Started
 
 ### Install with Docker
 
 We recommend installing Hummingbot using Docker if you want the simplest, easiest installation method and don't need to modify the Hummingbot codebase.
 
+
 **Prerequisites:**
 
 * MacOS 10.12.6+ / Linux (Ubuntu 20.04+, Debian 10+) / Windows 10+
 * Memory: 4 GB RAM per instance
 * Storage: 5 GB HDD space per instance
 * Install [Docker Compose](https://docs.docker.com/compose/)
```

### Comparing `hummingbot-20240429/bin/hummingbot_quickstart.py` & `hummingbot-20240520/bin/hummingbot_quickstart.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/__init__.py` & `hummingbot-20240520/hummingbot/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/__init__.py` & `hummingbot-20240520/hummingbot/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/__init__.py` & `hummingbot-20240520/hummingbot/client/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/balance_command.py` & `hummingbot-20240520/hummingbot/client/command/balance_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/config_command.py` & `hummingbot-20240520/hummingbot/client/command/config_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/connect_command.py` & `hummingbot-20240520/hummingbot/client/command/connect_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/create_command.py` & `hummingbot-20240520/hummingbot/client/command/create_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/exit_command.py` & `hummingbot-20240520/hummingbot/client/command/exit_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/export_command.py` & `hummingbot-20240520/hummingbot/client/command/export_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/gateway_api_manager.py` & `hummingbot-20240520/hummingbot/client/command/gateway_api_manager.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/gateway_command.py` & `hummingbot-20240520/hummingbot/client/command/gateway_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/help_command.py` & `hummingbot-20240520/hummingbot/client/command/help_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/history_command.py` & `hummingbot-20240520/hummingbot/client/command/history_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/import_command.py` & `hummingbot-20240520/hummingbot/client/command/import_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/mqtt_command.py` & `hummingbot-20240520/hummingbot/client/command/mqtt_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/order_book_command.py` & `hummingbot-20240520/hummingbot/client/command/order_book_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/previous_strategy_command.py` & `hummingbot-20240520/hummingbot/client/command/previous_strategy_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/rate_command.py` & `hummingbot-20240520/hummingbot/client/command/rate_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/silly_commands.py` & `hummingbot-20240520/hummingbot/client/command/silly_commands.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/start_command.py` & `hummingbot-20240520/hummingbot/client/command/start_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/status_command.py` & `hummingbot-20240520/hummingbot/client/command/status_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/stop_command.py` & `hummingbot-20240520/hummingbot/client/command/stop_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/command/ticker_command.py` & `hummingbot-20240520/hummingbot/client/command/ticker_command.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/client_config_map.py` & `hummingbot-20240520/hummingbot/client/config/client_config_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,14 @@
     def get_url(self, db_path: str) -> str:
         ...
 
 
 class DBSqliteMode(DBMode):
     db_engine: str = Field(
         default="sqlite",
-        const=True,
         client_data=ClientFieldData(
             prompt=lambda cm: (
                 "Please enter database engine you want to use (reference: https://docs.sqlalchemy.org/en/13/dialects/)"
             ),
         ),
     )
 
@@ -742,59 +741,54 @@
     def build_rate_source(self) -> RateSourceBase:
         return RATE_ORACLE_SOURCES[self.Config.title]()
 
 
 class AscendExRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="ascend_ex",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title = "ascend_ex"
 
 
 class BinanceRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="binance",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title = "binance"
 
 
 class BinanceUSRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="binance_us",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title = "binance_us"
 
 
 class CubeRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="cube",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title = "cube"
 
 
 class CoinGeckoRateSourceMode(RateSourceModeBase):
     name: str = Field(
         default="coin_gecko",
-        const=True,
         client_data=None,
     )
 
     extra_tokens: List[str] = Field(
         default=[],
         client_data=ClientFieldData(
             prompt=lambda cm: (
@@ -825,15 +819,14 @@
         RateOracle.get_instance().source.extra_token_ids = values["extra_tokens"]
         return values
 
 
 class CoinCapRateSourceMode(RateSourceModeBase):
     name: str = Field(
         default="coin_cap",
-        const=True,
         client_data=None,
     )
     assets_map: Dict[str, str] = Field(
         default=",".join(
             [
                 ":".join(pair) for pair in {
                     "BTC": "bitcoin",
@@ -906,37 +899,34 @@
         )
         return rate_source
 
 
 class KuCoinRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="kucoin",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title = "kucoin"
 
 
 class GateIoRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="gate_io",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title: str = "gate_io"
 
 
 class CoinbaseAdvancedTradeRateSourceMode(ExchangeRateSourceModeBase):
     name: str = Field(
         default="coinbase_advanced_trade",
-        const=True,
         client_data=None,
     )
 
     class Config:
         title: str = "coinbase_advanced_trade"
```

### Comparing `hummingbot-20240429/hummingbot/client/config/conf_migration.py` & `hummingbot-20240520/hummingbot/client/config/conf_migration.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/config_crypt.py` & `hummingbot-20240520/hummingbot/client/config/config_crypt.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/config_data_types.py` & `hummingbot-20240520/hummingbot/client/config/config_data_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Callable, Optional
 
 from pydantic import BaseModel, Extra, Field, validator
-from pydantic.schema import default_ref_template
 
 from hummingbot.client.config.config_methods import strategy_config_schema_encoder
 from hummingbot.client.config.config_validators import validate_connector, validate_decimal
 
 
 class ClientConfigEnum(Enum):
     def __str__(self):
@@ -33,19 +32,19 @@
         extra = Extra.forbid
         json_encoders = {
             datetime: lambda dt: dt.strftime("%Y-%m-%d %H:%M:%S"),
         }
 
     @classmethod
     def schema_json(
-        cls, *, by_alias: bool = True, ref_template: str = default_ref_template, **dumps_kwargs: Any
+        cls, *, by_alias: bool = True, **dumps_kwargs: Any
     ) -> str:
         # todo: make it ignore `client_data` all together
         return cls.__config__.json_dumps(
-            cls.schema(by_alias=by_alias, ref_template=ref_template),
+            cls.schema(by_alias=by_alias),
             default=strategy_config_schema_encoder,
             **dumps_kwargs
         )
 
     @classmethod
     def _clear_schema_cache(cls):
         cls.__schema_cache__ = {}
```

### Comparing `hummingbot-20240429/hummingbot/client/config/config_helpers.py` & `hummingbot-20240520/hummingbot/client/config/config_helpers.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/config_methods.py` & `hummingbot-20240520/hummingbot/client/config/config_methods.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/config_validators.py` & `hummingbot-20240520/hummingbot/client/config/config_validators.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/config_var.py` & `hummingbot-20240520/hummingbot/client/config/config_var.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/fee_overrides_config_map.py` & `hummingbot-20240520/hummingbot/client/config/fee_overrides_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/security.py` & `hummingbot-20240520/hummingbot/client/config/security.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/strategy_config_data_types.py` & `hummingbot-20240520/hummingbot/client/config/strategy_config_data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/config/trade_fee_schema_loader.py` & `hummingbot-20240520/hummingbot/client/config/trade_fee_schema_loader.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/hummingbot_application.py` & `hummingbot-20240520/hummingbot/client/hummingbot_application.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/performance.py` & `hummingbot-20240520/hummingbot/client/performance.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/platform.py` & `hummingbot-20240520/hummingbot/client/platform.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/settings.py` & `hummingbot-20240520/hummingbot/client/settings.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/tab/data_types.py` & `hummingbot-20240520/hummingbot/client/tab/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/tab/order_book_tab.py` & `hummingbot-20240520/hummingbot/client/tab/order_book_tab.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/tab/tab_base.py` & `hummingbot-20240520/hummingbot/client/tab/tab_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/tab/tab_example_tab.py` & `hummingbot-20240520/hummingbot/client/tab/tab_example_tab.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/__init__.py` & `hummingbot-20240520/hummingbot/client/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/completer.py` & `hummingbot-20240520/hummingbot/client/ui/completer.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/custom_widgets.py` & `hummingbot-20240520/hummingbot/client/ui/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/hummingbot_cli.py` & `hummingbot-20240520/hummingbot/client/ui/hummingbot_cli.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/interface_utils.py` & `hummingbot-20240520/hummingbot/client/ui/interface_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/keybindings.py` & `hummingbot-20240520/hummingbot/client/ui/keybindings.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/layout.py` & `hummingbot-20240520/hummingbot/client/ui/layout.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/parser.py` & `hummingbot-20240520/hummingbot/client/ui/parser.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/scroll_handlers.py` & `hummingbot-20240520/hummingbot/client/ui/scroll_handlers.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/stdout_redirection.py` & `hummingbot-20240520/hummingbot/client/ui/stdout_redirection.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/client/ui/style.py` & `hummingbot-20240520/hummingbot/client/ui/style.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/budget_checker.py` & `hummingbot-20240520/hummingbot/connector/budget_checker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/client_order_tracker.py` & `hummingbot-20240520/hummingbot/connector/client_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/connector_base.cpp` & `hummingbot-20240520/hummingbot/connector/connector_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/connector_metrics_collector.py` & `hummingbot-20240520/hummingbot/connector/connector_metrics_collector.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/binance_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/binance_perpetual/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/derivative/binance_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/bit_com_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/derivative/bit_com_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/bitget_perpetual/bitget_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/bybit_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/derivative/bybit_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/dydx_perpetual/dydx_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/gate_io_perpetual/gate_io_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_derivative.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,16 @@
                 "cloid": order_id
             },
         }
         cancel_result = await self._api_post(
             path_url=CONSTANTS.CANCEL_ORDER_URL,
             data=api_params,
             is_auth_required=True)
-        if "error" in cancel_result["response"]["data"]["statuses"][0]:
+
+        if cancel_result.get("status") == "err" or "error" in cancel_result["response"]["data"]["statuses"][0]:
             self.logger().debug(f"The order {order_id} does not exist on Hyperliquid Perpetuals. "
                                 f"No cancelation needed.")
             await self._order_tracker.process_order_not_found(order_id)
             raise IOError(f'{cancel_result["response"]["data"]["statuses"][0]["error"]}')
         if "success" in cancel_result["response"]["data"]["statuses"][0]:
             return True
         return False
@@ -393,15 +394,18 @@
                 "cloid": order_id,
             }
         }
         order_result = await self._api_post(
             path_url=CONSTANTS.CREATE_ORDER_URL,
             data=api_params,
             is_auth_required=True)
-        o_order_result = order_result['response']["data"]["statuses"][0]
+        if order_result.get("status") == "err":
+            raise IOError(f"Error submitting order {order_id}: {order_result['response']}")
+        else:
+            o_order_result = order_result['response']["data"]["statuses"][0]
         if "error" in o_order_result:
             raise IOError(f"Error submitting order {order_id}: {o_order_result['error']}")
         o_data = o_order_result.get("resting") or o_order_result.get("filled")
         o_id = str(o_data["oid"])
         return (o_id, self.current_timestamp)
 
     async def _update_trade_history(self):
@@ -534,56 +538,62 @@
                     continue
                 if channel == CONSTANTS.USER_ORDERS_ENDPOINT_NAME:
                     for order_msg in results:
                         self._process_order_message(order_msg)
                 elif channel == CONSTANTS.USEREVENT_ENDPOINT_NAME:
                     if "fills" in results:
                         for trade_msg in results["fills"]:
-                            self._process_trade_message(trade_msg)
+                            await self._process_trade_message(trade_msg)
             except asyncio.CancelledError:
                 raise
             except Exception:
                 self.logger().error(
                     "Unexpected error in user stream listener loop.", exc_info=True)
                 await self._sleep(5.0)
 
-    def _process_trade_message(self, trade: Dict[str, Any], client_order_id: Optional[str] = None):
+    async def _process_trade_message(self, trade: Dict[str, Any], client_order_id: Optional[str] = None):
         """
         Updates in-flight order and trigger order filled event for trade message received. Triggers order completed
         event if the total executed amount equals to the specified order amount.
         Example Trade:
         """
         exchange_order_id = str(trade.get("oid", ""))
         tracked_order = self._order_tracker.all_fillable_orders_by_exchange_order_id.get(exchange_order_id)
 
         if tracked_order is None:
-            self.logger().debug(f"Ignoring trade message with id {client_order_id}: not in in_flight_orders.")
-        else:
-            trading_pair_base_coin = tracked_order.base_asset
-            if trade["coin"] == trading_pair_base_coin:
-                position_action = PositionAction.OPEN if trade["dir"].split(" ")[0] == "Open" else PositionAction.CLOSE
-                fee_asset = tracked_order.quote_asset
-                fee = TradeFeeBase.new_perpetual_fee(
-                    fee_schema=self.trade_fee_schema(),
-                    position_action=position_action,
-                    percent_token=fee_asset,
-                    flat_fees=[TokenAmount(amount=Decimal(trade["fee"]), token=fee_asset)]
-                )
-                trade_update: TradeUpdate = TradeUpdate(
-                    trade_id=str(trade["tid"]),
-                    client_order_id=tracked_order.client_order_id,
-                    exchange_order_id=str(trade["oid"]),
-                    trading_pair=tracked_order.trading_pair,
-                    fill_timestamp=trade["time"] * 1e-3,
-                    fill_price=Decimal(trade["px"]),
-                    fill_base_amount=Decimal(trade["sz"]),
-                    fill_quote_amount=Decimal(trade["px"]) * Decimal(trade["sz"]),
-                    fee=fee,
-                )
-                self._order_tracker.process_trade_update(trade_update)
+            all_orders = self._order_tracker.all_fillable_orders
+            for k, v in all_orders.items():
+                await v.get_exchange_order_id()
+            _cli_tracked_orders = [o for o in all_orders.values() if exchange_order_id == o.exchange_order_id]
+            if not _cli_tracked_orders:
+                self.logger().debug(f"Ignoring trade message with id {client_order_id}: not in in_flight_orders.")
+                return
+            tracked_order = _cli_tracked_orders[0]
+        trading_pair_base_coin = tracked_order.base_asset
+        if trade["coin"] == trading_pair_base_coin:
+            position_action = PositionAction.OPEN if trade["dir"].split(" ")[0] == "Open" else PositionAction.CLOSE
+            fee_asset = tracked_order.quote_asset
+            fee = TradeFeeBase.new_perpetual_fee(
+                fee_schema=self.trade_fee_schema(),
+                position_action=position_action,
+                percent_token=fee_asset,
+                flat_fees=[TokenAmount(amount=Decimal(trade["fee"]), token=fee_asset)]
+            )
+            trade_update: TradeUpdate = TradeUpdate(
+                trade_id=str(trade["tid"]),
+                client_order_id=tracked_order.client_order_id,
+                exchange_order_id=str(trade["oid"]),
+                trading_pair=tracked_order.trading_pair,
+                fill_timestamp=trade["time"] * 1e-3,
+                fill_price=Decimal(trade["px"]),
+                fill_base_amount=Decimal(trade["sz"]),
+                fill_quote_amount=Decimal(trade["px"]) * Decimal(trade["sz"]),
+                fee=fee,
+            )
+            self._order_tracker.process_trade_update(trade_update)
 
     def _process_order_message(self, order_msg: Dict[str, Any]):
         """
         Updates in-flight order and triggers cancelation or failure event if needed.
 
         :param order_msg: The order response from either REST or web socket API (they are of the same format)
 
@@ -756,14 +766,16 @@
         try:
             set_leverage = await self._api_post(
                 path_url=CONSTANTS.SET_LEVERAGE_URL,
                 data=params,
                 is_auth_required=True)
             success = False
             msg = ""
+            if set_leverage.get("status") == "err":
+                raise IOError(f"{set_leverage}")
             if set_leverage["status"] == 'ok':
                 success = True
             else:
                 msg = 'Unable to set leverage'
             return success, msg
         except Exception as exception:
             success = False
```

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/hyperliquid_perpetual/hyperliquid_perpetual_web_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from decimal import Decimal
 from typing import Any, Dict, Optional, Tuple
 
 import hummingbot.connector.derivative.hyperliquid_perpetual.hyperliquid_perpetual_constants as CONSTANTS
 from hummingbot.core.api_throttler.async_throttler import AsyncThrottler
 from hummingbot.core.web_assistant.auth import AuthBase
 from hummingbot.core.web_assistant.connections.data_types import RESTRequest
 from hummingbot.core.web_assistant.rest_pre_processors import RESTPreProcessorBase
@@ -124,29 +125,32 @@
         return 1
     elif grouping == "positionTpsl":
         return 2
 
 
 def order_spec_to_order_wire(order_spec):
     return {
-        "asset": order_spec["asset"],
-        "isBuy": order_spec["isBuy"],
-        "limitPx": float_to_wire(order_spec["limitPx"]),
-        "sz": float_to_wire(order_spec["sz"]),
-        "reduceOnly": order_spec["reduceOnly"],
-        "orderType": order_type_to_wire(order_spec["orderType"]),
-        "cloid": order_spec["cloid"],
+        "a": order_spec["asset"],
+        "b": order_spec["isBuy"],
+        "p": float_to_wire(order_spec["limitPx"]),
+        "s": float_to_wire(order_spec["sz"]),
+        "r": order_spec["reduceOnly"],
+        "t": order_type_to_wire(order_spec["orderType"]),
+        "c": order_spec["cloid"],
     }
 
 
 def float_to_wire(x: float) -> str:
     rounded = "{:.8f}".format(x)
     if abs(float(rounded) - x) >= 1e-12:
         raise ValueError("float_to_wire causes rounding", x)
-    return rounded
+    if rounded == "-0":
+        rounded = "0"
+    normalized = Decimal(rounded).normalize()
+    return f"{normalized:f}"
 
 
 def order_type_to_wire(order_type):
     if "limit" in order_type:
         return {"limit": order_type["limit"]}
     elif "trigger" in order_type:
         return {
```

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/injective_v2_perpetual/injective_v2_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/kucoin_perpetual/kucoin_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     PositionMode.ONEWAY: POSITION_MODE_API_ONEWAY,
     PositionMode.HEDGE: POSITION_MODE_API_HEDGE,
 }
 
 ORDER_TYPE_MAP = {
     OrderType.LIMIT: "limit",
     OrderType.MARKET: "market",
+    OrderType.LIMIT_MAKER: "post_only",
 }
 
 GET = "GET"
 POST = "POST"
 METHOD = "METHOD"
 ENDPOINT = "ENDPOINT"
```

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/okx_perpetual/okx_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/perpetual_budget_checker.py` & `hummingbot-20240520/hummingbot/connector/derivative/perpetual_budget_checker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/phemex_perpetual/phemex_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/position.py` & `hummingbot-20240520/hummingbot/connector/derivative/position.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_data.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_derivative.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py` & `hummingbot-20240520/hummingbot/connector/derivative/vega_perpetual/vega_perpetual_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/derivative_base.py` & `hummingbot-20240520/hummingbot/connector/derivative_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/ascend_ex/ascend_ex_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/binance_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/binance/binance_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/binance/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/binance/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/__init__.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_active_order_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_in_flight_order.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.connector.exchange.bitfinex.bitfinex_order_book",
         "sources": [
             "hummingbot/connector/exchange/bitfinex/bitfinex_order_book.pyx"
         ]
     },
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitfinex/bitfinex_websocket.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/bitmart_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitmart/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/bitmart/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bitrue/bitrue_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/btc_markets/btc_markets_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/bybit_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/bybit_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/bybit/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/bybit/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/coinbase_advanced_trade_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_advanced_trade/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_active_order_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_in_flight_order.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.connector.exchange.coinbase_pro.coinbase_pro_order_book",
         "sources": [
             "hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book.pyx"
         ]
     },
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/coinbase_pro/coinbase_pro_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,15 +994,18 @@
         symbol = await self.exchange_symbol_associated_to_pair(trading_pair=trading_pair)
 
         # Filter tickers that match the trading pair
         tickers = [ticker for ticker in tickers if ticker["ticker_id"].upper() == symbol]
         # Get the first item
         ticker = tickers[0]
 
-        return float(ticker["last_price"])
+        if ticker.get("last_price", 0) is None:
+            return float(0)
+
+        return float(ticker.get("last_price", 0))
 
     def buy(
             self, trading_pair: str, amount: Decimal, order_type=OrderType.LIMIT, price: Decimal = s_decimal_NaN,
             **kwargs
     ) -> str:
         """
         Creates a promise to create a buy order using the parameters
@@ -1140,7 +1143,17 @@
         :return: True if the domain value is valid, False otherwise
         """
         valid_domains = [CONSTANTS.DEFAULT_DOMAIN, CONSTANTS.TESTNET_DOMAIN]
         if domain not in valid_domains:
             self.logger().error(f"Invalid domain: {domain}. Domain must be one of {valid_domains}")
             return False
         return True
+
+    async def all_trading_pairs(self) -> List[str]:
+        """
+        Returns a list of all trading pairs on the exchange
+        :return: a list of all trading pairs on the exchange
+        """
+        all_pairs: bidict = await self.trading_pair_symbol_map()
+        all_pairs_inverse = list(all_pairs.inverse)
+
+        return all_pairs_inverse
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/market_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi` & `hummingbot-20240520/hummingbot/connector/exchange/cube/cube_ws_protobufs/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/cube/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/cube/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_connector.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/foxbit/foxbit_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/gate_io_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/gate_io/placeholder.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/gate_io/placeholder.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_active_order_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py` & `hummingbot-20240520/hummingbot/connector/exchange/hitbtc/hitbtc_websocket.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/htx/htx_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/htx/htx_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/account_delegation_script.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/account_delegation_script.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_grantee_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_read_only_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/data_sources/injective_vaults_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_market.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_market.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_query_executor.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_query_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/injective_v2/injective_v2_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kraken/kraken_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/kraken/kraken_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/kucoin/kucoin_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/mexc/mexc_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/mexc/mexc_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_order_book_message.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py` & `hummingbot-20240520/hummingbot/connector/exchange/ndax/ndax_websocket_adaptor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "partially_filled": OrderState.PARTIALLY_FILLED,
     "canceled": OrderState.CANCELED,
 }
 
 ORDER_TYPE_MAP = {
     OrderType.LIMIT: "limit",
     OrderType.MARKET: "market",
+    OrderType.LIMIT_MAKER: "post_only",
 }
 
 NO_LIMIT = sys.maxsize
 
 RATE_LIMITS = [
     RateLimit(WS_CONNECTION_LIMIT_ID, limit=1, time_interval=1),
     RateLimit(WS_REQUEST_LIMIT_ID, limit=100, time_interval=10),
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/okx/okx_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/okx/okx_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/paper_trade/__init__.py` & `hummingbot-20240520/hummingbot/connector/exchange/paper_trade/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/paper_trade/market_config.py` & `hummingbot-20240520/hummingbot/connector/exchange/paper_trade/market_config.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/paper_trade/paper_trade_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 
 MAX_ID_LEN = 32
 CLIENT_ID_PREFIX = "HBOT"
 
 DEFAULT_DOMAIN = ""
 
 GRAPHQL_ENDPOINTS = {
-    DEFAULT_DOMAIN: "https://yx375ldozvcvthjk2nczch3fhq.appsync-api.eu-central-1.amazonaws.com/graphql",
+    DEFAULT_DOMAIN: "https://api.polkadex.trade/graphql",
+}
+# PolkaDEX team send this special URL for WS
+GRAPHQL_WS_ENDPOINTS = {
+    DEFAULT_DOMAIN: "wss://api.polkadex.trade/graphql/realtime",
 }
 BLOCKCHAIN_URLS = {
     DEFAULT_DOMAIN: "wss://polkadex.public.curie.radiumblock.co/ws",
 }
 POLKADEX_SS58_PREFIX = 88
 
 ORDERBOOK_UPDATES_STREAM_NAME = "ob-inc"
@@ -72,16 +76,16 @@
     RateLimit(
         limit_id=ALL_FILLS_LIMIT_ID,
         limit=NO_LIMIT,
         time_interval=SECOND,
     ),
     RateLimit(
         limit_id=PLACE_ORDER_LIMIT_ID,
-        limit=NO_LIMIT,
-        time_interval=SECOND,
+        limit=2,
+        time_interval=2,
     ),
     RateLimit(
         limit_id=CANCEL_ORDER_LIMIT_ID,
         limit=NO_LIMIT,
         time_interval=SECOND,
     ),
     RateLimit(
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import json
 import logging
 import time
 from decimal import Decimal
 from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple
 from urllib.parse import urlparse
 
+import gql
 from bidict import bidict
-from gql.transport.appsync_auth import AppSyncJWTAuthentication
 from scalecodec.base import RuntimeConfiguration
 from scalecodec.type_registry import load_type_registry_preset
 from substrateinterface import Keypair, KeypairType
 
 from hummingbot.connector.exchange.polkadex import polkadex_constants as CONSTANTS, polkadex_utils
 from hummingbot.connector.exchange.polkadex.polkadex_query_executor import GrapQLQueryExecutor
 from hummingbot.connector.trading_rule import TradingRule
@@ -44,49 +44,56 @@
 
     def __init__(
         self,
         connector: "ExchangePyBase",
         seed_phrase: str,
         domain: Optional[str] = CONSTANTS.DEFAULT_DOMAIN,
         trading_required: bool = True,
+        trading_pairs: list = [],
     ):
         self._connector = connector
         self._domain = domain
         self._trading_required = trading_required
         graphql_host = CONSTANTS.GRAPHQL_ENDPOINTS[self._domain]
-        netloc_host = urlparse(graphql_host).netloc
+        self.netloc_host = urlparse(graphql_host).netloc
         self._keypair = None
         self._user_main_address = None
+        self._seed_phrase = seed_phrase
+        self._trading_pairs = trading_pairs
         if seed_phrase is not None and len(seed_phrase) > 0:
             self._keypair = Keypair.create_from_mnemonic(
                 seed_phrase, CONSTANTS.POLKADEX_SS58_PREFIX, KeypairType.SR25519
             )
             self._user_proxy_address = self._keypair.ss58_address
-            self._auth = AppSyncJWTAuthentication(netloc_host, self._user_proxy_address)
+            self._auth = gql.transport.appsync_auth.AppSyncJWTAuthentication(self.netloc_host, self._user_proxy_address)
         else:
             self._user_proxy_address = "READ_ONLY"
-            self._auth = AppSyncJWTAuthentication(netloc_host, "READ_ONLY")
+            self._auth = gql.transport.appsync_auth.AppSyncJWTAuthentication(self.netloc_host, "READ_ONLY")
 
         # Load Polkadex Runtime Config
         self._runtime_config = RuntimeConfiguration()
         # Register core types
         self._runtime_config.update_type_registry(load_type_registry_preset("core"))
         # Register Orderbook specific types
         self._runtime_config.update_type_registry(CONSTANTS.CUSTOM_TYPES)
 
-        self._query_executor = GrapQLQueryExecutor(auth=self._auth, domain=self._domain)
-
         self._publisher = PubSub()
         self._last_received_message_time = 0
         # We create a throttler instance here just to have a fully valid instance from the first moment.
         # The connector using this data source should replace the throttler with the one used by the connector.
         self._throttler = AsyncThrottler(rate_limits=CONSTANTS.RATE_LIMITS)
         self._events_listening_tasks = []
         self._assets_map: Dict[str, str] = {}
 
+        self._query_executor = GrapQLQueryExecutor(
+            auth=self._auth,
+            domain=self._domain,
+            throttler=self._throttler
+        )
+
         self._polkadex_order_type = {
             OrderType.MARKET: "MARKET",
             OrderType.LIMIT: "LIMIT",
             OrderType.LIMIT_MAKER: "LIMIT",
         }
         self._hummingbot_order_type = {
             "LIMIT": OrderType.LIMIT,
@@ -98,20 +105,20 @@
         }
         self._hummingbot_trade_type = {
             "Bid": TradeType.BUY,
             "Ask": TradeType.SELL,
         }
 
     def is_started(self) -> bool:
+        # adds another status check
         return len(self._events_listening_tasks) > 0
 
     async def start(self, market_symbols: List[str]):
         if len(self._events_listening_tasks) > 0:
             raise AssertionError("Polkadex datasource is already listening to events and can't be started again")
-        await self._query_executor.create_ws_session()
 
         for market_symbol in market_symbols:
             self._events_listening_tasks.append(
                 asyncio.create_task(
                     self._query_executor.listen_to_orderbook_updates(
                         events_handler=self._process_order_book_event, market_symbol=market_symbol
                     )
@@ -137,130 +144,161 @@
             self._events_listening_tasks.append(
                 asyncio.create_task(
                     self._query_executor.listen_to_private_events(
                         events_handler=self._process_private_event, address=main_address
                     )
                 )
             )
+            self.logger().info("Started Polkadex_data_source")
+
+    async def check_status(self):
+        self.logger().info(f"Polkadex status is checked. self._query_executor._restart_initialization: {self._query_executor._restart_initialization}, self.trading_pairs {self._trading_pairs}")
+        if self._query_executor._restart_initialization:
+            self.logger().info("Polkadex status check - Need to reinitiate the query_executor")
+            await self.stop()
+            self.logger().info("Polkadex status check - Stopped the stackers")
+            await self.reinitiaite_query_executor()
+            self.logger().info("Polkadex status check - Reinitiated the trackers")
+            await self.start(self._trading_pairs)
+            self.logger().info("Polkadex status check - Started Again")
+
+    async def reinitiaite_query_executor(self):
+        self._query_executor = None
+        self.logger().info("Polkadex status check - Reinitiating the query executor")
+        if self._seed_phrase is not None and len(self._seed_phrase) > 0:
+            self._keypair = Keypair.create_from_mnemonic(
+                self._seed_phrase, CONSTANTS.POLKADEX_SS58_PREFIX, KeypairType.SR25519
+            )
+            self._user_proxy_address = self._keypair.ss58_address
+            self._auth = gql.transport.appsync_auth.AppSyncJWTAuthentication(self.netloc_host, self._user_proxy_address)
+        else:
+            self._user_proxy_address = "READ_ONLY"
+            self._auth = gql.transport.appsync_auth.AppSyncJWTAuthentication(self.netloc_host, "READ_ONLY")
+
+        self._query_executor = GrapQLQueryExecutor(auth=self._auth, domain=self._domain, throttler=self._throttler)
+        self.logger().info("Polkadex - Finished reinitiation")
 
     async def stop(self):
         for task in self._events_listening_tasks:
             task.cancel()
         self._events_listening_tasks = []
+        self.logger().info("Stopped Polkadex_data_source")
 
     def configure_throttler(self, throttler: AsyncThrottlerBase):
         self._throttler = throttler
 
     def last_received_message_time(self) -> float:
         return self._last_received_message_time
 
     def add_listener(self, event_tag: Enum, listener: EventListener):
         self._publisher.add_listener(event_tag=event_tag, listener=listener)
 
     def remove_listener(self, event_tag: Enum, listener: EventListener):
         self._publisher.remove_listener(event_tag=event_tag, listener=listener)
 
     async def exchange_status(self):
+        await self.check_status()
         all_assets = await self.assets_map()
 
         if len(all_assets) > 0:
             result = NetworkStatus.CONNECTED
         else:
             result = NetworkStatus.NOT_CONNECTED
 
         return result
 
+    async def get_all_open_orders(self) -> List[Dict[str, Any]]:
+        await self.check_status()
+        return await self._query_executor.list_open_orders_by_main_account(main_account=await self.user_main_address())
+
     async def assets_map(self) -> Dict[str, str]:
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ALL_ASSETS_LIMIT_ID):
-            all_assets = await self._query_executor.all_assets()
+        all_assets = await self._query_executor.all_assets()
+
         self._assets_map = {
             asset["asset_id"]: polkadex_utils.normalized_asset_name(
                 asset_id=asset["asset_id"], asset_name=asset["name"]
             )
-            for asset in all_assets["getAllAssets"]["items"]
+            for asset in all_assets
         }
 
         if len(self._assets_map) > 0:
             self._assets_map["polkadex"] = "PDEX"  # required due to inconsistent token name in private balance event
 
         return self._assets_map
 
     async def symbols_map(self) -> Mapping[str, str]:
         symbols_map = bidict()
         assets_map = await self.assets_map()
 
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ALL_MARKETS_LIMIT_ID):
-            markets = await self._query_executor.all_markets()
+        all_markets = await self._query_executor.all_markets()
 
-        for market_info in markets["getAllMarkets"]["items"]:
+        for market_info in all_markets:
             try:
                 base_asset, quote_asset = market_info["market"].split("-")
                 base = assets_map[base_asset]
                 quote = assets_map[quote_asset]
                 symbols_map[market_info["market"]] = combine_to_hb_trading_pair(base=base, quote=quote)
             except KeyError:
                 continue
         return symbols_map
 
     async def all_trading_rules(self) -> List[TradingRule]:
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ALL_MARKETS_LIMIT_ID):
-            markets = await self._query_executor.all_markets()
+        all_markets = await self._query_executor.all_markets()
 
         trading_rules = []
-        for market_info in markets["getAllMarkets"]["items"]:
+        for market_info in all_markets:
             try:
                 exchange_trading_pair = market_info["market"]
                 trading_pair = await self._connector.trading_pair_associated_to_exchange_symbol(
                     symbol=exchange_trading_pair
                 )
-                min_order_size = Decimal(market_info["min_order_qty"])
-                max_order_size = Decimal(market_info["max_order_qty"])
-                min_order_price = Decimal(market_info["min_order_price"])
                 amount_increment = Decimal(market_info["qty_step_size"])
                 price_increment = Decimal(market_info["price_tick_size"])
+                min_order_value = Decimal(market_info["min_volume"])
                 trading_rules.append(
                     TradingRule(
                         trading_pair=trading_pair,
-                        min_order_size=min_order_size,
-                        max_order_size=max_order_size,
+                        # New API doesn't return min/max order size
+                        # so we're trying to put some reasonable numbers here
+                        min_order_size=0,
+                        max_order_size=10**6,
                         min_price_increment=price_increment,
                         min_base_amount_increment=amount_increment,
                         min_quote_amount_increment=price_increment,
-                        min_notional_size=min_order_size * min_order_price,
-                        min_order_value=min_order_size * min_order_price,
+                        min_notional_size=min_order_value,
+                        min_order_value=min_order_value,
                     )
                 )
             except asyncio.CancelledError:
                 raise
             except Exception:
                 self.logger().exception(f"Error parsing the trading pair rule: {market_info}. Skipping...")
+                # QUICKFIX (dmitry): previously we were following "all or nothing" strategy here, but it was
+                # blocking the startup of the bot
 
         return trading_rules
 
     async def order_book_snapshot(self, market_symbol: str, trading_pair: str) -> OrderBookMessage:
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ORDERBOOK_LIMIT_ID):
-            snapshot_data = await self._query_executor.get_orderbook(market_symbol=market_symbol)
-
-        orderbook_entries = snapshot_data["getOrderbook"]["items"]
+        orderbook_items = await self._query_executor.get_orderbook(market_symbol)
 
         timestamp = self._time()
         update_id = -1
         bids = []
         asks = []
 
-        for orderbook_entry in orderbook_entries:
-            price = Decimal(str(orderbook_entry["p"]))
-            amount = Decimal(str(orderbook_entry["q"]))
+        for orderbook_item in orderbook_items:
+            price = Decimal(str(orderbook_item["p"]))
+            amount = Decimal(str(orderbook_item["q"]))
 
-            if orderbook_entry["s"] == "Bid":
+            if orderbook_item["s"] == "Bid":
                 bids.append((price, amount))
             else:
                 asks.append((price, amount))
 
-            update_id = max(update_id, int(orderbook_entry["stid"]))
+            update_id = max(update_id, int(orderbook_item["stid"]))
 
         order_book_message_content = {
             "trading_pair": trading_pair,
             "update_id": update_id,
             "bids": bids,
             "asks": asks,
         }
@@ -270,45 +308,40 @@
             timestamp=timestamp,
         )
 
         return snapshot_msg
 
     async def user_main_address(self):
         if self._user_main_address is None:
-            async with self._throttler.execute_task(limit_id=CONSTANTS.FIND_USER_LIMIT_ID):
-                self._user_main_address = await self._query_executor.main_account_from_proxy(
-                    proxy_account=self._user_proxy_address,
-                )
+            self._user_main_address = await self._query_executor.main_account_from_proxy(
+                proxy_account=self._user_proxy_address)
         return self._user_main_address
 
     async def last_price(self, market_symbol: str) -> float:
-        async with self._throttler.execute_task(limit_id=CONSTANTS.PUBLIC_TRADES_LIMIT_ID):
-            response = await self._query_executor.recent_trades(market_symbol=market_symbol, limit=1)
-        last_price = response["getRecentTrades"]["items"][0]["p"]
-
-        return float(last_price)
+        recent_trade = await self._query_executor.recent_trade(market_symbol=market_symbol)
+        return float(recent_trade["p"])
 
     async def all_balances(self) -> List[Dict[str, Any]]:
         result = []
         assets_map = await self.assets_map()
         main_account = await self.user_main_address()
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ALL_BALANCES_LIMIT_ID):
-            balances = await self._query_executor.get_all_balances_by_main_account(main_account=main_account)
+        balances = await self._query_executor.get_all_balances_by_main_account(main_account=main_account)
 
-        for token_balance in balances["getAllBalancesByMainAccount"]["items"]:
+        for token_balance in balances:
             try:
                 balance_info = {}
                 available_balance = Decimal(token_balance["f"])
                 locked_balance = Decimal(token_balance["r"])
                 balance_info["token_name"] = assets_map[token_balance["a"]]
                 balance_info["total_balance"] = available_balance + locked_balance
                 balance_info["available_balance"] = available_balance
                 result.append(balance_info)
             except KeyError:
                 continue
+
         return result
 
     async def place_order(
         self,
         market_symbol: str,
         client_order_id: str,
         price: Decimal,
@@ -332,52 +365,42 @@
             "order_type": self._polkadex_order_type[order_type],
             "side": self._polkadex_trade_type[trade_type],
         }
 
         place_order_request = self._runtime_config.create_scale_object("OrderPayload").encode(order_parameters)
         signature = self._keypair.sign(place_order_request)
 
-        async with self._throttler.execute_task(limit_id=CONSTANTS.PLACE_ORDER_LIMIT_ID):
-            response = await self._query_executor.place_order(
-                polkadex_order=order_parameters,
-                signature={"Sr25519": signature.hex()},
-            )
-            place_order_data = json.loads(response["place_order"])
-
-        exchange_order_id = None
-        if place_order_data["is_success"] is True:
-            exchange_order_id = place_order_data["body"]
+        exchange_order_id = await self._query_executor.place_order(
+            polkadex_order=order_parameters,
+            signature={"Sr25519": signature.hex()}
+        )
 
         if exchange_order_id is None:
             raise ValueError(f"Error in Polkadex creating order {client_order_id}")
 
         return exchange_order_id, timestamp
 
     async def cancel_order(self, order: InFlightOrder, market_symbol: str, timestamp: float) -> OrderState:
+        # TODO (dmitry): analyze this logic and move to query executor
         try:
             cancel_result = await self._place_order_cancel(order=order, market_symbol=market_symbol)
         except Exception as e:
             if "Order is not active" in str(e):
                 new_order_state = OrderState.CANCELED
             else:
                 raise
         else:
-            new_order_state = OrderState.PENDING_CANCEL if cancel_result["cancel_order"] else order.current_state
+            new_order_state = OrderState.PENDING_CANCEL if cancel_result else order.current_state
 
         return new_order_state
 
     async def order_update(self, order: InFlightOrder, market_symbol: str) -> OrderUpdate:
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ORDER_UPDATE_LIMIT_ID):
-            response = await self._query_executor.find_order_by_main_account(
-                main_account=self._user_proxy_address,
-                market_symbol=market_symbol,
-                order_id=order.exchange_order_id,
-            )
+        # TODO (dmitry): remove `market_symbol` from function signature, it's not needed
 
-        order_info = response["findOrderByMainAccount"]
+        order_info = await self._query_executor.find_order_by_id(order_id=order.exchange_order_id)
 
         if order_info is None:
             raise IOError(f"Order not found {order.client_order_id} ({order.exchange_order_id})")
 
         new_state = CONSTANTS.ORDER_STATE[order_info["st"]]
         filled_amount = Decimal(order_info["fq"])
         if new_state == OrderState.OPEN and filled_amount > 0:
@@ -392,31 +415,32 @@
         return order_update
 
     async def get_all_fills(
         self, from_timestamp: float, to_timestamp: float, orders: List[InFlightOrder]
     ) -> List[TradeUpdate]:
         trade_updates = []
 
-        async with self._throttler.execute_task(limit_id=CONSTANTS.ALL_FILLS_LIMIT_ID):
-            fills = await self._query_executor.get_order_fills_by_main_account(
-                from_timestamp=from_timestamp, to_timestamp=to_timestamp, main_account=self._user_proxy_address
-            )
+        fills = await self._query_executor.get_order_fills_by_main_account(
+            from_timestamp=from_timestamp,
+            to_timestamp=to_timestamp,
+            main_account=self._user_proxy_address
+        )
 
         exchange_order_id_to_order = {order.exchange_order_id: order for order in orders}
-        for fill in fills["listTradesByMainAccount"]["items"]:
+        for fill in fills:
             exchange_trading_pair = fill["m"]
             trading_pair = await self._connector.trading_pair_associated_to_exchange_symbol(
                 symbol=exchange_trading_pair
             )
 
             price = Decimal(fill["p"])
             size = Decimal(fill["q"])
-            order = exchange_order_id_to_order.get(fill["m_id"], None)
+            order = exchange_order_id_to_order.get(fill["maker_id"], None)
             if order is None:
-                order = exchange_order_id_to_order.get(fill["t_id"], None)
+                order = exchange_order_id_to_order.get(fill["taker_id"], None)
             if order is not None:
                 exchange_order_id = order.exchange_order_id
                 client_order_id = order.client_order_id
 
                 fee = await self._build_fee_for_event(event=fill, trade_type=order.trade_type)
                 trade_updates.append(
                     TradeUpdate(
@@ -434,22 +458,21 @@
 
         return trade_updates
 
     async def _place_order_cancel(self, order: InFlightOrder, market_symbol: str) -> Dict[str, Any]:
         cancel_request = self._runtime_config.create_scale_object("H256").encode(order.exchange_order_id)
         signature = self._keypair.sign(cancel_request)
 
-        async with self._throttler.execute_task(limit_id=CONSTANTS.CANCEL_ORDER_LIMIT_ID):
-            cancel_result = await self._query_executor.cancel_order(
-                order_id=order.exchange_order_id,
-                market_symbol=market_symbol,
-                main_address=self._user_main_address,
-                proxy_address=self._user_proxy_address,
-                signature={"Sr25519": signature.hex()},
-            )
+        cancel_result = await self._query_executor.cancel_order(
+            order_id=order.exchange_order_id,
+            market_symbol=market_symbol,
+            main_address=self._user_main_address,
+            proxy_address=self._user_proxy_address,
+            signature={"Sr25519": signature.hex()},
+        )
 
         return cancel_result
 
     def _process_order_book_event(self, event: Dict[str, Any], market_symbol: str):
         safe_ensure_future(self._process_order_book_event_async(event=event, market_symbol=market_symbol))
 
     async def _process_order_book_event_async(self, event: Dict[str, Any], market_symbol: str):
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,20 @@
         trading_required: bool = True,
         domain: str = CONSTANTS.DEFAULT_DOMAIN,
     ):
         self._trading_required = trading_required
         self._trading_pairs = trading_pairs
         self._domain = domain
         self._data_source = PolkadexDataSource(
-            connector=self, seed_phrase=polkadex_seed_phrase, domain=self._domain, trading_required=trading_required
+            connector=self, seed_phrase=polkadex_seed_phrase, domain=self._domain, trading_pairs=trading_pairs, trading_required=trading_required
         )
         super().__init__(client_config_map=client_config_map)
         self._data_source.configure_throttler(throttler=self._throttler)
         self._forwarders = []
+        self._open_oder_fetching_timestamp = float(0)
         self._configure_event_forwarders()
 
     @property
     def name(self) -> str:
         return CONSTANTS.EXCHANGE_NAME
 
     @property
@@ -314,16 +315,16 @@
                 )
 
                 for trade_update in trade_updates:
                     self._order_tracker.process_trade_update(trade_update=trade_update)
 
         except asyncio.CancelledError:
             raise
-        except Exception:
-            self.logger().warning("Error fetching trades updates.")
+        except Exception as e:
+            self.logger().warning(f"Error fetching trades updates. {e}")
 
     async def _all_trade_updates_for_order(self, order: InFlightOrder) -> List[TradeUpdate]:
         # not used
         raise NotImplementedError
 
     async def _request_order_status(self, tracked_order: InFlightOrder) -> OrderUpdate:
         symbol = await self.exchange_symbol_associated_to_pair(tracked_order.trading_pair)
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py` & `hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_query_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import asyncio
 import json
 import logging
+import sys
 from abc import ABC, abstractmethod
 from datetime import datetime
-from typing import Any, AsyncIterable, Callable, Dict, Optional
+from typing import Any, AsyncIterable, Callable, Dict, List, Optional
 
 from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.appsync_auth import AppSyncAuthentication
 from gql.transport.appsync_websockets import AppSyncWebsocketsTransport
 from graphql import DocumentNode
 
 from hummingbot.connector.exchange.polkadex import polkadex_constants as CONSTANTS
+from hummingbot.core.api_throttler.async_throttler import AsyncThrottler
 from hummingbot.logger import HummingbotLogger
 
 
 class BaseQueryExecutor(ABC):
     @abstractmethod
     async def all_assets(self):
         raise NotImplementedError  # pragma: no cover
@@ -29,15 +31,15 @@
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     async def main_account_from_proxy(self, proxy_account=str) -> str:
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
-    async def recent_trades(self, market_symbol: str, limit: int) -> Dict[str, Any]:
+    async def recent_trade(self, market_symbol: str) -> Dict[str, Any]:
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     async def get_all_balances_by_main_account(self, main_account: str) -> Dict[str, Any]:
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
@@ -58,21 +60,15 @@
         proxy_address: str,
         main_address: str,
         signature: Dict[str, Any],
     ) -> Dict[str, Any]:
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
-    async def list_order_history_by_account(
-        self, main_account: str, from_time: float, to_time: float
-    ) -> Dict[str, Any]:
-        raise NotImplementedError  # pragma: no cover
-
-    @abstractmethod
-    async def find_order_by_main_account(self, main_account: str, market_symbol: str, order_id: str) -> Dict[str, Any]:
+    async def find_order_by_id(self, order_id: str) -> Dict[str, Any]:
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     async def list_open_orders_by_main_account(self, main_account: str) -> Dict[str, Any]:
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
@@ -93,158 +89,184 @@
 
     @classmethod
     def logger(cls) -> HummingbotLogger:
         if cls._logger is None:
             cls._logger = logging.getLogger(HummingbotLogger.logger_name_for_class(cls))
         return cls._logger
 
-    def __init__(self, auth: AppSyncAuthentication, domain: Optional[str] = CONSTANTS.DEFAULT_DOMAIN):
+    def __init__(
+        self,
+        throttler: AsyncThrottler,
+        auth: AppSyncAuthentication,
+        domain: Optional[str] = CONSTANTS.DEFAULT_DOMAIN,
+    ):
         super().__init__()
         self._auth = auth
         self._domain = domain
-        self._client = None
-        self._ws_session = None
-
-    async def create_ws_session(self):
-        url = CONSTANTS.GRAPHQL_ENDPOINTS[self._domain]
-        transport = AppSyncWebsocketsTransport(url=url, auth=self._auth)
-        self._client = Client(transport=transport, fetch_schema_from_transport=False)
-        self._ws_session = await self._client.connect_async(reconnecting=True)
+        self._websocket_failure = False
+        self._websocket_failure_timestamp = float(0)
+        self._restart_initialization = False
+        self._throttler = throttler
 
-    async def all_assets(self):
+    async def all_assets(self) -> List[Dict[str, Any]]:
         query = gql(
             """
-            query GetAllAssets {
-                getAllAssets {
+            query getAllAssets($limit: Int, $nextToken: String) {
+                getAllAssets(limit: $limit, nextToken: $nextToken) {
                     items {
                         asset_id
                         name
                     }
+                    nextToken
                 }
             }
             """
         )
 
-        parameters = {}
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return await self._query_all_pages(
+            query=query,
+            parameters=None,
+            field_name="getAllAssets",
+            throttler_limit_id=CONSTANTS.ALL_ASSETS_LIMIT_ID
+        )
 
-    async def all_markets(self):
+    async def all_markets(self) -> List[Dict[str, Any]]:
         query = gql(
             """
             query MyQuery {
                 getAllMarkets {
                     items {
                         market
-                        max_order_price
-                        min_order_price
-                        min_order_qty
-                        max_order_qty
+                        min_volume
                         price_tick_size
                         qty_step_size
-                        base_asset_precision
-                        quote_asset_precision
                     }
                 }
             }
             """
         )
 
-        parameters = {}
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return (
+            await self._execute_query(
+                query=query,
+                parameters=None,
+                field_name="getAllMarkets",
+                throttler_limit_id=CONSTANTS.ALL_MARKETS_LIMIT_ID)
+        )["items"]
 
-    async def get_orderbook(self, market_symbol: str) -> Dict[str, Any]:
+    async def get_orderbook(self, market_symbol: str) -> List[Dict[str, Any]]:
         query = gql(
             """
             query getOrderbook($market: String!, $limit: Int, $nextToken: String) {
               getOrderbook(market: $market, limit: $limit, nextToken: $nextToken) {
-                nextToken
                 items {
                   p
                   q
                   s
                   stid
                 }
                 nextToken
               }
             }
             """
         )
 
-        parameters = {"market": market_symbol}
+        parameters = {
+            "market": market_symbol,
+        }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return await self._query_all_pages(
+            query=query,
+            parameters=parameters,
+            field_name="getOrderbook",
+            throttler_limit_id=CONSTANTS.ORDERBOOK_LIMIT_ID
+        )
 
     async def main_account_from_proxy(self, proxy_account=str) -> str:
+        # "proxy account" is actually a "trade account"
         query = gql(
             """
-            query findUserByProxyAccount($proxy_account: String!) {
-                findUserByProxyAccount(proxy_account: $proxy_account) {
-                    items {
-                        hash_key
-                        range_key
-                        stid
-                    }
+            query findUserByTradeAccount($trade_account: String!) {
+              findUserByTradeAccount(trade_account: $trade_account) {
+                items {
+                  main
                 }
+              }
             }
             """
         )
-        parameters = {"proxy_account": proxy_account}
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        main_account = result["findUserByProxyAccount"]["items"][0]["range_key"]
-        return main_account
+        parameters = {
+            "trade_account": proxy_account,
+        }
+
+        return (await self._execute_query(
+            query=query,
+            parameters=parameters,
+            field_name="findUserByTradeAccount",
+            throttler_limit_id=CONSTANTS.FIND_USER_LIMIT_ID
+        ))["items"][0]["main"]
 
-    async def recent_trades(self, market_symbol: str, limit: int) -> Dict[str, Any]:
+    async def recent_trade(self, market_symbol: str) -> Dict[str, Any]:
         query = gql(
             """
-            query getRecentTrades($market: String!, $limit: Int, $nextToken: String) {
-              getRecentTrades(m: $market, limit: $limit, nextToken: $nextToken) {
+            query listRecentTrades($market: String!, $limit: Int, $nextToken: String) {
+              listRecentTrades(m: $market, limit: $limit, nextToken: $nextToken) {
                 items {
-                    isReverted
-                    m
                     p
-                    q
-                    t
                 }
               }
             }
             """
         )
 
-        parameters = {"market": market_symbol, "limit": limit}
+        parameters = {
+            "market": market_symbol,
+            "limit": 1,
+        }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return (await self._execute_query(
+            query=query,
+            parameters=parameters,
+            field_name="listRecentTrades",
+            throttler_limit_id=CONSTANTS.PUBLIC_TRADES_LIMIT_ID
+        ))["items"][0]
 
-    async def get_all_balances_by_main_account(self, main_account: str) -> Dict[str, Any]:
+    async def get_all_balances_by_main_account(self, main_account: str) -> List[Dict[str, Any]]:
         query = gql(
             """
             query GetAllBalancesByMainAccount($main: String!) {
                 getAllBalancesByMainAccount(main_account: $main) {
                     items {
                         a
                         f
                         r
                     }
                 }
             }
             """
         )
 
-        parameters = {"main": main_account}
+        parameters = {
+            "main": main_account,
+        }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return (await self._execute_query(
+            query=query,
+            parameters=parameters,
+            field_name="getAllBalancesByMainAccount",
+            throttler_limit_id=CONSTANTS.ALL_BALANCES_LIMIT_ID
+        ))["items"]
 
     async def get_order_fills_by_main_account(
-        self, from_timestamp: float, to_timestamp: float, main_account: str
-    ) -> Dict[str, Any]:
+        self,
+        from_timestamp: float,
+        to_timestamp: float,
+        main_account: str,
+    ) -> List[Dict[str, Any]]:
         query = gql(
             """
             query listTradesByMainAccount(
                 $main_account:String!
                 $limit: Int
                 $from: AWSDateTime!
                 $to: AWSDateTime!
@@ -256,63 +278,93 @@
                     to: $to
                     limit: $limit
                     nextToken: $nextToken
                 ) {
                     items {
                         isReverted
                         m
-                        m_id
+                        maker_id
                         p
                         q
                         stid
                         t
-                        t_id
+                        taker_id
                         trade_id
                     }
+                    nextToken
                 }
             }
             """
         )
 
         parameters = {
             "main_account": main_account,
             "from": self._timestamp_to_aws_datetime_string(timestamp=from_timestamp),
             "to": self._timestamp_to_aws_datetime_string(timestamp=to_timestamp),
         }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-
-        return result
+        return await self._query_all_pages(
+            query=query,
+            parameters=parameters,
+            field_name="listTradesByMainAccount",
+            throttler_limit_id=CONSTANTS.ALL_FILLS_LIMIT_ID
+        )
 
-    async def place_order(self, polkadex_order: Dict[str, Any], signature: Dict[str, Any]) -> Dict[str, Any]:
+    async def place_order(self, polkadex_order: Dict[str, Any], signature: Dict[str, Any]) -> Optional[str]:
+        """
+        :return: Exchange order ID in case of success, None otherwise
+        """
         query = gql(
             """
             mutation PlaceOrder($payload: String!) {
                 place_order(input: {payload: $payload})
             }
             """
         )
 
         input_parameters = [
             polkadex_order,
             signature,
         ]
-        parameters = {"payload": json.dumps({"PlaceOrder": input_parameters})}
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        parameters = {
+            "payload": json.dumps({"PlaceOrder": input_parameters}),
+        }
+
+        response = await self._execute_query(
+            query=query,
+            parameters=parameters,
+            field_name="place_order",
+            throttler_limit_id=CONSTANTS.PLACE_ORDER_LIMIT_ID
+        )
+
+        # TODO (dmitry): leave only one format once PolkaDEX team would apply the change on their end
+        # so currently the format is like
+        # {'place_order': '{"is_success":true,"body":"exchange order id here"}'}
+        # but the new format would be simple JSON
+        # {"place_order": {"is_success":true,"body":"exchange order id here"}}
+        # so currently we have to support both of them
+
+        if isinstance(response, str):
+            response = json.loads(response)
+
+        exchange_order_id = None
+        if response["is_success"]:
+            exchange_order_id = response["body"]
+
+        return exchange_order_id
 
     async def cancel_order(
         self,
         order_id: str,
         market_symbol: str,
         main_address: str,
         proxy_address: str,
         signature: Dict[str, Any],
-    ) -> Dict[str, Any]:
+    ) -> Optional[Dict[str, Any]]:
         query = gql(
             """
             mutation CancelOrder($payload: String!) {
                 cancel_order(input: {payload: $payload})
             }
             """
         )
@@ -320,103 +372,56 @@
         input_parameters = [
             order_id,
             main_address,
             proxy_address,
             market_symbol,
             signature,
         ]
-        parameters = {"payload": json.dumps({"CancelOrder": input_parameters})}
-
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
-
-    async def list_order_history_by_account(
-        self, main_account: str, from_time: float, to_time: float
-    ) -> Dict[str, Any]:
-        query = gql(
-            """
-            query ListOrderHistory(
-                $main_account:String!
-                $limit: Int
-                $from: AWSDateTime!
-                $to: AWSDateTime!
-                $nextToken: String
-            ) {
-                listOrderHistorybyMainAccount(
-                    main_account: $main_account
-                    from: $from
-                    to: $to
-                    limit: $limit
-                    nextToken: $nextToken
-                ) {
-                    items {
-                        u
-                        cid
-                        id
-                        t
-                        m
-                        s
-                        ot
-                        st
-                        p
-                        q
-                        afp
-                        fq
-                        fee
-                        isReverted
-                    }
-                }
-            }
-            """
-        )
 
         parameters = {
-            "main_account": main_account,
-            "to": self._timestamp_to_aws_datetime_string(timestamp=to_time),
-            "from": self._timestamp_to_aws_datetime_string(timestamp=from_time),
+            "payload": json.dumps({"CancelOrder": input_parameters}),
         }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        try:
+            return await self._execute_query(
+                query=query,
+                parameters=parameters,
+                field_name="cancel_order",
+                throttler_limit_id=CONSTANTS.CANCEL_ORDER_LIMIT_ID
+            )
+        except Exception:
+            self.logger().error(f"Failed to cancel order {order_id}; query parameters: {parameters}")
+            raise
 
-    async def find_order_by_main_account(self, main_account: str, market_symbol: str, order_id: str) -> Dict[str, Any]:
+    async def find_order_by_id(self, order_id: str) -> Dict[str, Any]:
         query = gql(
             """
-            query FindOrder($main_account: String!, $market: String!, $order_id: String!) {
-                findOrderByMainAccount(main_account: $main_account, market: $market, order_id: $order_id) {
-                    afp
-                    cid
-                    fee
+            query FindOrderById($order_id: String!) {
+                findOrderById(order_id: $order_id) {
                     fq
                     id
-                    isReverted
-                    m
-                    ot
-                    p
-                    q
-                    s
                     st
-                    stid
-                    t
-                    u
                 }
             }
-        """
+            """
         )
 
         parameters = {
-            "main_account": main_account,
-            "market": market_symbol,
             "order_id": order_id,
         }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return await self._execute_query(
+            query=query,
+            parameters=parameters,
+            field_name="findOrderById",
+            # TODO (dmitry): define separate limit
+            throttler_limit_id=CONSTANTS.ORDER_UPDATE_LIMIT_ID
+        )
 
-    async def list_open_orders_by_main_account(self, main_account: str) -> Dict[str, Any]:
+    async def list_open_orders_by_main_account(self, main_account: str) -> List[Dict[str, Any]]:
         query = gql(
             """
             query ListOpenOrdersByMainAccount($main_account: String!, $limit: Int, $nextToken: String) {
                 listOpenOrdersByMainAccount(main_account: $main_account, limit: $limit, nextToken: $nextToken) {
                     items {
                         u
                         cid
@@ -430,82 +435,164 @@
                         q
                         afp
                         fq
                         fee
                         stid
                         isReverted
                     }
+                    nextToken
                 }
             }
         """
         )
 
-        parameters = {"main_account": main_account}
+        parameters = {
+            "main_account": main_account,
+        }
 
-        result = await self._execute_query(query=query, parameters=parameters)
-        return result
+        return await self._query_all_pages(
+            query=query,
+            parameters=parameters,
+            field_name="listOpenOrdersByMainAccount",
+            throttler_limit_id=CONSTANTS.LIST_OPEN_ORDERS_LIMIT_ID
+        )
 
     async def listen_to_orderbook_updates(self, events_handler: Callable, market_symbol: str):
         while True:
             try:
                 stream_name = f"{market_symbol}-{CONSTANTS.ORDERBOOK_UPDATES_STREAM_NAME}"
                 async for event in self._subscribe_to_stream(stream_name=stream_name):
                     events_handler(event=event, market_symbol=market_symbol)
             except asyncio.CancelledError:
                 raise
-            except Exception:
-                self.logger().error("Unexpected error listening to order book updates from Polkadex", exc_info=True)
+            except Exception as e:
+                self.logger().error(
+                    f"Unexpected error listening to order book updates from Polkadex. Error: {e}",
+                    exc_info=True
+                )
+                sys.exit()
+                # TODO (dmitry): add proper handling of exceptions to all WS listeners
+                # await self.websocket_connect_failure()
+
+    async def websocket_connect_failure(self):
+        self.logger().info(f"Websocket connect failure.{self._websocket_failure}")
+        if self._websocket_failure:
+            if abs(self._websocket_failure_timestamp - datetime.utcnow().timestamp()) > float(10):
+                self._restart_initialization = True
+        else:
+            await self.set_websocket_failure_timestamp()
+
+    async def set_websocket_failure_timestamp(self):
+        self._websocket_failure_timestamp = datetime.utcnow().timestamp()
+        self._websocket_failure = True
 
     async def listen_to_public_trades(self, events_handler: Callable, market_symbol: str):
         while True:
             try:
                 stream_name = f"{market_symbol}-{CONSTANTS.RECENT_TRADES_STREAM_NAME}"
                 async for event in self._subscribe_to_stream(stream_name=stream_name):
                     events_handler(event=event)
             except asyncio.CancelledError:
                 raise
-            except Exception:
-                self.logger().error("Unexpected error listening to public trades from Polkadex", exc_info=True)
+            except Exception as e:
+                self.logger().error(
+                    f"Unexpected error listening to public trades from Polkadex. Error: {e}",
+                    exc_info=True
+                )
+                sys.exit()
+                await self.websocket_connect_failure()
 
     async def listen_to_private_events(self, events_handler: Callable, address: str):
         while True:
             try:
                 async for event in self._subscribe_to_stream(stream_name=address):
                     events_handler(event=event)
             except asyncio.CancelledError:
                 raise
-            except Exception:
-                self.logger().error("Unexpected error listening to private updates from Polkadex", exc_info=True)
+            except Exception as e:
+                self.logger().error(
+                    f"Unexpected error listening to private updates from Polkadex. Error: {e}",
+                    exc_info=True
+                )
+                sys.exit()
 
     async def _execute_query(
         self,
         query: DocumentNode,
-        parameters: Optional[Dict[str, Any]] = None,
+        parameters: Optional[Dict[str, Any]],
+        field_name: str,
+        throttler_limit_id: str
     ):
-        # Extract host from url
-        url = CONSTANTS.GRAPHQL_ENDPOINTS[self._domain]
+        async with self._throttler.execute_task(limit_id=throttler_limit_id):
+            url = CONSTANTS.GRAPHQL_ENDPOINTS[self._domain]
 
-        transport = AIOHTTPTransport(url=url, auth=self._auth)
-        async with Client(transport=transport, fetch_schema_from_transport=False) as session:
-            result = await session.execute(query, variable_values=parameters, parse_result=True)
+            transport = AIOHTTPTransport(url=url, auth=self._auth)
+            async with Client(transport=transport, fetch_schema_from_transport=False) as session:
+                result = await session.execute(query, variable_values=parameters, parse_result=True)
 
-        return result
+            return result[field_name]
 
     async def _subscribe_to_stream(self, stream_name: str) -> AsyncIterable:
         query = gql(
             """
             subscription WebsocketStreamsMessage($name: String!) {
                 websocket_streams(name: $name) {
                     data
                 }
             }
             """
         )
         variables = {"name": stream_name}
 
-        async for result in self._ws_session.subscribe(query, variable_values=variables, parse_result=True):
-            yield result
+        url = CONSTANTS.GRAPHQL_WS_ENDPOINTS[self._domain]
+        transport = AppSyncWebsocketsTransport(url=url, auth=self._auth)
+
+        async with Client(transport=transport, fetch_schema_from_transport=False) as session:
+            async for result in session.subscribe(query, variable_values=variables, parse_result=True):
+                yield result
 
     @staticmethod
     def _timestamp_to_aws_datetime_string(timestamp: float) -> str:
         timestamp_string = datetime.utcfromtimestamp(timestamp).isoformat(timespec="milliseconds") + "Z"
         return timestamp_string
+
+    async def _query_all_pages(
+        self,
+        query: DocumentNode,
+        parameters: Optional[Dict[str, Any]],
+        field_name: str,
+        throttler_limit_id: str,
+        limit: int = 300
+    ) -> List[Dict[str, Any]]:
+        """
+        Most of the PolkaDEX API endpoints return paginated result. The pagination mechanism is based on two parameters:
+        `limit` and `nextToken`. First one is used to limit the number of entries on a page, the second one identifies
+        the next page. This function iterates through all the pages to get 100% of data.
+
+        IMPORTANT considerations:
+
+        * by default we set the page size to 300 entries, but in most of the cases PolkaDEX APIs will limit response
+        body size to 1MB
+
+        :param query: GraphQL query
+        :param parameters: query parameters
+        :param field_name: name of GraphQL field
+        :param throttler_limit_id: the string identifier for a throttling limit
+        :param limit: page size
+        """
+        if parameters is None:
+            parameters = {}
+
+        parameters["limit"] = limit
+
+        # execute first query and get nextToken from the response
+        data = await self._execute_query(query, parameters, field_name, throttler_limit_id)
+        items = data["items"]
+        next_token = data["nextToken"]
+
+        while next_token:
+            parameters["nextToken"] = next_token
+            data = await self._execute_query(query, parameters, field_name, throttler_limit_id)
+            items += data["items"]
+            next_token = data["nextToken"]
+
+        return items
```

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/polkadex/polkadex_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/polkadex/polkadex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/dummy.cpp` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_auth.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_constants.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_eip712_structs.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_exchange.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_order_book.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_order_book.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange/vertex/vertex_web_utils.py` & `hummingbot-20240520/hummingbot/connector/exchange/vertex/vertex_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange_base.cpp` & `hummingbot-20240520/hummingbot/connector/exchange_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/exchange_py_base.py` & `hummingbot-20240520/hummingbot/connector/exchange_py_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_algorand_amm.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_algorand_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_evm_amm.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_evm_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_near_amm.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_near_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm/gateway_tezos_amm.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm/gateway_tezos_amm.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm_lp/gateway_evm_amm_lp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm_lp/gateway_in_flight_lp_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm_lp/gateway_osmosis_amm_lp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py` & `hummingbot-20240520/hummingbot/connector/gateway/amm_perpetual/gateway_evm_amm_perpetual.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_perp/data_sources/clob_perp_api_data_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_perp/gateway_clob_perp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_perp/gateway_clob_perp_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/clob_api_data_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_api_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/dexalot/dexalot_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/gateway_clob_api_data_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_api_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_helpers.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/kujira/kujira_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_api_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/data_sources/xrpl/xrpl_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/gateway_clob_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py` & `hummingbot-20240520/hummingbot/connector/gateway/clob_spot/gateway_clob_spot.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/common_types.py` & `hummingbot-20240520/hummingbot/connector/gateway/common_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/gateway_in_flight_order.py` & `hummingbot-20240520/hummingbot/connector/gateway/gateway_in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/gateway_order_tracker.py` & `hummingbot-20240520/hummingbot/connector/gateway/gateway_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/gateway/gateway_price_shim.py` & `hummingbot-20240520/hummingbot/connector/gateway/gateway_price_shim.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/in_flight_order_base.cpp` & `hummingbot-20240520/hummingbot/connector/in_flight_order_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/markets_recorder.py` & `hummingbot-20240520/hummingbot/connector/markets_recorder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/parrot.py` & `hummingbot-20240520/hummingbot/connector/parrot.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/perpetual_derivative_py_base.py` & `hummingbot-20240520/hummingbot/connector/perpetual_derivative_py_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/perpetual_trading.py` & `hummingbot-20240520/hummingbot/connector/perpetual_trading.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/exchange_connector_test.py` & `hummingbot-20240520/hummingbot/connector/test_support/exchange_connector_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py` & `hummingbot-20240520/hummingbot/connector/test_support/gateway_clob_api_data_source_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/mock_order_tracker.py` & `hummingbot-20240520/hummingbot/connector/test_support/mock_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/mock_paper_exchange.cpp` & `hummingbot-20240520/hummingbot/connector/test_support/mock_paper_exchange.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/network_mocking_assistant.py` & `hummingbot-20240520/hummingbot/connector/test_support/network_mocking_assistant.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/oms_exchange_connector_test.py` & `hummingbot-20240520/hummingbot/connector/test_support/oms_exchange_connector_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/test_support/perpetual_derivative_test.py` & `hummingbot-20240520/hummingbot/connector/test_support/perpetual_derivative_test.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/time_synchronizer.py` & `hummingbot-20240520/hummingbot/connector/time_synchronizer.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/trading_rule.cpp` & `hummingbot-20240520/hummingbot/connector/trading_rule.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_api_user_stream_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_exchange.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py` & `hummingbot-20240520/hummingbot/connector/utilities/oms_connector/oms_connector_web_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/connector/utils.py` & `hummingbot-20240520/hummingbot/connector/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/api_throttler/async_request_context_base.py` & `hummingbot-20240520/hummingbot/core/api_throttler/async_request_context_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/api_throttler/async_throttler.py` & `hummingbot-20240520/hummingbot/core/api_throttler/async_throttler.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/api_throttler/async_throttler_base.py` & `hummingbot-20240520/hummingbot/core/api_throttler/async_throttler_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/api_throttler/data_types.py` & `hummingbot-20240520/hummingbot/core/api_throttler/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/clock.cpp` & `hummingbot-20240520/hummingbot/core/clock.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/LimitOrder.cpp` & `hummingbot-20240520/hummingbot/core/cpp/LimitOrder.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/LimitOrder.h` & `hummingbot-20240520/hummingbot/core/cpp/LimitOrder.h`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/OrderBookEntry.cpp` & `hummingbot-20240520/hummingbot/core/cpp/OrderBookEntry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/OrderBookEntry.h` & `hummingbot-20240520/hummingbot/core/cpp/OrderBookEntry.h`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/OrderExpirationEntry.cpp` & `hummingbot-20240520/hummingbot/core/cpp/OrderExpirationEntry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/OrderExpirationEntry.h` & `hummingbot-20240520/hummingbot/core/cpp/OrderExpirationEntry.h`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/PyRef.cpp` & `hummingbot-20240520/hummingbot/core/cpp/PyRef.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/cpp/TestOrderBookEntry.cpp` & `hummingbot-20240520/hummingbot/core/cpp/TestOrderBookEntry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/common.py` & `hummingbot-20240520/hummingbot/core/data_type/common.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/composite_order_book.cpp` & `hummingbot-20240520/hummingbot/core/data_type/composite_order_book.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.core.data_type.composite_order_book",
         "sources": [
             "hummingbot/core/data_type/composite_order_book.pyx",
             "hummingbot/core/cpp/OrderBookEntry.cpp"
         ]
```

### Comparing `hummingbot-20240429/hummingbot/core/data_type/funding_info.py` & `hummingbot-20240520/hummingbot/core/data_type/funding_info.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/in_flight_order.py` & `hummingbot-20240520/hummingbot/core/data_type/in_flight_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/limit_order.cpp` & `hummingbot-20240520/hummingbot/core/data_type/limit_order.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/market_order.py` & `hummingbot-20240520/hummingbot/core/data_type/market_order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book.cpp` & `hummingbot-20240520/hummingbot/core/data_type/order_book.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.core.data_type.order_book",
         "sources": [
             "hummingbot/core/data_type/order_book.pyx",
             "hummingbot/core/cpp/OrderBookEntry.cpp"
         ]
```

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book_message.py` & `hummingbot-20240520/hummingbot/core/data_type/order_book_message.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book_query_result.cpp` & `hummingbot-20240520/hummingbot/core/data_type/order_book_query_result.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book_row.py` & `hummingbot-20240520/hummingbot/core/data_type/order_book_row.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book_tracker.py` & `hummingbot-20240520/hummingbot/core/data_type/order_book_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book_tracker_data_source.py` & `hummingbot-20240520/hummingbot/core/data_type/order_book_tracker_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_book_tracker_entry.py` & `hummingbot-20240520/hummingbot/core/data_type/order_book_tracker_entry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_candidate.py` & `hummingbot-20240520/hummingbot/core/data_type/order_candidate.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/order_expiration_entry.cpp` & `hummingbot-20240520/hummingbot/core/data_type/order_expiration_entry.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/perpetual_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/core/data_type/perpetual_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/remote_api_order_book_data_source.py` & `hummingbot-20240520/hummingbot/core/data_type/remote_api_order_book_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/trade.py` & `hummingbot-20240520/hummingbot/core/data_type/trade.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/trade_fee.py` & `hummingbot-20240520/hummingbot/core/data_type/trade_fee.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/transaction_tracker.cpp` & `hummingbot-20240520/hummingbot/core/data_type/transaction_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/user_stream_tracker.py` & `hummingbot-20240520/hummingbot/core/data_type/user_stream_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/data_type/user_stream_tracker_data_source.py` & `hummingbot-20240520/hummingbot/core/data_type/user_stream_tracker_data_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/event/event_forwarder.py` & `hummingbot-20240520/hummingbot/core/event/event_forwarder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/event/event_listener.cpp` & `hummingbot-20240520/hummingbot/core/event/event_listener.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/event/event_logger.cpp` & `hummingbot-20240520/hummingbot/core/event/event_logger.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/event/event_reporter.cpp` & `hummingbot-20240520/hummingbot/core/event/event_reporter.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/event/events.py` & `hummingbot-20240520/hummingbot/core/event/events.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/gateway/__init__.py` & `hummingbot-20240520/hummingbot/core/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/gateway/gateway_http_client.py` & `hummingbot-20240520/hummingbot/core/gateway/gateway_http_client.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/gateway/gateway_status_monitor.py` & `hummingbot-20240520/hummingbot/core/gateway/gateway_status_monitor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/gateway/utils.py` & `hummingbot-20240520/hummingbot/core/gateway/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/management/console.py` & `hummingbot-20240520/hummingbot/core/management/console.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/management/diagnosis.py` & `hummingbot-20240520/hummingbot/core/management/diagnosis.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/mock_api/mock_mqtt_server.py` & `hummingbot-20240520/hummingbot/core/mock_api/mock_mqtt_server.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/mock_api/mock_web_server.py` & `hummingbot-20240520/hummingbot/core/mock_api/mock_web_server.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/mock_api/mock_web_socket_server.py` & `hummingbot-20240520/hummingbot/core/mock_api/mock_web_socket_server.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/network_base.py` & `hummingbot-20240520/hummingbot/core/network_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/network_iterator.cpp` & `hummingbot-20240520/hummingbot/core/network_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/pubsub.cpp` & `hummingbot-20240520/hummingbot/core/pubsub.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/py_time_iterator.cpp` & `hummingbot-20240520/hummingbot/core/py_time_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/rate_oracle.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/rate_oracle.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/ascend_ex_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/binance_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/binance_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/binance_us_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/coin_cap_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/coin_gecko_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/coinbase_advanced_trade_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/cube_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/cube_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/gate_io_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/kucoin_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/sources/rate_source_base.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/sources/rate_source_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/rate_oracle/utils.py` & `hummingbot-20240520/hummingbot/core/rate_oracle/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/time_iterator.cpp` & `hummingbot-20240520/hummingbot/core/time_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/__init__.py` & `hummingbot-20240520/hummingbot/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/async_call_scheduler.py` & `hummingbot-20240520/hummingbot/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/async_retry.py` & `hummingbot-20240520/hummingbot/core/utils/async_retry.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/async_utils.py` & `hummingbot-20240520/hummingbot/core/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/estimate_fee.py` & `hummingbot-20240520/hummingbot/core/utils/estimate_fee.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/fixed_rate_source.py` & `hummingbot-20240520/hummingbot/core/utils/fixed_rate_source.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/gateway_config_utils.py` & `hummingbot-20240520/hummingbot/core/utils/gateway_config_utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/kill_switch.py` & `hummingbot-20240520/hummingbot/core/utils/kill_switch.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/market_price.py` & `hummingbot-20240520/hummingbot/core/utils/market_price.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/ssl_cert.py` & `hummingbot-20240520/hummingbot/core/utils/ssl_cert.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/ssl_client_request.py` & `hummingbot-20240520/hummingbot/core/utils/ssl_client_request.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/tracking_nonce.py` & `hummingbot-20240520/hummingbot/core/utils/tracking_nonce.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/utils/trading_pair_fetcher.py` & `hummingbot-20240520/hummingbot/core/utils/trading_pair_fetcher.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/auth.py` & `hummingbot-20240520/hummingbot/core/web_assistant/auth.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/connections/connections_factory.py` & `hummingbot-20240520/hummingbot/core/web_assistant/connections/connections_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/connections/data_types.py` & `hummingbot-20240520/hummingbot/core/web_assistant/connections/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/connections/rest_connection.py` & `hummingbot-20240520/hummingbot/core/web_assistant/connections/rest_connection.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/connections/ws_connection.py` & `hummingbot-20240520/hummingbot/core/web_assistant/connections/ws_connection.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/rest_assistant.py` & `hummingbot-20240520/hummingbot/core/web_assistant/rest_assistant.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/web_assistants_factory.py` & `hummingbot-20240520/hummingbot/core/web_assistant/web_assistants_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/core/web_assistant/ws_assistant.py` & `hummingbot-20240520/hummingbot/core/web_assistant/ws_assistant.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/amm_gateway_data_feed.py` & `hummingbot-20240520/hummingbot/data_feed/amm_gateway_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/ascend_ex_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/ascend_ex_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_perpetual_candles/binance_perpetual_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_perpetual_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_spot_candles/binance_spot_candles.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,23 +78,23 @@
         return np.array(candles)[:, [0, 1, 2, 3, 4, 5, 7, 8, 9, 10]].astype(float)
 
     async def fill_historical_candles(self):
         max_request_needed = (self._candles.maxlen // 1000) + 1
         requests_executed = 0
         while not self.ready:
             missing_records = self._candles.maxlen - len(self._candles)
-            end_timestamp = int(self._candles[0][0])
+            end_timestamp = int(self._candles[-1][0])
             try:
                 if requests_executed < max_request_needed:
                     # we have to add one more since, the last row is not going to be included
                     candles = await self.fetch_candles(end_time=end_timestamp, limit=missing_records + 1)
                     # we are computing again the quantity of records again since the websocket process is able to
                     # modify the deque and if we extend it, the new observations are going to be dropped.
                     missing_records = self._candles.maxlen - len(self._candles)
-                    self._candles.extendleft(candles[-(missing_records + 1):-1][::-1])
+                    self._candles.extendleft(candles[-(missing_records + 1):-1])
                     requests_executed += 1
                 else:
                     self.logger().error(f"There is no data available for the quantity of "
                                         f"candles requested for {self.name}.")
                     raise
             except asyncio.CancelledError:
                 raise
```

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/binance_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/candles_base.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/candles_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/candles_factory.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/candles_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from hummingbot.data_feed.candles_feed.candles_base import CandlesBase
 from hummingbot.data_feed.candles_feed.data_types import CandlesConfig
 from hummingbot.data_feed.candles_feed.gate_io_perpetual_candles import GateioPerpetualCandles
 from hummingbot.data_feed.candles_feed.gate_io_spot_candles import GateioSpotCandles
 from hummingbot.data_feed.candles_feed.kraken_spot_candles.kraken_spot_candles import KrakenSpotCandles
 from hummingbot.data_feed.candles_feed.kucoin_spot_candles.kucoin_spot_candles import KucoinSpotCandles
 from hummingbot.data_feed.candles_feed.okx_perpetual_candles.okx_perpetual_candles import OKXPerpetualCandles
+from hummingbot.data_feed.candles_feed.okx_spot_candles.okx_spot_candles import OKXSpotCandles
 
 
 class UnsupportedConnectorException(Exception):
     """
     Exception raised when an unsupported connector is requested.
     """
     def __init__(self, connector: str):
@@ -30,14 +31,15 @@
         "binance_perpetual": BinancePerpetualCandles,
         "binance": BinanceSpotCandles,
         "gate_io": GateioSpotCandles,
         "gate_io_perpetual": GateioPerpetualCandles,
         "kucoin": KucoinSpotCandles,
         "ascend_ex": AscendExSpotCandles,
         "okx_perpetual": OKXPerpetualCandles,
+        "okx": OKXSpotCandles,
         "kraken": KrakenSpotCandles
     }
 
     @classmethod
     def get_candle(cls, candles_config: CandlesConfig) -> CandlesBase:
         """
         Returns a Candle object based on the specified configuration.
```

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/data_types.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_perpetual_candles/gate_io_perpetual_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/gate_io_spot_candles/gate_io_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/kraken_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     @property
     def intervals(self):
         return CONSTANTS.INTERVALS
 
     @property
     def candles_df(self) -> pd.DataFrame:
         df = pd.DataFrame(self._candles, columns=self.columns, dtype=float)
-        df["timestamp"] = df["timestamp"] * 1000
         return df.sort_values(by="timestamp", ascending=True)
 
     async def check_network(self) -> NetworkStatus:
         rest_assistant = await self._api_factory.get_rest_assistant()
         await rest_assistant.execute_request(url=self.health_check_url,
                                              throttler_limit_id=CONSTANTS.HEALTH_CHECK_ENDPOINT)
         return NetworkStatus.CONNECTED
@@ -79,38 +78,42 @@
     async def fetch_candles(self,
                             start_time: Optional[int] = None,
                             end_time: Optional[int] = None,
                             limit: Optional[int] = 1500):
         rest_assistant = await self._api_factory.get_rest_assistant()
         params = {"symbol": self._ex_trading_pair, "type": CONSTANTS.INTERVALS[self.interval]}
         if start_time:
-            params["startAt"] = start_time
+            params["startAt"] = start_time // 1000
         if end_time:
-            params["endAt"] = end_time
+            params["endAt"] = end_time // 1000
+        else:
+            params["endAt"] = start_time // 1000 + (limit * self.get_seconds_from_interval(self.interval))
+
         candles = await rest_assistant.execute_request(url=self.candles_url,
                                                        throttler_limit_id=CONSTANTS.CANDLES_ENDPOINT,
                                                        params=params)
-        arr = [[row[0], row[1], row[3], row[4], row[2], row[5], row[6]] for row in candles['data']]
-        return np.array(arr).astype(float)
+        candles = np.array([[row[0], row[1], row[3], row[4], row[2], row[5], row[6], 0., 0., 0.] for row in candles['data']]).astype(float)
+        candles[:, 0] = candles[:, 0] * 1000
+        return candles[::-1]
 
     async def fill_historical_candles(self):
         max_request_needed = (self._candles.maxlen // 1500) + 1
         requests_executed = 0
         while not self.ready:
             # missing_records = self._candles.maxlen - len(self._candles)
             try:
                 if requests_executed < max_request_needed:
-                    end_timestamp = int(self._candles[0][0] + 1)
+                    end_timestamp = int(self._candles[-1][0] + 1000)
                     # we have to add one more since, the last row is not going to be included
-                    start_time = end_timestamp - (1500 * self.get_seconds_from_interval(self.interval)) + 1
-                    candles = await self.fetch_candles(end_time=end_timestamp, start_time=start_time)
+                    start_time = (end_timestamp - (1500 * self.get_seconds_from_interval(self.interval)) * 1000) + 1000
+                    candles = await self.fetch_candles(end_time=end_timestamp, start_time=start_time, limit=1500)
                     # we are computing agaefin the quantity of records again since the websocket process is able to
                     # modify the deque and if we extend it, the new observations are going to be dropped.
                     missing_records = self._candles.maxlen - len(self._candles)
-                    self._candles.extendleft(candles[::-1][-(missing_records + 1):-1])
+                    self._candles.extendleft(candles[-(missing_records + 1):-1])
                     requests_executed += 1
                 else:
                     self.logger().error(f"There is no data available for the quantity of "
                                         f"candles requested for {self.name}.")
                     raise
             except asyncio.CancelledError:
                 raise
@@ -163,15 +166,15 @@
 
     async def _process_websocket_messages_from_candles(self, websocket_assistant: WSAssistant):
         async for ws_response in websocket_assistant.iter_messages():
             data: Dict[str, Any] = ws_response.data
             if data is not None and data.get(
                     "subject") == "trade.candles.update":  # data will be None when the websocket is disconnected
                 candles = data["data"]["candles"]
-                timestamp = float(candles[0])
+                timestamp = int(candles[0]) * 1000
                 open = candles[1]
                 close = candles[2]
                 high = candles[3]
                 low = candles[4]
                 volume = candles[5]
                 quote_asset_volume = candles[6]
                 n_trades = 0.
```

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py` & `hummingbot-20240520/hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import logging
 from typing import Any, Dict, Optional
 
 import numpy as np
+import pandas as pd
 
 from hummingbot.core.network_iterator import NetworkStatus, safe_ensure_future
 from hummingbot.core.web_assistant.connections.data_types import WSJSONRequest
 from hummingbot.core.web_assistant.ws_assistant import WSAssistant
 from hummingbot.data_feed.candles_feed.candles_base import CandlesBase
+from hummingbot.data_feed.candles_feed.data_types import HistoricalCandlesConfig
 from hummingbot.data_feed.candles_feed.okx_perpetual_candles import constants as CONSTANTS
 from hummingbot.logger import HummingbotLogger
 
 
 class OKXPerpetualCandles(CandlesBase):
     _logger: Optional[HummingbotLogger] = None
 
@@ -20,14 +22,33 @@
         if cls._logger is None:
             cls._logger = logging.getLogger(__name__)
         return cls._logger
 
     def __init__(self, trading_pair: str, interval: str = "1m",
                  max_records: int = CONSTANTS.MAX_RESULTS_PER_CANDLESTICK_REST_REQUEST):
         super().__init__(trading_pair, interval, max_records)
+        self.interval_to_milliseconds_dict = {
+            "1s": 1000,
+            "1m": 60000,
+            "3m": 180000,
+            "5m": 300000,
+            "15m": 900000,
+            "30m": 1800000,
+            "1h": 3600000,
+            "2h": 7200000,
+            "4h": 14400000,
+            "6h": 21600000,
+            "8h": 28800000,
+            "12h": 43200000,
+            "1d": 86400000,
+            "3d": 259200000,
+            "1w": 604800000,
+            "1M": 2592000000,
+            "3M": 7776000000
+        }
 
     @property
     def name(self):
         return f"okx_perpetual_{self._trading_pair}"
 
     @property
     def rest_url(self):
@@ -102,14 +123,35 @@
                 raise
             except Exception:
                 self.logger().exception(
                     "Unexpected error occurred when getting historical klines. Retrying in 1 seconds...",
                 )
                 await self._sleep(1.0)
 
+    async def get_historical_candles(self, config: HistoricalCandlesConfig):
+        try:
+            all_candles = []
+            current_start_time = config.start_time
+            while current_start_time <= config.end_time:
+                current_end_time = current_start_time + self.interval_to_milliseconds_dict[config.interval] * CONSTANTS.MAX_RESULTS_PER_CANDLESTICK_REST_REQUEST
+                fetched_candles = await self.fetch_candles(end_time=current_end_time)
+                if fetched_candles.size == 0:
+                    break
+
+                all_candles.append(fetched_candles[::-1])
+                last_timestamp = fetched_candles[0][0]  # Assuming the first column is the timestamp
+                current_start_time = int(last_timestamp)
+
+            final_candles = np.concatenate(all_candles, axis=0) if all_candles else np.array([])
+            candles_df = pd.DataFrame(final_candles, columns=self.columns)
+            candles_df.drop_duplicates(subset=["timestamp"], inplace=True)
+            return candles_df
+        except Exception as e:
+            self.logger().exception(f"Error fetching historical candles: {str(e)}")
+
     async def _subscribe_channels(self, ws: WSAssistant):
         """
         Subscribes to the candles events through the provided websocket connection.
         :param ws: the websocket assistant used to connect to the exchange
         """
         try:
             candle_args = []
```

### Comparing `hummingbot-20240429/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py` & `hummingbot-20240520/hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py` & `hummingbot-20240520/hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py` & `hummingbot-20240520/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py` & `hummingbot-20240520/hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/custom_api_data_feed.py` & `hummingbot-20240520/hummingbot/data_feed/custom_api_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/data_feed_base.py` & `hummingbot-20240520/hummingbot/data_feed/data_feed_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py` & `hummingbot-20240520/hummingbot/data_feed/liquidations_feed/binance/binance_liquidations.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from bidict import bidict
 
 from hummingbot.connector.utils import combine_to_hb_trading_pair
 from hummingbot.core.network_iterator import NetworkStatus
 from hummingbot.core.web_assistant.connections.data_types import WSJSONRequest
 from hummingbot.core.web_assistant.ws_assistant import WSAssistant
 from hummingbot.data_feed.liquidations_feed.binance import constants as CONSTANTS
-from hummingbot.data_feed.liquidations_feed.liquidations_base import Liquidation, LiquidationsBase
+from hummingbot.data_feed.liquidations_feed.liquidations_base import Liquidation, LiquidationsBase, LiquidationSide
 from hummingbot.logger import HummingbotLogger
 
 
 class BinancePerpetualLiquidations(LiquidationsBase):
     _logger: Optional[HummingbotLogger] = None
 
     @classmethod
@@ -153,16 +153,20 @@
         async for ws_response in websocket_assistant.iter_messages():
             data: Dict[str, Any] = ws_response.data
             if data.get("e") == "forceOrder":
                 timestamp = int(data["o"]["T"])
                 trading_pair = self._trading_pairs_map.get(data["o"]["s"])
                 quantity = float(data["o"]["q"])
                 price = float(data["o"]["ap"])
+                side = data["o"]["S"]
+                # SELL-Side means here, that a long position was forcefully liquidated and the other way round
+                liquidation_side = LiquidationSide.LONG if side == "SELL" else LiquidationSide.SHORT
 
                 if trading_pair not in self._liquidations:
                     self._liquidations[trading_pair] = []
 
                 self._liquidations[trading_pair].append(Liquidation(
                     timestamp=timestamp,
                     trading_pair=trading_pair,
                     quantity=quantity,
-                    price=price))
+                    price=price,
+                    side=liquidation_side))
```

### Comparing `hummingbot-20240429/hummingbot/data_feed/liquidations_feed/binance/constants.py` & `hummingbot-20240520/hummingbot/data_feed/liquidations_feed/binance/constants.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/liquidations_feed/liquidations_base.py` & `hummingbot-20240520/hummingbot/data_feed/liquidations_feed/liquidations_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import asyncio
 import time
 from dataclasses import dataclass, fields
+from enum import Enum
 from typing import Optional, Set
 
 import pandas as pd
 from bidict import bidict
 from pandas import DataFrame
 
 from hummingbot.core.api_throttler.async_throttler import AsyncThrottler
 from hummingbot.core.network_base import NetworkBase
 from hummingbot.core.network_iterator import NetworkStatus
 from hummingbot.core.utils.async_utils import safe_ensure_future
 from hummingbot.core.web_assistant.web_assistants_factory import WebAssistantsFactory
 from hummingbot.core.web_assistant.ws_assistant import WSAssistant
 
 
+class LiquidationSide(Enum):
+    SHORT = "SHORT"  # Short position got liquidated (=> price went long)
+    LONG = "LONG"  # Long position got liquidated (=> price went short)
+
+    def __str__(self):
+        return '%s' % self.value
+
+
 @dataclass
 class Liquidation:
     """
     Represents the information of a single liquidation
     """
     timestamp: int
     trading_pair: str
     quantity: float
     price: float
+    side: LiquidationSide
 
 
 class LiquidationsBase(NetworkBase):
     """
     This class serves as a base class for fetching and storing liquidation data from crypto exchanges. The storage
     is done in a time based manner - meaning an aggregation happens and you can decide how much history you wanto to keep.
     The class uses the WS Assistants for all the IO operations,
```

### Comparing `hummingbot-20240429/hummingbot/data_feed/liquidations_feed/liquidations_factory.py` & `hummingbot-20240520/hummingbot/data_feed/liquidations_feed/liquidations_factory.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/market_data_provider.py` & `hummingbot-20240520/hummingbot/data_feed/market_data_provider.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/data_feed/wallet_tracker_data_feed.py` & `hummingbot-20240520/hummingbot/data_feed/wallet_tracker_data_feed.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/exceptions.py` & `hummingbot-20240520/hummingbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/logger/__init__.py` & `hummingbot-20240520/hummingbot/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/logger/application_warning.py` & `hummingbot-20240520/hummingbot/logger/application_warning.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/logger/cli_handler.py` & `hummingbot-20240520/hummingbot/logger/cli_handler.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/logger/log_server_client.py` & `hummingbot-20240520/hummingbot/logger/log_server_client.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/logger/logger.py` & `hummingbot-20240520/hummingbot/logger/logger.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/logger/struct_logger.py` & `hummingbot-20240520/hummingbot/logger/struct_logger.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/__init__.py` & `hummingbot-20240520/hummingbot/model/__init__.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/db_migration/base_transformation.py` & `hummingbot-20240520/hummingbot/model/db_migration/base_transformation.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/db_migration/migrator.py` & `hummingbot-20240520/hummingbot/model/db_migration/migrator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/db_migration/transformations.py` & `hummingbot-20240520/hummingbot/model/db_migration/transformations.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/decimal_type_decorator.py` & `hummingbot-20240520/hummingbot/model/decimal_type_decorator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/executors.py` & `hummingbot-20240520/hummingbot/model/executors.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/funding_payment.py` & `hummingbot-20240520/hummingbot/model/funding_payment.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/inventory_cost.py` & `hummingbot-20240520/hummingbot/model/inventory_cost.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/market_data.py` & `hummingbot-20240520/hummingbot/model/market_data.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/market_state.py` & `hummingbot-20240520/hummingbot/model/market_state.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/order.py` & `hummingbot-20240520/hummingbot/model/order.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/order_status.py` & `hummingbot-20240520/hummingbot/model/order_status.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/range_position_collected_fees.py` & `hummingbot-20240520/hummingbot/model/range_position_collected_fees.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/range_position_update.py` & `hummingbot-20240520/hummingbot/model/range_position_update.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/sql_connection_manager.py` & `hummingbot-20240520/hummingbot/model/sql_connection_manager.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/trade_fill.py` & `hummingbot-20240520/hummingbot/model/trade_fill.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/model/transaction_base.py` & `hummingbot-20240520/hummingbot/model/transaction_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/notifier/telegram_notifier.py` & `hummingbot-20240520/hummingbot/notifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/pmm_script/pmm_script_base.py` & `hummingbot-20240520/hummingbot/pmm_script/pmm_script_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/pmm_script/pmm_script_interface.py` & `hummingbot-20240520/hummingbot/pmm_script/pmm_script_interface.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/pmm_script/pmm_script_iterator.cpp` & `hummingbot-20240520/hummingbot/pmm_script/pmm_script_iterator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/pmm_script/pmm_script_process.py` & `hummingbot-20240520/hummingbot/pmm_script/pmm_script_process.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/remote_iface/messages.py` & `hummingbot-20240520/hummingbot/remote_iface/messages.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/remote_iface/mqtt.py` & `hummingbot-20240520/hummingbot/remote_iface/mqtt.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/__utils__/ring_buffer.cpp` & `hummingbot-20240520/hummingbot/strategy/__utils__/ring_buffer.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py` & `hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/base_trailing_indicator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py` & `hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py` & `hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/historical_volatility.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py` & `hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/instant_volatility.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp` & `hummingbot-20240520/hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/OrderBookEntry.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core",
-            "hummingbot/core/data_type"
+            "hummingbot/core/data_type",
+            "hummingbot/core"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.__utils__.trailing_indicators.trading_intensity",
         "sources": [
             "hummingbot/strategy/__utils__/trailing_indicators/trading_intensity.pyx",
             "hummingbot/core/cpp/OrderBookEntry.cpp"
         ]
```

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_arb/amm_arb.py` & `hummingbot-20240520/hummingbot/strategy/amm_arb/amm_arb.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_arb/amm_arb_config_map.py` & `hummingbot-20240520/hummingbot/strategy/amm_arb/amm_arb_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_arb/data_types.py` & `hummingbot-20240520/hummingbot/strategy/amm_arb/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_arb/dummy.cpp` & `hummingbot-20240520/hummingbot/strategy/amm_arb/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_arb/start.py` & `hummingbot-20240520/hummingbot/strategy/amm_arb/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_arb/utils.py` & `hummingbot-20240520/hummingbot/strategy/amm_arb/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py` & `hummingbot-20240520/hummingbot/strategy/amm_v3_lp/amm_v3_lp.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py` & `hummingbot-20240520/hummingbot/strategy/amm_v3_lp/amm_v3_lp_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/amm_v3_lp/start.py` & `hummingbot-20240520/hummingbot/strategy/amm_v3_lp/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/api_asset_price_delegate.cpp` & `hummingbot-20240520/hummingbot/strategy/api_asset_price_delegate.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/asset_price_delegate.cpp` & `hummingbot-20240520/hummingbot/strategy/asset_price_delegate.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp` & `hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py` & `hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/avellaneda_market_making_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/avellaneda_market_making/start.py` & `hummingbot-20240520/hummingbot/strategy/avellaneda_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/conditional_execution_state.py` & `hummingbot-20240520/hummingbot/strategy/conditional_execution_state.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/cross_exchange_market_making_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/order_id_market_pair_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_market_making/start.py` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/cross_exchange_mining_pair.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/order_id_market_pair_tracker.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/cross_exchange_mining/start.py` & `hummingbot-20240520/hummingbot/strategy/cross_exchange_mining/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/data_types.py` & `hummingbot-20240520/hummingbot/strategy/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/directional_strategy_base.py` & `hummingbot-20240520/hummingbot/strategy/directional_strategy_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/hanging_orders_tracker.py` & `hummingbot-20240520/hummingbot/strategy/hanging_orders_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/hedge/hedge.py` & `hummingbot-20240520/hummingbot/strategy/hedge/hedge.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/hedge/hedge_config_map_pydantic.py` & `hummingbot-20240520/hummingbot/strategy/hedge/hedge_config_map_pydantic.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/hedge/start.py` & `hummingbot-20240520/hummingbot/strategy/hedge/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/liquidity_mining/data_types.py` & `hummingbot-20240520/hummingbot/strategy/liquidity_mining/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/liquidity_mining/dummy.cpp` & `hummingbot-20240520/hummingbot/strategy/liquidity_mining/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/liquidity_mining/liquidity_mining.py` & `hummingbot-20240520/hummingbot/strategy/liquidity_mining/liquidity_mining.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py` & `hummingbot-20240520/hummingbot/strategy/liquidity_mining/liquidity_mining_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/liquidity_mining/start.py` & `hummingbot-20240520/hummingbot/strategy/liquidity_mining/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/maker_taker_market_pair.py` & `hummingbot-20240520/hummingbot/strategy/maker_taker_market_pair.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/market_trading_pair_tuple.py` & `hummingbot-20240520/hummingbot/strategy/market_trading_pair_tuple.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/order_book_asset_price_delegate.cpp` & `hummingbot-20240520/hummingbot/strategy/order_book_asset_price_delegate.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/order_tracker.cpp` & `hummingbot-20240520/hummingbot/strategy/order_tracker.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/LimitOrder.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core/data_type",
-            "hummingbot/core"
+            "hummingbot/core",
+            "hummingbot/core/data_type"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.order_tracker",
         "sources": [
             "hummingbot/strategy/order_tracker.pyx"
         ]
     },
```

### Comparing `hummingbot-20240429/hummingbot/strategy/perpetual_market_making/data_types.py` & `hummingbot-20240520/hummingbot/strategy/perpetual_market_making/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/perpetual_market_making/dummy.cpp` & `hummingbot-20240520/hummingbot/strategy/perpetual_market_making/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py` & `hummingbot-20240520/hummingbot/strategy/perpetual_market_making/perpetual_market_making.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py` & `hummingbot-20240520/hummingbot/strategy/perpetual_market_making/perpetual_market_making_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py` & `hummingbot-20240520/hummingbot/strategy/perpetual_market_making/perpetual_market_making_order_tracker.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/perpetual_market_making/start.py` & `hummingbot-20240520/hummingbot/strategy/perpetual_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/data_types.py` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/inventory_cost_price_delegate.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/inventory_skew_calculator.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/moving_price_band.py` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/moving_price_band.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/pure_market_making.cpp` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/pure_market_making.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/pure_market_making_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 {
     "distutils": {
         "depends": [
             "hummingbot/core/cpp/LimitOrder.h",
             "hummingbot/core/cpp/PyRef.h"
         ],
         "include_dirs": [
-            "hummingbot/core/data_type",
-            "hummingbot/core"
+            "hummingbot/core",
+            "hummingbot/core/data_type"
         ],
         "language": "c++",
         "name": "hummingbot.strategy.pure_market_making.pure_market_making_order_tracker",
         "sources": [
             "hummingbot/strategy/pure_market_making/pure_market_making_order_tracker.pyx"
         ]
     },
```

### Comparing `hummingbot-20240429/hummingbot/strategy/pure_market_making/start.py` & `hummingbot-20240520/hummingbot/strategy/pure_market_making/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/script_strategy_base.py` & `hummingbot-20240520/hummingbot/strategy/script_strategy_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py` & `hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/arb_proposal.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp` & `hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py` & `hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py` & `hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/spot_perpetual_arbitrage_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/start.py` & `hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/spot_perpetual_arbitrage/utils.py` & `hummingbot-20240520/hummingbot/strategy/spot_perpetual_arbitrage/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/strategy_base.cpp` & `hummingbot-20240520/hummingbot/strategy/strategy_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/strategy_py_base.cpp` & `hummingbot-20240520/hummingbot/strategy/strategy_py_base.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/strategy_v2_base.py` & `hummingbot-20240520/hummingbot/strategy/strategy_v2_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/twap/dummy.cpp` & `hummingbot-20240520/hummingbot/strategy/twap/dummy.cpp`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/twap/start.py` & `hummingbot-20240520/hummingbot/strategy/twap/start.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/twap/twap.py` & `hummingbot-20240520/hummingbot/strategy/twap/twap.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/twap/twap_config_map.py` & `hummingbot-20240520/hummingbot/strategy/twap/twap_config_map.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy/utils.py` & `hummingbot-20240520/hummingbot/strategy/utils.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py` & `hummingbot-20240520/hummingbot/strategy_v2/backtesting/backtesting_data_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 from decimal import Decimal
 from typing import Dict
 
+import pandas as pd
+
 from hummingbot.connector.connector_base import ConnectorBase
 from hummingbot.core.data_type.common import PriceType
 from hummingbot.data_feed.candles_feed.candles_factory import CandlesFactory
 from hummingbot.data_feed.candles_feed.data_types import CandlesConfig, HistoricalCandlesConfig
 from hummingbot.data_feed.market_data_provider import MarketDataProvider
 
 
 class BacktestingDataProvider(MarketDataProvider):
-    def __init__(self, connectors: Dict[str, ConnectorBase], start_time: int, end_time: int):
+    def __init__(self, connectors: Dict[str, ConnectorBase]):
         super().__init__(connectors)
-        self.start_time = start_time
-        self.end_time = end_time
+        self.start_time = None
+        self.end_time = None
         self.prices = {}
-        self._time = start_time
+        self._time = None
 
     def time(self):
         return self._time
 
     async def initialize_candles_feed(self, config: CandlesConfig):
         await self.get_candles_feed(config)
 
+    def update_backtesting_time(self, start_time: int, end_time: int):
+        if (self.start_time is None or self.end_time is None) or \
+                (start_time < self.start_time or end_time > self.end_time):
+            self.candles_feeds = {}
+        self.start_time = start_time
+        self.end_time = end_time
+        self._time = start_time
+
     async def get_candles_feed(self, config: CandlesConfig):
         """
         Retrieves or creates and starts a candle feed based on the given configuration.
         If an existing feed has a higher or equal max_records, it is reused.
         :param config: CandlesConfig
         :return: Candle feed instance.
         """
         key = self._generate_candle_feed_key(config)
-        existing_feed = self.candles_feeds.get(key)
+        existing_feed = self.candles_feeds.get(key, pd.DataFrame())
 
-        if existing_feed:
+        if not existing_feed.empty:
             # Existing feed is sufficient, return it
             return existing_feed
         else:
             # Create a new feed or restart the existing one with updated max_records
             candle_feed = CandlesFactory.get_candle(config)
             candles_df = await candle_feed.get_historical_candles(config=HistoricalCandlesConfig(
                 connector_name=config.connector,
                 trading_pair=config.trading_pair,
                 interval=config.interval,
                 start_time=self.start_time,
                 end_time=self.end_time,
             ))
             self.candles_feeds[key] = candles_df
-            return candle_feed
+            return candles_df
 
     def get_candles_df(self, connector_name: str, trading_pair: str, interval: str, max_records: int = 500):
         """
         Retrieves the candles for a trading pair from the specified connector.
         :param connector_name: str
         :param trading_pair: str
         :param interval: str
         :param max_records: int
         :return: Candles dataframe.
         """
-        return self.candles_feeds.get(f"{connector_name}_{trading_pair}_{interval}")
+        candles_df = self.candles_feeds.get(f"{connector_name}_{trading_pair}_{interval}")
+        return candles_df[(candles_df["timestamp"] >= self.start_time) & (candles_df["timestamp"] <= self.end_time)]
 
     def get_price_by_type(self, connector_name: str, trading_pair: str, price_type: PriceType):
         """
         Retrieves the price for a trading pair from the specified connector based on the price type.
         :param connector_name: str
         :param trading_pair: str
         :param price_type: PriceType
```

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/backtesting/backtesting_engine_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import inspect
 import os
 from decimal import Decimal
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 import yaml
 
 from hummingbot.client import settings
 from hummingbot.core.data_type.common import TradeType
@@ -29,28 +29,37 @@
 from hummingbot.strategy_v2.models.executors_info import ExecutorInfo
 
 
 class BacktestingEngineBase:
     def __init__(self):
         self.controller = None
         self.backtesting_resolution = None
+        self.backtesting_data_provider = BacktestingDataProvider(connectors={})
         self.position_executor_simulator = PositionExecutorSimulator()
         self.dca_executor_simulator = DCAExecutorSimulator()
 
     @classmethod
-    def load_controller_config(cls, config_path: str) -> ControllerConfigBase:
+    def load_controller_config(cls, config_path: str) -> Dict:
         full_path = os.path.join(settings.CONTROLLERS_CONF_DIR_PATH, config_path)
         with open(full_path, 'r') as file:
             config_data = yaml.safe_load(file)
+        return config_data
 
+    @classmethod
+    def get_controller_config_instance_from_yml(cls, config_path: str) -> ControllerConfigBase:
+        config_data = cls.load_controller_config(config_path)
+        return cls.get_controller_config_instance_from_dict(config_data)
+
+    @classmethod
+    def get_controller_config_instance_from_dict(cls, config_data: dict) -> ControllerConfigBase:
         controller_type = config_data.get('controller_type')
         controller_name = config_data.get('controller_name')
 
         if not controller_type or not controller_name:
-            raise ValueError(f"Missing controller_type or controller_name in {config_path}")
+            raise ValueError("Missing controller_type or controller_name in the configuration.")
 
         module_path = f"{settings.CONTROLLERS_MODULE}.{controller_type}.{controller_name}"
         module = importlib.import_module(module_path)
 
         config_class = next((member for member_name, member in inspect.getmembers(module)
                              if inspect.isclass(member) and member not in [ControllerConfigBase,
                                                                            MarketMakingControllerConfigBase,
@@ -64,16 +73,16 @@
     async def run_backtesting(self,
                               controller_config: ControllerConfigBase,
                               start: int, end: int,
                               backtesting_resolution: str = "1m",
                               trade_cost=0.0006):
         # Load historical candles
         controller_class = controller_config.get_controller_class()
-        backtesting_data_provider = BacktestingDataProvider(connectors={}, start_time=start, end_time=end)
-        self.controller = controller_class(config=controller_config, market_data_provider=backtesting_data_provider,
+        self.backtesting_data_provider.update_backtesting_time(start, end)
+        self.controller = controller_class(config=controller_config, market_data_provider=self.backtesting_data_provider,
                                            actions_queue=None)
         self.backtesting_resolution = backtesting_resolution
         await self.initialize_backtesting_data_provider()
         await self.controller.update_processed_data()
         executors_info = self.simulate_execution(trade_cost=trade_cost)
         results = self.summarize_results(executors_info)
         return {
@@ -244,15 +253,15 @@
             total_long = (executors_with_position["side"] == TradeType.BUY).sum()
             total_short = (executors_with_position["side"] == TradeType.SELL).sum()
             correct_long = ((executors_with_position["side"] == TradeType.BUY) & (executors_with_position["net_pnl_quote"] > 0)).sum()
             correct_short = ((executors_with_position["side"] == TradeType.SELL) & (executors_with_position["net_pnl_quote"] > 0)).sum()
             accuracy_long = correct_long / total_long if total_long > 0 else 0
             accuracy_short = correct_short / total_short if total_short > 0 else 0
             executors_df["close_type_name"] = executors_df["close_type"].apply(lambda x: x.name)
-            close_types = executors_df.groupby("close_type_name")["timestamp"].count()
+            close_types = executors_df.groupby("close_type_name")["timestamp"].count().to_dict()
             executors_with_position = executors_df[executors_df["net_pnl_quote"] != 0].copy()
             # Additional metrics
             total_positions = executors_with_position.shape[0]
             win_signals = executors_with_position[executors_with_position["net_pnl_quote"] > 0]
             loss_signals = executors_with_position[executors_with_position["net_pnl_quote"] < 0]
             accuracy = win_signals.shape[0] / total_positions
             cumulative_returns = executors_with_position["net_pnl_quote"].cumsum()
@@ -269,32 +278,32 @@
             sharpe_ratio = returns.mean() / returns.std()
             total_won = win_signals.loc[:, "net_pnl_quote"].sum()
             total_loss = - loss_signals.loc[:, "net_pnl_quote"].sum()
             profit_factor = total_won / total_loss if total_loss > 0 else 1
             net_pnl_pct = net_pnl_quote / total_amount_quote
 
             return {
-                "net_pnl": net_pnl_pct,
-                "net_pnl_quote": net_pnl_quote,
-                "total_executors": total_executors,
-                "total_executors_with_position": total_executors_with_position,
-                "total_volume": total_volume,
-                "total_long": total_long,
-                "total_short": total_short,
+                "net_pnl": float(net_pnl_pct),
+                "net_pnl_quote": float(net_pnl_quote),
+                "total_executors": int(total_executors),
+                "total_executors_with_position": int(total_executors_with_position),
+                "total_volume": float(total_volume),
+                "total_long": int(total_long),
+                "total_short": int(total_short),
                 "close_types": close_types,
-                "accuracy_long": accuracy_long,
-                "accuracy_short": accuracy_short,
-                "total_positions": total_positions,
-                "accuracy": accuracy,
-                "max_drawdown_usd": max_draw_down,
-                "max_drawdown_pct": max_drawdown_pct,
-                "sharpe_ratio": sharpe_ratio,
-                "profit_factor": profit_factor,
-                "win_signals": win_signals.shape[0],
-                "loss_signals": loss_signals.shape[0],
+                "accuracy_long": float(accuracy_long),
+                "accuracy_short": float(accuracy_short),
+                "total_positions": int(total_positions),
+                "accuracy": float(accuracy),
+                "max_drawdown_usd": float(max_draw_down),
+                "max_drawdown_pct": float(max_drawdown_pct),
+                "sharpe_ratio": float(sharpe_ratio),
+                "profit_factor": float(profit_factor),
+                "win_signals": int(win_signals.shape[0]),
+                "loss_signals": int(loss_signals.shape[0]),
             }
         return {
             "net_pnl": 0,
             "net_pnl_quote": 0,
             "total_executors": 0,
             "total_executors_with_position": 0,
             "total_volume": 0,
```

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/backtesting/executor_simulator_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/backtesting/executor_simulator_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py` & `hummingbot-20240520/hummingbot/strategy_v2/backtesting/executors_simulator/dca_executor_simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             df_filtered[f'filled_amount_quote_{i}'] = 0.0
             df_filtered[f'net_pnl_quote_{i}'] = 0.0
             potential_dca_stages.append({
                 'level': i,
                 'entry_timestamp': entry_timestamp,
                 'price': float(price),
                 'amount': float(amount),
-                'break_even_price': break_even_price,
+                'break_even_price': float(break_even_price),
                 'close_timestamp': close_timestamp,
                 'close_type': close_type,
                 'cumulative_returns': cumulative_returns
             })
         if len(potential_dca_stages) == 0:
             return ExecutorSimulation(config=config, executor_simulation=df_filtered, close_type=CloseType.TIME_LIMIT)
         close_type = None
@@ -98,15 +98,16 @@
                 close_type = dca_stage['close_type']
                 last_timestamp = dca_stage['close_timestamp']
                 break
         df_filtered = df_filtered[df_filtered['timestamp'] <= last_timestamp].copy()
         df_filtered['filled_amount_quote'] = sum([df_filtered[f'filled_amount_quote_{i}'] for i in range(len(potential_dca_stages))])
         df_filtered['net_pnl_quote'] = sum([df_filtered[f'net_pnl_quote_{i}'] for i in range(len(potential_dca_stages))])
         df_filtered['cum_fees_quote'] = trade_cost * df_filtered['filled_amount_quote']
-        df_filtered['net_pnl_pct'] = df_filtered['net_pnl_quote'] / df_filtered['filled_amount_quote']
+        df_filtered.loc[df_filtered["filled_amount_quote"] > 0, "net_pnl_pct"] = df_filtered["net_pnl_quote"] / df_filtered["filled_amount_quote"]
+
         if close_type is None:
             close_type = CloseType.FAILED
 
         # Construct and return ExecutorSimulation object
         simulation = ExecutorSimulation(
             config=config,
             executor_simulation=df_filtered,
```

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py` & `hummingbot-20240520/hummingbot/strategy_v2/backtesting/executors_simulator/position_executor_simulator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/controllers/controller_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/controllers/controller_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/controllers/directional_trading_controller_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/controllers/market_making_controller_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/controllers/market_making_controller_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/arbitrage_executor/arbitrage_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/data_types.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/dca_executor/data_types.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/dca_executor/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/dca_executor/dca_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/executor_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/executor_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/executor_orchestrator.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/executor_orchestrator.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/position_executor/data_types.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/position_executor/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/position_executor/position_executor.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/position_executor/position_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/twap_executor/data_types.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/twap_executor/data_types.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/twap_executor/twap_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py` & `hummingbot-20240520/hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/models/executor_actions.py` & `hummingbot-20240520/hummingbot/strategy_v2/models/executor_actions.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/models/executors.py` & `hummingbot-20240520/hummingbot/strategy_v2/models/executors.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/models/executors_info.py` & `hummingbot-20240520/hummingbot/strategy_v2/models/executors_info.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/order_level_distributions/distributions.py` & `hummingbot-20240520/hummingbot/strategy_v2/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/order_level_distributions/order_level_builder.py` & `hummingbot-20240520/hummingbot/strategy_v2/utils/order_level_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel
 from pydantic.class_validators import validator
 
 from hummingbot.core.data_type.common import TradeType
 from hummingbot.strategy_v2.executors.position_executor.data_types import TripleBarrierConfig
-from hummingbot.strategy_v2.order_level_distributions.distributions import Distributions
+from hummingbot.strategy_v2.utils.distributions import Distributions
 
 
 class OrderLevel(BaseModel):
     level: int
     side: TradeType
     order_amount_usd: Decimal
     spread_factor: Decimal = Decimal("0.0")
```

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/runnable_base.py` & `hummingbot-20240520/hummingbot/strategy_v2/runnable_base.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/strategy_v2/utils/config_encoder_decoder.py` & `hummingbot-20240520/hummingbot/strategy_v2/utils/config_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_fee_overrides_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/conf_twap_strategy_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/templates/hummingbot_logs_TEMPLATE.yml` & `hummingbot-20240520/hummingbot/templates/hummingbot_logs_TEMPLATE.yml`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot/user/user_balances.py` & `hummingbot-20240520/hummingbot/user/user_balances.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/hummingbot.egg-info/PKG-INFO` & `hummingbot-20240520/hummingbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummingbot
-Version: 20240429
+Version: 20240520
 Summary: Hummingbot
 Home-page: https://github.com/hummingbot/hummingbot
 Author: Hummingbot Foundation
 Author-email: dev@hummingbot.org
 License: Apache 2.0
 License-File: LICENSE
 Requires-Dist: bidict
@@ -33,14 +33,15 @@
 Requires-Dist: eth-typing
 Requires-Dist: eth-utils
 Requires-Dist: flake8
 Requires-Dist: hexbytes
 Requires-Dist: importlib-metadata
 Requires-Dist: injective-py
 Requires-Dist: mypy-extensions
+Requires-Dist: msgpack
 Requires-Dist: nose
 Requires-Dist: nose-exclude
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pip
 Requires-Dist: pre-commit
 Requires-Dist: prompt-toolkit
```

### Comparing `hummingbot-20240429/hummingbot.egg-info/SOURCES.txt` & `hummingbot-20240520/hummingbot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -630,14 +630,17 @@
 hummingbot/data_feed/candles_feed/kraken_spot_candles/kraken_spot_candles.py
 hummingbot/data_feed/candles_feed/kucoin_spot_candles/__init__.py
 hummingbot/data_feed/candles_feed/kucoin_spot_candles/constants.py
 hummingbot/data_feed/candles_feed/kucoin_spot_candles/kucoin_spot_candles.py
 hummingbot/data_feed/candles_feed/okx_perpetual_candles/__init__.py
 hummingbot/data_feed/candles_feed/okx_perpetual_candles/constants.py
 hummingbot/data_feed/candles_feed/okx_perpetual_candles/okx_perpetual_candles.py
+hummingbot/data_feed/candles_feed/okx_spot_candles/__init__.py
+hummingbot/data_feed/candles_feed/okx_spot_candles/constants.py
+hummingbot/data_feed/candles_feed/okx_spot_candles/okx_spot_candles.py
 hummingbot/data_feed/coin_cap_data_feed/__init__.py
 hummingbot/data_feed/coin_cap_data_feed/coin_cap_constants.py
 hummingbot/data_feed/coin_cap_data_feed/coin_cap_data_feed.py
 hummingbot/data_feed/coin_gecko_data_feed/__init__.py
 hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_constants.py
 hummingbot/data_feed/coin_gecko_data_feed/coin_gecko_data_feed.py
 hummingbot/data_feed/liquidations_feed/__init__.py
@@ -807,20 +810,19 @@
 hummingbot/strategy_v2/executors/xemm_executor/data_types.py
 hummingbot/strategy_v2/executors/xemm_executor/xemm_executor.py
 hummingbot/strategy_v2/models/__init__.py
 hummingbot/strategy_v2/models/base.py
 hummingbot/strategy_v2/models/executor_actions.py
 hummingbot/strategy_v2/models/executors.py
 hummingbot/strategy_v2/models/executors_info.py
-hummingbot/strategy_v2/order_level_distributions/__init__.py
-hummingbot/strategy_v2/order_level_distributions/distributions.py
-hummingbot/strategy_v2/order_level_distributions/order_level_builder.py
 hummingbot/strategy_v2/utils/__init__.py
 hummingbot/strategy_v2/utils/common.py
 hummingbot/strategy_v2/utils/config_encoder_decoder.py
+hummingbot/strategy_v2/utils/distributions.py
+hummingbot/strategy_v2/utils/order_level_builder.py
 hummingbot/templates/conf_amm_arb_strategy_TEMPLATE.yml
 hummingbot/templates/conf_amm_v3_lp_strategy_TEMPLATE.yml
 hummingbot/templates/conf_fee_overrides_TEMPLATE.yml
 hummingbot/templates/conf_liquidity_mining_strategy_TEMPLATE.yml
 hummingbot/templates/conf_perpetual_market_making_strategy_TEMPLATE.yml
 hummingbot/templates/conf_pure_market_making_strategy_TEMPLATE.yml
 hummingbot/templates/conf_spot_perpetual_arbitrage_strategy_TEMPLATE.yml
```

### Comparing `hummingbot-20240429/hummingbot.egg-info/requires.txt` & `hummingbot-20240520/hummingbot.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 eth-typing
 eth-utils
 flake8
 hexbytes
 importlib-metadata
 injective-py
 mypy-extensions
+msgpack
 nose
 nose-exclude
 numpy
 pandas
 pip
 pre-commit
 prompt-toolkit
```

### Comparing `hummingbot-20240429/setup.py` & `hummingbot-20240520/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if os.name != "nt" and "-Wstrict-prototypes" in self.compiler.compiler_so:
             self.compiler.compiler_so.remove("-Wstrict-prototypes")
         super().build_extensions()
 
 
 def main():
     cpu_count = os.cpu_count() or 8
-    version = "20240429"
+    version = "20240520"
     all_packages = find_packages(include=["hummingbot", "hummingbot.*"], )
     excluded_paths = [
         "hummingbot.connector.gateway.clob_spot.data_sources.injective",
         "hummingbot.connector.gateway.clob_perp.data_sources.injective_perpetual"
     ]
     packages = [pkg for pkg in all_packages if not any(fnmatch.fnmatch(pkg, pattern) for pattern in excluded_paths)]
     package_data = {
@@ -74,14 +74,15 @@
         "eth-typing",
         "eth-utils",
         "flake8",
         "hexbytes",
         "importlib-metadata",
         "injective-py",
         "mypy-extensions",
+        "msgpack",
         "nose",
         "nose-exclude",
         "numpy",
         "pandas",
         "pip",
         "pre-commit",
         "prompt-toolkit",
```

### Comparing `hummingbot-20240429/test/test_isolated_asyncio_wrapper_test_case.py` & `hummingbot-20240520/test/test_isolated_asyncio_wrapper_test_case.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/test/test_local_class_event_loop_wrapper_test_case.py` & `hummingbot-20240520/test/test_local_class_event_loop_wrapper_test_case.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/test/test_local_test_event_loop_wrapper_test_case.py` & `hummingbot-20240520/test/test_local_test_event_loop_wrapper_test_case.py`

 * *Files identical despite different names*

### Comparing `hummingbot-20240429/test/test_logger_mixin_for_test.py` & `hummingbot-20240520/test/test_logger_mixin_for_test.py`

 * *Files identical despite different names*

