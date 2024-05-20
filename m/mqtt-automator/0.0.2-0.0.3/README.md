# Comparing `tmp/mqtt_automator-0.0.2.tar.gz` & `tmp/mqtt_automator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_automator-0.0.2.tar", last modified: Thu May 16 19:40:22 2024, max compression
+gzip compressed data, was "mqtt_automator-0.0.3.tar", last modified: Mon May 20 12:59:49 2024, max compression
```

## Comparing `mqtt_automator-0.0.2.tar` & `mqtt_automator-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:40:22.364575 mqtt_automator-0.0.2/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1068 2024-05-01 11:55:42.000000 mqtt_automator-0.0.2/LICENSE
--rw-r--r--   0 oleg      (1000) oleg      (1000)     6803 2024-05-16 19:40:22.360575 mqtt_automator-0.0.2/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4983 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/README.md
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:40:22.360575 mqtt_automator-0.0.2/mqtt_automator/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3767 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/automator.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      307 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/broker.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:40:22.360575 mqtt_automator-0.0.2/mqtt_automator/config/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/config/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4506 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/config/parser.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1165 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/config/time_parser.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:40:22.360575 mqtt_automator-0.0.2/mqtt_automator/devices/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       29 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/devices/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2822 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/devices/base.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1309 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/devices/lytko.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1289 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/devices/vakio.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1953 2024-05-16 19:36:52.000000 mqtt_automator-0.0.2/mqtt_automator/devices/yeelink.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:40:22.360575 mqtt_automator-0.0.2/mqtt_automator.egg-info/
--rw-r--r--   0 oleg      (1000) oleg      (1000)     6803 2024-05-16 19:40:22.000000 mqtt_automator-0.0.2/mqtt_automator.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      609 2024-05-16 19:40:22.000000 mqtt_automator-0.0.2/mqtt_automator.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2024-05-16 19:40:22.000000 mqtt_automator-0.0.2/mqtt_automator.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       69 2024-05-16 19:40:22.000000 mqtt_automator-0.0.2/mqtt_automator.egg-info/entry_points.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       79 2024-05-16 19:40:22.000000 mqtt_automator-0.0.2/mqtt_automator.egg-info/requires.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       15 2024-05-16 19:40:22.000000 mqtt_automator-0.0.2/mqtt_automator.egg-info/top_level.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1288 2024-05-16 19:38:24.000000 mqtt_automator-0.0.2/pyproject.toml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2024-05-16 19:40:22.364575 mqtt_automator-0.0.2/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1068 2024-05-01 11:55:42.000000 mqtt_automator-0.0.3/LICENSE
+-rw-r--r--   0 oleg      (1000) oleg      (1000)     7256 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5371 2024-05-16 19:47:21.000000 mqtt_automator-0.0.3/README.md
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.3/mqtt_automator/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3629 2024-05-20 12:53:26.000000 mqtt_automator-0.0.3/mqtt_automator/automator.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      226 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/broker.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator/config/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2024-05-16 19:36:52.000000 mqtt_automator-0.0.3/mqtt_automator/config/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6339 2024-05-20 12:56:20.000000 mqtt_automator-0.0.3/mqtt_automator/config/parser.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1308 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/config/time_parser.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator/devices/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       29 2024-05-16 19:36:52.000000 mqtt_automator-0.0.3/mqtt_automator/devices/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2860 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/base.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1411 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/lytko.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1344 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/vakio.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1927 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/mqtt_automator/devices/yeelink.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/mqtt_automator.egg-info/
+-rw-r--r--   0 oleg      (1000) oleg      (1000)     7256 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      637 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       69 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/entry_points.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       95 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       15 2024-05-20 12:59:49.000000 mqtt_automator-0.0.3/mqtt_automator.egg-info/top_level.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1258 2024-05-20 12:59:36.000000 mqtt_automator-0.0.3/pyproject.toml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2024-05-20 12:59:49.507128 mqtt_automator-0.0.3/tests/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2552 2024-05-20 11:48:34.000000 mqtt_automator-0.0.3/tests/test_config_parser.py
```

### Comparing `mqtt_automator-0.0.2/LICENSE` & `mqtt_automator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt_automator-0.0.2/PKG-INFO` & `mqtt_automator-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mqtt-automator
-Version: 0.0.2
-Summary: Simple smart-home automation system. Self-hosted, LAN only.
+Version: 0.0.3
+Summary: Simple smart-home automation system. Self-hosted, LAN only. Supports Vakio Lytko and Yeelink.
 Author-email: Oleg Strizhechenko <oleg.strizhechenko@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,32 +29,45 @@
 Keywords: mqtt,aiomqtt,vakio,lytko,yeelink,self-hosted
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML~=6.0.1
 Requires-Dist: aiomqtt~=2.1.0
 Requires-Dist: paho-mqtt~=2.1.0
+Requires-Dist: pydantic~=2.7.1
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pylint; extra == "test"
 
 ## Установка
 
 Тестировалось только на Ubuntu 22.04
 
+### Последняя версия
+
 ``` shell
 git clone https://codeberg.org/strizhechenko/mqtt_automator.git /opt/mqtt/
 apt install python3.11
 python3.11 -m pip install /opt/mqtt/
 cd /opt/mqtt/examples/config_example.yml /opt/mqtt/config.yml  # правим его под себя
 cp -va /opt/mqtt/automator.service /etc/systemd/system/mqtt-automator.service
 systemctl enable --now mqtt-automator
 ```
 
+### Обновление из pypi
+
+Установить с нуля таким образом не выйдет. Всё равно требуется установка systemd-юнита и написание config.yml, который должен лежать в `/opt/mqtt/`.
+
+``` shell
+pip3 install mqtt-automator
+```
+
+### Разработка
+
 Если планируется делать доработки и делиться ими: лучше использовать pyenv с python3.11, я тестировал только на нём. Внутри virtualenv выполните:
 
 ``` shell
 pip install '/opt/mqtt/[test]'
 pre-commit install-hooks
 ```
```

### Comparing `mqtt_automator-0.0.2/README.md` & `mqtt_automator-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 ## Установка
 
 Тестировалось только на Ubuntu 22.04
 
+### Последняя версия
+
 ``` shell
 git clone https://codeberg.org/strizhechenko/mqtt_automator.git /opt/mqtt/
 apt install python3.11
 python3.11 -m pip install /opt/mqtt/
 cd /opt/mqtt/examples/config_example.yml /opt/mqtt/config.yml  # правим его под себя
 cp -va /opt/mqtt/automator.service /etc/systemd/system/mqtt-automator.service
 systemctl enable --now mqtt-automator
 ```
 
+### Обновление из pypi
+
+Установить с нуля таким образом не выйдет. Всё равно требуется установка systemd-юнита и написание config.yml, который должен лежать в `/opt/mqtt/`.
+
+``` shell
+pip3 install mqtt-automator
+```
+
+### Разработка
+
 Если планируется делать доработки и делиться ими: лучше использовать pyenv с python3.11, я тестировал только на нём. Внутри virtualenv выполните:
 
 ``` shell
 pip install '/opt/mqtt/[test]'
 pre-commit install-hooks
 ```
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator/automator.py` & `mqtt_automator-0.0.3/mqtt_automator/automator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 import asyncio
 import logging
 
 from datetime import datetime
 
-from mqtt_automator.broker import Broker
 from mqtt_automator.config.parser import ConfigParser
 from mqtt_automator.devices import base, vakio, lytko, yeelink
 
 log = logging.getLogger(__name__)
 
 
 class Automator:
@@ -17,50 +16,48 @@
         'vakio': vakio.VakioClient,
         'yeelink': yeelink.YeelinkClient,
     }
 
     def __init__(self):
         self.config = ConfigParser()
         logging.basicConfig(
-            level=logging.getLevelName(self.config.settings.get('log_level', 'INFO')),
+            level=logging.getLevelName(self.config.settings.log_level),
             format='%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s:%(lineno)d: %(message)s'
         )
-        self.broker = Broker(**self.config.broker)
         self.devices: dict[str, base.BaseClient] = {
-            device_name: self.client_map[vendor](device_id, device_name, self.broker)
-            for vendor, device_name, device_id
-            in self.config.get_devices()
+            device.name: self.client_map[device.vendor](device, self.config.broker)
+            for device in self.config.get_devices()
         }
 
     async def run(self):
         log.info('main')
         await asyncio.wait([
             asyncio.create_task(self.feedback()),
             asyncio.create_task(self.scheduler())
         ])
 
     async def feedback(self):
         """mqtt_client is transport to a broker, device_client is a specific for device management"""
         subscriptions = dict()
-        async with self.broker.get_client() as mqtt_client:
+        async with self.config.broker.get_client() as mqtt_client:
             for device_client in self.devices.values():
                 for topic in device_client.subscriptions():
                     log.info('Subscribing to %s', topic)
                     subscriptions[topic] = device_client
                     await mqtt_client.subscribe(topic=topic)  # noqa
 
             try:
                 async for message in mqtt_client.messages:
                     device_client = subscriptions.get(message.topic.value)
                     if not device_client:
                         log.warning('Device client not found for %s', message.topic)
                         continue
                     log.debug('Received %s: %s', message.topic, message.payload)
                     device_client.receive(message.topic.value, message.payload.decode())
-                    log.debug('State of %s: %s', device_client.device_id, device_client.state)
+                    log.debug('State of %s: %s', device_client.device.id, device_client.state)
 
             except asyncio.CancelledError:
                 log.info('Received cancel')
                 for topic in subscriptions:
                     log.info('Unsubscribing from %s', topic)
                     await mqtt_client.unsubscribe(topic=topic)  # noqa
                 raise
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator/config/parser.py` & `mqtt_automator-0.0.3/mqtt_automator/config/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,89 @@
 import logging
 from datetime import datetime
 from pathlib import Path
+from typing import Optional, Self
 
+from pydantic import BaseModel, Field, model_validator, ValidationError
 import yaml
 
 from mqtt_automator.config.time_parser import match_time_range, match_range
+from mqtt_automator.broker import Broker
+from mqtt_automator.devices.base import Device
 
 log = logging.getLogger(__name__)
 
 
+class Settings(BaseModel):
+    log_level: str = Field(default='INFO')
+
+
+class Rule(BaseModel):
+    """
+    Rules are dictionaries with following members:
+    - workday - time range when rule will be active from monday to friday
+    - weekend - time range when rule will be active from saturday/sunday (there will be custom holidays later)
+    - time - time range when rule will be active independently of the day of the week
+    - action - dictionary of topic=payload that will be passed to the device when rule is active (optional)
+    - sub_rules - alternative to action if device should repeatedly change workmode.
+    """
+    workday: Optional[str] = Field(pattern=r'\d{2}:\d{2}-\d{2}:\d{2}', default=None)
+    weekend: Optional[str] = Field(pattern=r'\d{2}:\d{2}-\d{2}:\d{2}', default=None)
+    time: Optional[str] = Field(pattern=r'\d{2}:\d{2}-\d{2}:\d{2}', default=None)
+    action: Optional[dict] = Field(default=None)
+    sub_rules: Optional[dict] = Field(default=None)
+
+    @model_validator(mode='after')
+    def at_least_one_time_defined(self) -> Self:
+        if self.time:
+            if not self.weekend and not self.workday:
+                return self
+        elif self.weekend or self.workday:
+            return self
+        raise ValueError('Schedule is not defined or too defined')
+
+    @model_validator(mode='after')
+    def full_or_split(self) -> Self:
+        if self.action and self.sub_rules:
+            raise ValueError('Do not combine action and sub_rules in a single rule')
+        if not self.action and not self.sub_rules:
+            raise ValueError('action or sub_rules required')
+        return self
+
+
+class SubRule(BaseModel):
+    """
+    Sub-rules are dictionaries with following members:
+    - action - same as action in rules, but it's required now.
+    - hours: range when sub-rule is active. Example: 11-15. Parent rule must be active too.
+    - minutes: same as hours but for minutes. Example: 15-59.
+
+    Special sub-rules:
+    - fallback: if no sub-rule is active this sub-rule will be applied. Doesn't contain hours/minutes.
+    """
+    hours: Optional[str] = Field(pattern=r'\d{1,2}-\d{1,2}', default=None)
+    minutes: Optional[str] = Field(pattern=r'\d{1,2}-\d{1,2}', default=None)
+    action: dict
+
+
 class ConfigParser:
     system_keys = {'app', 'broker'}
 
-    def __init__(self):
+    def __init__(self, file_name: str = 'config.yml'):
         """
         config.yml should have a root-members:
         broker:
             ip: IPv4 of MQTT-broker
             protocol: version of MQTT proto used by broker (default 5)
         app:
             log_level: DEBUG (default INFO)
         """
-        self.config = yaml.load(Path('config.yml').read_text('utf-8'), yaml.SafeLoader)
-        self.broker: dict = self.config['broker']
-        self.settings: dict = self.config['app']
+        self.config = yaml.load(Path(file_name).read_text('utf-8'), yaml.SafeLoader)
+        self.broker = Broker(**self.config['broker'])
+        self.settings = Settings(**(self.config.get('app') or {}))
 
     def get_devices(self):
         """
         Generator that yields: tuple(vendor: str, device_name: str, device_id: str)
 
         vendors are living in the root of config to prevent highly nested structure
 
@@ -47,67 +103,59 @@
         """
         for vendor, devices in self.config.items():
             if vendor in self.system_keys:
                 continue
             for device_name, device in devices.items():
                 if device_name == 'common':
                     continue
-                yield vendor, device_name, device.get('device', device_name)
+                yield Device(vendor=vendor, name=device_name, id=device.get('device', device_name))
 
     def get_active_rules(self):
-        """
-        Rules are dictionaries with following members:
-        - workday - time range when rule will be active from monday to friday
-        - weekend - time range when rule will be active from saturday/sunday (there will be custom holidays later)
-        - time - time range when rule will be active independently of the day of the week
-        - action - dictionary of topic=payload that will be passed to the device when rule is active (optional)
-        - sub_rules - alternative to action if device should repeatedly change workmode.
-        """
+        """For rule structure see class Rule"""
         now = datetime.now()
-        is_workday, now_time = now.isoweekday() > 5, now.time()
+        is_workday, now_time = now.isoweekday() <= 5, now.time()
         for vendor, devices in self.config.items():
             if vendor in self.system_keys:
                 continue
 
             common = devices['common'] if 'common' in devices else dict()
 
             for device, rules in devices.items():
                 if device == 'common':
                     continue
 
                 log.debug('Looking for device %s', device)
-                for name, rule in (rules | common).items():
+                for name, rule_ in (rules | common).items():
                     if name == 'device':
                         continue
-                    schedule = rule.get('workday' if is_workday else 'weekend') or rule.get('time')
+                    rule = Rule(**rule_)
+                    schedule = (rule.workday if is_workday else rule.weekend) or rule.time
                     log.debug('Checking rule %s schedule %s', name, schedule)
                     if schedule and match_time_range(schedule, now_time):
                         log.debug('rule %s schedule %s matched! yielding %s', name, schedule, rule)
-                        yield device, name, rule
+                        yield device, name, rule.model_dump(exclude_unset=True)
 
     @staticmethod
     def get_active_sub_rules(sub_rules: dict):
-        """
-        Sub-rules are dictionaries with following members:
-        - action - same as action in rules, but it's required now.
-        - hours: range when sub-rule is active. Example: 11-15. Parent rule must be active too.
-        - minutes: same as hours but for minutes. Example: 15-59.
-        - fallback: if no sub-rule is active this sub-rule will be applied.
-        """
+        """For sub-rule structure see class SubRule"""
         found, has_fallback = False, False
         now = datetime.now().time()
 
-        for name, rule in sub_rules.items():
-            if 'action' not in rule:
-                log.warning('%s has no action key', rule)
-            elif name == 'fallback':
+        for name, rule_ in sub_rules.items():
+            try:
+                rule = SubRule(**rule_)
+            except ValidationError:
+                log.info("Bad rule %s", rule_, exc_info=True)
+                continue
+
+            if name == 'fallback':
                 has_fallback = True
-            elif 'hours' in rule and not match_range(rule['hours'], now.hour):
+            elif rule.hours and not match_range(rule.hours, now.hour):
                 pass
-            elif 'minutes' in rule and not match_range(rule['minutes'], now.minute):
+            elif rule.minutes and not match_range(rule.minutes, now.minute):
                 pass
             else:
                 found = True
-                yield name, rule
+                yield name, rule.model_dump(exclude_unset=True)
 
         if not found and has_fallback:
             yield 'fallback', sub_rules['fallback']
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator/config/time_parser.py` & `mqtt_automator-0.0.3/mqtt_automator/config/time_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,23 @@
     """
     return [parse_time(t) for t in time_range.split('-', 1)]
 
 
 def match_range(range_: str, value: int) -> bool:
     """
     No overflow required, so naive realisation is enough for both hours and minutes
+    Also there is a bug, it works like value in `[min, max)`
     >>> match_range('3-10', 5)
     True
     >>> match_range('3-10', 2)
     False
+    >>> match_range('3-10', 3)
+    True
+    >>> match_range('3-10', 10)
+    False
     """
     return value in range(*map(int, range_.split('-')))
 
 
 def match_time_range(time_range: str, current_time: time) -> bool:
     """
     >>> match_time_range('09:00-23:00', time(15, 0))
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator/devices/base.py` & `mqtt_automator-0.0.3/mqtt_automator/devices/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import abc
 import logging
 from datetime import datetime, timedelta
 from typing import Generator
 
+from pydantic import BaseModel
+
 from mqtt_automator.broker import Broker
 
 CLIENT_BLOCK_SECONDS = timedelta(hours=4).seconds
 
 log = logging.getLogger(__name__)
 
 
+class Device(BaseModel):
+    vendor: str
+    id: str
+    name: str
+
+
 class BaseClient(abc.ABC):
     topic_template: str
 
-    def __init__(self, device_id: str, device_name: str, broker: Broker = None):
+    def __init__(self, device: Device, broker: Broker = None):
         self.broker = broker
-        self.device_id = device_id
-        self.device_name = device_name
+        self.device = device
         self.state = dict()
         self.started_at = datetime.now()
         self.block = dict()
 
     def __str__(self):
-        return f'{type(self).__name__.replace("Client", "")} {self.device_name} ({self.device_id})'
+        return f'{type(self).__name__.replace("Client", "")} {self.device.name} ({self.device.id})'
 
     async def publish(self, sub_topic: str, payload):
         if isinstance(payload, bool):
             payload = 'on' if payload else 'off'
 
         if self.state.get(sub_topic) == payload:
             log.debug('Skipped %s %s because state-match %s', self, sub_topic, self.state)
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator/devices/vakio.py` & `mqtt_automator-0.0.3/mqtt_automator/devices/vakio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from mqtt_automator.devices.base import BaseClient
+from mqtt_automator.devices.base import BaseClient, Device
 
 log = logging.getLogger(__name__)
 
 
 class VakioClient(BaseClient):
     def receive(self, topic: str, payload: str):
         sub_topic = topic.split('/')[-1]
@@ -13,19 +13,20 @@
 
     def subscriptions(self):
         for sub_topic in ('state', 'workmode', 'speed'):
             yield self.build_topic_name(sub_topic)
 
     def build_topic_name(self, sub_topic) -> str:
         """
-        >>> cabinet = VakioClient('cabinet_mqtt', 'cabinet_pretty_name', '127.0.0.1')
+        >>> device = Device(vendor='vakio', id='cabinet_mqtt', name='cabinet_pretty_name')
+        >>> cabinet = VakioClient(device)
         >>> cabinet.build_topic_name('speed')
         'cabinet_mqtt/speed'
         """
-        return f'{self.device_id}/{sub_topic}'
+        return f'{self.device.id}/{sub_topic}'
 
     async def disable(self):
         await self.publish('state', 'off')
 
     async def enable(self):
         await self.publish('state', 'on')
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator/devices/yeelink.py` & `mqtt_automator-0.0.3/mqtt_automator/devices/yeelink.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import asyncio
 import json
 import logging
 
 from mqtt_automator.broker import Broker
-from mqtt_automator.devices.base import BaseClient
+from mqtt_automator.devices.base import BaseClient, Device
 
 log = logging.getLogger(__name__)
 
 
 class YeelinkClient(BaseClient):
     port = 55443
     max_message_id = 65000
 
-    def __init__(self, device_id: str, device_name: str, broker: Broker = None):
-        super().__init__(device_id, device_name, broker)
+    def __init__(self, device: Device, broker: Broker = None):
+        super().__init__(device, broker)
         self.message_id = 0
 
     def subscriptions(self):
         """Not subscribing on lamps, there is no MQTT at all, it's enough to disable it at 23:00"""
         return ()
 
     async def publish(self, sub_topic: str, payload):
         if self.state.get(sub_topic) == payload:
             log.debug('Skipped because state-match %s', self.state)
             return
 
         self.message_id = ((self.message_id + 1) % self.max_message_id) + 1
         self.state[sub_topic] = payload
         try:
-            _, writer = await asyncio.open_connection(self.device_id, self.port)
+            _, writer = await asyncio.open_connection(self.device.id, self.port)
         except OSError:
             # If device is switched off, no problem, keep _desired_ state and skip further requests
             log.warning("Can't connect to %s", self)
             return
         writer.write(
             (
                     json.dumps({
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator.egg-info/PKG-INFO` & `mqtt_automator-0.0.3/mqtt_automator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mqtt-automator
-Version: 0.0.2
-Summary: Simple smart-home automation system. Self-hosted, LAN only.
+Version: 0.0.3
+Summary: Simple smart-home automation system. Self-hosted, LAN only. Supports Vakio Lytko and Yeelink.
 Author-email: Oleg Strizhechenko <oleg.strizhechenko@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -29,32 +29,45 @@
 Keywords: mqtt,aiomqtt,vakio,lytko,yeelink,self-hosted
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML~=6.0.1
 Requires-Dist: aiomqtt~=2.1.0
 Requires-Dist: paho-mqtt~=2.1.0
+Requires-Dist: pydantic~=2.7.1
 Provides-Extra: test
 Requires-Dist: pre-commit; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pylint; extra == "test"
 
 ## Установка
 
 Тестировалось только на Ubuntu 22.04
 
+### Последняя версия
+
 ``` shell
 git clone https://codeberg.org/strizhechenko/mqtt_automator.git /opt/mqtt/
 apt install python3.11
 python3.11 -m pip install /opt/mqtt/
 cd /opt/mqtt/examples/config_example.yml /opt/mqtt/config.yml  # правим его под себя
 cp -va /opt/mqtt/automator.service /etc/systemd/system/mqtt-automator.service
 systemctl enable --now mqtt-automator
 ```
 
+### Обновление из pypi
+
+Установить с нуля таким образом не выйдет. Всё равно требуется установка systemd-юнита и написание config.yml, который должен лежать в `/opt/mqtt/`.
+
+``` shell
+pip3 install mqtt-automator
+```
+
+### Разработка
+
 Если планируется делать доработки и делиться ими: лучше использовать pyenv с python3.11, я тестировал только на нём. Внутри virtualenv выполните:
 
 ``` shell
 pip install '/opt/mqtt/[test]'
 pre-commit install-hooks
 ```
```

### Comparing `mqtt_automator-0.0.2/mqtt_automator.egg-info/SOURCES.txt` & `mqtt_automator-0.0.3/mqtt_automator.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 mqtt_automator/config/__init__.py
 mqtt_automator/config/parser.py
 mqtt_automator/config/time_parser.py
 mqtt_automator/devices/__init__.py
 mqtt_automator/devices/base.py
 mqtt_automator/devices/lytko.py
 mqtt_automator/devices/vakio.py
-mqtt_automator/devices/yeelink.py
+mqtt_automator/devices/yeelink.py
+tests/test_config_parser.py
```

### Comparing `mqtt_automator-0.0.2/pyproject.toml` & `mqtt_automator-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = 'mqtt-automator'
 authors = [
     {name = 'Oleg Strizhechenko', email = 'oleg.strizhechenko@gmail.com'},
 ]
-version = 'v0.0.2'
+version = 'v0.0.3'
 readme = 'README.md'
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 keywords = ["mqtt", "aiomqtt", "vakio", "lytko", "yeelink", "self-hosted"]
-description = '''Simple smart-home automation system. Self-hosted, LAN only.
-Can manage Vakio Base Smart recuperators, Lytko 101 thermostats, and turn on/off Yeelink lamps.'''
+description = 'Simple smart-home automation system. Self-hosted, LAN only. Supports Vakio Lytko and Yeelink.'
 dependencies = [
     'PyYAML ~= 6.0.1',
     'aiomqtt~=2.1.0',
     'paho-mqtt~=2.1.0',
+    'pydantic~=2.7.1',
 ]
 
 [project.scripts]
 mqtt-automator = "mqtt_automator.automator:main_cli"
 
 [project.optional-dependencies]
 test = [
@@ -31,14 +31,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules"
 testpaths = [
     "mqtt_automator",
+    "tests",
 ]
 
 [tool.autopep8]
 max_line_length = 120
 
 [tool.pylint.'FORMAT']
 max-line-length = 120
```

