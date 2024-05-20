# Comparing `tmp/seam-0.7.0.tar.gz` & `tmp/seam-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.7.0.tar", max compression
+gzip compressed data, was "seam-0.7.1.tar", max compression
```

## Comparing `seam-0.7.0.tar` & `seam-0.7.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1087 2024-05-16 15:45:20.934088 seam-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     9355 2024-05-16 15:45:20.938088 seam-0.7.0/README.rst
--rw-r--r--   0        0        0      726 2024-05-16 15:45:20.938088 seam-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      397 2024-05-16 15:45:20.938088 seam-0.7.0/seam/__init__.py
--rw-r--r--   0        0        0     4076 2024-05-16 15:45:20.938088 seam-0.7.0/seam/auth.py
--rw-r--r--   0        0        0       72 2024-05-16 15:45:20.938088 seam-0.7.0/seam/constants.py
--rw-r--r--   0        0        0     2018 2024-05-16 15:45:20.938088 seam-0.7.0/seam/options.py
--rw-r--r--   0        0        0      623 2024-05-16 15:45:20.938088 seam-0.7.0/seam/parse_options.py
--rw-r--r--   0        0        0     1337 2024-05-16 15:45:20.938088 seam-0.7.0/seam/request.py
--rw-r--r--   0        0        0    11981 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/access_codes.py
--rw-r--r--   0        0        0      915 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/access_codes_simulate.py
--rw-r--r--   0        0        0     3991 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1824 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs.py
--rw-r--r--   0        0        0     2513 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_access_groups.py
--rw-r--r--   0        0        0      730 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_credential_pools.py
--rw-r--r--   0        0        0     1807 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4964 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_credentials.py
--rw-r--r--   0        0        0     2180 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_entrances.py
--rw-r--r--   0        0        0     1476 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_systems.py
--rw-r--r--   0        0        0     6505 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/acs_users.py
--rw-r--r--   0        0        0     3982 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/action_attempts.py
--rw-r--r--   0        0        0     5780 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/client_sessions.py
--rw-r--r--   0        0        0     3321 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/connect_webviews.py
--rw-r--r--   0        0        0     2549 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/connected_accounts.py
--rw-r--r--   0        0        0     4804 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/devices.py
--rw-r--r--   0        0        0      546 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/devices_simulate.py
--rw-r--r--   0        0        0     3352 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/devices_unmanaged.py
--rw-r--r--   0        0        0     2414 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/events.py
--rw-r--r--   0        0        0     4210 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/locks.py
--rw-r--r--   0        0        0      794 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/networks.py
--rw-r--r--   0        0        0      757 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/noise_sensors.py
--rw-r--r--   0        0        0     4362 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      623 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1099 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/phones.py
--rw-r--r--   0        0        0     1214 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/phones_simulate.py
--rw-r--r--   0        0        0     1436 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/routes.py
--rw-r--r--   0        0        0     8962 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/thermostats.py
--rw-r--r--   0        0        0     6955 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    64963 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/types.py
--rw-r--r--   0        0        0     6732 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/user_identities.py
--rw-r--r--   0        0        0     2928 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      864 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1844 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/webhooks.py
--rw-r--r--   0        0        0     2182 2024-05-16 15:45:20.938088 seam-0.7.0/seam/routes/workspaces.py
--rw-r--r--   0        0        0     2555 2024-05-16 15:45:20.938088 seam-0.7.0/seam/seam.py
--rw-r--r--   0        0        0     2418 2024-05-16 15:45:20.938088 seam-0.7.0/seam/seam_multi_workspace.py
--rw-r--r--   0        0        0     1027 2024-05-16 15:45:20.938088 seam-0.7.0/seam/token.py
--rw-r--r--   0        0        0     3242 2024-05-16 15:45:20.938088 seam-0.7.0/seam/types.py
--rw-r--r--   0        0        0    10105 1970-01-01 00:00:00.000000 seam-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-20 16:46:52.747360 seam-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0    10091 2024-05-20 16:46:52.747360 seam-0.7.1/README.rst
+-rw-r--r--   0        0        0      726 2024-05-20 16:46:52.747360 seam-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      397 2024-05-20 16:46:52.747360 seam-0.7.1/seam/__init__.py
+-rw-r--r--   0        0        0     4076 2024-05-20 16:46:52.747360 seam-0.7.1/seam/auth.py
+-rw-r--r--   0        0        0       72 2024-05-20 16:46:52.747360 seam-0.7.1/seam/constants.py
+-rw-r--r--   0        0        0     2018 2024-05-20 16:46:52.751360 seam-0.7.1/seam/options.py
+-rw-r--r--   0        0        0      623 2024-05-20 16:46:52.751360 seam-0.7.1/seam/parse_options.py
+-rw-r--r--   0        0        0     1337 2024-05-20 16:46:52.751360 seam-0.7.1/seam/request.py
+-rw-r--r--   0        0        0    11981 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/access_codes.py
+-rw-r--r--   0        0        0      915 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/access_codes_simulate.py
+-rw-r--r--   0        0        0     3991 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1824 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs.py
+-rw-r--r--   0        0        0     2513 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_access_groups.py
+-rw-r--r--   0        0        0      730 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_credential_pools.py
+-rw-r--r--   0        0        0     1807 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4964 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_credentials.py
+-rw-r--r--   0        0        0     2180 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_entrances.py
+-rw-r--r--   0        0        0     1476 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_systems.py
+-rw-r--r--   0        0        0     6505 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_users.py
+-rw-r--r--   0        0        0     3982 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/action_attempts.py
+-rw-r--r--   0        0        0     5780 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/client_sessions.py
+-rw-r--r--   0        0        0     3321 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/connect_webviews.py
+-rw-r--r--   0        0        0     2549 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/connected_accounts.py
+-rw-r--r--   0        0        0     4804 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/devices.py
+-rw-r--r--   0        0        0      546 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/devices_simulate.py
+-rw-r--r--   0        0        0     3352 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/devices_unmanaged.py
+-rw-r--r--   0        0        0     2414 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/events.py
+-rw-r--r--   0        0        0     4210 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/locks.py
+-rw-r--r--   0        0        0      794 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/networks.py
+-rw-r--r--   0        0        0      757 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/noise_sensors.py
+-rw-r--r--   0        0        0     4362 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      623 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1099 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/phones.py
+-rw-r--r--   0        0        0     1214 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/phones_simulate.py
+-rw-r--r--   0        0        0     1436 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/routes.py
+-rw-r--r--   0        0        0     8962 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/thermostats.py
+-rw-r--r--   0        0        0     6955 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64963 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/types.py
+-rw-r--r--   0        0        0     6732 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/user_identities.py
+-rw-r--r--   0        0        0     2928 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1844 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/webhooks.py
+-rw-r--r--   0        0        0     2182 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/workspaces.py
+-rw-r--r--   0        0        0     2555 2024-05-20 16:46:52.751360 seam-0.7.1/seam/seam.py
+-rw-r--r--   0        0        0     2418 2024-05-20 16:46:52.751360 seam-0.7.1/seam/seam_multi_workspace.py
+-rw-r--r--   0        0        0     1027 2024-05-20 16:46:52.751360 seam-0.7.1/seam/token.py
+-rw-r--r--   0        0        0     3242 2024-05-20 16:46:52.751360 seam-0.7.1/seam/types.py
+-rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 seam-0.7.1/PKG-INFO
```

### Comparing `seam-0.7.0/LICENSE.txt` & `seam-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/README.rst` & `seam-0.7.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -187,14 +187,32 @@
 
       print("Door unlocked")
   except SeamActionAttemptFailedError as e:
       print("Could not unlock the door")
   except SeamActionAttemptTimeoutError as e:
       print("Door took too long to unlock")
 
+Interacting with Multiple Workspaces
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Some Seam API endpoints interact with multiple workspaces. The ``SeamMultiWorkspace`` client is not bound to a specific workspace and may use those endpoints with a personal access token authentication method.
+
+A Personal Access Token is scoped to a Seam Console user. Obtain one from the Seam Console.
+
+.. code-block:: python
+
+  # Pass as an option the constructor
+  seam = SeamMultiWorkspace(personal_access_token="your-personal-access-token")
+
+  # Use the factory method
+  seam = SeamMultiWorkspace.from_personal_access_token("your-personal-access-token")
+
+  # List workspaces authorized for this Personal Access Token
+  workspaces = seam.workspaces.list()
+
 Advanced Usage
 ~~~~~~~~~~~~~~
 
 Setting the endpoint
 ^^^^^^^^^^^^^^^^^^^^
 
 Some contexts may need to override the API endpoint,
```

### Comparing `seam-0.7.0/pyproject.toml` & `seam-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seam"
-version = "0.7.0"
+version = "0.7.1"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
```

### Comparing `seam-0.7.0/seam/auth.py` & `seam-0.7.1/seam/auth.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/options.py` & `seam-0.7.1/seam/options.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/parse_options.py` & `seam-0.7.1/seam/parse_options.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/access_codes.py` & `seam-0.7.1/seam/routes/access_codes.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/access_codes_simulate.py` & `seam-0.7.1/seam/routes/access_codes_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/access_codes_unmanaged.py` & `seam-0.7.1/seam/routes/access_codes_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs.py` & `seam-0.7.1/seam/routes/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_access_groups.py` & `seam-0.7.1/seam/routes/acs_access_groups.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_credential_pools.py` & `seam-0.7.1/seam/routes/acs_credential_pools.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_credential_provisioning_automations.py` & `seam-0.7.1/seam/routes/acs_credential_provisioning_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_credentials.py` & `seam-0.7.1/seam/routes/acs_credentials.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_entrances.py` & `seam-0.7.1/seam/routes/acs_entrances.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_systems.py` & `seam-0.7.1/seam/routes/acs_systems.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/acs_users.py` & `seam-0.7.1/seam/routes/acs_users.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/action_attempts.py` & `seam-0.7.1/seam/routes/action_attempts.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/client_sessions.py` & `seam-0.7.1/seam/routes/client_sessions.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/connect_webviews.py` & `seam-0.7.1/seam/routes/connect_webviews.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/connected_accounts.py` & `seam-0.7.1/seam/routes/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/devices.py` & `seam-0.7.1/seam/routes/devices.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/devices_simulate.py` & `seam-0.7.1/seam/routes/devices_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/devices_unmanaged.py` & `seam-0.7.1/seam/routes/devices_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/events.py` & `seam-0.7.1/seam/routes/events.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/locks.py` & `seam-0.7.1/seam/routes/locks.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/networks.py` & `seam-0.7.1/seam/routes/networks.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/noise_sensors.py` & `seam-0.7.1/seam/routes/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/noise_sensors_noise_thresholds.py` & `seam-0.7.1/seam/routes/noise_sensors_noise_thresholds.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/noise_sensors_simulate.py` & `seam-0.7.1/seam/routes/noise_sensors_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/phones.py` & `seam-0.7.1/seam/routes/phones.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/phones_simulate.py` & `seam-0.7.1/seam/routes/phones_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/routes.py` & `seam-0.7.1/seam/routes/routes.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/thermostats.py` & `seam-0.7.1/seam/routes/thermostats.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/thermostats_climate_setting_schedules.py` & `seam-0.7.1/seam/routes/thermostats_climate_setting_schedules.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/types.py` & `seam-0.7.1/seam/routes/types.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/user_identities.py` & `seam-0.7.1/seam/routes/user_identities.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/user_identities_enrollment_automations.py` & `seam-0.7.1/seam/routes/user_identities_enrollment_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/utils/deep_attr_dict.py` & `seam-0.7.1/seam/routes/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/webhooks.py` & `seam-0.7.1/seam/routes/webhooks.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/routes/workspaces.py` & `seam-0.7.1/seam/routes/workspaces.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/seam.py` & `seam-0.7.1/seam/seam.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/seam_multi_workspace.py` & `seam-0.7.1/seam/seam_multi_workspace.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/token.py` & `seam-0.7.1/seam/token.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.0/seam/types.py` & `seam-0.7.1/seam/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Self
 import abc
 
 from seam.routes.types import AbstractRoutes, Workspace
 
 
-class SeamApiException(Exception):
+class SeamHttpApiError(Exception):
     def __init__(
         self,
         response,
     ):
         self.status_code = response.status_code
         self.request_id = response.headers.get("seam-request-id", None)
 
         self.metadata = None
         if "application/json" in response.headers["content-type"]:
             parsed_response = response.json()
             self.metadata = parsed_response.get("error", None)
 
         super().__init__(
-            f"SeamApiException: status={self.status_code}, request_id={self.request_id}, metadata={self.metadata}"
+            f"SeamHttpApiError: status={self.status_code}, request_id={self.request_id}, metadata={self.metadata}"
         )
 
 
 class AbstractRequestMixin(abc.ABC):
     @abc.abstractmethod
     def make_request(self, method: str, path: str, **kwargs):
         raise NotImplementedError
```

### Comparing `seam-0.7.0/PKG-INFO` & `seam-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.7.0
+Version: 0.7.1
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -207,14 +207,32 @@
 
       print("Door unlocked")
   except SeamActionAttemptFailedError as e:
       print("Could not unlock the door")
   except SeamActionAttemptTimeoutError as e:
       print("Door took too long to unlock")
 
+Interacting with Multiple Workspaces
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Some Seam API endpoints interact with multiple workspaces. The ``SeamMultiWorkspace`` client is not bound to a specific workspace and may use those endpoints with a personal access token authentication method.
+
+A Personal Access Token is scoped to a Seam Console user. Obtain one from the Seam Console.
+
+.. code-block:: python
+
+  # Pass as an option the constructor
+  seam = SeamMultiWorkspace(personal_access_token="your-personal-access-token")
+
+  # Use the factory method
+  seam = SeamMultiWorkspace.from_personal_access_token("your-personal-access-token")
+
+  # List workspaces authorized for this Personal Access Token
+  workspaces = seam.workspaces.list()
+
 Advanced Usage
 ~~~~~~~~~~~~~~
 
 Setting the endpoint
 ^^^^^^^^^^^^^^^^^^^^
 
 Some contexts may need to override the API endpoint,
```

