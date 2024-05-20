# Comparing `tmp/cdk_gw_tools-0.4.4.tar.gz` & `tmp/cdk_gw_tools-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_gw_tools-0.4.4.tar", max compression
+gzip compressed data, was "cdk_gw_tools-3.0.0.tar", max compression
```

## Comparing `cdk_gw_tools-0.4.4.tar` & `cdk_gw_tools-3.0.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0    10280 2023-10-03 07:26:27.903958 cdk_gw_tools-0.4.4/LICENSE
--rw-r--r--   0        0        0     1478 2023-10-03 07:18:39.205038 cdk_gw_tools-0.4.4/README.md
--rw-r--r--   0        0        0      181 2023-12-07 17:50:55.519482 cdk_gw_tools-0.4.4/cdk_gw_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-10-03 07:35:36.973679 cdk_gw_tools-0.4.4/cdk_gw_tools/aws/__init__.py
--rw-r--r--   0        0        0     8606 2023-10-05 06:41:58.038581 cdk_gw_tools-0.4.4/cdk_gw_tools/aws/gw_handling.py
--rw-r--r--   0        0        0     5431 2023-12-04 16:40:19.917989 cdk_gw_tools-0.4.4/cdk_gw_tools/aws/secrets_rotation.py
--rw-r--r--   0        0        0     2936 2023-12-07 17:50:29.921031 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/__init__.py
--rw-r--r--   0        0        0      680 2023-12-04 14:47:11.881778 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/__init__.py
--rw-r--r--   0        0        0      706 2023-12-04 16:39:25.552081 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/plugins.py
--rw-r--r--   0        0        0     1363 2023-12-06 10:45:05.533903 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/user_mappings.py
--rw-r--r--   0        0        0     1465 2023-12-04 16:40:19.879990 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/__init__.py
--rw-r--r--   0        0        0     1163 2023-12-04 16:39:25.555081 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/auth.py
--rw-r--r--   0        0        0     2342 2023-12-04 16:40:19.888990 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/interceptors.py
--rw-r--r--   0        0        0     3094 2023-12-04 16:40:19.915989 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/topic_mappings.py
--rw-r--r--   0        0        0      776 2023-12-04 15:05:55.458949 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/user_mappings.py
--rw-r--r--   0        0        0        0 2023-12-04 15:01:37.549027 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/gw_parsers/__init__.py
--rw-r--r--   0        0        0      468 2023-10-03 08:14:54.251455 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/gw_parsers/plugins.py
--rw-r--r--   0        0        0     1245 2023-12-04 16:20:02.672369 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/gw_parsers/user_mappings.py
--rw-r--r--   0        0        0     2339 2023-12-04 16:40:19.893990 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/main_parser.py
--rw-r--r--   0        0        0     5251 2023-12-04 15:03:04.318311 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/vclusters_parser/__init__.py
--rw-r--r--   0        0        0     2565 2023-11-29 13:24:10.814182 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/vclusters_parser/interceptors.py
--rw-r--r--   0        0        0     1391 2023-12-04 14:59:01.487087 cdk_gw_tools-0.4.4/cdk_gw_tools/cli/vclusters_parser/user_mappings.py
--rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0     3892 2023-12-07 17:50:29.929031 cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/import_from_config.py
--rw-r--r--   0        0        0    11346 2023-12-06 15:49:53.566330 cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/import_tenants_mappings.py
--rw-r--r--   0        0        0     2539 2023-12-04 16:39:25.577081 cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/set_update_interceptors.py
--rw-r--r--   0        0        0     2587 2023-12-06 10:05:16.750631 cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/user_mappings_tools.py
--rw-r--r--   0        0        0       93 2023-10-03 07:19:14.926413 cdk_gw_tools-0.4.4/cdk_gw_tools/common/__init__.py
--rw-r--r--   0        0        0     1937 2023-10-03 08:06:39.037234 cdk_gw_tools-0.4.4/cdk_gw_tools/common/logging.py
--rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_gw_tools-0.4.4/cdk_gw_tools/specs/__init__.py
--rw-r--r--   0        0        0     2268 2023-09-12 20:28:26.429973 cdk_gw_tools-0.4.4/cdk_gw_tools/specs/profiles_config.spec.json
--rw-r--r--   0        0        0     5049 2023-10-18 20:38:14.461426 cdk_gw_tools-0.4.4/cdk_gw_tools/specs/tenant_mappings-input.json
--rw-r--r--   0        0        0     1015 2023-12-04 17:06:04.663044 cdk_gw_tools-0.4.4/cdk_gw_tools/specs/user-mappings.spec.json
--rw-r--r--   0        0        0      407 2023-12-04 17:06:08.515967 cdk_gw_tools-0.4.4/cdk_gw_tools/specs/user_mappings.py
--rw-r--r--   0        0        0     2170 2023-12-07 17:50:55.519482 cdk_gw_tools-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 cdk_gw_tools-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-10-03 07:26:27.903958 cdk_gw_tools-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1478 2023-10-03 07:18:39.205038 cdk_gw_tools-3.0.0/README.md
+-rw-r--r--   0        0        0      181 2024-05-20 06:46:56.129863 cdk_gw_tools-3.0.0/cdk_gw_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-03 07:35:36.973679 cdk_gw_tools-3.0.0/cdk_gw_tools/aws/__init__.py
+-rw-r--r--   0        0        0     8604 2024-05-20 06:46:56.129863 cdk_gw_tools-3.0.0/cdk_gw_tools/aws/gw_handling.py
+-rw-r--r--   0        0        0     5431 2023-12-04 16:40:19.917989 cdk_gw_tools-3.0.0/cdk_gw_tools/aws/secrets_rotation.py
+-rw-r--r--   0        0        0      326 2024-05-20 06:46:56.130863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/__init__.py
+-rw-r--r--   0        0        0     1083 2024-05-20 06:46:56.130863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/auth.py
+-rw-r--r--   0        0        0     3125 2024-05-20 06:46:56.130863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/interceptors.py
+-rw-r--r--   0        0        0     3064 2024-05-20 06:46:56.130863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/main_parser.py
+-rw-r--r--   0        0        0      468 2024-05-20 06:46:56.130863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/plugins.py
+-rw-r--r--   0        0        0     2971 2024-05-20 06:46:56.130863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/user_mappings.py
+-rw-r--r--   0        0        0     4989 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/vclusters_parser/__init__.py
+-rw-r--r--   0        0        0     2007 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli/vclusters_parser/concentration_rules.py
+-rw-r--r--   0        0        0     2912 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/__init__.py
+-rw-r--r--   0        0        0     1340 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/auth.py
+-rw-r--r--   0        0        0      590 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/common.py
+-rw-r--r--   0        0        0     2808 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/interceptors.py
+-rw-r--r--   0        0        0      721 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/plugins.py
+-rw-r--r--   0        0        0     2419 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/user_mappings.py
+-rw-r--r--   0        0        0     2581 2024-05-20 06:46:56.131863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/vclusters/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-20 06:46:56.132863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/vclusters/topic_mappings.py
+-rw-r--r--   0        0        0      800 2023-03-26 16:00:22.879474 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0     3892 2024-04-09 06:29:37.878031 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/import_from_config.py
+-rw-r--r--   0        0        0    11513 2024-05-20 06:46:56.132863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/import_tenants_mappings.py
+-rw-r--r--   0        0        0     3783 2024-05-20 06:46:56.132863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/set_update_interceptors.py
+-rw-r--r--   0        0        0     8076 2024-05-20 06:46:56.132863 cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/user_mappings_tools.py
+-rw-r--r--   0        0        0       93 2023-10-03 07:19:14.926413 cdk_gw_tools-3.0.0/cdk_gw_tools/common/__init__.py
+-rw-r--r--   0        0        0     1937 2023-10-03 08:06:39.037234 cdk_gw_tools-3.0.0/cdk_gw_tools/common/logging.py
+-rw-r--r--   0        0        0        0 2023-03-14 12:46:32.223933 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/__init__.py
+-rw-r--r--   0        0        0     2960 2024-05-20 06:46:56.132863 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/interceptors-config.spec.json
+-rw-r--r--   0        0        0     1532 2024-05-20 06:46:56.132863 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/interceptors_config.py
+-rw-r--r--   0        0        0     2268 2023-09-12 20:28:26.429973 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/profiles_config.spec.json
+-rw-r--r--   0        0        0     4920 2024-05-20 06:46:56.133863 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/tenant_mappings-input.json
+-rw-r--r--   0        0        0     2049 2024-05-20 06:46:56.133863 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/user-mappings.spec.json
+-rw-r--r--   0        0        0      912 2024-05-20 06:46:56.133863 cdk_gw_tools-3.0.0/cdk_gw_tools/specs/user_mappings.py
+-rw-r--r--   0        0        0     2118 2024-05-20 06:46:56.134863 cdk_gw_tools-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 cdk_gw_tools-3.0.0/PKG-INFO
```

### Comparing `cdk_gw_tools-0.4.4/LICENSE` & `cdk_gw_tools-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/README.md` & `cdk_gw_tools-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/aws/gw_handling.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/aws/gw_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from datetime import datetime
 
 import jwt
 import yaml
 from boto3 import Session
 from cdk_proxy_api_client.client_wrapper import ApiClient
 from cdk_proxy_api_client.proxy_api import ProxyClient
-from cdk_proxy_api_client.vclusters import VirturalClusters
+from cdk_proxy_api_client.vclusters import VirtualClusters
 from compose_x_common.aws import get_assume_role_session
 from compose_x_common.compose_x_common import keyisset
 
 if logging.getLogger().hasHandlers():
     logging.getLogger().setLevel(logging.INFO)
 else:
     logging.basicConfig(level=logging.INFO)
@@ -193,15 +193,15 @@
         )
         api_client = ApiClient(
             username=gw_admin_secret["username"],
             password=gw_admin_secret["password"],
             url=CDK_API_ENDPOINT,
         )
         proxy_client = ProxyClient(api_client)
-        admin_client = VirturalClusters(proxy_client)
+        admin_client = VirtualClusters(proxy_client)
         logger.debug(admin_client.list_vclusters(as_list=True))
         token = admin_client.create_vcluster_user_token(
             vcluster=vcluster["vcluster"],
             username=vcluster["username"],
             lifetime_in_seconds=life,
             token_only=token_only,
         )
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/aws/secrets_rotation.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/aws/secrets_rotation.py`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/__init__.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-#   SPDX-License-Identifier: Apache-2.0
-#   Copyright 2023 John Mille <john@ews-network.net>
+# SPDX-License-Identifier: Apache-2.0
+# Copyright 2023 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 import json
 import logging
-import sys
 
 import yaml
+from cdk_proxy_api_client.client_wrapper import ApiClient
+from cdk_proxy_api_client.proxy_api import ProxyClient
+from yaml import Dumper
 
-try:
-    from yaml import Dumper
-except ImportError:
-    from yaml import CDumper as Dumper
-
-from cdk_proxy_api_client.proxy_api import ApiClient, ProxyClient
-
-from cdk_gw_tools.cli.actions import format_return
-from cdk_gw_tools.cli.actions.plugins import plugins_actions
-from cdk_gw_tools.cli.actions.user_mappings import gw_user_mappings_actions
-from cdk_gw_tools.cli.actions.vclusters import vclusters_actions
-from cdk_gw_tools.cli.actions.vclusters.interceptors import interceptors_actions
 from cdk_gw_tools.cli.main_parser import set_parser
+from cdk_gw_tools.cli_actions.auth import auth_actions
+from cdk_gw_tools.cli_actions.interceptors import interceptors_actions
+from cdk_gw_tools.cli_actions.plugins import plugins_actions
+from cdk_gw_tools.cli_actions.user_mappings import user_mappings_actions
+from cdk_gw_tools.cli_actions.vclusters import vclusters_actions
 from cdk_gw_tools.cli_tools.import_from_config import import_client
 from cdk_gw_tools.common.logging import LOG
 
 
 def main():
     _PARSER = set_parser()
     _args = _PARSER.parse_args()
@@ -67,15 +62,17 @@
     _category = _vars.pop("category")
     _action = _vars.pop("action")
     _proxy = ProxyClient(_client)
 
     _categories_mappings: dict = {
         "vclusters": vclusters_actions,
         "plugins": plugins_actions,
-        "user-mappings": gw_user_mappings_actions,
+        "user-mappings": user_mappings_actions,
+        "interceptors": interceptors_actions,
+        "auth": auth_actions,
     }
     dest_function = _categories_mappings[_category]
     response = dest_function(_proxy, _action, **_vars)
     if not response:
         return
     if isinstance(response, str):
         print(response)
@@ -84,11 +81,7 @@
         if _args.output_format == "json":
             print(json.dumps(response, indent=2))
         else:
             print(yaml.dump(response, Dumper=Dumper))
     except Exception as error:
         print(error)
         print(response)
-
-
-if __name__ == "__main__":
-    sys.exit(main())
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/plugins.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 from cdk_proxy_api_client.plugins import Plugins
 from cdk_proxy_api_client.proxy_api import ProxyClient
 from compose_x_common.compose_x_common import keyisset
 
-from cdk_gw_tools.cli import format_return
+from cdk_gw_tools.cli_actions.common import format_return
 
 
 @format_return
 def plugins_actions(proxy: ProxyClient, action: str, **kwargs):
     _plugins = Plugins(proxy)
     if action == "list":
         req = _plugins.list_all_plugins(
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/user_mappings.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2023 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
-from dataclasses import asdict
+from typing import TYPE_CHECKING
 
-from cdk_proxy_api_client.proxy_api import ProxyClient
-from cdk_proxy_api_client.usermappings import UserMappings
-from cdk_proxy_api_client.vclusters import VirturalClusters
+if TYPE_CHECKING:
+    from cdk_proxy_api_client.proxy_api import ProxyClient
+
+from cdk_proxy_api_client.vclusters import VirtualClusters
 from compose_x_common.compose_x_common import keyisset
 
-from cdk_gw_tools.cli import format_return
-from cdk_gw_tools.cli_tools import load_config_file
-from cdk_gw_tools.cli_tools.user_mappings_tools import (
-    create_export_config,
-    import_mappings_from_file,
-    validate_identities_are_unique,
-)
-
-
-@format_return
-def gw_user_mappings_actions(proxy: ProxyClient, action: str, **kwargs) -> dict:
-    vclusters = VirturalClusters(proxy)
-    user_mappings = UserMappings(proxy)
-    if action == "export":
-        req = create_export_config(vclusters, user_mappings)
-    elif action == "import":
-        config = load_config_file(kwargs["import_file"])
-        req = import_mappings_from_file(
-            vclusters, user_mappings, config, keyisset("remove_unset", kwargs)
+
+def auth_actions(proxy_client: ProxyClient, action: str, **kwargs):
+    """Manages cli_actions for auth vClusters subparser"""
+    username = kwargs.get("username") or kwargs["vcluster_name"]
+    if action == "create":
+        vcluster_client = VirtualClusters(proxy_client)
+        req = vcluster_client.create_vcluster_user_token(
+            vcluster=kwargs.get("vcluster_name"),
+            username=username,
+            lifetime_in_seconds=int(kwargs.get("token_lifetime_in_seconds")),
+            token_only=keyisset("token_only", kwargs),
         )
-    elif action == "validate":
-        config = load_config_file(kwargs["import_file"])
-        validate_identities_are_unique(config)
     else:
-        raise NotImplementedError(f"Action {action} is not implemented yet.")
-    return asdict(req)
+        raise NotImplementedError(f"Action {action} not yet implemented.")
+    if keyisset("as_kafka_config", kwargs):
+        req = req.json()
+        return """security.protocol=SASL_SSL
+sasl.mechanism=PLAIN
+sasl.jaas.config=org.apache.kafka.common.security.plain.PlainLoginModule required username="{}" password="{}";
+client.id=CLI_{}""".format(
+            username, req["token"], username
+        )
+    return req
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/interceptors.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/interceptors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,78 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2023 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 import json
+import warnings
+
+import yaml
+
+try:
+    from yaml import CLoader as Loader
+except ImportError:
+    from yaml import Loader
 
 from cdk_proxy_api_client.interceptors import Interceptors
 from cdk_proxy_api_client.proxy_api import ProxyClient
 from compose_x_common.compose_x_common import keyisset, set_else_none
 
 from cdk_gw_tools.cli_tools import load_config_file
 
 
 def interceptors_actions(proxy: ProxyClient, action: str, **kwargs):
     """Triggers function according to CLI Input"""
 
     _interceptor_client = Interceptors(proxy)
+    if action == "list-all":
+        return _interceptor_client.get_all_gw_interceptors().json()
     if action == "list":
-        _interceptors = _interceptor_client.list_vcluster_interceptors(
-            vcluster_name=kwargs["vcluster_name"], as_list=True
-        )
+        _interceptors = _interceptor_client.get_all_interceptor(
+            is_global=kwargs.get("is_global"),
+            username=kwargs.get("username"),
+            group_name=kwargs.get("group_name"),
+            vcluster_name=kwargs.get("vcluster_name"),
+        ).json()
         if keyisset("IgnoreReadOnly", kwargs):
             return [
                 _interceptor
                 for _interceptor in _interceptors.values()
                 if _interceptor["pluginClass"]
                 != "io.conduktor.gateway.interceptor.safeguard.ReadOnlyTopicPolicyPlugin"
             ]
         return _interceptors
     elif action == "create-update":
-        with open(kwargs["config"]) as config_fd:
-            config_raw = config_fd.read()
-            config_json = json.loads(config_raw)
-        _req = _interceptor_client.create_vcluster_interceptor(
-            vcluster_name=kwargs["vcluster_name"],
-            interceptor_name=config_json["name"],
-            plugin_class=config_json["pluginClass"],
-            priority=config_json["priority"],
-            config=config_json["config"],
-            username=set_else_none("vcluster_username", kwargs, None),
+        warnings.warn(
+            "We highly recommend to use this command for testing only."
+            "Use the import command to declare the interceptors you want to define as-code"
         )
+        config = load_config_file(kwargs["config_file_path"])
+
+        _req = _interceptor_client.update_interceptor(
+            kwargs.get("interceptor_name"),
+            config,
+            is_global=kwargs.get("is_global"),
+            vcluster_name=kwargs["vcluster_name"],
+            username=kwargs.get("username"),
+            group_name=kwargs.get("group_name"),
+        ).json()
         return _req
     elif action == "delete":
-        _req = _interceptor_client.delete_vcluster_interceptor(
-            kwargs["vcluster_name"],
-            kwargs["interceptor_name"],
-            set_else_none("vcluster_username", kwargs, None),
-        )
+        _req = _interceptor_client.delete_interceptor(
+            interceptor_name=kwargs.get("interceptor_name"),
+            is_global=kwargs.get("is_global"),
+            vcluster_name=kwargs["vcluster_name"],
+            username=kwargs.get("username"),
+            group_name=kwargs.get("group_name"),
+        ).status_code
         return _req
     elif action == "import-from-config":
-        _loaded_config = load_config_file(kwargs["InputConfigFile"])
+        _loaded_config = load_config_file(kwargs["config_file_path"])
         if not keyisset("interceptors", _loaded_config):
             return
         from cdk_gw_tools.cli_tools.set_update_interceptors import (
             set_update_interceptors,
         )
 
-        _req = set_update_interceptors(
-            proxy, kwargs["vcluster_name"], _loaded_config["interceptors"]
-        )
+        _req = set_update_interceptors(proxy, _loaded_config)
     return None
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/actions/vclusters/topic_mappings.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_actions/vclusters/topic_mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from os import path
 from typing import Union
 
 from cdk_proxy_api_client.proxy_api import ProxyClient
-from cdk_proxy_api_client.vclusters import VirturalClusters
+from cdk_proxy_api_client.vclusters import VirtualClusters
 from compose_x_common.compose_x_common import keyisset, set_else_none
 
 from cdk_gw_tools.cli_tools import load_config_file
 from cdk_gw_tools.cli_tools.import_tenants_mappings import import_tenants_mappings
 
 
 def format_vcluster_mappings_list(
@@ -29,18 +29,18 @@
         else:
             mappings_list.append(_mapping)
     if keyisset("as_import_config", options):
         return {"tenant": vcluster_name, "mappings": mappings_list}
     return mappings_list
 
 
-def tenant_mappings_actions(
-    proxy: ProxyClient, vcluster: VirturalClusters, action: str, **kwargs
+def vcluster_mappings_actions(
+    proxy: ProxyClient, vcluster: VirtualClusters, action: str, **kwargs
 ):
-    """Manages actions for mappings vClusters actions"""
+    """Manages cli_actions for mappings vClusters cli_actions"""
 
     vcluster_name = set_else_none("vcluster_name", kwargs)
     if action == "list":
         req = format_vcluster_mappings_list(
             vcluster_name,
             vcluster.list_vcluster_topic_mappings(vcluster_name).json(),
             kwargs,
@@ -50,27 +50,26 @@
         req = import_tenants_mappings(proxy, content, vcluster_name)
     elif action == "create":
         req = vcluster.create_vcluster_topic_mapping(
             vcluster=vcluster_name,
             logical_topic_name=kwargs["logical_topic_name"],
             physical_topic_name=kwargs["physical_topic_name"],
             read_only=keyisset("ReadOnly", kwargs),
-            concentrated=keyisset("concentrated", kwargs),
             cluster_id=kwargs.get("cluster_id"),
         )
     elif action == "import-from-tenant":
         source_tenant = kwargs.pop("source_tenant")
         content = {
             "vcluster_name": vcluster_name,
             "mappings": [],
             "ignore_duplicates_conflict": True,
             "import_from_tenant": {"include_regex": [rf"^{source_tenant}$"]},
         }
         req = import_tenants_mappings(proxy, content, vcluster_name)
-    elif action == "delete-topic-mapping":
+    elif action == "delete":
         to_delete = kwargs.pop("logicalTopicName")
         req = vcluster.delete_vcluster_topic_mapping(
             vcluster=vcluster_name, logical_topic_name=to_delete
         )
     elif action == "delete-all-mappings":
         req = vcluster.delete_vcluster_topics_mappings(vcluster_name)
     else:
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/main_parser.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli/main_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 # Copyright 2023 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from argparse import ArgumentParser
 from os import environ
 
-from cdk_gw_tools.cli.gw_parsers.plugins import set_plugings_actions_parsers
-from cdk_gw_tools.cli.gw_parsers.user_mappings import (
+from cdk_gw_tools.cli.auth import set_auth_actions
+from cdk_gw_tools.cli.interceptors import set_interceptors_actions_parsers
+from cdk_gw_tools.cli.plugins import set_plugings_actions_parsers
+from cdk_gw_tools.cli.user_mappings import (
     set_gw_user_mappings_actions_parsers,
+    set_user_mappings_actions_parsers,
 )
 from cdk_gw_tools.cli.vclusters_parser import set_vclusters_actions_parsers
 
 
 def set_parser():
     main_parser = ArgumentParser("CDK Proxy CLI", add_help=True)
     main_parser.add_argument(
@@ -50,20 +53,34 @@
     vclusters_subparsers = vclusters_parser.add_subparsers(
         dest="action", help="vCluster management"
     )
     set_vclusters_actions_parsers(vclusters_subparsers)
 
     plugins_parser = cmd_parser.add_parser(name="plugins", help="Manage plugins")
     plugins_subparsers = plugins_parser.add_subparsers(
-        dest="action", help="Manage plugins actions"
+        dest="action", help="Manage plugins cli_actions"
     )
     set_plugings_actions_parsers(plugins_subparsers)
 
-    gw_user_mappings_parser = cmd_parser.add_parser(
-        name="user-mappings", help="Manage user mappings at the GW level"
+    interceptors_parser = cmd_parser.add_parser(
+        name="interceptors", help="Manage interceptors"
     )
-    gw_user_mappings_subparsers = gw_user_mappings_parser.add_subparsers(
-        dest="action", help="Manage GW user mappings actions"
+    interceptors_subparsers = interceptors_parser.add_subparsers(
+        dest="action", help="Manage plugins cli_actions"
     )
-    set_gw_user_mappings_actions_parsers(gw_user_mappings_subparsers)
+    set_interceptors_actions_parsers(interceptors_subparsers)
+    user_mappings_parser = cmd_parser.add_parser(
+        name="user-mappings", help="Manage user-mappings"
+    )
+    user_mappings_subparsers = user_mappings_parser.add_subparsers(
+        dest="action", help="Manage user-mappings cli_actions"
+    )
+    set_user_mappings_actions_parsers(user_mappings_subparsers)
+    set_gw_user_mappings_actions_parsers(user_mappings_subparsers)
+
+    auth_parser = cmd_parser.add_parser(name="auth", help="Manage user-mappings")
+    auth_subparsers = auth_parser.add_subparsers(
+        dest="action", help="Manage auth/credentials actions"
+    )
+    set_auth_actions(auth_subparsers)
 
     return main_parser
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/vclusters_parser/__init__.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli/vclusters_parser/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2023 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from argparse import ArgumentParser
 
-from .interceptors import set_interceptors_actions_parsers
-from .user_mappings import set_user_mappings_actions_parsers
+from cdk_gw_tools.cli.vclusters_parser.concentration_rules import (
+    set_vcluster_concentration_actions,
+)
 
 VCLUSTER_PARSER = ArgumentParser(add_help=False)
 VCLUSTER_PARSER.add_argument(
     "--vcluster-name",
     dest="vcluster_name",
     required=True,
     help="Name of the vcluster to make operations for",
@@ -49,16 +50,15 @@
     tenant_token_create_parser.add_argument(
         "--as-kafka-config",
         action="store_true",
         help="Returns the kafka config file",
         default=False,
     )
     set_vcluster_mappings_actions(vclusters_subparsers)
-    set_interceptors_actions_parsers(vclusters_subparsers)
-    set_user_mappings_actions_parsers(vclusters_subparsers)
+    set_vcluster_concentration_actions(vclusters_subparsers)
 
 
 def set_vcluster_mappings_actions(vclusters_subparsers):
     # Mappings
     mappings_parser = vclusters_subparsers.add_parser(
         name="mappings",
         help="Manages vCluster mappings",
@@ -99,45 +99,38 @@
         required=False,
         default=False,
         dest="ReadOnly",
         action="store_true",
         help="Creates mapping in ReadOnly (defaults to Read-Write)",
     )
     create_parser.add_argument(
-        "--concentrated",
-        required=False,
-        default=False,
-        action="store_true",
-        help="Create concentrated mapping",
-    )
-    create_parser.add_argument(
         "--cluster-id",
         type=str,
         required=False,
         help="Creates a mapping for merged cluster",
     )
     # Delete action parsers
     delete_all_mappings_parser = mappings_subparsers.add_parser(
         name="delete-all-mappings",
         help="Delete all topics mappings for a given vCluster",
         parents=[],
     )
     delete_topic_mapping_parser = mappings_subparsers.add_parser(
-        name="delete-topic-mapping",
+        name="delete",
         help="Delete a topic mapping for a given vCluster",
         parents=[],
     )
     delete_topic_mapping_parser.add_argument(
         "--logical-topic-name",
         dest="logicalTopicName",
         required=True,
         help="Topic name as seen in the vCluster.",
     )
 
-    # Custom actions
+    # Custom cli_actions
     import_from_vclusters_parser = mappings_subparsers.add_parser(
         name="import-from-vclusters-config",
         help="Create topic mappings from existing vclusters",
     )
     import_from_vclusters_parser.add_argument(
         "-f",
         "--import-config-file",
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli/vclusters_parser/interceptors.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli/interceptors.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,78 +5,101 @@
 
 from argparse import ArgumentParser
 
 VCLUSTER_PARSER = ArgumentParser(add_help=False)
 VCLUSTER_PARSER.add_argument(
     "--vcluster-name",
     dest="vcluster_name",
-    required=True,
-    help="Name of the vcluster to make operations for",
+    required=False,
+    help="Name of the vCluster to make operations for",
 )
 
 USERNAME_PARSER = ArgumentParser(add_help=False)
 USERNAME_PARSER.add_argument(
     "--username",
-    dest="vcluster_username",
+    dest="username",
+    required=False,
+    help="Specify username to get interceptors for",
+)
+GROUP_PARSER = ArgumentParser(add_help=False)
+GROUP_PARSER.add_argument(
+    "--group",
+    dest="group",
     required=False,
     help="Specify username to get interceptors for",
 )
 
 
-def set_interceptors_actions_parsers(vclusters_subparsers):
-    """Creates all the parser and subparsers for vClusters API endpoints"""
-
-    interceptors_parser = vclusters_subparsers.add_parser(
-        name="interceptors",
-        help="Manage vCluster interceptors",
-        parents=[VCLUSTER_PARSER],
+def set_interceptors_actions_parsers(interceptors_subparsers):
+    """Creates all the parser and subparsers for GW API endpoints"""
+    list_all_parser = interceptors_subparsers.add_parser(
+        name="list-all",
+        help="List all the interceptors on GW for all contexts",
     )
-    interceptors_subparsers = interceptors_parser.add_subparsers(dest="sub_action")
+
     list_parser = interceptors_subparsers.add_parser(
         name="list",
-        help="List interceptors for vcluster/username",
-        parents=[USERNAME_PARSER],
+        help="List interceptors",
+        parents=[USERNAME_PARSER, VCLUSTER_PARSER, GROUP_PARSER],
     )
     list_parser.add_argument(
-        "--ignore-readonly",
+        "--global",
         action="store_true",
-        help="Ignore the read only interceptors",
-        dest="IgnoreReadOnly",
+        help="List global interceptors.",
+        dest="is_global",
     )
+
     create_parser = interceptors_subparsers.add_parser(
         name="create-update",
         help="Create or update a new vCluster mapping",
-        parents=[USERNAME_PARSER],
+        parents=[USERNAME_PARSER, VCLUSTER_PARSER, GROUP_PARSER],
+    )
+    create_parser.add_argument(
+        "--interceptor-name",
+        dest="interceptor_name",
+        required=True,
+        help="Name of the interceptor to create or update",
+    )
+    create_parser.add_argument(
+        "--global",
+        action="store_true",
+        help="Create or update a global interceptor",
+        dest="is_global",
     )
-    # create_parser.add_argument("--interceptor-name", type=str, required=True)
     create_parser.add_argument(
         "--config",
         type=str,
         required=True,
         help="Path to config (YAML/JSON) to use for interceptor",
+        dest="config_file_path",
     )
 
     # Delete action parsers
     delete_interceptor_mapping_parser = interceptors_subparsers.add_parser(
         name="delete",
         help="Delete interceptor",
-        parents=[USERNAME_PARSER],
+        parents=[USERNAME_PARSER, VCLUSTER_PARSER, GROUP_PARSER],
     )
     delete_interceptor_mapping_parser.add_argument(
         "--interceptor-name",
         dest="interceptor_name",
         required=True,
         help="Interceptor name to delete as seen in the vCluster.",
     )
+    delete_interceptor_mapping_parser.add_argument(
+        "--global",
+        action="store_true",
+        help="Delete global interceptor",
+        dest="is_global",
+    )
     import_from_config_parser = interceptors_subparsers.add_parser(
         name="import-from-config",
         help="Import interceptors from config file",
-        parents=[USERNAME_PARSER],
     )
     import_from_config_parser.add_argument(
         "-f",
         "--config-file",
-        dest="InputConfigFile",
+        dest="config_file_path",
         type=str,
         help="Path to the config file (YAML)",
         required=True,
     )
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/__init__.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/import_from_config.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/import_from_config.py`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/cli_tools/import_tenants_mappings.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/cli_tools/import_tenants_mappings.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re
 from copy import deepcopy
 from json import loads
 
 from cdk_proxy_api_client.common.logging import LOG
 from cdk_proxy_api_client.errors import ProxyApiException, ProxyGenericException
 from cdk_proxy_api_client.proxy_api import ProxyClient
-from cdk_proxy_api_client.vclusters import VirturalClusters
+from cdk_proxy_api_client.vclusters import VirtualClusters
 from compose_x_common.compose_x_common import keyisset, set_else_none
 from importlib_resources import files as pkg_files
 from jsonschema import validate
 
 DEFAULT_SCHEMA_PATH = pkg_files("cdk_gw_tools").joinpath(
     "specs/tenant_mappings-input.json"
 )
@@ -28,15 +28,15 @@
     """
     Returns the list of topics (logical name) from a given tenant topics mappings. Ignores
     :param ProxyClient proxy:
     :param str tenant_name:
     :param bool include_read_only:
     :return: List of topics logical available in the tenant.
     """
-    tenant_mappings = VirturalClusters(proxy)
+    tenant_mappings = VirtualClusters(proxy)
 
     topics_list: list[dict] = []
     for _topic in tenant_mappings.list_vcluster_topic_mappings(
         tenant_name, as_list=True
     ):
         if _topic["readOnly"] is True and not include_read_only:
             continue
@@ -55,15 +55,15 @@
     """Matches tenant based on simple string regex"""
     try:
         _pattern = re.compile(include_regex)
     except Exception as error:
         print(error)
         print(include_regex, "Not a valid regex")
         return
-    tenant_mappings = VirturalClusters(proxy)
+    tenant_mappings = VirtualClusters(proxy)
     for _tenant in tenants:
         if _pattern.match(_tenant):
             if process_once and _tenant in processed_tenants:
                 print(
                     f"Tenant {_tenant} was already processed. Skipping",
                     processed_tenants,
                 )
@@ -125,15 +125,15 @@
                 LOG.error(
                     "logical_topics_include_regexes",
                     _include_pattern,
                     "Not a valid regex. Skipping",
                 )
                 return
 
-    tenant_mappings = VirturalClusters(proxy)
+    tenant_mappings = VirtualClusters(proxy)
     for _tenant in tenants:
         if _pattern.match(_tenant):
             if process_once and _tenant in processed_tenants:
                 LOG.debug(
                     "Tenant {} was already processed. Skipping {}".format(
                         _tenant, processed_tenants
                     ),
@@ -195,15 +195,15 @@
                 )
 
 
 def import_from_other_tenants(
     proxy: ProxyClient, import_config: dict, tenant_name: str
 ) -> None:
     """Allows to import existing topics from other tenants in read-only"""
-    tenants: list[str] = VirturalClusters(proxy).list_vclusters(as_list=True)[
+    tenants: list[str] = VirtualClusters(proxy).list_vclusters(as_list=True)[
         "vclusters"
     ]
     exclude_list = set_else_none("exclude_regex", import_config, [])
     include_list = set_else_none("include_regex", import_config, [])
     processed_tenants: list[str] = []
     process_once: bool = keyisset("process_tenant_only_once", import_config)
     if not include_list:
@@ -243,53 +243,58 @@
                 type(_include_item),
                 "expected one of",
                 (str, dict),
             )
 
 
 def propagate_tenant_mappings(
-    tenant_mappings: VirturalClusters,
+    tenant_mappings: VirtualClusters,
     mappings: list[dict],
     vcluster_name: str,
     ignore_conflicts: bool = False,
 ) -> None:
     for mapping in mappings:
         try:
             tenant_mappings.create_vcluster_topic_mapping(
                 vcluster=vcluster_name,
                 logical_topic_name=mapping["logicalTopicName"],
                 physical_topic_name=mapping["physicalTopicName"],
                 read_only=keyisset("readOnly", mapping),
-                concentrated=keyisset("concentrated", mapping),
             )
             LOG.debug(
                 "Successfully created mapping {} -> {}".format(
                     mapping["logicalTopicName"], mapping["physicalTopicName"]
                 )
             )
         except ProxyGenericException as error:
             if error.code == 409 and ignore_conflicts:
                 print(error)
                 pass
+            elif error.code == 400:
+                LOG.error(error.details["message"])
+                pass
+            else:
+                print("Unexpected 4xx error", error.details["message"])
+                raise error
         except Exception as error:
-            print("ERROR", error)
+            print("Unexpected error", error)
             raise error
 
 
 def import_tenants_mappings(
     client: ProxyClient, config_content: dict, tenant_name: str, schema: dict = None
 ) -> list[dict]:
     """Will create mappings from the config content, and return the final mappings for the tenant"""
     if not schema:
         schema = loads(DEFAULT_SCHEMA_PATH.read_text())
     validate(config_content, schema)
     tenant_name = set_else_none("tenant_name", config_content, tenant_name)
     ignore_conflicts = keyisset("ignore_duplicates_conflict", config_content)
     mappings = config_content["mappings"]
-    tenant_mappings = VirturalClusters(client)
+    tenant_mappings = VirtualClusters(client)
     propagate_tenant_mappings(tenant_mappings, mappings, tenant_name, ignore_conflicts)
     import_from_other_tenants_config = set_else_none(
         "import_from_tenant", config_content
     )
     if import_from_other_tenants_config:
         import_from_other_tenants(client, import_from_other_tenants_config, tenant_name)
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/common/logging.py` & `cdk_gw_tools-3.0.0/cdk_gw_tools/common/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/specs/profiles_config.spec.json` & `cdk_gw_tools-3.0.0/cdk_gw_tools/specs/profiles_config.spec.json`

 * *Files identical despite different names*

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/specs/tenant_mappings-input.json` & `cdk_gw_tools-3.0.0/cdk_gw_tools/specs/tenant_mappings-input.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333333%*

 * *Differences: {"'definitions'": "{'TenantMapping': {'properties': {delete: ['concentrated']}}}"}*

```diff
@@ -39,18 +39,14 @@
             ],
             "type": "object"
         },
         "TenantMapping": {
             "additionalProperties": false,
             "description": "Tenant mapping as defined in the API definition",
             "properties": {
-                "concentrated": {
-                    "description": "Whether the mapping is concentrated",
-                    "type": "boolean"
-                },
                 "logicalTopicName": {
                     "maxLength": 255,
                     "type": "string"
                 },
                 "physicalTopicName": {
                     "maxLength": 255,
                     "type": "string"
```

### Comparing `cdk_gw_tools-0.4.4/cdk_gw_tools/specs/user-mappings.spec.json` & `cdk_gw_tools-3.0.0/cdk_gw_tools/specs/user-mappings.spec.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9701562499999999%*

 * *Differences: {"'definitions'": "{'identities': {'items': {replace: OrderedDict([('oneOf', "*

 * *                  "[OrderedDict([('type', 'string')]), OrderedDict([('$ref', "*

 * *                  "'#/definitions/detailed_identity')])])])}, 'description': 'Sets the "*

 * *                  "username/principal only. The username and principal will use the same value.'}, "*

 * *                  "'detailed_identity': OrderedDict([('type', 'object'), ('additionalProperties', "*

 * *                  "False), ('patternProperties', OrderedDict([(' […]*

```diff
@@ -1,15 +1,51 @@
 {
     "$id": "user-mappings.spec.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "definitions": {
+        "detailed_identity": {
+            "additionalProperties": false,
+            "patternProperties": {
+                "x-": {}
+            },
+            "properties": {
+                "groups": {
+                    "description": "List of groups to be mapped to the principal. Groups apply to all of GW, not just the vClusters",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array",
+                    "uniqueItems": true
+                },
+                "principal": {
+                    "description": "The Identity ID (i.e. claims.sub value when using OAuth)",
+                    "type": "string"
+                },
+                "username": {
+                    "description": "Human friendly username used for ACLs/Interceptors",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "username"
+            ],
+            "type": "object"
+        },
         "identities": {
+            "description": "Sets the username/principal only. The username and principal will use the same value.",
             "items": {
-                "type": "string"
+                "oneOf": [
+                    {
+                        "type": "string"
+                    },
+                    {
+                        "$ref": "#/definitions/detailed_identity"
+                    }
+                ]
             },
             "type": "array",
             "uniqueItems": true
         }
     },
     "description": "Specification for user-mapping management",
     "id": "user-mappings.spec.json",
@@ -19,15 +55,15 @@
     "properties": {
         "userMappings": {
             "additionalProperties": false,
             "minProperties": 1,
             "patternProperties": {
                 "^[a-zA-Z0-9_\\-\\.]+$": {
                     "additionalProperties": false,
-                    "description": "vCluster identities user-mappings",
+                    "description": "vCluster identities user-mappings.",
                     "properties": {
                         "identities": {
                             "$ref": "#/definitions/identities"
                         }
                     },
                     "required": [
                         "identities"
```

### Comparing `cdk_gw_tools-0.4.4/pyproject.toml` & `cdk_gw_tools-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "cdk-gw-tools"
 description = "Conduktor Proxy API Client"
-version = "0.4.4"
+version = "3.0.0"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.md"
 license = "LICENSE"
 packages = [{ include = "cdk_gw_tools" }]
 keywords = ["compose-x", "conduktor", "kafka", "proxy"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 include = [
     "cdk_gw_tools/**/*.json",
@@ -28,19 +27,19 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/JohnPreston/cdk-gw-tools/issues"
 "Source (GitHub)" = "https://github.com/JohnPreston/cdk-gw-tools"
 "Source (CodeBerg)" = "https://codeberg.org/JohnPreston/cdk-gw-tools"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-cdk-proxy-api-client = "^0.7"
-compose-x-common = "^1.4.1"
-jsonschema = ">=4.15,<4.18"
-importlib-resources = "^6.1.0"
+python = "^3.9"
+cdk-proxy-api-client = "3.0.0"
+compose-x-common = "^1.4.7"
+jsonschema = ">=4.18"
+importlib-resources = "^6.4"
 pyyaml = "^6.0"
 dacite = "^1.8.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 black = "^23.9"
 isort = "^5.12"
@@ -52,15 +51,15 @@
 cdk-cli = "cdk_gw_tools.cli:main"
 
 
 [tool.tbump]
 github_url = "https://github.com/JohnPreston/cdk-gw-tools"
 
 [tool.tbump.version]
-current = "0.4.4"
+current = "3.0.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `cdk_gw_tools-0.4.4/PKG-INFO` & `cdk_gw_tools-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: cdk-gw-tools
-Version: 0.4.4
+Version: 3.0.0
 Summary: Conduktor Proxy API Client
 License: LICENSE
 Keywords: compose-x,conduktor,kafka,proxy
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cdk-proxy-api-client (>=0.7,<0.8)
-Requires-Dist: compose-x-common (>=1.4.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: cdk-proxy-api-client (==3.0.0)
+Requires-Dist: compose-x-common (>=1.4.7,<2.0.0)
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
-Requires-Dist: importlib-resources (>=6.1.0,<7.0.0)
-Requires-Dist: jsonschema (>=4.15,<4.18)
+Requires-Dist: importlib-resources (>=6.4,<7.0)
+Requires-Dist: jsonschema (>=4.18)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Bug Tracker, https://github.com/JohnPreston/cdk-gw-tools/issues
 Project-URL: Source (GitHub), https://github.com/JohnPreston/cdk-gw-tools
 Project-URL: Source (CodeBerg), https://codeberg.org/JohnPreston/cdk-gw-tools
 Description-Content-Type: text/markdown
 
 # cdk-gw-tools
```

