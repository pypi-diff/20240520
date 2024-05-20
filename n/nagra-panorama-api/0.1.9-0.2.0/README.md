# Comparing `tmp/nagra_panorama_api-0.1.9.tar.gz` & `tmp/nagra_panorama_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagra_panorama_api-0.1.9.tar", max compression
+gzip compressed data, was "nagra_panorama_api-0.2.0.tar", max compression
```

## Comparing `nagra_panorama_api-0.1.9.tar` & `nagra_panorama_api-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,23 @@
--rw-r--r--   0        0        0     1934 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-11-30 10:34:33.670102 nagra_panorama_api-0.1.9/nagra_panorama_api/__init__.py
--rw-r--r--   0        0        0      312 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/nagra_panorama_api/__main__.py
--rw-r--r--   0        0        0     6032 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/nagra_panorama_api/config.py
--rw-r--r--   0        0        0     1934 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/nagra_panorama_api/constants.py
--rw-r--r--   0        0        0    11224 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/nagra_panorama_api/dump_dir.py
--rw-r--r--   0        0        0    14704 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/nagra_panorama_api/rest_resources.py
--rw-r--r--   0        0        0     9798 2023-11-27 10:41:19.831599 nagra_panorama_api-0.1.9/nagra_panorama_api/restapi.py
--rw-r--r--   0        0        0     3368 2023-11-27 10:41:19.835600 nagra_panorama_api-0.1.9/nagra_panorama_api/utils.py
--rw-r--r--   0        0        0      682 2023-11-27 10:41:19.835600 nagra_panorama_api-0.1.9/nagra_panorama_api/wrappers.py
--rw-r--r--   0        0        0    13995 2023-11-27 10:41:19.835600 nagra_panorama_api-0.1.9/nagra_panorama_api/xmlapi.py
--rw-r--r--   0        0        0      886 2023-11-30 10:34:33.430101 nagra_panorama_api-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 nagra_panorama_api-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2583 2024-05-20 18:55:46.627517 nagra_panorama_api-0.2.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-20 18:55:46.627517 nagra_panorama_api-0.2.0/nagra_panorama_api/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-20 18:55:46.627517 nagra_panorama_api-0.2.0/nagra_panorama_api/__main__.py
+-rw-r--r--   0        0        0      484 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/commands/__init__.py
+-rw-r--r--   0        0        0     1779 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/commands/common.py
+-rw-r--r--   0        0        0     4354 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/commands/dump_configs.py
+-rw-r--r--   0        0        0    11698 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/commands/dump_dir.py
+-rw-r--r--   0        0        0    15198 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/commands/software_update.py
+-rw-r--r--   0        0        0     1715 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/commands/utils.py
+-rw-r--r--   0        0        0     1763 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/constants.py
+-rw-r--r--   0        0        0      849 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/panorama.py
+-rw-r--r--   0        0        0       36 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/restapi/__init__.py
+-rw-r--r--   0        0        0    15111 2024-05-20 18:55:46.631517 nagra_panorama_api-0.2.0/nagra_panorama_api/restapi/rest_resources.py
+-rw-r--r--   0        0        0     8590 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/restapi/restapi.py
+-rw-r--r--   0        0        0      402 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/utils.py
+-rw-r--r--   0        0        0       27 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/__init__.py
+-rw-r--r--   0        0        0     4259 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/base.py
+-rw-r--r--   0        0        0    31427 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/client.py
+-rw-r--r--   0        0        0      166 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/constants.py
+-rw-r--r--   0        0        0     9283 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/types/__init__.py
+-rw-r--r--   0        0        0     3937 2024-05-20 18:55:46.635517 nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/utils.py
+-rw-r--r--   0        0        0      969 2024-05-20 19:01:09.639173 nagra_panorama_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 nagra_panorama_api-0.2.0/PKG-INFO
```

### Comparing `nagra_panorama_api-0.1.9/README.md` & `nagra_panorama_api-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 # README
 
-## Why the need for this library ?
-
-For simple resource retrieval, the existing API is enough, but:
+This repository contains a wrapper around Panorama/PaloAlto API.
+It also provides a cli tool `panorama_api`
 
-* The libraries available are not practical for it, the manual management of urls is easier
-
-* For more complex operation, this does not suits well
 
-The python SDK of PaloAltoNetworks itself relies on a third party wrapper for their API.
+## CLI
+This package also provide a CLI tool for some operations:
+* Generating an API Key
+* Upgrading a group of devices
+* Generating a boilerplate configuration file for the upgrades
 
 
+```bash
+pip install nagra_panorama_api
+panorama_api --help
+```
 
-## Design
-
-The library provides 2 things:
 
-* A simple client for the API
+## Why the need for this library ?
 
-* Tool to manage the xml configuration
+For simple resource retrieval, the existing API is enough, but:
 
-We will pull the whole configuration and search on it locally. We can then use the client to do some operations
+* The libraries available are not practical for it, the manual management of urls is easier
+* For more complex operation, this does not suits well
 
+The [official python SDK of PaloAltoNetworks](https://github.com/PaloAltoNetworks/pan-os-python) itself relies on a [third party wrapper](https://github.com/kevinsteves/pan-python) for their API.
 
 
-We don't want to combine both the client and the management tool. This would requires a lot of boilerplate code that would be difficult to maintain.
+This library takes a more popular approach when wrapping the API, making it easier to use. It also provides types' wrappers to simplify their usage or utility functions to re-structure the data we receive.
+It provides a client for the REST API and for the XML API
 
+* A simple client for the API
+* Tool to manage the xml configuration
 
 
-## Usage
+## Library Usage Example
 
 ```python
 client = XMLApi(HOST, API_KEY)
 tree = client.get_tree()
 
 # Find your object using its name (may not be unique)
 my_object = config.find_by_name("my_object_name")[0]
@@ -51,21 +57,22 @@
 # We can also revert it
 # client.revert_changes()
 ```
 
 The library currently doesn't provide helper tools to know how to edit the configuration. Theses changes must be done manually
 
 
-
-
-
 ## TODO
 
 * Provide wrapper classes for the resources.
 
   ```python
   nat = NatPolicy(...)
   tree.insert(nat)  # or nat.insertInto(tree)
   client.create(nat.insert_xpath, nat.xml)
   ```
 * # Mix Rest API and XML API ?
-  https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/get-started-with-the-pan-os-rest-api/create-security-policy-rule-rest-api
+  https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/get-started-with-the-pan-os-rest-api/create-security-policy-rule-rest-api
+
+
+## Links
+* [Official upgrade procedure on HA with API](https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/pan-os-xml-api-use-cases/upgrade-pan-os-on-multiple-ha-firewalls-through-panorama-api)
```

### Comparing `nagra_panorama_api-0.1.9/nagra_panorama_api/constants.py` & `nagra_panorama_api-0.2.0/nagra_panorama_api/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-PATH_SEARCH_PREFIX = "./devices/entry/device-group"
-CONFIG_XPATH = "/config/devices/entry/device-group"
-PATH_NAME_PREFIX = "/config/devices/entry/device-group/entry"
-
 # https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/get-started-with-the-pan-os-rest-api/pan-os-rest-api-error-codes
 PANORAMA_ERRORS = {
     1: "The operation was canceled, typically by the caller.",
     2: "Unknown internal server error.",
     3: "Bad request. The caller specified an invalid parameter.",
     4: (
         "Gateway timeout. A firewall or Panorama module timed out "
```

### Comparing `nagra_panorama_api-0.1.9/nagra_panorama_api/dump_dir.py` & `nagra_panorama_api-0.2.0/nagra_panorama_api/commands/dump_dir.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 from pathlib import Path
 
 import click
 
 # https://stackoverflow.com/questions/27981545/suppress-insecurerequestwarning-unverified-https-request-is-being-made-in-pytho
 import urllib3
 
-from .restapi import PanoramaClient
-from .utils import el2dict
-from .xmlapi import XMLApi
+from nagra_panorama_api.restapi import PanoramaClient
+from nagra_panorama_api.xmlapi import XMLApi
+from nagra_panorama_api.xmlapi.utils import el2dict
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-log = logging.getLogger("Dump")
 
 
 def xpath(el, expr):
     res = el.xpath(expr)
     if not res:
         return None
     return res[0]
@@ -97,15 +96,15 @@
 def _flatten_dict(d):
     if not isinstance(d, dict):
         yield (d,)  # Use a tuple because it will be unpacked
         return
     for k, v in d.items():
         tmp = list(_flatten_dict(v))
         for *keys, data in tmp:
-            yield k, *keys, data
+            yield (k, *keys, data)
 
 
 def flatten_grouped_rules(rules):
     "device-group -> pre/post -> rule"
     groups = group_rules(rules)
     return list(_flatten_dict(groups))
 
@@ -202,18 +201,18 @@
         ),
     },
 ]
 
 
 def dump_dir_xml(output, host, api_key):
     client = XMLApi(host, api_key)
-    log.info("Starting to retrieve the data (extended informations)")
+    logging.info("Starting to retrieve the data (extended informations)")
     tree = client.get_tree(extended=True)
 
-    log.info("Data retrieved, starting the export")
+    logging.info("Data retrieved, starting the export")
     output = Path(output).resolve()
     output.mkdir(parents=True, exist_ok=True)
 
     address_elements = tree.xpath("devices/entry/device-group/*/address/entry")
     address_group_elements = tree.xpath(
         "devices/entry/device-group/*/address-group/entry",
     )
@@ -230,15 +229,15 @@
     with open(output / "addresses.json", "w") as f:
         json.dump(addresses, f)
     with open(output / "addressGroups.json", "w") as f:
         json.dump(addresses_groups, f)
 
     prepare_rules(tree, RULES)
     dump_rules(output, RULES)
-    log.info("Export done")
+    logging.info("Export done")
 
 
 def get_rest_rules(client, device_group):
     return [
         {
             "rule_type": "security",
             "folder": "securityRules",
@@ -283,14 +282,26 @@
                 inherited=False,
             ),
             "post-data": client.policies.ApplicationOverridePostRules.get(
                 device_group=device_group,
                 inherited=False,
             ),
         },
+        {
+            "rule_type": "decryption",
+            "folder": "decryption",
+            "pre-data": client.policies.DecryptionPreRules.get(
+                device_group=device_group,
+                inherited=False,
+            ),
+            "post-data": client.policies.DecryptionPostRules.get(
+                device_group=device_group,
+                inherited=False,
+            ),
+        },
     ]
 
 
 def grouped_rest_rules(rules):
     # device-group -> pre/post -> rule
     grouped = {}
     for r in rules:
@@ -322,33 +333,33 @@
         for filename, rules in data:
             with open(directory / filename, "w") as f:
                 json.dump(rules, f)
 
 
 def dump_dir_rest(output, host, api_key):
     client = PanoramaClient(host, api_key)
-    log.info("Starting to retrieve the data (extended informations)")
+    logging.info("Starting to retrieve the data (extended informations)")
     groups = [d["@name"] for d in client.panorama.DeviceGroups.get()]
     addresses = client.objects.Addresses.get(device_group=groups, inherited=False)
     addresses_groups = client.objects.AddressGroups.get(
         device_group=groups,
         inherited=False,
     )
 
     rules = get_rest_rules(client, groups)
-    log.info("Data retrieved, starting the export")
+    logging.info("Data retrieved, starting the export")
     output = Path(output).resolve()
     output.mkdir(parents=True, exist_ok=True)
 
     with open(output / "addresses.json", "w") as f:
         json.dump(addresses, f)
     with open(output / "addressGroups.json", "w") as f:
         json.dump(addresses_groups, f)
     dump_rest_rules(output, rules)
-    log.info("Export done")
+    logging.info("Export done")
 
 
 @click.command(
     "dump-dir",
     help="Dump data from palo alto",
 )
 @click.option("-o", "--output", help="Output directory", default="output")
```

### Comparing `nagra_panorama_api-0.1.9/nagra_panorama_api/rest_resources.py` & `nagra_panorama_api-0.2.0/nagra_panorama_api/restapi/rest_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         client,
         host,
         resource_type,
         resource,
         version="v10.1",
         default_params=None,
     ):
+        """
+        client:
+        """
         self.DEFAULT_PARAMS = default_params or DEFAULT_PARAMS
         if not host.startswith("http"):
             host = "https://" + host
         self._client = client
         self._name = f"{resource_type}/{resource}"
         self._url = f"{host}/restapi/{version}/{resource_type}/{resource}"
 
@@ -80,14 +83,16 @@
             )
             if not isinstance(res, list):
                 return []  # Error happened
             if not inherited:
                 res = [r for r in res if r["@device-group"] == r["@loc"]]
             return res
 
+        if device_group is None:
+            return func(params)
         if isinstance(device_group, str):
             device_group = [device_group]
         if len(device_group) == 1:
             params = {"device-group": device_group}
             return func(params)
         if len(device_group) > 1:
             params_list = [{"device-group": dg} for dg in device_group]
@@ -176,14 +181,18 @@
                 version=version,
             )
 
         self.DeviceGroups = resource("DeviceGroups")
 
 
 class PanoramaObjectsResourceType(PanoramaResourceType):
+    """
+    Represent the 'Objects' subsection in the API.
+    """
+
     resource_type = "Objects"
 
     def __init__(self, client, domain, version="v10.1"):
         resource_type = self.resource_type
         super().__init__(client, resource_type)
 
         def resource(name):
@@ -232,24 +241,28 @@
         self.SDWANPathQualityProfiles = resource("SDWANPathQualityProfiles")
         self.SDWANTrafficDistributionProfiles = resource(
             "SDWANTrafficDistributionProfiles",
         )
 
 
 class PanoramaPoliciesResourceType(PanoramaResourceType):
+    """
+    Represent the 'Policies' subsection in the API.
+    """
+
     resource_type = "Policies"
 
     def __init__(self, client, domain, version="v10.1"):
         resource_type = self.resource_type
         super().__init__(client, resource_type)
 
         def resource(name):
             return PanoramaResource(
                 client,
-                domain,
+                domain,  # host
                 resource_type,
                 name,
                 version=version,
             )
 
         self.SecurityPreRules = resource("SecurityPreRules")
         self.SecurityPostRules = resource("SecurityPostRules")
@@ -298,14 +311,18 @@
         self.DoSRules = GroupedResources(self.DoSPreRules, self.DoSPostRules)
         self.SDWANPreRules = resource("SDWANPreRules")
         self.SDWANPostRules = resource("SDWANPostRules")
         self.SDWANRules = GroupedResources(self.SDWANPreRules, self.SDWANPostRules)
 
 
 class PanoramaNetworkResourceType(PanoramaResourceType):
+    """
+    Represent the 'Network' subsection in the API.
+    """
+
     DEFAULT_PARAMS: ClassVar = {
         "location": "template",
     }
     resource_type = "Network"
 
     def __init__(self, client, domain, version="v10.1"):
         resource_type = self.resource_type
@@ -363,14 +380,18 @@
         self.ZoneProtectionNetworkProfiles = resource("ZoneProtectionNetworkProfiles")
         self.QoSNetworkProfiles = resource("QoSNetworkProfiles")
         self.LLDPNetworkProfiles = resource("LLDPNetworkProfiles")
         self.SDWANInterfaceProfiles = resource("SDWANInterfaceProfiles")
 
 
 class PanoramaDevicesResourceType(PanoramaResourceType):
+    """
+    Represent the 'Devices' subsection in the API.
+    """
+
     DEFAULT_PARAMS: ClassVar = {
         "location": "template",
     }
     resource_type = "Device"
 
     def __init__(self, client, domain, version="v10.1"):
         resource_type = self.resource_type
```

### Comparing `nagra_panorama_api-0.1.9/nagra_panorama_api/restapi.py` & `nagra_panorama_api-0.2.0/nagra_panorama_api/restapi/restapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,69 +4,27 @@
 
 import requests
 
 # Remove warning for unverified certificate
 # https://stackoverflow.com/questions/27981545/suppress-insecurerequestwarning-unverified-https-request-is-being-made-in-pytho
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
+from nagra_panorama_api.constants import PANORAMA_ERRORS, SUCCESS_CODE
+from nagra_panorama_api.utils import clean_url_host
+
 from .rest_resources import (
     PanoramaDevicesResourceType,
     PanoramaNetworkResourceType,
     PanoramaObjectsResourceType,
     PanoramaPanoramaResourceType,
     PanoramaPoliciesResourceType,
 )
 
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
-log = logging.getLogger(__name__)
-
-# https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/get-started-with-the-pan-os-rest-api/pan-os-rest-api-error-codes
-PANORAMA_ERRORS = {
-    1: ("The operation was canceled, typically by the caller."),
-    2: ("Unknown internal server error."),
-    3: ("Bad request. The caller specified an invalid parameter."),
-    4: (
-        "Gateway timeout. A firewall or Panorama module timed out "
-        "before a backend operation completed."
-    ),
-    5: ("Not found. The requested entity was not found."),
-    6: ("Conflict. The entity that the caller attempted to create already exists."),
-    7: (
-        "Forbidden. The caller does not have permission "
-        "to execute the specified operation."
-    ),
-    8: ("Resource exhausted. Some resource has been exhausted."),
-    9: (
-        "Failed precondition. The operation was rejected because "
-        "the system is not in a state required "
-        "for the execution of the operation."
-    ),
-    10: ("Aborted because of conflict. A typical cause is a concurrency issue."),
-    11: (
-        "Out of range. The operation was attempted past a valid range. "
-        "And example is reaching an end-of-file."
-    ),
-    12: (
-        "Not implemented. The operation is disabled, not implemented, "
-        "or not supported."
-    ),
-    13: (
-        "Internal server error. An unexpected and potentially serious "
-        "internal error occurred."
-    ),
-    14: ("Service unavailable. The service is temporarily unavailable."),
-    15: ("Internal server error. Unrecoverable data loss or data corruption occurred."),
-    16: (
-        "Unauthorized. The request does not have "
-        "valid authentication credentials to perform the operation."
-    ),
-}
-SUCCESS_CODE = 19
-
 OBJECT_RESOURCES = [
     "Addresses",
     "AddressGroups",
     "Regions",
     "Applications",
     "ApplicationGroups",
     "ApplicationFilters",
@@ -153,18 +111,19 @@
 
 DEFAULT_PARAMS = {
     "output-format": "json",
 }
 
 
 class PanoramaAPI:
-    def __init__(self, api_key=None, verbose=False, verify=False):
+    def __init__(self, api_key=None, verbose=False, verify=False, logger=None):
         self._verbose = verbose
         self._verify = verify
         self._api_key = api_key
+        self.logger = logger or logging
 
     def _inner_request(
         self,
         method,
         url,
         params=None,
         headers=None,
@@ -195,19 +154,21 @@
         # if not res.ok:
         #     return None
         try:
             data = res.json()
             code = int(
                 data.get("@code") or data.get("code") or SUCCESS_CODE,
             )  # Sometimes, the code is a string, some other times it is a int
+            status = data.get("@status", "")
+            success = status == "success"
             error_occured = (
                 not res.ok
-                or data.get("@status", "") != "success"
-                # In case of success, the value 19 is used
-                or code < SUCCESS_CODE
+                or (
+                    not success and code < SUCCESS_CODE
+                )  # In case of success, the value 19 is used
             )
             if not error_occured:
                 return data, None
             message = (
                 data.get("message")
                 or PANORAMA_ERRORS.get(data["@code"])
                 or "Something happened: " + json.dumps(data)
@@ -247,15 +208,15 @@
                 data=data,
                 verify=verify,
             )
             or {}
         )
         if error:
             if no_exception:
-                log.error(f"Could not {method.lower()} {url}: {error}")
+                self.logger.error(f"Could not {method.lower()} {url}: {error}")
                 return data, error
             raise Exception(error)
         data = data.get("result", {}).get("entry") or []
         return data, error
 
     def request(self, method, url, params=None, headers=None, data=None, verify=None):
         data, _ = (
@@ -298,22 +259,30 @@
             )
             or {}
         )
         return data
 
 
 class PanoramaClient:
+    """
+    Wrapper for the PaloAlto REST API
+    Resources (e.g. Addresses, Tags, ..) are grouped under their resource types.
+
+    See https://docs.paloaltonetworks.com/pan-os/10-1/pan-os-panorama-api/get-started-with-the-pan-os-rest-api/access-the-rest-api#id0e536ca4-6154-4188-b70f-227c2c113ec4
+    """
+
     def __init__(
         self,
         domain,
         api_key=None,
         version="v10.1",
         verify=False,
         verbose=False,
     ):
+        domain, _, _ = clean_url_host(domain)
         client = PanoramaAPI(api_key=api_key, verbose=verbose, verify=verify)
         self.client = client
         self.objects = PanoramaObjectsResourceType(client, domain, version=version)
         self.policies = PanoramaPoliciesResourceType(client, domain, version=version)
         self.network = PanoramaNetworkResourceType(client, domain, version=version)
         self.device = PanoramaDevicesResourceType(client, domain, version=version)
         self.panorama = PanoramaPanoramaResourceType(client, domain, version=version)
```

### Comparing `nagra_panorama_api-0.1.9/nagra_panorama_api/utils.py` & `nagra_panorama_api-0.2.0/nagra_panorama_api/xmlapi/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,45 @@
 # import defusedxml.lxml
-import urllib.parse
-
-import xmltodict
-from diff_match_patch import diff_match_patch
-from lxml import etree  # nosec B410
-
 # Safe XML parsing with custom options (solution of the author)
 # https://github.com/tiran/defusedxml/issues/102
 # Nb: From issue #33, defusedxml.lxml should be depracted by the author.
 # PARSER = etree.Parser(remove_blank_text=True, resolve_entities=False)
 # LOOKUP = etree.ElementDefaultClassLookup(defusedxml.lxml.RestrictedElement)
 # PARSER.set_element_class_lookup(LOOKUP)
-
 # https://stackoverflow.com/questions/3310614/remove-whitespaces-in-xml-string
+import time
+import urllib.parse
+
+import xmltodict
+from diff_match_patch import diff_match_patch
+from lxml import etree  # nosec B410
+
+
+def pprint(n):
+    print(etree_tostring(n, True).decode())
+
+
+def wait_attempts(attempts=100, pool_delay=20, start_index=0):
+    for i in range(start_index, start_index + attempts):
+        yield i
+        time.sleep(pool_delay)
+    return
+
+
+def wait_with_duration(duration=1800, pool_delay=20):
+    start = time.perf_counter()
+    while True:
+        delta = time.perf_counter() - start
+        yield delta
+        if delta >= duration:
+            return
+        time.sleep(pool_delay)
+
+
+wait = wait_with_duration
 
 
 def etree_fromstring(string, remove_blank_text=True):
     parser = etree.XMLParser(remove_blank_text=remove_blank_text)
     return etree.XML(string, parser=parser)
 
 
@@ -84,14 +107,15 @@
         if e.tag in children:
             continue
         dest.append(e)
     return dest
 
 
 def el2dict(e):
+    e.tail = None
     return xmltodict.parse(etree_tostring(e))
 
 
 # =============================================
 # Utility function to compare the changes between configurations
 # Nb: native difflib is too slow
```

### Comparing `nagra_panorama_api-0.1.9/pyproject.toml` & `nagra_panorama_api-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [tool.poetry]
 name = "nagra-panorama-api"
-version = "0.1.9"
+version = "0.2.0"
 description = ""
 authors = ["David Gallay <david.gallay@nagra.com>"]
 readme = "README.md"
 packages = [{include = "nagra_panorama_api", from="."}]
 
 # [tool.setuptools.dynamic]
 # version = {attr = "nagra_network_misc_utils.__version__"}
 
 [tool.poetry.scripts]
 panorama_api = "nagra_panorama_api.__main__:cli"
 
 [tool.poetry.dependencies]
 # https://stackoverflow.com/questions/65945929/poetry-how-to-publish-project-packages-targeting-multiple-python-versions
-python = ">=3.9.0,<4.0.0"
+python = ">=3.7.0,<4.0.0"
 # pan-os-python = "^1.11.0"
 lxml = "^4.9.3"
 xmltodict = "^0.13.0"
 requests = "^2.31.0"
 addict = "^2.4.0"
-nagra-network-misc-utils = "0.2.2"
+nagra-network-misc-utils = "0.2.3"
 # defusedxml = "^0.7.1"
 diff-match-patch = "^20230430"
+pan-os-python = "^1.11.0"
+ping3 = "^4.0.4"
+pydantic = "^2.5.3"
+pyaml = "^23.5.8"
 
 
 [tool.poetry.group.dev.dependencies]
-python-dotenv = "^1.0.0"
+# python-dotenv = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nagra_panorama_api-0.1.9/PKG-INFO` & `nagra_panorama_api-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 Metadata-Version: 2.1
 Name: nagra-panorama-api
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: David Gallay
 Author-email: david.gallay@nagra.com
-Requires-Python: >=3.9.0,<4.0.0
+Requires-Python: >=3.7.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: diff-match-patch (>=20230430,<20230431)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
-Requires-Dist: nagra-network-misc-utils (==0.2.2)
+Requires-Dist: nagra-network-misc-utils (==0.2.3)
+Requires-Dist: pan-os-python (>=1.11.0,<2.0.0)
+Requires-Dist: ping3 (>=4.0.4,<5.0.0)
+Requires-Dist: pyaml (>=23.5.8,<24.0.0)
+Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # README
 
-## Why the need for this library ?
-
-For simple resource retrieval, the existing API is enough, but:
+This repository contains a wrapper around Panorama/PaloAlto API.
+It also provides a cli tool `panorama_api`
 
-* The libraries available are not practical for it, the manual management of urls is easier
-
-* For more complex operation, this does not suits well
 
-The python SDK of PaloAltoNetworks itself relies on a third party wrapper for their API.
+## CLI
+This package also provide a CLI tool for some operations:
+* Generating an API Key
+* Upgrading a group of devices
+* Generating a boilerplate configuration file for the upgrades
 
 
+```bash
+pip install nagra_panorama_api
+panorama_api --help
+```
 
-## Design
-
-The library provides 2 things:
 
-* A simple client for the API
+## Why the need for this library ?
 
-* Tool to manage the xml configuration
+For simple resource retrieval, the existing API is enough, but:
 
-We will pull the whole configuration and search on it locally. We can then use the client to do some operations
+* The libraries available are not practical for it, the manual management of urls is easier
+* For more complex operation, this does not suits well
 
+The [official python SDK of PaloAltoNetworks](https://github.com/PaloAltoNetworks/pan-os-python) itself relies on a [third party wrapper](https://github.com/kevinsteves/pan-python) for their API.
 
 
-We don't want to combine both the client and the management tool. This would requires a lot of boilerplate code that would be difficult to maintain.
+This library takes a more popular approach when wrapping the API, making it easier to use. It also provides types' wrappers to simplify their usage or utility functions to re-structure the data we receive.
+It provides a client for the REST API and for the XML API
 
+* A simple client for the API
+* Tool to manage the xml configuration
 
 
-## Usage
+## Library Usage Example
 
 ```python
 client = XMLApi(HOST, API_KEY)
 tree = client.get_tree()
 
 # Find your object using its name (may not be unique)
 my_object = config.find_by_name("my_object_name")[0]
@@ -71,22 +83,23 @@
 # We can also revert it
 # client.revert_changes()
 ```
 
 The library currently doesn't provide helper tools to know how to edit the configuration. Theses changes must be done manually
 
 
-
-
-
 ## TODO
 
 * Provide wrapper classes for the resources.
 
   ```python
   nat = NatPolicy(...)
   tree.insert(nat)  # or nat.insertInto(tree)
   client.create(nat.insert_xpath, nat.xml)
   ```
 * # Mix Rest API and XML API ?
   https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/get-started-with-the-pan-os-rest-api/create-security-policy-rule-rest-api
 
+
+## Links
+* [Official upgrade procedure on HA with API](https://docs.paloaltonetworks.com/pan-os/9-1/pan-os-panorama-api/pan-os-xml-api-use-cases/upgrade-pan-os-on-multiple-ha-firewalls-through-panorama-api)
+
```

