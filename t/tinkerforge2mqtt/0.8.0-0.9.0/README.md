# Comparing `tmp/tinkerforge2mqtt-0.8.tar.gz` & `tmp/tinkerforge2mqtt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinkerforge2mqtt-0.8.tar", last modified: Fri Apr 12 16:47:54 2024, max compression
+gzip compressed data, was "tinkerforge2mqtt-0.9.0.tar", last modified: Mon May 20 09:24:35 2024, max compression
```

## Comparing `tinkerforge2mqtt-0.8.tar` & `tinkerforge2mqtt-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/
--rw-rw-r--   0 jens      (1000) users      (100)      310 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.283756 tinkerforge2mqtt-0.8/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1670 2024-03-12 08:31:19.000000 tinkerforge2mqtt-0.8/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      116 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/.gitignore
--rw-r--r--   0 jens      (1000) users      (100)     3731 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     2404 2024-03-26 08:26:20.000000 tinkerforge2mqtt-0.8/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3159 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3089 2024-03-12 08:31:08.000000 tinkerforge2mqtt-0.8/dev-cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     4935 2024-03-27 11:29:05.000000 tinkerforge2mqtt-0.8/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    75311 2024-04-12 16:47:21.000000 tinkerforge2mqtt-0.8/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    11451 2024-04-12 16:47:21.000000 tinkerforge2mqtt-0.8/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/setup.cfg
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/
--rw-rw-r--   0 jens      (1000) users      (100)      137 2024-04-12 16:43:07.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      178 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/
--rw-rw-r--   0 jens      (1000) users      (100)     1364 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3981 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/discovering.py
--rw-rw-r--   0 jens      (1000) users      (100)     2563 2024-03-23 12:12:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/publish.py
--rw-rw-r--   0 jens      (1000) users      (100)     1395 2024-03-12 08:36:23.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/settings.py
--rw-rw-r--   0 jens      (1000) users      (100)     2486 2024-03-12 08:36:51.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/systemd.py
--rw-rw-r--   0 jens      (1000) users      (100)      806 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/update_readme_history.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/
--rw-rw-r--   0 jens      (1000) users      (100)     2163 2024-03-23 12:13:34.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      968 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/code_style.py
--rw-rw-r--   0 jens      (1000) users      (100)     2325 2024-03-16 07:49:08.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/packaging.py
--rw-rw-r--   0 jens      (1000) users      (100)     1520 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/testing.py
--rw-rw-r--   0 jens      (1000) users      (100)      179 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/
--rw-rw-r--   0 jens      (1000) users      (100)     1236 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1949 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/brick_hat_zero.py
--rw-rw-r--   0 jens      (1000) users      (100)     2848 2024-04-12 16:46:27.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py
--rw-rw-r--   0 jens      (1000) users      (100)     2820 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     2817 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
--rw-rw-r--   0 jens      (1000) users      (100)     1998 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     2332 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     1903 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
--rw-rw-r--   0 jens      (1000) users      (100)     3677 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4214 2024-03-27 11:30:50.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/base.py
--rw-rw-r--   0 jens      (1000) users      (100)      566 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/generics.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2024-03-13 18:56:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2664 2024-03-25 16:32:13.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/devices_handler.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/
--rw-rw-r--   0 jens      (1000) users      (100)     1197 2024-03-08 19:27:47.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      227 2024-03-10 18:32:00.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     1478 2024-03-12 08:25:52.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     1227 2024-03-25 16:26:57.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt/user_settings.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-12 16:47:54.287756 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/
--rw-r--r--   0 jens      (1000) users      (100)     3731 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1729 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)      125 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      270 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       17 2024-04-12 16:47:54.000000 tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/top_level.txt
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/
+-rw-rw-r--   0 jens      (1000) jens      (1000)      310 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.editorconfig
+-rw-rw-r--   0 jens      (1000) jens      (1000)      153 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.flake8
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.148477 tinkerforge2mqtt-0.9.0/.github/
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/.github/workflows/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1670 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) jens      (1000)      116 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/.gitignore
+-rw-r--r--   0 jens      (1000) jens      (1000)     3731 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/PKG-INFO
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2404 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/README.md
+-rwxrwxr-x   0 jens      (1000) jens      (1000)     3159 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/cli.py
+-rwxrwxr-x   0 jens      (1000) jens      (1000)     3089 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/dev-cli.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     4935 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/pyproject.toml
+-rw-rw-r--   0 jens      (1000) jens      (1000)    75058 2024-05-20 08:34:35.000000 tinkerforge2mqtt-0.9.0/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)    11196 2024-05-20 08:34:00.000000 tinkerforge2mqtt-0.9.0/requirements.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       38 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/setup.cfg
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/
+-rw-rw-r--   0 jens      (1000) jens      (1000)      137 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      178 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/__main__.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1364 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3981 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/discovering.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2563 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/publish.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1395 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/settings.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2486 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/systemd.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      806 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/update_readme_history.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2163 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      968 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/code_style.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2472 2024-05-20 08:41:33.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/packaging.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1520 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/testing.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      179 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/constants.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1236 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1949 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/brick_hat_zero.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2848 2024-04-17 16:12:57.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3638 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2817 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1998 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2332 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1903 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3677 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     4214 2024-04-09 16:58:58.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/base.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      566 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/generics.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.152477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2664 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/devices_handler.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1197 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)      227 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1478 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1227 2024-03-26 18:35:03.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/user_settings.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1283 2024-05-20 09:16:15.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/utilities/dew_point.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2024-05-20 09:24:35.156477 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/
+-rw-r--r--   0 jens      (1000) jens      (1000)     3731 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1808 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)        1 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)      125 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)      270 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       17 2024-05-20 09:24:35.000000 tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/top_level.txt
```

### Comparing `tinkerforge2mqtt-0.8/.github/workflows/tests.yml` & `tinkerforge2mqtt-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/PKG-INFO` & `tinkerforge2mqtt-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkerforge2mqtt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Emit MQTT events from Tinkerforge devices
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tinkerforge2mqtt
 Project-URL: Source, https://github.com/jedie/tinkerforge2mqtt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tinkerforge2mqtt-0.8/README.md` & `tinkerforge2mqtt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/cli.py` & `tinkerforge2mqtt-0.9.0/cli.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/dev-cli.py` & `tinkerforge2mqtt-0.9.0/dev-cli.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/pyproject.toml` & `tinkerforge2mqtt-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/requirements.dev.txt` & `tinkerforge2mqtt-0.9.0/requirements.dev.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,45 +34,45 @@
     # via manageprojects
 autopep8==2.1.0 \
     --hash=sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7 \
     --hash=sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-backports-tarfile==1.0.0 \
-    --hash=sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75 \
-    --hash=sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4
+backports-tarfile==1.1.1 \
+    --hash=sha256:73e0179647803d3726d82e76089d01d8549ceca9bace469953fcb4d97cf2d417 \
+    --hash=sha256:9c2ef9696cb73374f7164e17fc761389393ca76777036f5aad42e8b93fcd8009
     # via jaraco-context
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-black==24.3.0 \
-    --hash=sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f \
-    --hash=sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93 \
-    --hash=sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11 \
-    --hash=sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0 \
-    --hash=sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9 \
-    --hash=sha256:56f52cfbd3dabe2798d76dbdd299faa046a901041faf2cf33288bc4e6dae57b5 \
-    --hash=sha256:65b76c275e4c1c5ce6e9870911384bff5ca31ab63d19c76811cb1fb162678213 \
-    --hash=sha256:65c02e4ea2ae09d16314d30912a58ada9a5c4fdfedf9512d23326128ac08ac3d \
-    --hash=sha256:6905238a754ceb7788a73f02b45637d820b2f5478b20fec82ea865e4f5d4d9f7 \
-    --hash=sha256:79dcf34b33e38ed1b17434693763301d7ccbd1c5860674a8f871bd15139e7837 \
-    --hash=sha256:7bb041dca0d784697af4646d3b62ba4a6b028276ae878e53f6b4f74ddd6db99f \
-    --hash=sha256:7d5e026f8da0322b5662fa7a8e752b3fa2dac1c1cbc213c3d7ff9bdd0ab12395 \
-    --hash=sha256:9f50ea1132e2189d8dff0115ab75b65590a3e97de1e143795adb4ce317934995 \
-    --hash=sha256:a0c9c4a0771afc6919578cec71ce82a3e31e054904e7197deacbc9382671c41f \
-    --hash=sha256:aadf7a02d947936ee418777e0247ea114f78aff0d0959461057cae8a04f20597 \
-    --hash=sha256:b5991d523eee14756f3c8d5df5231550ae8993e2286b8014e2fdea7156ed0959 \
-    --hash=sha256:bf21b7b230718a5f08bd32d5e4f1db7fc8788345c8aea1d155fc17852b3410f5 \
-    --hash=sha256:c45f8dff244b3c431b36e3224b6be4a127c6aca780853574c00faf99258041eb \
-    --hash=sha256:c7ed6668cbbfcd231fa0dc1b137d3e40c04c7f786e626b405c62bcd5db5857e4 \
-    --hash=sha256:d7de8d330763c66663661a1ffd432274a2f92f07feeddd89ffd085b5744f85e7 \
-    --hash=sha256:e19cb1c6365fd6dc38a6eae2dcb691d7d83935c10215aef8e6c38edee3f77abd \
-    --hash=sha256:e2af80566f43c85f5797365077fb64a393861a3730bd110971ab7a0c94e873e7
+black==24.4.2 \
+    --hash=sha256:257d724c2c9b1660f353b36c802ccece186a30accc7742c176d29c146df6e474 \
+    --hash=sha256:37aae07b029fa0174d39daf02748b379399b909652a806e5708199bd93899da1 \
+    --hash=sha256:415e686e87dbbe6f4cd5ef0fbf764af7b89f9057b97c908742b6008cc554b9c0 \
+    --hash=sha256:48a85f2cb5e6799a9ef05347b476cce6c182d6c71ee36925a6c194d074336ef8 \
+    --hash=sha256:7768a0dbf16a39aa5e9a3ded568bb545c8c2727396d063bbaf847df05b08cd96 \
+    --hash=sha256:7e122b1c4fb252fd85df3ca93578732b4749d9be076593076ef4d07a0233c3e1 \
+    --hash=sha256:88c57dc656038f1ab9f92b3eb5335ee9b021412feaa46330d5eba4e51fe49b04 \
+    --hash=sha256:8e537d281831ad0e71007dcdcbe50a71470b978c453fa41ce77186bbe0ed6021 \
+    --hash=sha256:98e123f1d5cfd42f886624d84464f7756f60ff6eab89ae845210631714f6db94 \
+    --hash=sha256:accf49e151c8ed2c0cdc528691838afd217c50412534e876a19270fea1e28e2d \
+    --hash=sha256:b1530ae42e9d6d5b670a34db49a94115a64596bc77710b1d05e9801e62ca0a7c \
+    --hash=sha256:b9176b9832e84308818a99a561e90aa479e73c523b3f77afd07913380ae2eab7 \
+    --hash=sha256:bdde6f877a18f24844e381d45e9947a49e97933573ac9d4345399be37621e26c \
+    --hash=sha256:be8bef99eb46d5021bf053114442914baeb3649a89dc5f3a555c88737e5e98fc \
+    --hash=sha256:bf10f7310db693bb62692609b397e8d67257c55f949abde4c67f9cc574492cc7 \
+    --hash=sha256:c872b53057f000085da66a19c55d68f6f8ddcac2642392ad3a355878406fbd4d \
+    --hash=sha256:d36ed1124bb81b32f8614555b34cc4259c3fbc7eec17870e8ff8ded335b58d8c \
+    --hash=sha256:da33a1a5e49c4122ccdfd56cd021ff1ebc4a1ec4e2d01594fef9b6f267a9e741 \
+    --hash=sha256:dd1b5a14e417189db4c7b64a6540f31730713d173f0b63e55fabd52d61d8fdce \
+    --hash=sha256:e151054aa00bad1f4e1f04919542885f89f5f7d086b8a59e5000e6c616896ffb \
+    --hash=sha256:eaea3008c281f1038edb473c1aa8ed8143a5535ff18f978a318f10302b254063 \
+    --hash=sha256:ef703f83fc32e131e9bcc0a5094cfe85599e7109f896fe8bc96cc402f3eb4b6e
     # via darker
 build==1.2.1 \
     --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
     --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
     # via pip-tools
 bx-py-utils==92 \
     --hash=sha256:38641b2e1a09ed0c64cd6ba0e03c97fea347302439db0234a0492c365ae32719 \
@@ -271,203 +271,200 @@
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
 cookiecutter==2.6.0 \
     --hash=sha256:a54a8e37995e4ed963b3e82831072d1ad4b005af736bb17b99c2cbd9d41b6e2d \
     --hash=sha256:db21f8169ea4f4fdc2408d48ca44859349de2647fbe494a9d6c3edfc0542c21c
     # via manageprojects
-coverage==7.4.4 \
-    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
-    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
-    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
-    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
-    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
-    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
-    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
-    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
-    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
-    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
-    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
-    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
-    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
-    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
-    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
-    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
-    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
-    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
-    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
-    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
-    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
-    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
-    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
-    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
-    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
-    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
-    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
-    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
-    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
-    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
-    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
-    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
-    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
-    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
-    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
-    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
-    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
-    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
-    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
-    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
-    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
-    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
-    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
-    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
-    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
-    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
-    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
-    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
-    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
-    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
-    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
-    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
+coverage==7.5.1 \
+    --hash=sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de \
+    --hash=sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661 \
+    --hash=sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26 \
+    --hash=sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41 \
+    --hash=sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d \
+    --hash=sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981 \
+    --hash=sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2 \
+    --hash=sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34 \
+    --hash=sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f \
+    --hash=sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a \
+    --hash=sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35 \
+    --hash=sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223 \
+    --hash=sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1 \
+    --hash=sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746 \
+    --hash=sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90 \
+    --hash=sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c \
+    --hash=sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca \
+    --hash=sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8 \
+    --hash=sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596 \
+    --hash=sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e \
+    --hash=sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd \
+    --hash=sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e \
+    --hash=sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3 \
+    --hash=sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e \
+    --hash=sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312 \
+    --hash=sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7 \
+    --hash=sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572 \
+    --hash=sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428 \
+    --hash=sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f \
+    --hash=sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07 \
+    --hash=sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e \
+    --hash=sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4 \
+    --hash=sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136 \
+    --hash=sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5 \
+    --hash=sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8 \
+    --hash=sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d \
+    --hash=sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228 \
+    --hash=sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206 \
+    --hash=sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa \
+    --hash=sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e \
+    --hash=sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be \
+    --hash=sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5 \
+    --hash=sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668 \
+    --hash=sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601 \
+    --hash=sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057 \
+    --hash=sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146 \
+    --hash=sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f \
+    --hash=sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8 \
+    --hash=sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7 \
+    --hash=sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987 \
+    --hash=sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19 \
+    --hash=sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece
     # via tinkerforge2mqtt (pyproject.toml)
-cryptography==42.0.5 \
-    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
-    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
-    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
-    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
-    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
-    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
-    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
-    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
-    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
-    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
-    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
-    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
-    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
-    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
-    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
-    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
-    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
-    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
-    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
-    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
-    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
-    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
-    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
-    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
-    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
-    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
-    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
-    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
-    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
-    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
-    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
-    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+cryptography==42.0.7 \
+    --hash=sha256:02c0eee2d7133bdbbc5e24441258d5d2244beb31da5ed19fbb80315f4bbbff55 \
+    --hash=sha256:0d563795db98b4cd57742a78a288cdbdc9daedac29f2239793071fe114f13785 \
+    --hash=sha256:16268d46086bb8ad5bf0a2b5544d8a9ed87a0e33f5e77dd3c3301e63d941a83b \
+    --hash=sha256:1a58839984d9cb34c855197043eaae2c187d930ca6d644612843b4fe8513c886 \
+    --hash=sha256:2954fccea107026512b15afb4aa664a5640cd0af630e2ee3962f2602693f0c82 \
+    --hash=sha256:2e47577f9b18723fa294b0ea9a17d5e53a227867a0a4904a1a076d1646d45ca1 \
+    --hash=sha256:31adb7d06fe4383226c3e963471f6837742889b3c4caa55aac20ad951bc8ffda \
+    --hash=sha256:3577d029bc3f4827dd5bf8bf7710cac13527b470bbf1820a3f394adb38ed7d5f \
+    --hash=sha256:36017400817987670037fbb0324d71489b6ead6231c9604f8fc1f7d008087c68 \
+    --hash=sha256:362e7197754c231797ec45ee081f3088a27a47c6c01eff2ac83f60f85a50fe60 \
+    --hash=sha256:3de9a45d3b2b7d8088c3fbf1ed4395dfeff79d07842217b38df14ef09ce1d8d7 \
+    --hash=sha256:4f698edacf9c9e0371112792558d2f705b5645076cc0aaae02f816a0171770fd \
+    --hash=sha256:5482e789294854c28237bba77c4c83be698be740e31a3ae5e879ee5444166582 \
+    --hash=sha256:5e44507bf8d14b36b8389b226665d597bc0f18ea035d75b4e53c7b1ea84583cc \
+    --hash=sha256:779245e13b9a6638df14641d029add5dc17edbef6ec915688f3acb9e720a5858 \
+    --hash=sha256:789caea816c6704f63f6241a519bfa347f72fbd67ba28d04636b7c6b7da94b0b \
+    --hash=sha256:7f8b25fa616d8b846aef64b15c606bb0828dbc35faf90566eb139aa9cff67af2 \
+    --hash=sha256:8cb8ce7c3347fcf9446f201dc30e2d5a3c898d009126010cbd1f443f28b52678 \
+    --hash=sha256:93a3209f6bb2b33e725ed08ee0991b92976dfdcf4e8b38646540674fc7508e13 \
+    --hash=sha256:a3a5ac8b56fe37f3125e5b72b61dcde43283e5370827f5233893d461b7360cd4 \
+    --hash=sha256:a47787a5e3649008a1102d3df55424e86606c9bae6fb77ac59afe06d234605f8 \
+    --hash=sha256:a79165431551042cc9d1d90e6145d5d0d3ab0f2d66326c201d9b0e7f5bf43604 \
+    --hash=sha256:a987f840718078212fdf4504d0fd4c6effe34a7e4740378e59d47696e8dfb477 \
+    --hash=sha256:a9bc127cdc4ecf87a5ea22a2556cab6c7eda2923f84e4f3cc588e8470ce4e42e \
+    --hash=sha256:bd13b5e9b543532453de08bcdc3cc7cebec6f9883e886fd20a92f26940fd3e7a \
+    --hash=sha256:c65f96dad14f8528a447414125e1fc8feb2ad5a272b8f68477abbcc1ea7d94b9 \
+    --hash=sha256:d8e3098721b84392ee45af2dd554c947c32cc52f862b6a3ae982dbb90f577f14 \
+    --hash=sha256:e6b79d0adb01aae87e8a44c2b64bc3f3fe59515280e00fb6d57a7267a2583cda \
+    --hash=sha256:e6b8f1881dac458c34778d0a424ae5769de30544fc678eac51c1c8bb2183e9da \
+    --hash=sha256:e9b2a6309f14c0497f348d08a065d52f3020656f675819fc405fb63bbcd26562 \
+    --hash=sha256:ecbfbc00bf55888edda9868a4cf927205de8499e7fabe6c050322298382953f2 \
+    --hash=sha256:efd0bf5205240182e0f13bcaea41be4fdf5c22c5129fc7ced4a0282ac86998c9
     # via
     #   authlib
     #   secretstorage
-darker[color,flynt,isort]==2.1.0 \
-    --hash=sha256:13ce2f14ac416d3032b7bc12d650a098416794df1f40308bd7818a17162fb639 \
-    --hash=sha256:29eaaeb00d0dc6b15e0fd64f00ed6359707b35b8962a387794a26b59da281057
+darker[color,flynt,isort]==2.1.1 \
+    --hash=sha256:a6e6a682c0604e76fe9aec7650e96a944f517563c69b28fcc076db9d957d98ea \
+    --hash=sha256:ead701414c45359fc0312bc285614d3285fc135476d43f3bc08d989ee19d9020
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-darkgraylib==1.1.1 \
-    --hash=sha256:240b993a5492b3f6f68f305a409e87d146fc55768368dd783483bda0ae38ea5d \
-    --hash=sha256:471c7934907a99bb282bb8649dad5ab71e028cdbef51d01c160f63f958709ec6
+darkgraylib==1.2.1 \
+    --hash=sha256:60c59de69842367ce0c78c32c451fa8e9d29500e681312d9864a7416bcdb7792 \
+    --hash=sha256:a5dd6a2015a470d9047278cdd01a91ccb1d746675f8fd4562b3b5f6b8cbda930
     # via
     #   darker
     #   graylint
 distlib==0.3.8 \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
     # via virtualenv
-docutils==0.21.1 \
-    --hash=sha256:14c8d34a55b46c88f9f714adb29cefbdd69fb82f3fef825e59c5faab935390d8 \
-    --hash=sha256:65249d8a5345bc95e0f40f280ba63c98eb24de35c6c8f5b662e3e8948adea83f
+docutils==0.21.2 \
+    --hash=sha256:3a6b18732edf182daa3cd12775bbb338cf5691468f91eeeb109deff6ebfa986f \
+    --hash=sha256:dafca5b9e384f0e419294eb4d2ff9fa826435bf15f15b7bd45723e8ad76811b2
     # via readme-renderer
 dparse==0.6.4b0 \
     --hash=sha256:592ff183348b8a5ea0a18442a7965e29445d3a26063654ec2c7e8ef42cd5753c \
     --hash=sha256:f8d49b41a527f3d16a269f854e6665245b325e50e41d2c213810cb984553e5c8
     # via
     #   safety
     #   safety-schemas
 editorconfig==0.12.4 \
     --hash=sha256:24857fa1793917dd9ccf0c7810a07e05404ce9b823521c7dce22a4fb5d125f80
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-filelock==3.13.4 \
-    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
-    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
+filelock==3.14.0 \
+    --hash=sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f \
+    --hash=sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0 \
     --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
     --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
     # via
     #   flake8-bugbear
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-flake8-bugbear==24.2.6 \
-    --hash=sha256:663ef5de80cd32aacd39d362212983bc4636435a6f83700b4ed35acbd0b7d1b8 \
-    --hash=sha256:f9cb5f2a9e792dd80ff68e89a14c12eed8620af8b41a49d823b7a33064ac9658
+flake8-bugbear==24.4.26 \
+    --hash=sha256:cb430dd86bc821d79ccc0b030789a9c87a47a369667f12ba06e80f11305e8258 \
+    --hash=sha256:ff8d4ba5719019ebf98e754624c30c05cef0dadcf18a65d91c7567300e52a130
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
 flynt==1.0.1 \
     --hash=sha256:65d1c546434827275123222a98408e9561bcd67db832dd58f530ff17b8329ec1 \
     --hash=sha256:988aac00672a5469726cc0a17cef7d1178c284a9fe8563458db2475d0aaed965
     # via darker
-frozendict==2.4.1 \
-    --hash=sha256:0187974c3cfc0ac77dc20f9af272f69c8436d2e994dfce85eb7cca269f4d0b7a \
-    --hash=sha256:107a9953272410cd05fcfba4dcf31f01825cd6b3c17f3cf616072e9611480034 \
-    --hash=sha256:1b01ebe8772ab30ab593e72dfe3f06e5d97db508bfd72613c243fd08f5ba96e4 \
-    --hash=sha256:1b32eb2f30bb734b7a699ee7003c86f81964f1c3b6e0e0f18efcbbdeb5b220bf \
-    --hash=sha256:1ed0f607c73e6482e8a8080ea22d9d9f057f0624225e04e7e3e16a94ec215827 \
-    --hash=sha256:2dfeca22e383d64d92301378ca5d10265d7ef05d989501ea5f37520052a0c9fd \
-    --hash=sha256:2f7b202617b410f9b8d528ce82cdb4b16a7e80ccd58601d0d1d8e15231e49292 \
-    --hash=sha256:2fa000d16b1af7315b8d9fbc15e6929303e1c447a9f06c10bfef62b7c9ea266f \
-    --hash=sha256:42077b882ed0e117e1b7f9c7b00453aecddbe268a80f5ca1a73c163c79025dbb \
-    --hash=sha256:42b3906ac43cf2c77f1e69fe7bdd93347044d1a0bc15bf5b733d47c39bfe2e3a \
-    --hash=sha256:4d2d2987b280fae3b46a77cbc3d51394b671c8d8b7270ab2e6d767a42dac15b1 \
-    --hash=sha256:4e8477396a166f5b8cfaaebd623ff05b7bacca830afa8e8d377ad3ed951a8bb2 \
-    --hash=sha256:4fc7b05120500e13a2f319ba4cbfba7f832c04441348ca20dbdcf776b5d2332f \
-    --hash=sha256:53eb5d19ff5b71d3f7806620000e80c1d2478a22c481799ea7b16fb218d42923 \
-    --hash=sha256:5b64b5c6ac3542a4028a431c01d39c60bfb809316cdd8c940d252d084437787f \
-    --hash=sha256:7bd5b958264646ca0c5589a4c82ec4be2bf7ff0d4d1202b9d9599f24be4d51c7 \
-    --hash=sha256:7cc4f1be80760080ca9ee83977c43ad202db91d0ee1e46e9f7c44ebcc05a3b81 \
-    --hash=sha256:7d6b51d2a726ecb169765261bd7e73f63669cf849e882d94d382d8ff682f0292 \
-    --hash=sha256:81ffbac40077c6f56355d47e18adb36e11816ae114ca9d9ee90b842b907d92f5 \
-    --hash=sha256:884a3cbaff8cfd1b36f07a8749b48a6cfebd7fca196e13b9664d33df38b38d27 \
-    --hash=sha256:9030e487d0d433aeaf2d7f741a47d9b890e2572951588f80f29d0161cfd5553a \
-    --hash=sha256:971017c706db1b76abdd7db285592d9f232aff6e8f47dffbd1cd0a020873b164 \
-    --hash=sha256:992cc157b6cdf788c1f24ab9531ba37104aba2d21f1520949a03bf3f9af7935e \
-    --hash=sha256:9f0172c1c3a52714b6530ec56621a6be2962776fa1a4638c4e40576b32e33355 \
-    --hash=sha256:a571fbbe8c0cb0d0d31dce24b1026301013d3884b2fc3099741ba7a9bd5764df \
-    --hash=sha256:accdebc212ef31e0de5b54fbeb275f79c5380e02b250b3d1c4341f6ccf73e876 \
-    --hash=sha256:ace99e4430802bb3d52969870a9432d68919cd33af18f9086ccd6a3a46ac6e7c \
-    --hash=sha256:b06df1995b14fca1e9acc53b1423a4c2dca072517acd619c1576fc6b352428ec \
-    --hash=sha256:c113eb12f0713b53f6d0bbf3bced19dd429e17cac1cf3c350bf05c82c573613d \
-    --hash=sha256:ccf4943a5276a99ff98000890fcbc76fcbc5f43f51250270ddab65da0ee61883 \
-    --hash=sha256:d1b02f873866f5d245a4bc4f9f2647aacb0d5f9a4d47e1de52c46cf03368c8cc \
-    --hash=sha256:d5619bd7f092b1f7ab69163ddcdff674e6786b7a19aea1217a6a46b942430631 \
-    --hash=sha256:d8312598598c9e79653da50c49315fc89d017dbaa4406160958c64d85a707edd \
-    --hash=sha256:de9f7194f4edbacdc609c66f49f583a658ec130e0f68e482fccae35d1befddaf \
-    --hash=sha256:ee12840600814adf4fb1fb84eafb8098bf1701d536949ead096158e3b11cf6f8 \
-    --hash=sha256:eebe6b4c054f987d83477f797f24a149ed409e8dc1c11c1fedc98d721f6ea905
+frozendict==2.4.4 \
+    --hash=sha256:07c3a5dee8bbb84cba770e273cdbf2c87c8e035903af8f781292d72583416801 \
+    --hash=sha256:12a342e439aef28ccec533f0253ea53d75fe9102bd6ea928ff530e76eac38906 \
+    --hash=sha256:1697793b5f62b416c0fc1d94638ec91ed3aa4ab277f6affa3a95216ecb3af170 \
+    --hash=sha256:199a4d32194f3afed6258de7e317054155bc9519252b568d9cfffde7e4d834e5 \
+    --hash=sha256:259528ba6b56fa051bc996f1c4d8b57e30d6dd3bc2f27441891b04babc4b5e73 \
+    --hash=sha256:2b70b431e3a72d410a2cdf1497b3aba2f553635e0c0f657ce311d841bf8273b6 \
+    --hash=sha256:2bd009cf4fc47972838a91e9b83654dc9a095dc4f2bb3a37c3f3124c8a364543 \
+    --hash=sha256:2d8536e068d6bf281f23fa835ac07747fb0f8851879dd189e9709f9567408b4d \
+    --hash=sha256:3148062675536724502c6344d7c485dd4667fdf7980ca9bd05e338ccc0c4471e \
+    --hash=sha256:3f7c031b26e4ee6a3f786ceb5e3abf1181c4ade92dce1f847da26ea2c96008c7 \
+    --hash=sha256:4297d694eb600efa429769125a6f910ec02b85606f22f178bafbee309e7d3ec7 \
+    --hash=sha256:4a59578d47b3949437519b5c39a016a6116b9e787bb19289e333faae81462e59 \
+    --hash=sha256:4ae8d05c8d0b6134bfb6bfb369d5fa0c4df21eabb5ca7f645af95fdc6689678e \
+    --hash=sha256:5d58d9a8d9e49662c6dafbea5e641f97decdb3d6ccd76e55e79818415362ba25 \
+    --hash=sha256:63aa49f1919af7d45fb8fd5dec4c0859bc09f46880bd6297c79bb2db2969b63d \
+    --hash=sha256:6874fec816b37b6eb5795b00e0574cba261bf59723e2de607a195d5edaff0786 \
+    --hash=sha256:6eb716e6a6d693c03b1d53280a1947716129f5ef9bcdd061db5c17dea44b80fe \
+    --hash=sha256:705efca8d74d3facbb6ace80ab3afdd28eb8a237bfb4063ed89996b024bc443d \
+    --hash=sha256:78c94991944dd33c5376f720228e5b252ee67faf3bac50ef381adc9e51e90d9d \
+    --hash=sha256:7f79c26dff10ce11dad3b3627c89bb2e87b9dd5958c2b24325f16a23019b8b94 \
+    --hash=sha256:7fee9420475bb6ff357000092aa9990c2f6182b2bab15764330f4ad7de2eae49 \
+    --hash=sha256:812ab17522ba13637826e65454115a914c2da538356e85f43ecea069813e4b33 \
+    --hash=sha256:85375ec6e979e6373bffb4f54576a68bf7497c350861d20686ccae38aab69c0a \
+    --hash=sha256:87ebcde21565a14fe039672c25550060d6f6d88cf1f339beac094c3b10004eb0 \
+    --hash=sha256:93a7b19afb429cbf99d56faf436b45ef2fa8fe9aca89c49eb1610c3bd85f1760 \
+    --hash=sha256:b3b967d5065872e27b06f785a80c0ed0a45d1f7c9b85223da05358e734d858ca \
+    --hash=sha256:c6bf9260018d653f3cab9bd147bd8592bf98a5c6e338be0491ced3c196c034a3 \
+    --hash=sha256:c8f92425686323a950337da4b75b4c17a3327b831df8c881df24038d560640d4 \
+    --hash=sha256:d13b4310db337f4d2103867c5a05090b22bc4d50ca842093779ef541ea9c9eea \
+    --hash=sha256:d9647563e76adb05b7cde2172403123380871360a114f546b4ae1704510801e5 \
+    --hash=sha256:dc2228874eacae390e63fd4f2bb513b3144066a977dc192163c9f6c7f6de6474 \
+    --hash=sha256:e1b941132d79ce72d562a13341d38fc217bc1ee24d8c35a20d754e79ff99e038 \
+    --hash=sha256:fefeb700bc7eb8b4c2dc48704e4221860d254c8989fb53488540bc44e44a1ac2
     # via ha-services
-graylint==1.0.1 \
-    --hash=sha256:857c84bd430ccf261b0acd80d565b6d16dba6fa5055ddbe6d738eda5a59a59ba \
-    --hash=sha256:ab433865aacd5f072edd5fc2db3938aaf10d869c2e5d266821f2d1fb87574dd6
+graylint==1.1.1 \
+    --hash=sha256:0fd8e02972ca03d0ef2bf0adea76b5343efcd492d7afb5f658f3e3a724f55a36 \
+    --hash=sha256:b7e0eab6c159684dbf5ef84e942c3340f6a6549b02a3d11b1a1763cc4f8f0593
     # via darker
-ha-services==2.5.0 \
-    --hash=sha256:7dce3cb3804f52aa66b5b737661b0f6618a8af24ceb7575574ac03f56d371248 \
-    --hash=sha256:fab10eacd2cb910b29b64fe6d8708f255da98d12f53ce08f5293790ab13b5e16
+ha-services==2.6.0 \
+    --hash=sha256:55468ad8454e0b87a1f0ec5b934b1c98d864a1ae200faf4bdc3efd5c8c61c963 \
+    --hash=sha256:d6887bdfda0a014ca4cf77fa08897604db0692d680fe1a7cc7c72644fdd288db
     # via tinkerforge2mqtt (pyproject.toml)
 idna==3.7 \
     --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
     --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 importlib-metadata==7.1.0 \
     --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
@@ -483,33 +480,33 @@
     --hash=sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd \
     --hash=sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790
     # via keyring
 jaraco-context==5.3.0 \
     --hash=sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266 \
     --hash=sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2
     # via keyring
-jaraco-functools==4.0.0 \
-    --hash=sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925 \
-    --hash=sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d
+jaraco-functools==4.0.1 \
+    --hash=sha256:3b24ccb921d6b593bdceb56ce14799204f473976e2a9d4b15b04d0f2c2326664 \
+    --hash=sha256:d33fa765374c0611b52f8b3a795f8900869aa88c84769d4d1746cd68fb28c3e8
     # via keyring
 jeepney==0.8.0 \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.3 \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+jinja2==3.1.4 \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
     # via
     #   cookiecutter
     #   safety
-keyring==25.1.0 \
-    --hash=sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427 \
-    --hash=sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893
+keyring==25.2.1 \
+    --hash=sha256:2458681cdefc0dbc0b7eb6cf75d0b98e59f9ad9b2d4edd319d18f68bdca95e50 \
+    --hash=sha256:daaffd42dbda25ddafb1ad5fec4024e5bbcfe424597ca1ca452b299861e49f1b
     # via twine
 manageprojects==0.17.1 \
     --hash=sha256:355d970261f14b53b574d102e7e82462fe6769baa06c479f00f07a0bcfcb8e4d \
     --hash=sha256:4662ff7f0e64ea9b420b67c270594c88542858a1434ebe8b5f93b7bf2ae2e706
     # via tinkerforge2mqtt (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
@@ -573,17 +570,17 @@
     --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
     --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
     --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
     --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
     --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
     --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
     # via jinja2
-marshmallow==3.21.1 \
-    --hash=sha256:4e65e9e0d80fc9e609574b9983cf32579f305c718afb30d7233ab818571768c3 \
-    --hash=sha256:f085493f79efb0644f270a9bf2892843142d80d7174bbbd2f3713f2a589dc633
+marshmallow==3.21.2 \
+    --hash=sha256:70b54a6282f4704d12c0a41599682c5c5450e843b9ec406308653b47c59648a1 \
+    --hash=sha256:82408deadd8b33d56338d2182d455db632c6313aa2af61916672146bb32edc56
     # via safety
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
     # via flake8
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
@@ -629,42 +626,42 @@
     --hash=sha256:e77e56ffe2701e83a96e35770c6adb655ffc074d530018d1b584a8e635b4f36f \
     --hash=sha256:e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466 \
     --hash=sha256:f7d9faed6dfff654a9ca7d9b0068456517f63dbc3aa704a527f493b9200b210a \
     --hash=sha256:fac5834e14ac4da1fca373753e0c4ec9c8069d1fe5f534fa5208453b6065d5be \
     --hash=sha256:fd62e5818731a66aaa8e9b0a1e5543dc979a46278da01e85c3c9a1a4f047ef7e \
     --hash=sha256:fda4c357145cf0b760000c4ad597e19b53adf01382b711f281720a10a0fe72b7
     # via ha-services
-mypy==1.9.0 \
-    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
-    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
-    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
-    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
-    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
-    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
-    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
-    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
-    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
-    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
-    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
-    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
-    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
-    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
-    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
-    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
-    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
-    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
-    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
-    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
-    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
-    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
-    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
-    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
-    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
-    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
-    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
+mypy==1.10.0 \
+    --hash=sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061 \
+    --hash=sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99 \
+    --hash=sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de \
+    --hash=sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a \
+    --hash=sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9 \
+    --hash=sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec \
+    --hash=sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1 \
+    --hash=sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131 \
+    --hash=sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f \
+    --hash=sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821 \
+    --hash=sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5 \
+    --hash=sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee \
+    --hash=sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e \
+    --hash=sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746 \
+    --hash=sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2 \
+    --hash=sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0 \
+    --hash=sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b \
+    --hash=sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53 \
+    --hash=sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30 \
+    --hash=sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda \
+    --hash=sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051 \
+    --hash=sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2 \
+    --hash=sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7 \
+    --hash=sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee \
+    --hash=sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727 \
+    --hash=sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976 \
+    --hash=sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4
     # via
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
@@ -697,40 +694,40 @@
     #   cli-base-utilities
     #   dparse
     #   marshmallow
     #   pyproject-api
     #   safety
     #   safety-schemas
     #   tox
-paho-mqtt==2.0.0 \
-    --hash=sha256:13b205f29251e4f2c66a6c923c31fc4fd780561e03b2d775cff8e4f2915cf947 \
-    --hash=sha256:2ef745073dfc9aa68bfec30d0b9b6f0304ea75182bae85a7c77a80cefce1eff5
+paho-mqtt==2.1.0 \
+    --hash=sha256:12d6e7511d4137555a3f6ea167ae846af2c7357b10bc6fa4f7c3968fc1723834 \
+    --hash=sha256:6db9ba9b34ed5bc6b6e3812718c7e06e2fd7444540df2455d2c51bd58808feee
     # via ha-services
 pathspec==0.12.1 \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
     # via black
 pip-tools==7.4.1 \
     --hash=sha256:4c690e5fbae2f21e87843e89c26191f0d9454f362d8acdbd695716493ec8b3a9 \
     --hash=sha256:864826f5073864450e24dbeeb85ce3920cdfb09848a3d69ebf537b521f14bcc9
     # via tinkerforge2mqtt (pyproject.toml)
 pkginfo==1.10.0 \
     --hash=sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297 \
     --hash=sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097
     # via twine
-platformdirs==4.2.0 \
-    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
-    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
+platformdirs==4.2.2 \
+    --hash=sha256:2d7a1657e36a80ea911db832a8a6ece5ee53d8de21edd5cc5879af6530b1bfee \
+    --hash=sha256:38b7b51f512eed9e84a22788b4bce1de17c0adb134d6becb09836e37d8654cd3
     # via
     #   black
     #   tox
     #   virtualenv
-pluggy==1.4.0 \
-    --hash=sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981 \
-    --hash=sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be
+pluggy==1.5.0 \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
     # via tox
 psutil==5.9.8 \
     --hash=sha256:02615ed8c5ea222323408ceba16c60e99c3f91639b07da6373fb7e6539abc56d \
     --hash=sha256:05806de88103b25903dff19bb6692bd2e714ccf9e668d050d144012055cbca73 \
     --hash=sha256:26bd09967ae00920df88e0352a91cff1a78f8d69b3ecabbfe733610c0af486c8 \
     --hash=sha256:27cc40c3493bb10de1be4b3f07cae4c010ce715290a5be22b98493509c6299e2 \
     --hash=sha256:36f435891adb138ed3c9e58c6af3e2e6ca9ac2f365efe1f9cfef2794e6c93b4e \
@@ -752,123 +749,123 @@
     # via
     #   autopep8
     #   flake8
 pycparser==2.22 \
     --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
     --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
     # via cffi
-pydantic==2.7.0 \
-    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
-    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
+pydantic==2.7.1 \
+    --hash=sha256:e029badca45266732a9a79898a15ae2e8b14840b1eabbb25844be28f0b33f3d5 \
+    --hash=sha256:e9dbb5eada8abe4d9ae5f46b9939aead650cd2b68f249bb3a8139dbe125803cc
     # via
     #   safety
     #   safety-schemas
-pydantic-core==2.18.1 \
-    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
-    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
-    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
-    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
-    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
-    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
-    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
-    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
-    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
-    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
-    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
-    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
-    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
-    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
-    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
-    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
-    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
-    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
-    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
-    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
-    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
-    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
-    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
-    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
-    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
-    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
-    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
-    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
-    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
-    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
-    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
-    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
-    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
-    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
-    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
-    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
-    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
-    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
-    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
-    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
-    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
-    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
-    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
-    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
-    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
-    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
-    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
-    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
-    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
-    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
-    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
-    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
-    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
-    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
-    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
-    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
-    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
-    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
-    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
-    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
-    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
-    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
-    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
-    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
-    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
-    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
-    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
-    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
-    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
-    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
-    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
-    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
-    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
-    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
-    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
-    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
-    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
-    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
-    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
+pydantic-core==2.18.2 \
+    --hash=sha256:0098300eebb1c837271d3d1a2cd2911e7c11b396eac9661655ee524a7f10587b \
+    --hash=sha256:042473b6280246b1dbf530559246f6842b56119c2926d1e52b631bdc46075f2a \
+    --hash=sha256:05b7133a6e6aeb8df37d6f413f7705a37ab4031597f64ab56384c94d98fa0e90 \
+    --hash=sha256:0680b1f1f11fda801397de52c36ce38ef1c1dc841a0927a94f226dea29c3ae3d \
+    --hash=sha256:0d69b4c2f6bb3e130dba60d34c0845ba31b69babdd3f78f7c0c8fae5021a253e \
+    --hash=sha256:1404c69d6a676245199767ba4f633cce5f4ad4181f9d0ccb0577e1f66cf4c46d \
+    --hash=sha256:182245ff6b0039e82b6bb585ed55a64d7c81c560715d1bad0cbad6dfa07b4027 \
+    --hash=sha256:1a388a77e629b9ec814c1b1e6b3b595fe521d2cdc625fcca26fbc2d44c816804 \
+    --hash=sha256:1d90c3265ae107f91a4f279f4d6f6f1d4907ac76c6868b27dc7fb33688cfb347 \
+    --hash=sha256:20aca1e2298c56ececfd8ed159ae4dde2df0781988c97ef77d5c16ff4bd5b400 \
+    --hash=sha256:219da3f096d50a157f33645a1cf31c0ad1fe829a92181dd1311022f986e5fbe3 \
+    --hash=sha256:22057013c8c1e272eb8d0eebc796701167d8377441ec894a8fed1af64a0bf399 \
+    --hash=sha256:223ee893d77a310a0391dca6df00f70bbc2f36a71a895cecd9a0e762dc37b349 \
+    --hash=sha256:224c421235f6102e8737032483f43c1a8cfb1d2f45740c44166219599358c2cd \
+    --hash=sha256:2334ce8c673ee93a1d6a65bd90327588387ba073c17e61bf19b4fd97d688d63c \
+    --hash=sha256:269322dcc3d8bdb69f054681edff86276b2ff972447863cf34c8b860f5188e2e \
+    --hash=sha256:2728b01246a3bba6de144f9e3115b532ee44bd6cf39795194fb75491824a1413 \
+    --hash=sha256:2b8ed04b3582771764538f7ee7001b02e1170223cf9b75dff0bc698fadb00cf3 \
+    --hash=sha256:2e29d20810dfc3043ee13ac7d9e25105799817683348823f305ab3f349b9386e \
+    --hash=sha256:36789b70d613fbac0a25bb07ab3d9dba4d2e38af609c020cf4d888d165ee0bf3 \
+    --hash=sha256:390193c770399861d8df9670fb0d1874f330c79caaca4642332df7c682bf6b91 \
+    --hash=sha256:3a6515ebc6e69d85502b4951d89131ca4e036078ea35533bb76327f8424531ce \
+    --hash=sha256:3f9a801e7c8f1ef8718da265bba008fa121243dfe37c1cea17840b0944dfd72c \
+    --hash=sha256:43f0f463cf89ace478de71a318b1b4f05ebc456a9b9300d027b4b57c1a2064fb \
+    --hash=sha256:4456f2dca97c425231d7315737d45239b2b51a50dc2b6f0c2bb181fce6207664 \
+    --hash=sha256:470b94480bb5ee929f5acba6995251ada5e059a5ef3e0dfc63cca287283ebfa6 \
+    --hash=sha256:4774f3184d2ef3e14e8693194f661dea5a4d6ca4e3dc8e39786d33a94865cefd \
+    --hash=sha256:4b4356d3538c3649337df4074e81b85f0616b79731fe22dd11b99499b2ebbdf3 \
+    --hash=sha256:553ef617b6836fc7e4df130bb851e32fe357ce36336d897fd6646d6058d980af \
+    --hash=sha256:6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043 \
+    --hash=sha256:6a46e22a707e7ad4484ac9ee9f290f9d501df45954184e23fc29408dfad61350 \
+    --hash=sha256:6e5c584d357c4e2baf0ff7baf44f4994be121e16a2c88918a5817331fc7599d7 \
+    --hash=sha256:75250dbc5290e3f1a0f4618db35e51a165186f9034eff158f3d490b3fed9f8a0 \
+    --hash=sha256:75f7e9488238e920ab6204399ded280dc4c307d034f3924cd7f90a38b1829563 \
+    --hash=sha256:78363590ef93d5d226ba21a90a03ea89a20738ee5b7da83d771d283fd8a56761 \
+    --hash=sha256:7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72 \
+    --hash=sha256:800d60565aec896f25bc3cfa56d2277d52d5182af08162f7954f938c06dc4ee3 \
+    --hash=sha256:82d5d4d78e4448683cb467897fe24e2b74bb7b973a541ea1dcfec1d3cbce39fb \
+    --hash=sha256:852e966fbd035a6468fc0a3496589b45e2208ec7ca95c26470a54daed82a0788 \
+    --hash=sha256:868649da93e5a3d5eacc2b5b3b9235c98ccdbfd443832f31e075f54419e1b96b \
+    --hash=sha256:886eec03591b7cf058467a70a87733b35f44707bd86cf64a615584fd72488b7c \
+    --hash=sha256:8b172601454f2d7701121bbec3425dd71efcb787a027edf49724c9cefc14c038 \
+    --hash=sha256:95b9d5e72481d3780ba3442eac863eae92ae43a5f3adb5b4d0a1de89d42bb250 \
+    --hash=sha256:98758d627ff397e752bc339272c14c98199c613f922d4a384ddc07526c86a2ec \
+    --hash=sha256:997abc4df705d1295a42f95b4eec4950a37ad8ae46d913caeee117b6b198811c \
+    --hash=sha256:9b5155ff768083cb1d62f3e143b49a8a3432e6789a3abee8acd005c3c7af1c74 \
+    --hash=sha256:9e08e867b306f525802df7cd16c44ff5ebbe747ff0ca6cf3fde7f36c05a59a81 \
+    --hash=sha256:9fdad8e35f278b2c3eb77cbdc5c0a49dada440657bf738d6905ce106dc1de439 \
+    --hash=sha256:a1874c6dd4113308bd0eb568418e6114b252afe44319ead2b4081e9b9521fe75 \
+    --hash=sha256:a8309f67285bdfe65c372ea3722b7a5642680f3dba538566340a9d36e920b5f0 \
+    --hash=sha256:ae0a8a797a5e56c053610fa7be147993fe50960fa43609ff2a9552b0e07013e8 \
+    --hash=sha256:b14d82cdb934e99dda6d9d60dc84a24379820176cc4a0d123f88df319ae9c150 \
+    --hash=sha256:b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438 \
+    --hash=sha256:b3ef08e20ec49e02d5c6717a91bb5af9b20f1805583cb0adfe9ba2c6b505b5ae \
+    --hash=sha256:b89ed9eb7d616ef5714e5590e6cf7f23b02d0d539767d33561e3675d6f9e3857 \
+    --hash=sha256:c4fcf5cd9c4b655ad666ca332b9a081112cd7a58a8b5a6ca7a3104bc950f2038 \
+    --hash=sha256:c6fdc8627910eed0c01aed6a390a252fe3ea6d472ee70fdde56273f198938374 \
+    --hash=sha256:c9bd70772c720142be1020eac55f8143a34ec9f82d75a8e7a07852023e46617f \
+    --hash=sha256:ca7b0c1f1c983e064caa85f3792dd2fe3526b3505378874afa84baf662e12241 \
+    --hash=sha256:cbca948f2d14b09d20268cda7b0367723d79063f26c4ffc523af9042cad95592 \
+    --hash=sha256:cc1cfd88a64e012b74e94cd00bbe0f9c6df57049c97f02bb07d39e9c852e19a4 \
+    --hash=sha256:ccdd111c03bfd3666bd2472b674c6899550e09e9f298954cfc896ab92b5b0e6d \
+    --hash=sha256:cfeecd1ac6cc1fb2692c3d5110781c965aabd4ec5d32799773ca7b1456ac636b \
+    --hash=sha256:d4d938ec0adf5167cb335acb25a4ee69a8107e4984f8fbd2e897021d9e4ca21b \
+    --hash=sha256:d7d904828195733c183d20a54230c0df0eb46ec746ea1a666730787353e87182 \
+    --hash=sha256:d91cb5ea8b11607cc757675051f61b3d93f15eca3cefb3e6c704a5d6e8440f4e \
+    --hash=sha256:d9319e499827271b09b4e411905b24a426b8fb69464dfa1696258f53a3334641 \
+    --hash=sha256:e0e8b1be28239fc64a88a8189d1df7fad8be8c1ae47fcc33e43d4be15f99cc70 \
+    --hash=sha256:e18609ceaa6eed63753037fc06ebb16041d17d28199ae5aba0052c51449650a9 \
+    --hash=sha256:e1b395e58b10b73b07b7cf740d728dd4ff9365ac46c18751bf8b3d8cca8f625a \
+    --hash=sha256:e23ec367a948b6d812301afc1b13f8094ab7b2c280af66ef450efc357d2ae543 \
+    --hash=sha256:e25add29b8f3b233ae90ccef2d902d0ae0432eb0d45370fe315d1a5cf231004b \
+    --hash=sha256:e6dac87ddb34aaec85f873d737e9d06a3555a1cc1a8e0c44b7f8d5daeb89d86f \
+    --hash=sha256:ef26c9e94a8c04a1b2924149a9cb081836913818e55681722d7f29af88fe7b38 \
+    --hash=sha256:eff2de745698eb46eeb51193a9f41d67d834d50e424aef27df2fcdee1b153845 \
+    --hash=sha256:f0a21cbaa69900cbe1a2e7cad2aa74ac3cf21b10c3efb0fa0b80305274c0e8a2 \
+    --hash=sha256:f459a5ce8434614dfd39bbebf1041952ae01da6bed9855008cb33b875cb024c0 \
+    --hash=sha256:f93a8a2e3938ff656a7c1bc57193b1319960ac015b6e87d76c76bf14fe0244b4 \
+    --hash=sha256:fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
     # via pydantic
 pyflakes==3.2.0 \
     --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
     --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
     # via
     #   autoflake
     #   flake8
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
-pygments==2.17.2 \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
+pygments==2.18.0 \
+    --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
+    --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
     # via
     #   darker
     #   readme-renderer
     #   rich
 pyproject-api==1.6.1 \
     --hash=sha256:1817dc018adc0d1ff9ca1ed8c60e1623d5aaca40814b953af14a9cf9a5cae538 \
     --hash=sha256:4c0116d60476b0786c88692cf4e325a9814965e2469c5998b830bba16b183675
     # via tox
-pyproject-hooks==1.0.0 \
-    --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
-    --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
+pyproject-hooks==1.1.0 \
+    --hash=sha256:4b37730834edbd6bd37f26ece6b44802fb1c1ee2ece0e54ddff8bfc06db86965 \
+    --hash=sha256:7ceeefe9aec63a1064c18d939bdc3adf2d8aa1988a510afec15151578b232aa2
     # via
     #   build
     #   pip-tools
 python-dateutil==2.9.0.post0 \
     --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
     --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
     # via arrow
@@ -964,17 +961,17 @@
     #   ha-services
     #   manageprojects
     #   rich-click
     #   safety
     #   tinkerforge2mqtt (pyproject.toml)
     #   twine
     #   typer
-rich-click==1.7.4 \
-    --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
-    --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
+rich-click==1.8.2 \
+    --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
+    --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
     # via
     #   cli-base-utilities
     #   ha-services
     #   manageprojects
     #   tinkerforge2mqtt (pyproject.toml)
 ruamel-yaml==0.18.6 \
     --hash=sha256:57b53ba33def16c4f3d807c0ccbc00f8a6081827e81ba2491691b76882d0c636 \
@@ -1030,17 +1027,17 @@
     --hash=sha256:e2b4c44b60eadec492926a7270abb100ef9f72798e18743939bdbf037aab8c28 \
     --hash=sha256:e79e5db08739731b0ce4850bed599235d601701d5694c36570a99a0c5ca41a9d \
     --hash=sha256:ebc06178e8821efc9692ea7544aa5644217358490145629914d8020042c24aa1 \
     --hash=sha256:edaef1c1200c4b4cb914583150dcaa3bc30e592e907c01117c08b13a07255ec2 \
     --hash=sha256:f481f16baec5290e45aebdc2a5168ebc6d35189ae6fea7a58787613a25f6e875 \
     --hash=sha256:fff3573c2db359f091e1589c3d7c5fc2f86f5bdb6f24252c2d8e539d4e45f412
     # via ruamel-yaml
-safety==3.1.0 \
-    --hash=sha256:71f47b82ece153ec2f240e277f7cbfa70d5da2e0d143162c67f63b2f7459a1aa \
-    --hash=sha256:f2ba2d36f15ac1e24751547a73b854509a7d6db31efd30b57f64ffdf9d021934
+safety==3.2.0 \
+    --hash=sha256:8bd5cab5f3d8a61ce0ea6e98f267c1006d056097c45c644fee7afeff7d5949c1 \
+    --hash=sha256:a432fc9d17e79a4386c4f093656b617c56f839cde022649cfa796d72c7a544de
     # via tinkerforge2mqtt (pyproject.toml)
 safety-schemas==0.0.2 \
     --hash=sha256:277c077ce6e53221874a87c29515ffdd2f3773a6db4d035a9f67cc98db3b8c7f \
     --hash=sha256:7d1b040ec06480f05cff6b45ea7a93e09c8942df864fb0d01ddeb67c323cfa8c
     # via safety
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
@@ -1073,28 +1070,28 @@
     #   darkgraylib
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   cli-base-utilities
     #   tinkerforge2mqtt (pyproject.toml)
-tomlkit==0.12.4 \
-    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
-    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+tomlkit==0.12.5 \
+    --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
+    --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
     # via
     #   cli-base-utilities
     #   ha-services
     #   manageprojects
-tox==4.14.2 \
-    --hash=sha256:0defb44f6dafd911b61788325741cc6b2e12ea71f987ac025ad4d649f1f1a104 \
-    --hash=sha256:2900c4eb7b716af4a928a7fdc2ed248ad6575294ed7cfae2ea41203937422847
+tox==4.15.0 \
+    --hash=sha256:300055f335d855b2ab1b12c5802de7f62a36d4fd53f30bd2835f6a201dda46ea \
+    --hash=sha256:7a0beeef166fbe566f54f795b4906c31b428eddafc0102ac00d20998dd1933f6
     # via tinkerforge2mqtt (pyproject.toml)
-twine==5.0.0 \
-    --hash=sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4 \
-    --hash=sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0
+twine==5.1.0 \
+    --hash=sha256:4d74770c88c4fcaf8134d2a6a9d863e40f08255ff7d8e2acb3cbbd57d25f6e9d \
+    --hash=sha256:fe1d814395bfe50cfbe27783cb74efe93abeac3f66deaeb6c8390e4e92bacb43
     # via tinkerforge2mqtt (pyproject.toml)
 typeguard==4.2.1 \
     --hash=sha256:7da3bd46e61f03e0852f8d251dcbdc2a336aa495d7daff01e092b55327796eb8 \
     --hash=sha256:c556a1b95948230510070ca53fa0341fb0964611bd05d598d87fb52115d65fee
     # via tinkerforge2mqtt (pyproject.toml)
 typer==0.12.3 \
     --hash=sha256:070d7ca53f785acbccba8e7d28b08dcd88f79f1fbda035ade0aecec71ca5c914 \
@@ -1120,31 +1117,31 @@
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via
     #   requests
     #   safety
     #   tinkerforge2mqtt (pyproject.toml)
     #   twine
-virtualenv==20.25.1 \
-    --hash=sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a \
-    --hash=sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197
+virtualenv==20.26.2 \
+    --hash=sha256:82bf0f4eebbb78d36ddaee0283d43fe5736b53880b8a8cdcd37390a07ac3741c \
+    --hash=sha256:a624db5e94f01ad993d476b9ee5346fdf7b9de43ccaee0e0197012dc838a0e9b
     # via tox
 wheel==0.43.0 \
     --hash=sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85 \
     --hash=sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81
     # via pip-tools
-zipp==3.18.1 \
-    --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
-    --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
+zipp==3.18.2 \
+    --hash=sha256:6278d9ddbcfb1f1089a88fde84481528b07b0e10474e09dcfe53dad4069fa059 \
+    --hash=sha256:dce197b859eb796242b0622af1b8beb0a722d52aa2f57133ead08edd5bf5374e
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0 \
     --hash=sha256:ba0d021a166865d2265246961bec0152ff124de910c5cc39f1156ce3fa7c69dc \
     --hash=sha256:ea9bd1a847e8c5774a5777bb398c19e80bcd4e2aa16a4b301b718fe6f593aba2
     # via pip-tools
-setuptools==69.3.0 \
-    --hash=sha256:48c518e350470d98cfa2944a31edbfc897c9a7d8fa4847da66d89f0f5fb64b57 \
-    --hash=sha256:e1fd0ca7ba442e4be8a415dcca867b8018777dd5f95f4492bb4dc7d77dbc8bd8
+setuptools==69.5.1 \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
     # via
     #   pip-tools
     #   safety
```

### Comparing `tinkerforge2mqtt-0.8/requirements.txt` & `tinkerforge2mqtt-0.9.0/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -24,55 +24,52 @@
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via
     #   cli-base-utilities
     #   ha-services
     #   rich-click
     #   tinkerforge2mqtt (pyproject.toml)
-frozendict==2.4.1 \
-    --hash=sha256:0187974c3cfc0ac77dc20f9af272f69c8436d2e994dfce85eb7cca269f4d0b7a \
-    --hash=sha256:107a9953272410cd05fcfba4dcf31f01825cd6b3c17f3cf616072e9611480034 \
-    --hash=sha256:1b01ebe8772ab30ab593e72dfe3f06e5d97db508bfd72613c243fd08f5ba96e4 \
-    --hash=sha256:1b32eb2f30bb734b7a699ee7003c86f81964f1c3b6e0e0f18efcbbdeb5b220bf \
-    --hash=sha256:1ed0f607c73e6482e8a8080ea22d9d9f057f0624225e04e7e3e16a94ec215827 \
-    --hash=sha256:2dfeca22e383d64d92301378ca5d10265d7ef05d989501ea5f37520052a0c9fd \
-    --hash=sha256:2f7b202617b410f9b8d528ce82cdb4b16a7e80ccd58601d0d1d8e15231e49292 \
-    --hash=sha256:2fa000d16b1af7315b8d9fbc15e6929303e1c447a9f06c10bfef62b7c9ea266f \
-    --hash=sha256:42077b882ed0e117e1b7f9c7b00453aecddbe268a80f5ca1a73c163c79025dbb \
-    --hash=sha256:42b3906ac43cf2c77f1e69fe7bdd93347044d1a0bc15bf5b733d47c39bfe2e3a \
-    --hash=sha256:4d2d2987b280fae3b46a77cbc3d51394b671c8d8b7270ab2e6d767a42dac15b1 \
-    --hash=sha256:4e8477396a166f5b8cfaaebd623ff05b7bacca830afa8e8d377ad3ed951a8bb2 \
-    --hash=sha256:4fc7b05120500e13a2f319ba4cbfba7f832c04441348ca20dbdcf776b5d2332f \
-    --hash=sha256:53eb5d19ff5b71d3f7806620000e80c1d2478a22c481799ea7b16fb218d42923 \
-    --hash=sha256:5b64b5c6ac3542a4028a431c01d39c60bfb809316cdd8c940d252d084437787f \
-    --hash=sha256:7bd5b958264646ca0c5589a4c82ec4be2bf7ff0d4d1202b9d9599f24be4d51c7 \
-    --hash=sha256:7cc4f1be80760080ca9ee83977c43ad202db91d0ee1e46e9f7c44ebcc05a3b81 \
-    --hash=sha256:7d6b51d2a726ecb169765261bd7e73f63669cf849e882d94d382d8ff682f0292 \
-    --hash=sha256:81ffbac40077c6f56355d47e18adb36e11816ae114ca9d9ee90b842b907d92f5 \
-    --hash=sha256:884a3cbaff8cfd1b36f07a8749b48a6cfebd7fca196e13b9664d33df38b38d27 \
-    --hash=sha256:9030e487d0d433aeaf2d7f741a47d9b890e2572951588f80f29d0161cfd5553a \
-    --hash=sha256:971017c706db1b76abdd7db285592d9f232aff6e8f47dffbd1cd0a020873b164 \
-    --hash=sha256:992cc157b6cdf788c1f24ab9531ba37104aba2d21f1520949a03bf3f9af7935e \
-    --hash=sha256:9f0172c1c3a52714b6530ec56621a6be2962776fa1a4638c4e40576b32e33355 \
-    --hash=sha256:a571fbbe8c0cb0d0d31dce24b1026301013d3884b2fc3099741ba7a9bd5764df \
-    --hash=sha256:accdebc212ef31e0de5b54fbeb275f79c5380e02b250b3d1c4341f6ccf73e876 \
-    --hash=sha256:ace99e4430802bb3d52969870a9432d68919cd33af18f9086ccd6a3a46ac6e7c \
-    --hash=sha256:b06df1995b14fca1e9acc53b1423a4c2dca072517acd619c1576fc6b352428ec \
-    --hash=sha256:c113eb12f0713b53f6d0bbf3bced19dd429e17cac1cf3c350bf05c82c573613d \
-    --hash=sha256:ccf4943a5276a99ff98000890fcbc76fcbc5f43f51250270ddab65da0ee61883 \
-    --hash=sha256:d1b02f873866f5d245a4bc4f9f2647aacb0d5f9a4d47e1de52c46cf03368c8cc \
-    --hash=sha256:d5619bd7f092b1f7ab69163ddcdff674e6786b7a19aea1217a6a46b942430631 \
-    --hash=sha256:d8312598598c9e79653da50c49315fc89d017dbaa4406160958c64d85a707edd \
-    --hash=sha256:de9f7194f4edbacdc609c66f49f583a658ec130e0f68e482fccae35d1befddaf \
-    --hash=sha256:ee12840600814adf4fb1fb84eafb8098bf1701d536949ead096158e3b11cf6f8 \
-    --hash=sha256:eebe6b4c054f987d83477f797f24a149ed409e8dc1c11c1fedc98d721f6ea905
+frozendict==2.4.4 \
+    --hash=sha256:07c3a5dee8bbb84cba770e273cdbf2c87c8e035903af8f781292d72583416801 \
+    --hash=sha256:12a342e439aef28ccec533f0253ea53d75fe9102bd6ea928ff530e76eac38906 \
+    --hash=sha256:1697793b5f62b416c0fc1d94638ec91ed3aa4ab277f6affa3a95216ecb3af170 \
+    --hash=sha256:199a4d32194f3afed6258de7e317054155bc9519252b568d9cfffde7e4d834e5 \
+    --hash=sha256:259528ba6b56fa051bc996f1c4d8b57e30d6dd3bc2f27441891b04babc4b5e73 \
+    --hash=sha256:2b70b431e3a72d410a2cdf1497b3aba2f553635e0c0f657ce311d841bf8273b6 \
+    --hash=sha256:2bd009cf4fc47972838a91e9b83654dc9a095dc4f2bb3a37c3f3124c8a364543 \
+    --hash=sha256:2d8536e068d6bf281f23fa835ac07747fb0f8851879dd189e9709f9567408b4d \
+    --hash=sha256:3148062675536724502c6344d7c485dd4667fdf7980ca9bd05e338ccc0c4471e \
+    --hash=sha256:3f7c031b26e4ee6a3f786ceb5e3abf1181c4ade92dce1f847da26ea2c96008c7 \
+    --hash=sha256:4297d694eb600efa429769125a6f910ec02b85606f22f178bafbee309e7d3ec7 \
+    --hash=sha256:4a59578d47b3949437519b5c39a016a6116b9e787bb19289e333faae81462e59 \
+    --hash=sha256:4ae8d05c8d0b6134bfb6bfb369d5fa0c4df21eabb5ca7f645af95fdc6689678e \
+    --hash=sha256:5d58d9a8d9e49662c6dafbea5e641f97decdb3d6ccd76e55e79818415362ba25 \
+    --hash=sha256:63aa49f1919af7d45fb8fd5dec4c0859bc09f46880bd6297c79bb2db2969b63d \
+    --hash=sha256:6874fec816b37b6eb5795b00e0574cba261bf59723e2de607a195d5edaff0786 \
+    --hash=sha256:6eb716e6a6d693c03b1d53280a1947716129f5ef9bcdd061db5c17dea44b80fe \
+    --hash=sha256:705efca8d74d3facbb6ace80ab3afdd28eb8a237bfb4063ed89996b024bc443d \
+    --hash=sha256:78c94991944dd33c5376f720228e5b252ee67faf3bac50ef381adc9e51e90d9d \
+    --hash=sha256:7f79c26dff10ce11dad3b3627c89bb2e87b9dd5958c2b24325f16a23019b8b94 \
+    --hash=sha256:7fee9420475bb6ff357000092aa9990c2f6182b2bab15764330f4ad7de2eae49 \
+    --hash=sha256:812ab17522ba13637826e65454115a914c2da538356e85f43ecea069813e4b33 \
+    --hash=sha256:85375ec6e979e6373bffb4f54576a68bf7497c350861d20686ccae38aab69c0a \
+    --hash=sha256:87ebcde21565a14fe039672c25550060d6f6d88cf1f339beac094c3b10004eb0 \
+    --hash=sha256:93a7b19afb429cbf99d56faf436b45ef2fa8fe9aca89c49eb1610c3bd85f1760 \
+    --hash=sha256:b3b967d5065872e27b06f785a80c0ed0a45d1f7c9b85223da05358e734d858ca \
+    --hash=sha256:c6bf9260018d653f3cab9bd147bd8592bf98a5c6e338be0491ced3c196c034a3 \
+    --hash=sha256:c8f92425686323a950337da4b75b4c17a3327b831df8c881df24038d560640d4 \
+    --hash=sha256:d13b4310db337f4d2103867c5a05090b22bc4d50ca842093779ef541ea9c9eea \
+    --hash=sha256:d9647563e76adb05b7cde2172403123380871360a114f546b4ae1704510801e5 \
+    --hash=sha256:dc2228874eacae390e63fd4f2bb513b3144066a977dc192163c9f6c7f6de6474 \
+    --hash=sha256:e1b941132d79ce72d562a13341d38fc217bc1ee24d8c35a20d754e79ff99e038 \
+    --hash=sha256:fefeb700bc7eb8b4c2dc48704e4221860d254c8989fb53488540bc44e44a1ac2
     # via ha-services
-ha-services==2.5.0 \
-    --hash=sha256:7dce3cb3804f52aa66b5b737661b0f6618a8af24ceb7575574ac03f56d371248 \
-    --hash=sha256:fab10eacd2cb910b29b64fe6d8708f255da98d12f53ce08f5293790ab13b5e16
+ha-services==2.6.0 \
+    --hash=sha256:55468ad8454e0b87a1f0ec5b934b1c98d864a1ae200faf4bdc3efd5c8c61c963 \
+    --hash=sha256:d6887bdfda0a014ca4cf77fa08897604db0692d680fe1a7cc7c72644fdd288db
     # via tinkerforge2mqtt (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
     # via rich
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
@@ -116,17 +113,17 @@
     --hash=sha256:fd62e5818731a66aaa8e9b0a1e5543dc979a46278da01e85c3c9a1a4f047ef7e \
     --hash=sha256:fda4c357145cf0b760000c4ad597e19b53adf01382b711f281720a10a0fe72b7
     # via ha-services
 packaging==24.0 \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
     --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
     # via cli-base-utilities
-paho-mqtt==2.0.0 \
-    --hash=sha256:13b205f29251e4f2c66a6c923c31fc4fd780561e03b2d775cff8e4f2915cf947 \
-    --hash=sha256:2ef745073dfc9aa68bfec30d0b9b6f0304ea75182bae85a7c77a80cefce1eff5
+paho-mqtt==2.1.0 \
+    --hash=sha256:12d6e7511d4137555a3f6ea167ae846af2c7357b10bc6fa4f7c3968fc1723834 \
+    --hash=sha256:6db9ba9b34ed5bc6b6e3812718c7e06e2fd7444540df2455d2c51bd58808feee
     # via ha-services
 psutil==5.9.8 \
     --hash=sha256:02615ed8c5ea222323408ceba16c60e99c3f91639b07da6373fb7e6539abc56d \
     --hash=sha256:05806de88103b25903dff19bb6692bd2e714ccf9e668d050d144012055cbca73 \
     --hash=sha256:26bd09967ae00920df88e0352a91cff1a78f8d69b3ecabbfe733610c0af486c8 \
     --hash=sha256:27cc40c3493bb10de1be4b3f07cae4c010ce715290a5be22b98493509c6299e2 \
     --hash=sha256:36f435891adb138ed3c9e58c6af3e2e6ca9ac2f365efe1f9cfef2794e6c93b4e \
@@ -138,43 +135,43 @@
     --hash=sha256:8db4c1b57507eef143a15a6884ca10f7c73876cdf5d51e713151c1236a0e68cf \
     --hash=sha256:aee678c8720623dc456fa20659af736241f575d79429a0e5e9cf88ae0605cc81 \
     --hash=sha256:bc56c2a1b0d15aa3eaa5a60c9f3f8e3e565303b465dbf57a1b730e7a2b9844e0 \
     --hash=sha256:bd1184ceb3f87651a67b2708d4c3338e9b10c5df903f2e3776b62303b26cb631 \
     --hash=sha256:d06016f7f8625a1825ba3732081d77c94589dca78b7a3fc072194851e88461a4 \
     --hash=sha256:d16bbddf0693323b8c6123dd804100241da461e41d6e332fb0ba6058f630f8c8
     # via ha-services
-pygments==2.17.2 \
-    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
-    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
+pygments==2.18.0 \
+    --hash=sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199 \
+    --hash=sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
     # via rich
 rich==13.7.1 \
     --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
     --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
     # via
     #   cli-base-utilities
     #   ha-services
     #   rich-click
     #   tinkerforge2mqtt (pyproject.toml)
-rich-click==1.7.4 \
-    --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
-    --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
+rich-click==1.8.2 \
+    --hash=sha256:8e29bdede858b59aa2859a1ab1c4ccbd39ed7ed5870262dae756fba6b5dc72e8 \
+    --hash=sha256:b57856f304e4fe0394b82d7ce0784450758f8c8b4e201ccc4320501cc201806b
     # via
     #   cli-base-utilities
     #   ha-services
     #   tinkerforge2mqtt (pyproject.toml)
 tinkerforge==2.1.31 \
     --hash=sha256:e6fa1e395de53f9a1533c2a1262cd67c26cd20070ddd265f16516140ae33bd85
     # via tinkerforge2mqtt (pyproject.toml)
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via cli-base-utilities
-tomlkit==0.12.4 \
-    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
-    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+tomlkit==0.12.5 \
+    --hash=sha256:af914f5a9c59ed9d0762c7b64d3b5d5df007448eb9cd2edc8a46b1eafead172f \
+    --hash=sha256:eef34fba39834d4d6b73c9ba7f3e4d1c417a4e56f89a7e96e090dd0d24b8fb3c
     # via
     #   cli-base-utilities
     #   ha-services
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via rich-click
```

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/__init__.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/discovering.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/discovering.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/publish.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/publish.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/settings.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/settings.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/systemd.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/systemd.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_app/update_readme_history.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_app/update_readme_history.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/__init__.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/code_style.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/code_style.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/packaging.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/packaging.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,22 @@
 
 
 @cli.command()
 def safety():
     """
     Run safety check against current requirements files
     """
-    verbose_check_call('safety', 'check', '-r', 'requirements.dev.txt')
+    verbose_check_call(
+        'safety',
+        'check',
+        '-r',
+        'requirements.dev.txt',
+        '--ignore',
+        '67599',  # Ignore CVE-2018-20225: We do not use the `--extra-index-url` option
+    )
 
 
 @cli.command()
 def update():
     """
     Update "requirements*.txt" dependencies files
     """
```

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/cli_dev/testing.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/cli_dev/testing.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/__init__.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/brick_hat_zero.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/brick_hat_zero.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_analog_in_v3.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_humidity_v2.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_temperature_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 import logging
 
 from ha_services.mqtt4homeassistant.components.sensor import Sensor
-from tinkerforge.bricklet_humidity_v2 import BrickletHumidityV2
+from tinkerforge.bricklet_temperature_v2 import BrickletTemperatureV2
 
 from tinkerforge2mqtt.device_map import register_map_class
 from tinkerforge2mqtt.device_map_utils.base import DeviceMapBase, print_exception_decorator
 
 
 logger = logging.getLogger(__name__)
 
 
 @register_map_class()
-class BrickletHumidityV2Mapper(DeviceMapBase):
-    # https://www.tinkerforge.com/de/doc/Software/Bricklets/HumidityV2_Bricklet_Python.html
+class BrickletTemperatureV2Mapper(DeviceMapBase):
+    # https://www.tinkerforge.com/de/doc/Software/Bricks/HATZero_Brick_Python.html
 
-    device_identifier = BrickletHumidityV2.DEVICE_IDENTIFIER
+    device_identifier = BrickletTemperatureV2.DEVICE_IDENTIFIER
 
-    def __init__(self, *, device: BrickletHumidityV2, **kwargs):
-        self.device: BrickletHumidityV2 = device
+    def __init__(self, *, device: BrickletTemperatureV2, **kwargs):
+        self.device: BrickletTemperatureV2 = device
         super().__init__(device=device, **kwargs)
 
     @print_exception_decorator
     def setup_sensors(self):
         super().setup_sensors()
-
-        self.humidity = Sensor(
-            device=self.mqtt_device,
-            name='Humidity',
-            uid='humidity',
-            device_class='humidity',
-            state_class='measurement',
-            unit_of_measurement='%',
-            suggested_display_precision=2,
-        )
         self.temperature = Sensor(
             device=self.mqtt_device,
             name='Temperature',
             uid='temperature',
             device_class='temperature',
             state_class='measurement',
             unit_of_measurement='°C',
@@ -46,34 +36,18 @@
     @print_exception_decorator
     def setup_callbacks(self):
         super().setup_callbacks()
         self.device.set_temperature_callback_configuration(
             period=self.user_settings.callback_period * 1000,
             value_has_to_change=False,
             option=self.device.THRESHOLD_OPTION_OFF,
-            min=0,
-            max=0,
+            min=-999,
+            max=999,
         )
         self.device.register_callback(self.device.CALLBACK_TEMPERATURE, self.callback_temperature)
 
-        self.device.set_humidity_callback_configuration(
-            period=self.user_settings.callback_period * 1000,
-            value_has_to_change=False,
-            option=self.device.THRESHOLD_OPTION_OFF,
-            min=0,
-            max=0,
-        )
-        self.device.register_callback(self.device.CALLBACK_HUMIDITY, self.callback_humidity)
-
     @print_exception_decorator
     def callback_temperature(self, value):
         temperature = value / 100
         logger.info(f'Temperature callback: {temperature}°C (UID: {self.device.uid_string})')
         self.temperature.set_state(temperature)
         self.temperature.publish(self.mqtt_client)
-
-    @print_exception_decorator
-    def callback_humidity(self, value):
-        humidity = value / 100
-        logger.info(f'Temperature callback: {humidity}°C (UID: {self.device.uid_string})')
-        self.humidity.set_state(humidity)
-        self.humidity.publish(self.mqtt_client)
```

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_industrial_dual_relay.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_motion_detector_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_solid_state_relay_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map/bricklet_voltage_current_v2.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/base.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/base.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_map_utils/generics.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_map_utils/generics.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/device_registry/devices_handler.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/device_registry/devices_handler.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/__init__.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/tests/test_project_setup.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt/user_settings.py` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt/user_settings.py`

 * *Files identical despite different names*

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/PKG-INFO` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinkerforge2mqtt
-Version: 0.8.0
+Version: 0.9.0
 Summary: Emit MQTT events from Tinkerforge devices
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/tinkerforge2mqtt
 Project-URL: Source, https://github.com/jedie/tinkerforge2mqtt
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `tinkerforge2mqtt-0.8/tinkerforge2mqtt.egg-info/SOURCES.txt` & `tinkerforge2mqtt-0.9.0/tinkerforge2mqtt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,10 @@
 tinkerforge2mqtt/device_map_utils/__init__.py
 tinkerforge2mqtt/device_map_utils/base.py
 tinkerforge2mqtt/device_map_utils/generics.py
 tinkerforge2mqtt/device_registry/__init__.py
 tinkerforge2mqtt/device_registry/devices_handler.py
 tinkerforge2mqtt/tests/__init__.py
 tinkerforge2mqtt/tests/test_doctests.py
-tinkerforge2mqtt/tests/test_project_setup.py
+tinkerforge2mqtt/tests/test_project_setup.py
+tinkerforge2mqtt/utilities/__init__.py
+tinkerforge2mqtt/utilities/dew_point.py
```

