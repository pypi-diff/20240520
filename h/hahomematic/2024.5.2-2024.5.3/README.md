# Comparing `tmp/hahomematic-2024.5.2.tar.gz` & `tmp/hahomematic-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2024.5.2.tar", last modified: Tue May 14 15:12:07 2024, max compression
+gzip compressed data, was "hahomematic-2024.5.3.tar", last modified: Mon May 20 14:37:53 2024, max compression
```

## Comparing `hahomematic-2024.5.2.tar` & `hahomematic-2024.5.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/async_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/caches/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/central/
--rw-r--r--   0 runner    (1001) docker     (127)    55193 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/command_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/central/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.852034 hahomematic-2024.5.2/hahomematic/client/
--rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/client/json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/client/xml_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.856034 hahomematic-2024.5.2/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.856034 hahomematic-2024.5.2/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26229 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    26938 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    30391 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 15:12:07.000000 hahomematic-2024.5.2/hahomematic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.860034 hahomematic-2024.5.2/hahomematic_support/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/hahomematic_support/client_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:12:07.864034 hahomematic-2024.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_central.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_central_pydevccu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_climate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35492 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_json_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_siren.py
--rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-14 15:11:43.000000 hahomematic-2024.5.2/tests/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.053923 hahomematic-2024.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-20 14:37:53.053923 hahomematic-2024.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.037923 hahomematic-2024.5.3/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/async_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.041923 hahomematic-2024.5.3/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/caches/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.041923 hahomematic-2024.5.3/hahomematic/central/
+-rw-r--r--   0 runner    (1001) docker     (127)    55193 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/central/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/central/command_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/central/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/central/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.041923 hahomematic-2024.5.3/hahomematic/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    46155 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34886 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/client/json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/client/xml_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.045923 hahomematic-2024.5.3/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.045923 hahomematic-2024.5.3/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27110 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30203 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44099 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30275 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.049923 hahomematic-2024.5.3/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.049923 hahomematic-2024.5.3/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.049923 hahomematic-2024.5.3/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.053923 hahomematic-2024.5.3/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-20 14:37:53.000000 hahomematic-2024.5.3/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-20 14:37:53.000000 hahomematic-2024.5.3/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:37:53.000000 hahomematic-2024.5.3/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:37:52.000000 hahomematic-2024.5.3/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 14:37:53.000000 hahomematic-2024.5.3/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 14:37:53.000000 hahomematic-2024.5.3/hahomematic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.049923 hahomematic-2024.5.3/hahomematic_support/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/hahomematic_support/client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18951 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-20 14:37:53.053923 hahomematic-2024.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:37:53.053923 hahomematic-2024.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_central.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_central_pydevccu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16791 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35513 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_json_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39142 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-20 14:37:27.000000 hahomematic-2024.5.3/tests/test_text.py
```

### Comparing `hahomematic-2024.5.2/LICENSE` & `hahomematic-2024.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/PKG-INFO` & `hahomematic-2024.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.2/README.md` & `hahomematic-2024.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/__init__.py` & `hahomematic-2024.5.3/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/async_support.py` & `hahomematic-2024.5.3/hahomematic/async_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,21 @@
 import asyncio
 from collections.abc import Callable, Collection, Coroutine
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures._base import CancelledError
 from functools import wraps
 import logging
 from time import monotonic
-from typing import Any, Final, ParamSpec, TypeVar, cast
+from typing import Any, Final, cast
 
 from hahomematic.const import BLOCK_LOG_TIMEOUT
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.support import debug_enabled, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
-_P = ParamSpec("_P")
-_R = TypeVar("_R")
-_T = TypeVar("_T")
 
 
 class Looper:
     """Helper class for event loop support."""
 
     def __init__(self) -> None:
         """Init the loop helper."""
@@ -73,15 +70,17 @@
         except CancelledError:
             _LOGGER.debug(
                 "create_task: task cancelled for %s",
                 name,
             )
             return
 
-    def _async_create_task(self, target: Coroutine[Any, Any, _R], name: str) -> asyncio.Task[_R]:
+    def _async_create_task[_R](
+        self, target: Coroutine[Any, Any, _R], name: str
+    ) -> asyncio.Task[_R]:
         """Create a task from within the event_loop. This method must be run in the event_loop."""
         task = self._loop.create_task(target, name=name)
         self._tasks.add(task)
         task.add_done_callback(self._tasks.remove)
         return task
 
     def run_coroutine(self, coro: Coroutine, name: str) -> Any:
@@ -91,15 +90,15 @@
         except CancelledError:  # pragma: no cover
             _LOGGER.debug(
                 "run_coroutine: coroutine interrupted for %s",
                 name,
             )
             return None
 
-    def async_add_executor_job(
+    def async_add_executor_job[_T](
         self,
         target: Callable[..., _T],
         *args: Any,
         name: str,
         executor: ThreadPoolExecutor | None = None,
     ) -> asyncio.Future[_T]:
         """Add an executor job from within the event_loop."""
@@ -117,15 +116,15 @@
 
 
 def cancelling(task: asyncio.Future[Any]) -> bool:
     """Return True if task is cancelling."""
     return bool((cancelling_ := getattr(task, "cancelling", None)) and cancelling_())
 
 
-def loop_check(func: Callable[_P, _R]) -> Callable[_P, _R]:
+def loop_check[**_P, _R](func: Callable[_P, _R]) -> Callable[_P, _R]:
     """Annotation to mark method that must be run within the event loop."""
 
     _with_loop: set = set()
 
     @wraps(func)
     def wrapper_loop_check(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         """Wrap loop check."""
```

### Comparing `hahomematic-2024.5.2/hahomematic/caches/dynamic.py` & `hahomematic-2024.5.3/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/caches/persistent.py` & `hahomematic-2024.5.3/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/caches/visibility.py` & `hahomematic-2024.5.3/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/central/__init__.py` & `hahomematic-2024.5.3/hahomematic/central/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/central/command_queue.py` & `hahomematic-2024.5.3/hahomematic/central/command_queue.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/central/decorators.py` & `hahomematic-2024.5.3/hahomematic/central/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Awaitable, Callable
 from datetime import datetime
 from functools import wraps
 import logging
-from typing import Any, Final, ParamSpec, TypeVar, cast
+from typing import Any, Final, cast
 
 from hahomematic import central as hmcu, client as hmcl
 import hahomematic.central.xml_rpc_server as xmlrpc
 from hahomematic.const import BackendSystemEvent
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.support import reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
-_P = ParamSpec("_P")
-_R = TypeVar("_R")
-
 _INTERFACE_ID: Final = "interface_id"
 
 
 def callback_backend_system(system_event: BackendSystemEvent) -> Callable:
     """Check if backend_system_callback is set and call it AFTER original function."""
 
-    def decorator_backend_system_callback(
+    def decorator_backend_system_callback[**_P, _R](
         func: Callable[_P, _R | Awaitable[_R]],
     ) -> Callable[_P, _R | Awaitable[_R]]:
         """Decorate callback system events."""
 
         @wraps(func)
         async def async_wrapper_backend_system_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
             """Wrap async callback system events."""
@@ -86,15 +83,15 @@
         if asyncio.iscoroutinefunction(func):
             return async_wrapper_backend_system_callback
         return wrapper_backend_system_callback
 
     return decorator_backend_system_callback
 
 
-def callback_event(
+def callback_event[**_P, _R](
     func: Callable[_P, _R],
 ) -> Callable:
     """Check if event_callback is set and call it AFTER original function."""
 
     @wraps(func)
     async def async_wrapper_event_callback(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         """Wrap callback events."""
```

### Comparing `hahomematic-2024.5.2/hahomematic/central/xml_rpc_server.py` & `hahomematic-2024.5.3/hahomematic/central/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/client/__init__.py` & `hahomematic-2024.5.3/hahomematic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/client/json_rpc.py` & `hahomematic-2024.5.3/hahomematic/client/json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/client/xml_rpc.py` & `hahomematic-2024.5.3/hahomematic/client/xml_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/config.py` & `hahomematic-2024.5.3/hahomematic/config.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/const.py` & `hahomematic-2024.5.3/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/converter.py` & `hahomematic-2024.5.3/hahomematic/converter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/exceptions.py` & `hahomematic-2024.5.3/hahomematic/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Awaitable, Callable
 from functools import wraps
 import logging
-from typing import Any, Final, ParamSpec, TypeVar, cast
+from typing import Any, Final, cast
 
 _LOGGER: Final = logging.getLogger(__name__)
 
-_P = ParamSpec("_P")
-_R = TypeVar("_R")
-
 
 class BaseHomematicException(Exception):
     """hahomematic base exception."""
 
     def __init__(self, name: str, *args: Any) -> None:
         """Init the HaHomematicException."""
         if args and isinstance(args[0], BaseException):
@@ -92,15 +89,15 @@
 
 
 def _reduce_args(args: tuple[Any, ...]) -> tuple[Any, ...] | Any:
     """Return the first arg, if there is only one arg."""
     return args[0] if len(args) == 1 else args
 
 
-def log_exception(
+def log_exception[**_P, _R](
     ex_type: type[BaseException],
     logger: logging.Logger = _LOGGER,
     level: int = logging.ERROR,
     extra_msg: str = "",
     re_raise: bool = False,
     ex_return: Any = None,
 ) -> Callable:
```

### Comparing `hahomematic-2024.5.2/hahomematic/hmcli.py` & `hahomematic-2024.5.3/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/performance.py` & `hahomematic-2024.5.3/hahomematic/performance.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable
 from datetime import datetime
 from functools import wraps
 import logging
-from typing import Any, Final, TypeVar
+from typing import Any, Final
 
 _LOGGER: Final = logging.getLogger(__name__)
-_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
 
 
-def measure_execution_time(func: _CallableT) -> _CallableT:
+def measure_execution_time[_CallableT: Callable[..., Any]](func: _CallableT) -> _CallableT:
     """Decorate function to measure the function execution time."""
 
     is_enabled = _LOGGER.isEnabledFor(level=logging.DEBUG)
 
     @wraps(func)
     async def async_wrapper(*args: Any, **kwargs: Any) -> Any:
         """Wrap method."""
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/__init__.py` & `hahomematic-2024.5.3/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/__init__.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/climate.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/climate.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,20 @@
     """Base HomeMatic climate entity."""
 
     _platform = HmPlatform.CLIMATE
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
-        self._e_humidity: HmSensor = self._get_entity(field=Field.HUMIDITY, entity_type=HmSensor)
+        self._e_humidity: HmSensor[int | None] = self._get_entity(
+            field=Field.HUMIDITY, entity_type=HmSensor[int | None]
+        )
         self._e_setpoint: HmFloat = self._get_entity(field=Field.SETPOINT, entity_type=HmFloat)
-        self._e_temperature: HmSensor = self._get_entity(
-            field=Field.TEMPERATURE, entity_type=HmSensor
+        self._e_temperature: HmSensor[float | None] = self._get_entity(
+            field=Field.TEMPERATURE, entity_type=HmSensor[float | None]
         )
         self._e_temperature_maximum: HmFloat = self._get_entity(
             field=Field.TEMPERATURE_MAXIMUM, entity_type=HmFloat
         )
         self._e_temperature_minimum: HmFloat = self._get_entity(
             field=Field.TEMPERATURE_MINIMUM, entity_type=HmFloat
         )
@@ -137,25 +139,25 @@
         return min_temp
 
     @value_property
     def max_temp(self) -> float:
         """Return the maximum temperature."""
         if self._e_temperature_maximum.value is not None:
             return float(self._e_temperature_maximum.value)
-        return self._e_setpoint.max
+        return self._e_setpoint.max  # type: ignore[no-any-return]
 
     @value_property
     def current_humidity(self) -> int | None:
         """Return the current humidity."""
-        return self._e_humidity.value  # type: ignore[no-any-return]
+        return self._e_humidity.value
 
     @value_property
     def current_temperature(self) -> float | None:
         """Return current temperature."""
-        return self._e_temperature.value  # type: ignore[no-any-return]
+        return self._e_temperature.value
 
     @value_property
     def target_temperature(self) -> float | None:
         """Return target temperature."""
         return self._e_setpoint.value
 
     @config_property
@@ -269,19 +271,19 @@
         self._e_manu_mode: HmAction = self._get_entity(field=Field.MANU_MODE, entity_type=HmAction)
         self._e_comfort_mode: HmAction = self._get_entity(
             field=Field.COMFORT_MODE, entity_type=HmAction
         )
         self._e_lowering_mode: HmAction = self._get_entity(
             field=Field.LOWERING_MODE, entity_type=HmAction
         )
-        self._e_control_mode: HmSensor = self._get_entity(
-            field=Field.CONTROL_MODE, entity_type=HmSensor
+        self._e_control_mode: HmSensor[str | None] = self._get_entity(
+            field=Field.CONTROL_MODE, entity_type=HmSensor[str | None]
         )
-        self._e_valve_state: HmSensor = self._get_entity(
-            field=Field.VALVE_STATE, entity_type=HmSensor
+        self._e_valve_state: HmSensor[int | None] = self._get_entity(
+            field=Field.VALVE_STATE, entity_type=HmSensor[int | None]
         )
 
     @value_property
     def hvac_action(self) -> HvacAction | None:
         """Return the hvac action."""
         if self._e_valve_state.value is None:
             return None
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/const.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/cover.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/cover.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from hahomematic.platforms.generic.select import HmSelect
 from hahomematic.platforms.generic.sensor import HmSensor
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 _CLOSED_LEVEL: Final[float] = 0.0  # must be float!
 _OPEN_LEVEL: Final[float] = 1.0  # must be float!
-_OPEN_TILT_LEVEL: Final[float] = 0.5  # must be float!
+_OPEN_TILT_LEVEL: Final[float] = 1.0  # must be float!
 _WD_CLOSED_LEVEL: Final[float] = -0.005  # must be float! HM-Sec-Win
 
 
 class StateChangeArg(StrEnum):
     """Enum with cover state change arguments."""
 
     CLOSE = "close"
@@ -94,19 +94,21 @@
     _closed_level: float = _CLOSED_LEVEL
     _open_level: float = _OPEN_LEVEL
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
         self._command_processing_lock = asyncio.Lock()
-        self._e_direction: HmSensor = self._get_entity(field=Field.DIRECTION, entity_type=HmSensor)
+        self._e_direction: HmSensor[str | None] = self._get_entity(
+            field=Field.DIRECTION, entity_type=HmSensor[str | None]
+        )
         self._e_level: HmFloat = self._get_entity(field=Field.LEVEL, entity_type=HmFloat)
         self._e_stop: HmAction = self._get_entity(field=Field.STOP, entity_type=HmAction)
-        self._e_channel_level: HmSensor = self._get_entity(
-            field=Field.CHANNEL_LEVEL, entity_type=HmSensor
+        self._e_channel_level: HmSensor[float | None] = self._get_entity(
+            field=Field.CHANNEL_LEVEL, entity_type=HmSensor[float | None]
         )
 
     @property
     def _channel_level(self) -> float:
         """Return the channel level of the cover."""
         if self._e_channel_level.value is not None and self.usage == EntityUsage.CE_PRIMARY:
             return float(self._e_channel_level.value)
@@ -234,16 +236,16 @@
     """Class for HomeMatic blind entities."""
 
     _open_tilt_level: float = _OPEN_TILT_LEVEL
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
-        self._e_channel_level_2: HmSensor = self._get_entity(
-            field=Field.CHANNEL_LEVEL_2, entity_type=HmSensor
+        self._e_channel_level_2: HmSensor[float | None] = self._get_entity(
+            field=Field.CHANNEL_LEVEL_2, entity_type=HmSensor[float | None]
         )
         self._e_level_2: HmFloat = self._get_entity(field=Field.LEVEL_2, entity_type=HmFloat)
         self._e_combined: HmAction = self._get_entity(
             field=Field.LEVEL_COMBINED, entity_type=HmAction
         )
 
     @property
@@ -464,21 +466,23 @@
     """Class for HomeMatic garage entities."""
 
     _platform = HmPlatform.COVER
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
-        self._e_door_state: HmSensor = self._get_entity(
-            field=Field.DOOR_STATE, entity_type=HmSensor
+        self._e_door_state: HmSensor[str | None] = self._get_entity(
+            field=Field.DOOR_STATE, entity_type=HmSensor[str | None]
         )
         self._e_door_command: HmAction = self._get_entity(
             field=Field.DOOR_COMMAND, entity_type=HmAction
         )
-        self._e_section: HmSensor = self._get_entity(field=Field.SECTION, entity_type=HmSensor)
+        self._e_section: HmSensor[str | None] = self._get_entity(
+            field=Field.SECTION, entity_type=HmSensor[str | None]
+        )
 
     @value_property
     def current_position(self) -> int | None:
         """Return current position of the garage door ."""
         if self._e_door_state.value == GarageDoorState.OPEN:
             return CoverPosition.OPEN
         if self._e_door_state.value == GarageDoorState.VENTILATION_POSITION:
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/definition.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/entity.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module with base class for custom entities."""
 
 from __future__ import annotations
 
 from collections.abc import Callable, Mapping
 from datetime import datetime
 import logging
-from typing import Any, Final, TypeVar, cast
+from typing import Any, Final, cast
 
 from hahomematic.const import CALLBACK_TYPE, ENTITY_KEY, INIT_DATETIME, CallSource, EntityUsage
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import DeviceProfile, Field
 from hahomematic.platforms.custom.support import ExtendedConfig
 from hahomematic.platforms.decorators import config_property
@@ -19,15 +19,14 @@
     EntityNameData,
     check_channel_is_the_only_primary_channel,
     get_custom_entity_name,
 )
 from hahomematic.support import get_channel_address
 
 _LOGGER: Final = logging.getLogger(__name__)
-_EntityT = TypeVar("_EntityT", bound=hmge.GenericEntity)
 
 
 class CustomEntity(BaseEntity):
     """Base class for custom entities."""
 
     def __init__(
         self,
@@ -273,18 +272,21 @@
         for parameter in parameters:
             entity = self._device.get_generic_entity(
                 channel_address=channel_address, parameter=parameter
             )
             if entity:
                 entity.set_usage(EntityUsage.ENTITY)
 
-    def _get_entity(self, field: Field, entity_type: type[_EntityT]) -> _EntityT:
+    def _get_entity[_EntityT: hmge.GenericEntity](
+        self, field: Field, entity_type: type[_EntityT]
+    ) -> _EntityT:
         """Get entity."""
         if entity := self._data_entities.get(field):
-            if not isinstance(entity, entity_type):
+            if type(entity).__name__ != entity_type.__name__:
+                # not isinstance(entity, entity_type): # does not work with generic type
                 _LOGGER.debug(  # pragma: no cover
                     "GET_ENTITY: type mismatch for requested sub entity: "
                     "expected: %s, but is %s for field name %s of entity %s",
                     entity_type.name,
                     type(entity),
                     field,
                     self.name,
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/light.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,16 +140,16 @@
     _platform = HmPlatform.LIGHT
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         OnTimeMixin.__init__(self)
         super()._init_entity_fields()
         self._e_level: HmFloat = self._get_entity(field=Field.LEVEL, entity_type=HmFloat)
-        self._e_channel_level: HmSensor = self._get_entity(
-            field=Field.CHANNEL_LEVEL, entity_type=HmSensor
+        self._e_channel_level: HmSensor[float | None] = self._get_entity(
+            field=Field.CHANNEL_LEVEL, entity_type=HmSensor[float | None]
         )
         self._e_on_time_value: HmAction = self._get_entity(
             field=Field.ON_TIME_VALUE, entity_type=HmAction
         )
         self._e_ramp_time_value: HmAction = self._get_entity(
             field=Field.RAMP_TIME_VALUE, entity_type=HmAction
         )
@@ -433,16 +433,16 @@
 
 class CeIpRGBWLight(CeDimmer):
     """Class for HomematicIP HmIP-RGBW light entities."""
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
-        self._e_activity_state: HmSensor = self._get_entity(
-            field=Field.DIRECTION, entity_type=HmSensor
+        self._e_activity_state: HmSensor[str | None] = self._get_entity(
+            field=Field.DIRECTION, entity_type=HmSensor[str | None]
         )
         self._e_color_temperature_kelvin: HmInteger = self._get_entity(
             field=Field.COLOR_TEMPERATURE, entity_type=HmInteger
         )
         self._e_device_operation_mode: HmSelect = self._get_entity(
             field=Field.DEVICE_OPERATION_MODE, entity_type=HmSelect
         )
@@ -704,22 +704,22 @@
     def color_name(self) -> str | None:
         """Return the name of the color."""
         return self._e_color.value
 
     @value_property
     def channel_color_name(self) -> str | None:
         """Return the name of the channel color."""
-        return self._e_channel_color.value  # type: ignore[no-any-return]
+        return self._e_channel_color.value
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
         self._e_color: HmSelect = self._get_entity(field=Field.COLOR, entity_type=HmSelect)
-        self._e_channel_color: HmSensor = self._get_entity(
-            field=Field.CHANNEL_COLOR, entity_type=HmSensor
+        self._e_channel_color: HmSensor[str | None] = self._get_entity(
+            field=Field.CHANNEL_COLOR, entity_type=HmSensor[str | None]
         )
         self._e_on_time_unit: HmAction = self._get_entity(
             field=Field.ON_TIME_UNIT, entity_type=HmAction
         )
         self._e_ramp_time_unit: HmAction = self._get_entity(
             field=Field.RAMP_TIME_UNIT, entity_type=HmAction
         )
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/lock.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/lock.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,24 +26,38 @@
 class LockActivity(StrEnum):
     """Enum with lock activities."""
 
     LOCKING = "DOWN"
     UNLOCKING = "UP"
 
 
+class LockError(StrEnum):
+    """Enum with lock errors."""
+
+    NO_ERROR = "NO_ERROR"
+    CLUTCH_FAILURE = "CLUTCH_FAILURE"
+    MOTOR_ABORTED = "MOTOR_ABORTED"
+
+
 class LockState(StrEnum):
     """Enum with lock states."""
 
     LOCKED = "LOCKED"
-    NO_ERROR = "NO_ERROR"
-    OPEN = "OPEN"
     UNKNOWN = "UNKNOWN"
     UNLOCKED = "UNLOCKED"
 
 
+class LockTargetLevel(StrEnum):
+    """Enum with lock target levels."""
+
+    LOCKED = "LOCKED"
+    OPEN = "OPEN"
+    UNLOCKED = "UNLOCKED"
+
+
 class BaseLock(CustomEntity):
     """Class for HomematicIP lock entities."""
 
     _platform = HmPlatform.LOCK
 
     @value_property
     @abstractmethod
@@ -80,26 +94,28 @@
 
 class CeIpLock(BaseLock):
     """Class for HomematicIP lock entities."""
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
-        self._e_lock_state: HmSensor = self._get_entity(
-            field=Field.LOCK_STATE, entity_type=HmSensor
+        self._e_lock_state: HmSensor[str | None] = self._get_entity(
+            field=Field.LOCK_STATE, entity_type=HmSensor[str | None]
         )
         self._e_lock_target_level: HmAction = self._get_entity(
             field=Field.LOCK_TARGET_LEVEL, entity_type=HmAction
         )
-        self._e_direction: HmSensor = self._get_entity(field=Field.DIRECTION, entity_type=HmSensor)
+        self._e_direction: HmSensor[str | None] = self._get_entity(
+            field=Field.DIRECTION, entity_type=HmSensor[str | None]
+        )
 
     @value_property
     def is_locked(self) -> bool:
         """Return true if lock is on."""
-        return self._e_lock_state.value == LockState.LOCKED  # type: ignore[no-any-return]
+        return self._e_lock_state.value == LockState.LOCKED
 
     @value_property
     def is_locking(self) -> bool | None:
         """Return true if the lock is locking."""
         if self._e_direction.value is not None:
             return str(self._e_direction.value) == LockActivity.LOCKING
         return None
@@ -115,37 +131,45 @@
     def is_jammed(self) -> bool:
         """Return true if lock is jammed."""
         return False
 
     @bind_collector()
     async def lock(self, collector: CallParameterCollector | None = None) -> None:
         """Lock the lock."""
-        await self._e_lock_target_level.send_value(value=LockState.LOCKED, collector=collector)
+        await self._e_lock_target_level.send_value(
+            value=LockTargetLevel.LOCKED, collector=collector
+        )
 
     @bind_collector()
     async def unlock(self, collector: CallParameterCollector | None = None) -> None:
         """Unlock the lock."""
-        await self._e_lock_target_level.send_value(value=LockState.UNLOCKED, collector=collector)
+        await self._e_lock_target_level.send_value(
+            value=LockTargetLevel.UNLOCKED, collector=collector
+        )
 
     @bind_collector()
     async def open(self, collector: CallParameterCollector | None = None) -> None:
         """Open the lock."""
-        await self._e_lock_target_level.send_value(value=LockState.OPEN, collector=collector)
+        await self._e_lock_target_level.send_value(value=LockTargetLevel.OPEN, collector=collector)
 
 
 class CeRfLock(BaseLock):
     """Class for classic HomeMatic lock entities."""
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
         self._e_state: HmSwitch = self._get_entity(field=Field.STATE, entity_type=HmSwitch)
         self._e_open: HmAction = self._get_entity(field=Field.OPEN, entity_type=HmAction)
-        self._e_direction: HmSensor = self._get_entity(field=Field.DIRECTION, entity_type=HmSensor)
-        self._e_error: HmSensor = self._get_entity(field=Field.ERROR, entity_type=HmSensor)
+        self._e_direction: HmSensor[str | None] = self._get_entity(
+            field=Field.DIRECTION, entity_type=HmSensor[str | None]
+        )
+        self._e_error: HmSensor[str | None] = self._get_entity(
+            field=Field.ERROR, entity_type=HmSensor[str | None]
+        )
 
     @value_property
     def is_locked(self) -> bool:
         """Return true if lock is on."""
         return self._e_state.value is not True
 
     @value_property
@@ -161,15 +185,15 @@
         if self._e_direction.value is not None:
             return str(self._e_direction.value) == LockActivity.UNLOCKING
         return None
 
     @value_property
     def is_jammed(self) -> bool:
         """Return true if lock is jammed."""
-        return self._e_error.value is not None and self._e_error.value != LockState.NO_ERROR
+        return self._e_error.value is not None and self._e_error.value != LockError.NO_ERROR
 
     @bind_collector()
     async def lock(self, collector: CallParameterCollector | None = None) -> None:
         """Lock the lock."""
         await self._e_state.send_value(value=False, collector=collector)
 
     @bind_collector()
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/siren.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/siren.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,16 +184,16 @@
 
 class CeIpSirenSmoke(BaseSiren):
     """Class for HomematicIP siren smoke entities."""
 
     def _init_entity_fields(self) -> None:
         """Init the entity fields."""
         super()._init_entity_fields()
-        self._e_smoke_detector_alarm_status: HmSensor = self._get_entity(
-            field=Field.SMOKE_DETECTOR_ALARM_STATUS, entity_type=HmSensor
+        self._e_smoke_detector_alarm_status: HmSensor[str | None] = self._get_entity(
+            field=Field.SMOKE_DETECTOR_ALARM_STATUS, entity_type=HmSensor[str | None]
         )
         self._e_smoke_detector_command: HmAction = self._get_entity(
             field=Field.SMOKE_DETECTOR_COMMAND, entity_type=HmAction
         )
 
     @value_property
     def is_on(self) -> bool:
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/support.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/custom/switch.py` & `hahomematic-2024.5.3/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/decorators.py` & `hahomematic-2024.5.3/hahomematic/platforms/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 """Decorators for entities used within hahomematic."""
 
 from __future__ import annotations
 
 from collections.abc import Callable, Mapping
-from typing import Any, Generic, TypeVar
-
-G = TypeVar("G")
-S = TypeVar("S")
+from typing import Any
 
 
 # pylint: disable=invalid-name
-class generic_property(Generic[G, S], property):
+class generic_property[_GETTER, _SETTER](property):
     """Generic property implementation."""
 
-    fget: Callable[[Any], G] | None
-    fset: Callable[[Any, S], None] | None
+    fget: Callable[[Any], _GETTER] | None
+    fset: Callable[[Any, _SETTER], None] | None
     fdel: Callable[[Any], None] | None
 
     def __init__(
         self,
-        fget: Callable[[Any], G] | None = None,
-        fset: Callable[[Any, S], None] | None = None,
+        fget: Callable[[Any], _GETTER] | None = None,
+        fset: Callable[[Any, _SETTER], None] | None = None,
         fdel: Callable[[Any], None] | None = None,
         doc: str | None = None,
     ) -> None:
         """Init the generic property."""
         super().__init__(fget, fset, fdel, doc)
         if doc is None and fget is not None:
             doc = fget.__doc__
         self.__doc__ = doc
 
-    def getter(self, __fget: Callable[[Any], G]) -> generic_property:
+    def getter(self, __fget: Callable[[Any], _GETTER]) -> generic_property:
         """Return generic getter."""
         return type(self)(__fget, self.fset, self.fdel, self.__doc__)  # pragma: no cover
 
-    def setter(self, __fset: Callable[[Any, S], None]) -> generic_property:
+    def setter(self, __fset: Callable[[Any, _SETTER], None]) -> generic_property:
         """Return generic setter."""
         return type(self)(self.fget, __fset, self.fdel, self.__doc__)
 
     def deleter(self, __fdel: Callable[[Any], None]) -> generic_property:
         """Return generic deleter."""
         return type(self)(self.fget, self.fset, __fdel, self.__doc__)
 
-    def __get__(self, __obj: Any, __type: type | None = None) -> G:
+    def __get__(self, __obj: Any, __type: type | None = None) -> _GETTER:
         """Return the attribute."""
         if __obj is None:
             return self  # type: ignore[return-value]
         if self.fget is None:
             raise AttributeError("unreadable attribute")  # pragma: no cover
         return self.fget(__obj)
 
@@ -60,20 +57,20 @@
         """Delete the attribute."""
         if self.fdel is None:
             raise AttributeError("can't delete attribute")  # pragma: no cover
         self.fdel(__obj)
 
 
 # pylint: disable=invalid-name
-class config_property(generic_property[G, S], property):
+class config_property[_GETTER, _SETTER](generic_property[_GETTER, _SETTER]):
     """Decorate to mark own config properties."""
 
 
 # pylint: disable=invalid-name
-class value_property(generic_property[G, S], property):
+class value_property[_GETTER, _SETTER](generic_property[_GETTER, _SETTER]):
     """Decorate to mark own value properties."""
 
 
 def _get_public_attributes_by_decorator(
     data_object: Any, property_decorator: type
 ) -> Mapping[str, Any]:
     """Return the object attributes by decorator."""
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/device.py` & `hahomematic-2024.5.3/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/entity.py` & `hahomematic-2024.5.3/hahomematic/platforms/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Mapping
 from datetime import datetime
 from functools import partial, wraps
 from inspect import getfullargspec
 import logging
-from typing import Any, Final, Generic, TypeVar, cast
+from typing import Any, Final, cast
 
 import voluptuous as vol
 
 from hahomematic import central as hmcu, client as hmcl, support as hms
 from hahomematic.async_support import loop_check
 from hahomematic.config import WAIT_FOR_CALLBACK
 from hahomematic.const import (
@@ -39,24 +39,23 @@
     ParamsetKey,
 )
 from hahomematic.exceptions import HaHomematicException
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.decorators import config_property, value_property
 from hahomematic.platforms.support import (
     EntityNameData,
+    GenericParameterType,
     PayloadMixin,
     convert_value,
     generate_channel_unique_id,
 )
 from hahomematic.support import get_entity_key, reduce_args
 
 _LOGGER: Final = logging.getLogger(__name__)
 
-_CallableT = TypeVar("_CallableT", bound=Callable[..., Any])
-
 _CONFIGURABLE_CHANNEL: Final[tuple[str, ...]] = (
     "KEY_TRANSCEIVER",
     "MULTI_MODE_INPUT_TRANSMITTER",
 )
 _COLLECTOR_ARGUMENT_NAME = "collector"
 
 _FIX_UNIT_REPLACE: Final[Mapping[str, str]] = {
@@ -383,19 +382,18 @@
         """Provide some useful information."""
         return (
             f"address_path: {self.address_path}, type: {self._device.device_type}, "
             f"name: {self.full_name}"
         )
 
 
-InputParameterT = TypeVar("InputParameterT", bool, int, float, str, int | float | str, None)
-ParameterT = TypeVar("ParameterT", bool, int, float, str, int | str, None)
-
-
-class BaseParameterEntity(Generic[ParameterT, InputParameterT], BaseEntity):
+class BaseParameterEntity[
+    ParameterT: GenericParameterType,
+    InputParameterT: GenericParameterType,
+](BaseEntity):
     """Base class for stateless entities."""
 
     def __init__(
         self,
         device: hmd.HmDevice,
         unique_id: str,
         channel_address: str,
@@ -421,16 +419,16 @@
                 device_type=self._device.device_type,
                 channel_no=self._channel_no,
                 paramset_key=self._paramset_key,
                 parameter=self._parameter,
                 custom_only=True,
             )
         )
-        self._value: ParameterT | None = None
-        self._old_value: ParameterT | None = None
+        self._value: ParameterT = None  # type: ignore[assignment]
+        self._old_value: ParameterT = None  # type: ignore[assignment]
         self._last_updated: datetime = INIT_DATETIME
         self._last_refreshed: datetime = INIT_DATETIME
         self._state_uncertain: bool = True
         self._is_forced_sensor: bool = False
         self._assign_parameter_data(parameter_data=parameter_data)
 
     def _assign_parameter_data(self, parameter_data: Mapping[str, Any]) -> None:
@@ -540,38 +538,38 @@
 
     @property
     def last_refreshed(self) -> datetime:
         """Return the last refreshed datetime value."""
         return self._last_refreshed
 
     @property
-    def unconfirmed_last_value_send(self) -> ParameterT | None:
+    def unconfirmed_last_value_send(self) -> ParameterT:
         """Return the unconfirmed value send for the entity."""
         return cast(
-            ParameterT | None,
+            ParameterT,
             self._client.last_value_send_cache.get_last_value_send(entity_key=self.entity_key),
         )
 
     @property
-    def old_value(self) -> ParameterT | None:
+    def old_value(self) -> ParameterT:
         """Return the old value of the entity."""
         return self._old_value
 
     @config_property
     def platform(self) -> HmPlatform:
         """Return, the platform of the entity."""
         return HmPlatform.SENSOR if self._is_forced_sensor else self._platform
 
     @property
     def state_uncertain(self) -> bool:
         """Return, if the state is uncertain."""
         return self._state_uncertain
 
     @value_property
-    def value(self) -> ParameterT | None:
+    def value(self) -> ParameterT:
         """Return the value of the entity."""
         return self._value
 
     @property
     def supports_events(self) -> bool:
         """Return, if entity is supports events."""
         return bool(self._operations & Operations.EVENT)
@@ -677,22 +675,22 @@
                 paramset_key=self._paramset_key,
                 parameter=self._parameter,
                 call_source=call_source,
                 direct_call=direct_call,
             )
         )
 
-    def write_value(self, value: Any) -> tuple[ParameterT | None, ParameterT | None]:
+    def write_value(self, value: Any) -> tuple[ParameterT, ParameterT]:
         """Update value of the entity."""
         old_value = self._value
         if value == NO_CACHE_ENTRY:
             if self.last_refreshed != INIT_DATETIME:
                 self._state_uncertain = True
                 self.fire_entity_updated_callback()
-            return (old_value, None)
+            return (old_value, None)  # type: ignore[return-value]
 
         new_value = self._convert_value(value)
         if old_value == new_value:
             self._set_last_refreshed()
         else:
             self._set_last_updated()
             self._old_value = old_value
@@ -821,15 +819,15 @@
 def bind_collector(
     wait_for_callback: int | None = WAIT_FOR_CALLBACK,
     use_command_queue: bool = False,
     use_put_paramset: bool = True,
 ) -> Callable:
     """Decorate function to automatically add collector if not set."""
 
-    def decorator_bind_collector(func: _CallableT) -> _CallableT:
+    def decorator_bind_collector[_CallableT: Callable[..., Any]](func: _CallableT) -> _CallableT:
         """Decorate function to automatically add collector if not set."""
         argument_index = getfullargspec(func).args.index(_COLLECTOR_ARGUMENT_NAME)
 
         @wraps(func)
         async def wrapper_collector(*args: Any, **kwargs: Any) -> Any:
             """Wrap method to add collector."""
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/event.py` & `hahomematic-2024.5.3/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/__init__.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/action.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/binary_sensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from __future__ import annotations
 
 from hahomematic.const import HmPlatform
 from hahomematic.platforms.decorators import value_property
 from hahomematic.platforms.generic.entity import GenericEntity
 
 
-class HmBinarySensor(GenericEntity[bool, bool]):
+class HmBinarySensor(GenericEntity[bool | None, bool]):
     """
     Implementation of a binary_sensor.
 
     This is a default platform that gets automatically generated.
     """
 
     _platform = HmPlatform.BINARY_SENSOR
 
     @value_property
     def value(self) -> bool | None:  # type: ignore[override]
         """Return the value of the entity."""
         if self._value is not None:
-            return self._value
-        return self._default
+            return self._value  # type: ignore[no-any-return]
+        return self._default  # type: ignore[no-any-return]
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/button.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/entity.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from collections.abc import Mapping
 import logging
 from typing import Any, Final
 
 from hahomematic.const import CallSource, EntityUsage, HomematicEventType, Parameter, ParamsetKey
 from hahomematic.platforms import device as hmd, entity as hme
 from hahomematic.platforms.decorators import config_property
-from hahomematic.platforms.support import EntityNameData, get_entity_name
+from hahomematic.platforms.support import EntityNameData, GenericParameterType, get_entity_name
 
 _LOGGER: Final = logging.getLogger(__name__)
 
 
-class GenericEntity(hme.BaseParameterEntity[hme.ParameterT, hme.InputParameterT]):
+class GenericEntity[ParameterT: GenericParameterType, InputParameterT: GenericParameterType](
+    hme.BaseParameterEntity
+):
     """Base class for generic entities."""
 
     _validate_state_change: bool = True
     is_hmtype: Final = True
 
     def __init__(
         self,
@@ -80,15 +82,15 @@
             self._central.fire_homematic_callback(
                 event_type=HomematicEventType.DEVICE_AVAILABILITY,
                 event_data=self.get_event_data(new_value),
             )
 
     async def send_value(
         self,
-        value: hme.InputParameterT,
+        value: InputParameterT,
         collector: hme.CallParameterCollector | None = None,
         collector_order: int = 50,
         do_validate: bool = True,
     ) -> None:
         """Send value to ccu, or use collector if set."""
         if not self.is_writeable:
             _LOGGER.error(
@@ -113,16 +115,16 @@
             channel_address=self._channel_address,
             paramset_key=self._paramset_key,
             parameter=self._parameter,
             value=converted_value,
         )
 
     def _prepare_value_for_sending(
-        self, value: hme.InputParameterT, do_validate: bool = True
-    ) -> hme.ParameterT:
+        self, value: InputParameterT, do_validate: bool = True
+    ) -> ParameterT:
         """Prepare value, if required, before send."""
         return value  # type: ignore[return-value]
 
     def _get_entity_name(self) -> EntityNameData:
         """Create the name for the entity."""
         return get_entity_name(
             central=self._central,
@@ -143,15 +145,15 @@
 
         return (
             EntityUsage.NO_CREATE
             if self._device.has_custom_entity_definition
             else EntityUsage.ENTITY
         )
 
-    def is_state_change(self, value: hme.ParameterT) -> bool:
+    def is_state_change(self, value: ParameterT) -> bool:
         """
         Check if the state/value changes.
 
         If the state is uncertain, the state should also marked as changed.
         """
         if value != self._value:
             return True
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/number.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/select.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,42 @@
 """
-Module for entities implemented using the number platform.
+Module for entities implemented using the select platform.
 
-See https://www.home-assistant.io/integrations/number/.
+See https://www.home-assistant.io/integrations/select/.
 """
 
 from __future__ import annotations
 
 from hahomematic.const import HmPlatform
-from hahomematic.platforms.entity import ParameterT
+from hahomematic.platforms.decorators import value_property
 from hahomematic.platforms.generic.entity import GenericEntity
+from hahomematic.platforms.support import get_value_from_value_list
 
 
-class BaseNumber(GenericEntity[ParameterT, int | float | str]):
+class HmSelect(GenericEntity[int | str, int | float | str]):
     """
-    Implementation of a number.
+    Implementation of a select entity.
 
     This is a default platform that gets automatically generated.
     """
 
-    _platform = HmPlatform.NUMBER
+    _platform = HmPlatform.SELECT
 
-
-class HmFloat(BaseNumber[float]):
-    """
-    Implementation of a Float.
-
-    This is a default platform that gets automatically generated.
-    """
-
-    def _prepare_value_for_sending(
-        self, value: int | float | str, do_validate: bool = True
-    ) -> float:
-        """Prepare value before sending."""
-        if not do_validate or (
-            value is not None
-            and isinstance(value, int | float)
-            and self._min <= float(value) <= self._max
-        ):
-            return float(value)
-        if self._special and isinstance(value, str) and value in self._special:
-            return float(self._special[value])
-        raise ValueError(
-            f"NUMBER.FLOAT failed: Invalid value: {value} (min: {self._min}, "
-            f"max: {self._max}, special:{self._special})"
-        )
-
-
-class HmInteger(BaseNumber[int]):
-    """
-    Implementation of an Integer.
-
-    This is a default platform that gets automatically generated.
-    """
+    @value_property
+    def value(self) -> str | None:  # type: ignore[override]
+        """Get the value of the entity."""
+        if (
+            value := get_value_from_value_list(value=self._value, value_list=self.values)
+        ) is not None:
+            return value
+        return str(self._default)
 
     def _prepare_value_for_sending(
         self, value: int | float | str, do_validate: bool = True
     ) -> int:
         """Prepare value before sending."""
-        if not do_validate or (
-            value is not None
-            and isinstance(value, int | float)
-            and self._min <= int(value) <= self._max
-        ):
+        # We allow setting the value via index as well, just in case.
+        if isinstance(value, int | float) and self._values and 0 <= value < len(self._values):
             return int(value)
-        if self._special and isinstance(value, str) and value in self._special:
-            return int(self._special[value])
-
-        raise ValueError(
-            f"NUMBER.INT failed: Invalid value: {value} (min: {self._min}, "
-            f"max: {self._max}, special:{self._special})"
-        )
+        if self._values and value in self._values:
+            return self._values.index(value)
+        raise ValueError(f"Value not in value_list for {self.name}/{self.unique_id}")
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/select.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/sensor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,71 @@
 """
-Module for entities implemented using the select platform.
+Module for entities implemented using the sensor platform.
 
-See https://www.home-assistant.io/integrations/select/.
+See https://www.home-assistant.io/integrations/sensor/.
 """
 
 from __future__ import annotations
 
-from hahomematic.const import HmPlatform
+from collections.abc import Mapping
+import logging
+from typing import Any, Final
+
+from hahomematic.const import HmPlatform, Parameter
 from hahomematic.platforms.decorators import value_property
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.support import get_value_from_value_list
 
+_LOGGER: Final = logging.getLogger(__name__)
+
 
-class HmSelect(GenericEntity[int | str, int | float | str]):
+class HmSensor[SensorT: float | int | str | None](GenericEntity[SensorT, None]):
     """
-    Implementation of a select entity.
+    Implementation of a sensor.
 
     This is a default platform that gets automatically generated.
     """
 
-    _platform = HmPlatform.SELECT
+    _platform = HmPlatform.SENSOR
 
     @value_property
-    def value(self) -> str | None:  # type: ignore[override]
-        """Get the value of the entity."""
+    def value(self) -> SensorT:  # type: ignore[override]
+        """Return the value."""
         if (
             value := get_value_from_value_list(value=self._value, value_list=self.values)
         ) is not None:
+            return value  # type: ignore[return-value]
+        if convert_func := self._get_converter_func():
+            return convert_func(self._value)  # type: ignore[no-any-return]
+        return self._value  # type: ignore[no-any-return]
+
+    def _get_converter_func(self) -> Any:
+        """Return a converter based on sensor."""
+        if convert_func := CONVERTERS_BY_PARAM.get(self.parameter):
+            return convert_func
+        return None
+
+
+def _fix_rssi(value: Any) -> int | None:
+    """
+    Fix rssi value.
+
+    See https://github.com/danielperna84/hahomematic/blob/devel/docs/rssi_fix.md.
+    """
+    if value is None:
+        return None
+    if isinstance(value, int):
+        if -127 < value < 0:
             return value
-        return str(self._default)
+        if 1 < value < 127:
+            return value * -1
+        if -256 < value < -129:
+            return (value * -1) - 256
+        if 129 < value < 256:
+            return value - 256
+    return None
+
 
-    def _prepare_value_for_sending(
-        self, value: int | float | str, do_validate: bool = True
-    ) -> int:
-        """Prepare value before sending."""
-        # We allow setting the value via index as well, just in case.
-        if isinstance(value, int | float) and self._values and 0 <= value < len(self._values):
-            return int(value)
-        if self._values and value in self._values:
-            return self._values.index(value)
-        raise ValueError(f"Value not in value_list for {self.name}/{self.unique_id}")
+CONVERTERS_BY_PARAM: Mapping[str, Any] = {
+    Parameter.RSSI_PEER: _fix_rssi,
+    Parameter.RSSI_DEVICE: _fix_rssi,
+}
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/generic/switch.py` & `hahomematic-2024.5.3/hahomematic/platforms/generic/switch.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 from hahomematic.platforms.decorators import value_property
 from hahomematic.platforms.entity import CallParameterCollector
 from hahomematic.platforms.generic.entity import GenericEntity
 
 _PARAM_ON_TIME: Final = "ON_TIME"
 
 
-class HmSwitch(GenericEntity[bool, bool]):
+class HmSwitch(GenericEntity[bool | None, bool]):
     """
     Implementation of a switch.
 
     This is a default platform that gets automatically generated.
     """
 
     _platform = HmPlatform.SWITCH
 
     @value_property
     def value(self) -> bool | None:  # type: ignore[override]
         """Get the value of the entity."""
         if self._type == ParameterType.ACTION:
             return False
-        return self._value
+        return self._value  # type: ignore[no-any-return]
 
     async def turn_on(
         self, collector: CallParameterCollector | None = None, on_time: float | None = None
     ) -> None:
         """Turn the switch on."""
         if on_time is not None:
             await self.set_on_time(on_time=on_time)
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/__init__.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/button.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/entity.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/number.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/select.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/sensor.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/hub/text.py` & `hahomematic-2024.5.3/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/support.py` & `hahomematic-2024.5.3/hahomematic/platforms/support.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from collections.abc import Mapping
 from datetime import datetime
 from enum import StrEnum
 import logging
-from typing import Any, Final
+from typing import Any, Final, TypeAlias
 
 from hahomematic import central as hmcu, support as hms
 from hahomematic.const import (
     INIT_DATETIME,
     PROGRAM_ADDRESS,
     SYSVAR_ADDRESS,
     VIRTUAL_REMOTE_ADDRESSES,
@@ -24,14 +24,16 @@
     get_public_attributes_for_config_property,
     get_public_attributes_for_value_property,
 )
 from hahomematic.support import to_bool
 
 _LOGGER: Final = logging.getLogger(__name__)
 
+GenericParameterType: TypeAlias = bool | int | float | str | None
+
 # dict with binary_sensor relevant value lists and the corresponding TRUE value
 _BINARY_SENSOR_TRUE_VALUE_DICT_FOR_VALUE_LIST: Final[Mapping[tuple[str, ...], str]] = {
     ("CLOSED", "OPEN"): "OPEN",
     ("DRY", "RAIN"): "RAIN",
     ("STABLE", "NOT_STABLE"): "NOT_STABLE",
 }
```

### Comparing `hahomematic-2024.5.2/hahomematic/platforms/update.py` & `hahomematic-2024.5.3/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2024.5.3/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2024.5.3/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2024.5.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic/support.py` & `hahomematic-2024.5.3/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic.egg-info/PKG-INFO` & `hahomematic-2024.5.3/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2024.5.2
+Version: 2024.5.3
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2024.5.2/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2024.5.3/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/hahomematic_support/client_local.py` & `hahomematic-2024.5.3/hahomematic_support/client_local.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/pyproject.toml` & `hahomematic-2024.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=69.2.0", "wheel~=0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2024.5.2"
+version     = "2024.5.3"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

### Comparing `hahomematic-2024.5.2/tests/test_action.py` & `hahomematic-2024.5.3/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_binary_sensor.py` & `hahomematic-2024.5.3/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_button.py` & `hahomematic-2024.5.3/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_central.py` & `hahomematic-2024.5.3/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_central_pydevccu.py` & `hahomematic-2024.5.3/tests/test_central_pydevccu.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_climate.py` & `hahomematic-2024.5.3/tests/test_climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_cover.py` & `hahomematic-2024.5.3/tests/test_cover.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,27 +172,27 @@
     assert cover.current_position == 81
     assert cover.is_closed is False
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
-        value="L2=50,L=100",
+        value="L2=100,L=100",
         wait_for_callback=WAIT_FOR_CALLBACK,
     )
     assert cover._e_level.unconfirmed_last_value_send == _OPEN_LEVEL
     assert cover._e_level_2.unconfirmed_last_value_send == _OPEN_TILT_LEVEL
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL", _OPEN_LEVEL)
     await central.event(const.INTERFACE_ID, "VCU7807849:1", "LEVEL_2", _OPEN_TILT_LEVEL)
     await central.event(const.INTERFACE_ID, "VCU7807849:2", "LEVEL", _OPEN_LEVEL)
     await central.event(const.INTERFACE_ID, "VCU7807849:2", "LEVEL_2", _OPEN_TILT_LEVEL)
     assert cover._e_level.unconfirmed_last_value_send is None
     assert cover._e_level_2.unconfirmed_last_value_send is None
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 50
+    assert cover.current_tilt_position == 100
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU7807849:2",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
         wait_for_callback=WAIT_FOR_CALLBACK,
@@ -317,21 +317,21 @@
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
-        value="0xc8,0x64",
+        value="0xc8,0xc8",
         wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL", _OPEN_LEVEL)
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 50
+    assert cover.current_tilt_position == 100
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x00",
@@ -343,20 +343,20 @@
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
-        value="0x00,0x64",
+        value="0x00,0xc8",
         wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     assert cover.current_position == 0
-    assert cover.current_tilt_position == 50
+    assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU0000145:1",
         paramset_key="VALUES",
         parameter="LEVEL_COMBINED",
         value="0x00,0x5a",
@@ -409,15 +409,15 @@
     )
 
     await cover.open_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.open_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _OPEN_TILT_LEVEL)
-    assert call_count == len(mock_client.method_calls) - 5
+    assert call_count == len(mock_client.method_calls) - 1
 
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     call_count = len(mock_client.method_calls)
     await cover.close_tilt()
     await central.event(const.INTERFACE_ID, "VCU0000145:1", "LEVEL_SLATS", _CLOSED_LEVEL)
     assert call_count == len(mock_client.method_calls) - 1
@@ -520,21 +520,21 @@
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
-        value="L2=50,L=100",
+        value="L2=100,L=100",
         wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", _OPEN_TILT_LEVEL)
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL", _OPEN_LEVEL)
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 50
+    assert cover.current_tilt_position == 100
 
     await cover.close()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
         value="L2=0,L=0",
@@ -546,15 +546,15 @@
     assert cover.current_tilt_position == 0
 
     await cover.open_tilt()
     assert mock_client.method_calls[-1] == call.set_value(
         channel_address="VCU1223813:4",
         paramset_key="VALUES",
         parameter="COMBINED_PARAMETER",
-        value="L2=50,L=0",
+        value="L2=100,L=0",
         wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU1223813:4", "LEVEL_2", 1.0)
     assert cover.current_position == 0
     assert cover.current_tilt_position == 100
 
     await cover.set_position(tilt_position=45)
@@ -666,21 +666,21 @@
     assert cover.current_position == 81
     assert cover.current_tilt_position == 0
 
     await cover.open()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
-        values={"LEVEL_2": 0.5, "LEVEL": _OPEN_LEVEL},
+        values={"LEVEL_2": _OPEN_TILT_LEVEL, "LEVEL": _OPEN_LEVEL},
         wait_for_callback=WAIT_FOR_CALLBACK,
     )
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL_2", _OPEN_TILT_LEVEL)
     await central.event(const.INTERFACE_ID, "VCU3560967:1", "LEVEL", _OPEN_LEVEL)
     assert cover.current_position == 100
-    assert cover.current_tilt_position == 50
+    assert cover.current_tilt_position == 100
 
     await cover.close()
     assert mock_client.method_calls[-3] == call.put_paramset(
         channel_address="VCU3560967:1",
         paramset_key="VALUES",
         values={"LEVEL_2": _CLOSED_LEVEL, "LEVEL": _CLOSED_LEVEL},
         wait_for_callback=WAIT_FOR_CALLBACK,
```

### Comparing `hahomematic-2024.5.2/tests/test_decorator.py` & `hahomematic-2024.5.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_device.py` & `hahomematic-2024.5.3/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_entity.py` & `hahomematic-2024.5.3/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_event.py` & `hahomematic-2024.5.3/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_json_rpc.py` & `hahomematic-2024.5.3/tests/test_json_rpc.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_light.py` & `hahomematic-2024.5.3/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_lock.py` & `hahomematic-2024.5.3/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_number.py` & `hahomematic-2024.5.3/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_select.py` & `hahomematic-2024.5.3/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_sensor.py` & `hahomematic-2024.5.3/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_siren.py` & `hahomematic-2024.5.3/tests/test_siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_support.py` & `hahomematic-2024.5.3/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_switch.py` & `hahomematic-2024.5.3/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2024.5.2/tests/test_text.py` & `hahomematic-2024.5.3/tests/test_text.py`

 * *Files identical despite different names*

