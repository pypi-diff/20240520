# Comparing `tmp/synthetic_home-0.1.0.tar.gz` & `tmp/synthetic_home-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetic_home-0.1.0.tar", last modified: Sat May 18 05:49:11 2024, max compression
+gzip compressed data, was "synthetic_home-2.0.0.tar", last modified: Mon May 20 14:50:19 2024, max compression
```

## Comparing `synthetic_home-0.1.0.tar` & `synthetic_home-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-18 05:49:11.861648 synthetic_home-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/synthetic_home/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/synthetic_home/registry/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/synthetic_home/synthetic_home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/synthetic_home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 05:49:11.000000 synthetic_home-0.1.0/synthetic_home.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:49:11.857648 synthetic_home-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-18 05:49:07.000000 synthetic_home-0.1.0/tests/test_synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/synthetic_home/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/synthetic_home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/synthetic_home/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/synthetic_home/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/synthetic_home/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/synthetic_home/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/synthetic_home/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/synthetic_home/synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/synthetic_home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-20 14:50:19.000000 synthetic_home-2.0.0/synthetic_home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 14:50:19.000000 synthetic_home-2.0.0/synthetic_home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:50:19.000000 synthetic_home-2.0.0/synthetic_home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 14:50:19.000000 synthetic_home-2.0.0/synthetic_home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 14:50:19.000000 synthetic_home-2.0.0/synthetic_home.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:50:19.745274 synthetic_home-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-20 14:50:12.000000 synthetic_home-2.0.0/tests/test_synthetic_home.py
```

### Comparing `synthetic_home-0.1.0/LICENSE` & `synthetic_home-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthetic_home-0.1.0/PKG-INFO` & `synthetic_home-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 0.1.0
+Version: 2.0.0
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -96,42 +96,38 @@
 
 ### Entities
 
 Entities are specified by platform, where each value is an entity description
 key defined in the code somewhere. That is, adding a new entity type requires
 it being implemented somewhere in the smart home (e.g. `home-assistant-synthetic-home` custom component).
 
-### Supported Attributes and State
+### Device State
 
-A device type can have attributes like `unit_of_measure` that can vary for any
-specific instance of the device that is configured. One complication is that
-attributes on a device need to map to specific entities inside Home Assistant.
-Therefore we define `supported_attributes` at the device level and a mapping to
-`supported_attributes` on each entity.
-
-We make a distinction between `supported_attributes` and `supported_state_attributes`
-where the latter are attributes that may change throughout the lifecycle of the
-device. See _Restorable attributes below_. Both types of attributes can be used
-with entity supported attributes.
-
-An entity can map attributes with key value pair like `native_value=current_temperature`
-that maps the device attribute `current_temperature` to the entities
-`native_value`.
-
-### Pre-defined states
-
-A device type can define `predefined_states` that can support a pre-canned
-restorable states that can be used for testing and evaluating the other systems
-using synthetic entities.
+A device type defines `device_states` that can support a pre-defined states that
+can be used for testing and evaluating the other systems using synthetic entities.
 
 For example: When testing an HVAC device there are many different state attributes
 but there may only be a few _interesting_ states to evaluate such as:
 
 - The device is not running
 - The device target temperature is set to a normal range
 - The device target temperature is set to an abnormal range
 
-We use the pre-canned restorable states to simplify data generation to not need
+We use the pre-canned device states to simplify data generation to not need
 to consider every possibibility. This is implemented effectively as if setting
 these attributes in the config file.
 
-These should only be used with `supported_state_attributes`.
+### Device State Example
+
+You can set a `device_state` inline in the home. A `motion-sensor` devices three
+states by default `on`, `off`, and `battery-low`.  Be careful for special yaml
+truthy values, hence the value below is in quotes:
+
+```yaml
+---
+name: Family Farmhouse
+devices:
+  Front Yard:
+    - name: Front Yard Motion
+      device_type: motion-sensor
+      device_state: "on"
+```
```

### Comparing `synthetic_home-0.1.0/README.md` & `synthetic_home-2.0.0/synthetic_home.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: synthetic_home
+Version: 2.0.0
+Summary: Library for managing synthetic home device registry
+Home-page: https://github.com/allenporter/synthetic-home
+Author: Allen Porter
+Author-email: allen.porter@gmail.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mashumaro>=3.13
+
 # synthetic-home
 
 Library for managing synthetic home device registry. This project is primarily
 used by the [home-assistant-synthetic-home](https://github.com/allenporter/home-assistant-synthetic-home)
 custom component and the [home-assistant-datasets](https://github.com/allenporter/home-assistant-datasets)
 which creates instances of synthetic homes.
 
@@ -80,42 +96,38 @@
 
 ### Entities
 
 Entities are specified by platform, where each value is an entity description
 key defined in the code somewhere. That is, adding a new entity type requires
 it being implemented somewhere in the smart home (e.g. `home-assistant-synthetic-home` custom component).
 
-### Supported Attributes and State
+### Device State
 
-A device type can have attributes like `unit_of_measure` that can vary for any
-specific instance of the device that is configured. One complication is that
-attributes on a device need to map to specific entities inside Home Assistant.
-Therefore we define `supported_attributes` at the device level and a mapping to
-`supported_attributes` on each entity.
-
-We make a distinction between `supported_attributes` and `supported_state_attributes`
-where the latter are attributes that may change throughout the lifecycle of the
-device. See _Restorable attributes below_. Both types of attributes can be used
-with entity supported attributes.
-
-An entity can map attributes with key value pair like `native_value=current_temperature`
-that maps the device attribute `current_temperature` to the entities
-`native_value`.
-
-### Pre-defined states
-
-A device type can define `predefined_states` that can support a pre-canned
-restorable states that can be used for testing and evaluating the other systems
-using synthetic entities.
+A device type defines `device_states` that can support a pre-defined states that
+can be used for testing and evaluating the other systems using synthetic entities.
 
 For example: When testing an HVAC device there are many different state attributes
 but there may only be a few _interesting_ states to evaluate such as:
 
 - The device is not running
 - The device target temperature is set to a normal range
 - The device target temperature is set to an abnormal range
 
-We use the pre-canned restorable states to simplify data generation to not need
+We use the pre-canned device states to simplify data generation to not need
 to consider every possibibility. This is implemented effectively as if setting
 these attributes in the config file.
 
-These should only be used with `supported_state_attributes`.
+### Device State Example
+
+You can set a `device_state` inline in the home. A `motion-sensor` devices three
+states by default `on`, `off`, and `battery-low`.  Be careful for special yaml
+truthy values, hence the value below is in quotes:
+
+```yaml
+---
+name: Family Farmhouse
+devices:
+  Front Yard:
+    - name: Front Yard Motion
+      device_type: motion-sensor
+      device_state: "on"
+```
```

### Comparing `synthetic_home-0.1.0/pyproject.toml` & `synthetic_home-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synthetic_home-0.1.0/setup.cfg` & `synthetic_home-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = synthetic_home
-version = 0.1.0
+version = 2.0.0
 description = Library for managing synthetic home device registry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/synthetic-home
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `synthetic_home-0.1.0/synthetic_home.egg-info/PKG-INFO` & `synthetic_home-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: synthetic_home
-Version: 0.1.0
-Summary: Library for managing synthetic home device registry
-Home-page: https://github.com/allenporter/synthetic-home
-Author: Allen Porter
-Author-email: allen.porter@gmail.com
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: mashumaro>=3.13
-
 # synthetic-home
 
 Library for managing synthetic home device registry. This project is primarily
 used by the [home-assistant-synthetic-home](https://github.com/allenporter/home-assistant-synthetic-home)
 custom component and the [home-assistant-datasets](https://github.com/allenporter/home-assistant-datasets)
 which creates instances of synthetic homes.
 
@@ -96,42 +80,38 @@
 
 ### Entities
 
 Entities are specified by platform, where each value is an entity description
 key defined in the code somewhere. That is, adding a new entity type requires
 it being implemented somewhere in the smart home (e.g. `home-assistant-synthetic-home` custom component).
 
-### Supported Attributes and State
+### Device State
 
-A device type can have attributes like `unit_of_measure` that can vary for any
-specific instance of the device that is configured. One complication is that
-attributes on a device need to map to specific entities inside Home Assistant.
-Therefore we define `supported_attributes` at the device level and a mapping to
-`supported_attributes` on each entity.
-
-We make a distinction between `supported_attributes` and `supported_state_attributes`
-where the latter are attributes that may change throughout the lifecycle of the
-device. See _Restorable attributes below_. Both types of attributes can be used
-with entity supported attributes.
-
-An entity can map attributes with key value pair like `native_value=current_temperature`
-that maps the device attribute `current_temperature` to the entities
-`native_value`.
-
-### Pre-defined states
-
-A device type can define `predefined_states` that can support a pre-canned
-restorable states that can be used for testing and evaluating the other systems
-using synthetic entities.
+A device type defines `device_states` that can support a pre-defined states that
+can be used for testing and evaluating the other systems using synthetic entities.
 
 For example: When testing an HVAC device there are many different state attributes
 but there may only be a few _interesting_ states to evaluate such as:
 
 - The device is not running
 - The device target temperature is set to a normal range
 - The device target temperature is set to an abnormal range
 
-We use the pre-canned restorable states to simplify data generation to not need
+We use the pre-canned device states to simplify data generation to not need
 to consider every possibibility. This is implemented effectively as if setting
 these attributes in the config file.
 
-These should only be used with `supported_state_attributes`.
+### Device State Example
+
+You can set a `device_state` inline in the home. A `motion-sensor` devices three
+states by default `on`, `off`, and `battery-low`.  Be careful for special yaml
+truthy values, hence the value below is in quotes:
+
+```yaml
+---
+name: Family Farmhouse
+devices:
+  Front Yard:
+    - name: Front Yard Motion
+      device_type: motion-sensor
+      device_state: "on"
+```
```

### Comparing `synthetic_home-0.1.0/tests/test_synthetic_home.py` & `synthetic_home-2.0.0/tests/test_synthetic_home.py`

 * *Files identical despite different names*

