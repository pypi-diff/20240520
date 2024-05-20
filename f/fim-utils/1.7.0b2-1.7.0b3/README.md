# Comparing `tmp/fim-utils-1.7.0b2.tar.gz` & `tmp/fim-utils-1.7.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim-utils-1.7.0b2.tar", last modified: Sun May 12 19:25:26 2024, max compression
+gzip compressed data, was "fim-utils-1.7.0b3.tar", last modified: Mon May 20 21:39:57 2024, max compression
```

## Comparing `fim-utils-1.7.0b2.tar` & `fim-utils-1.7.0b3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1955 2024-01-04 15:38:10.582923 fim-utils-1.7.0b2/.gitignore
--rw-r--r--   0        0        0     1071 2024-01-04 15:38:10.583073 fim-utils-1.7.0b2/LICENSE
--rw-r--r--   0        0        0      201 2024-01-04 15:38:10.583205 fim-utils-1.7.0b2/MANIFEST.in
--rw-r--r--   0        0        0     8671 2024-05-11 02:27:13.133092 fim-utils-1.7.0b2/README.md
--rw-r--r--   0        0        0      158 2024-05-12 19:19:59.482720 fim-utils-1.7.0b2/fimutil/__init__.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.583760 fim-utils-1.7.0b2/fimutil/al2s/__init__.py
--rw-r--r--   0        0        0       70 2024-02-27 14:27:42.901969 fim-utils-1.7.0b2/fimutil/al2s/al2s.conf.template
--rw-r--r--   0        0        0    12377 2024-02-27 14:27:42.902156 fim-utils-1.7.0b2/fimutil/al2s/al2s_api.py
--rw-r--r--   0        0        0     9603 2024-02-27 14:27:42.903191 fim-utils-1.7.0b2/fimutil/al2s/arm.py
--rw-r--r--   0        0        0      667 2024-01-04 15:38:10.584096 fim-utils-1.7.0b2/fimutil/al2s/cloud_cfg.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.584401 fim-utils-1.7.0b2/fimutil/netam/__init__.py
--rw-r--r--   0        0        0    21817 2024-05-10 08:58:33.558511 fim-utils-1.7.0b2/fimutil/netam/arm.py
--rw-r--r--   0        0        0     4247 2024-01-04 15:38:10.584715 fim-utils-1.7.0b2/fimutil/netam/nso.py
--rw-r--r--   0        0        0     3439 2024-01-04 15:38:10.584875 fim-utils-1.7.0b2/fimutil/netam/sr_pce.py
--rw-r--r--   0        0        0        2 2024-01-04 15:38:10.585206 fim-utils-1.7.0b2/fimutil/ralph/__init__.py
--rw-r--r--   0        0        0     3478 2024-05-10 17:29:54.447929 fim-utils-1.7.0b2/fimutil/ralph/asset.py
--rw-r--r--   0        0        0     2454 2024-01-04 15:38:10.585509 fim-utils-1.7.0b2/fimutil/ralph/dp_switch.py
--rw-r--r--   0        0        0     3991 2024-01-04 15:38:10.585652 fim-utils-1.7.0b2/fimutil/ralph/ethernetport.py
--rw-r--r--   0        0        0    25892 2024-05-12 19:22:30.018036 fim-utils-1.7.0b2/fimutil/ralph/fim_helper.py
--rw-r--r--   0        0        0     2574 2024-01-04 15:38:10.586028 fim-utils-1.7.0b2/fimutil/ralph/fpga.py
--rw-r--r--   0        0        0     2088 2024-02-27 14:24:50.635061 fim-utils-1.7.0b2/fimutil/ralph/gpu.py
--rw-r--r--   0        0        0     3307 2024-01-04 15:38:10.586277 fim-utils-1.7.0b2/fimutil/ralph/model.py
--rw-r--r--   0        0        0     1725 2024-01-04 15:38:10.586428 fim-utils-1.7.0b2/fimutil/ralph/nvme.py
--rw-r--r--   0        0        0     1974 2024-05-12 17:01:53.392063 fim-utils-1.7.0b2/fimutil/ralph/p4_switch.py
--rw-r--r--   0        0        0     1384 2024-01-04 15:38:10.586557 fim-utils-1.7.0b2/fimutil/ralph/ralph_uri.py
--rw-r--r--   0        0        0     8381 2024-05-10 20:05:45.369295 fim-utils-1.7.0b2/fimutil/ralph/site.py
--rw-r--r--   0        0        0      885 2024-01-04 15:38:10.586904 fim-utils-1.7.0b2/fimutil/ralph/storage.py
--rw-r--r--   0        0        0    11349 2024-05-11 02:27:13.139125 fim-utils-1.7.0b2/fimutil/ralph/worker_node.py
--rw-r--r--   0        0        0        0 2024-01-04 15:38:10.587417 fim-utils-1.7.0b2/fimutil/utilities/__init__.py
--rw-r--r--   0        0        0     6216 2024-01-04 15:56:37.608653 fim-utils-1.7.0b2/fimutil/utilities/generate_instance_flavors.py
--rw-r--r--   0        0        0     1363 2024-02-27 14:27:42.903349 fim-utils-1.7.0b2/fimutil/utilities/scan_al2s.py
--rw-r--r--   0        0        0     1877 2024-01-04 15:38:10.588111 fim-utils-1.7.0b2/fimutil/utilities/scan_net.py
--rw-r--r--   0        0        0     5625 2024-01-04 15:38:10.588590 fim-utils-1.7.0b2/fimutil/utilities/scan_site.py
--rw-r--r--   0        0        0     2121 2024-01-04 15:38:10.588804 fim-utils-1.7.0b2/fimutil/utilities/scan_worker.py
--rw-r--r--   0        0        0     1032 2024-05-12 19:19:31.473571 fim-utils-1.7.0b2/pyproject.toml
--rw-r--r--   0        0        0      984 2024-01-04 15:38:10.589207 fim-utils-1.7.0b2/setup.py
--rw-r--r--   0        0        0     1513 2024-02-27 14:27:42.903591 fim-utils-1.7.0b2/test/al2s_test.py
--rw-r--r--   0        0        0     1114 2024-01-04 15:38:10.589872 fim-utils-1.7.0b2/test/netam_test.py
--rw-r--r--   0        0        0      326 2024-01-04 15:38:10.590054 fim-utils-1.7.0b2/test/ralph_test.py
--rw-r--r--   0        0        0     9397 1970-01-01 00:00:00.000000 fim-utils-1.7.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1955 2024-01-04 15:38:10.582923 fim-utils-1.7.0b3/.gitignore
+-rw-r--r--   0        0        0     1071 2024-01-04 15:38:10.583073 fim-utils-1.7.0b3/LICENSE
+-rw-r--r--   0        0        0      201 2024-01-04 15:38:10.583205 fim-utils-1.7.0b3/MANIFEST.in
+-rw-r--r--   0        0        0     8671 2024-05-11 02:27:13.133092 fim-utils-1.7.0b3/README.md
+-rw-r--r--   0        0        0      158 2024-05-20 21:34:37.660482 fim-utils-1.7.0b3/fimutil/__init__.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.583760 fim-utils-1.7.0b3/fimutil/al2s/__init__.py
+-rw-r--r--   0        0        0       70 2024-02-27 14:27:42.901969 fim-utils-1.7.0b3/fimutil/al2s/al2s.conf.template
+-rw-r--r--   0        0        0    12377 2024-02-27 14:27:42.902156 fim-utils-1.7.0b3/fimutil/al2s/al2s_api.py
+-rw-r--r--   0        0        0     9603 2024-02-27 14:27:42.903191 fim-utils-1.7.0b3/fimutil/al2s/arm.py
+-rw-r--r--   0        0        0      667 2024-01-04 15:38:10.584096 fim-utils-1.7.0b3/fimutil/al2s/cloud_cfg.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.584401 fim-utils-1.7.0b3/fimutil/netam/__init__.py
+-rw-r--r--   0        0        0    21817 2024-05-10 08:58:33.558511 fim-utils-1.7.0b3/fimutil/netam/arm.py
+-rw-r--r--   0        0        0     4247 2024-01-04 15:38:10.584715 fim-utils-1.7.0b3/fimutil/netam/nso.py
+-rw-r--r--   0        0        0     3439 2024-01-04 15:38:10.584875 fim-utils-1.7.0b3/fimutil/netam/sr_pce.py
+-rw-r--r--   0        0        0        2 2024-01-04 15:38:10.585206 fim-utils-1.7.0b3/fimutil/ralph/__init__.py
+-rw-r--r--   0        0        0     3478 2024-05-10 17:29:54.447929 fim-utils-1.7.0b3/fimutil/ralph/asset.py
+-rw-r--r--   0        0        0     2454 2024-01-04 15:38:10.585509 fim-utils-1.7.0b3/fimutil/ralph/dp_switch.py
+-rw-r--r--   0        0        0     3991 2024-01-04 15:38:10.585652 fim-utils-1.7.0b3/fimutil/ralph/ethernetport.py
+-rw-r--r--   0        0        0    26151 2024-05-20 21:01:12.191690 fim-utils-1.7.0b3/fimutil/ralph/fim_helper.py
+-rw-r--r--   0        0        0     2574 2024-01-04 15:38:10.586028 fim-utils-1.7.0b3/fimutil/ralph/fpga.py
+-rw-r--r--   0        0        0     2088 2024-02-27 14:24:50.635061 fim-utils-1.7.0b3/fimutil/ralph/gpu.py
+-rw-r--r--   0        0        0     3307 2024-01-04 15:38:10.586277 fim-utils-1.7.0b3/fimutil/ralph/model.py
+-rw-r--r--   0        0        0     1725 2024-01-04 15:38:10.586428 fim-utils-1.7.0b3/fimutil/ralph/nvme.py
+-rw-r--r--   0        0        0     1974 2024-05-12 17:01:53.392063 fim-utils-1.7.0b3/fimutil/ralph/p4_switch.py
+-rw-r--r--   0        0        0     1384 2024-01-04 15:38:10.586557 fim-utils-1.7.0b3/fimutil/ralph/ralph_uri.py
+-rw-r--r--   0        0        0     8381 2024-05-10 20:05:45.369295 fim-utils-1.7.0b3/fimutil/ralph/site.py
+-rw-r--r--   0        0        0      885 2024-01-04 15:38:10.586904 fim-utils-1.7.0b3/fimutil/ralph/storage.py
+-rw-r--r--   0        0        0    11410 2024-05-20 21:17:34.454934 fim-utils-1.7.0b3/fimutil/ralph/worker_node.py
+-rw-r--r--   0        0        0        0 2024-01-04 15:38:10.587417 fim-utils-1.7.0b3/fimutil/utilities/__init__.py
+-rw-r--r--   0        0        0     6216 2024-01-04 15:56:37.608653 fim-utils-1.7.0b3/fimutil/utilities/generate_instance_flavors.py
+-rw-r--r--   0        0        0     1363 2024-02-27 14:27:42.903349 fim-utils-1.7.0b3/fimutil/utilities/scan_al2s.py
+-rw-r--r--   0        0        0     1877 2024-01-04 15:38:10.588111 fim-utils-1.7.0b3/fimutil/utilities/scan_net.py
+-rw-r--r--   0        0        0     5625 2024-01-04 15:38:10.588590 fim-utils-1.7.0b3/fimutil/utilities/scan_site.py
+-rw-r--r--   0        0        0     2121 2024-01-04 15:38:10.588804 fim-utils-1.7.0b3/fimutil/utilities/scan_worker.py
+-rw-r--r--   0        0        0     1032 2024-05-20 21:34:37.664203 fim-utils-1.7.0b3/pyproject.toml
+-rw-r--r--   0        0        0      984 2024-01-04 15:38:10.589207 fim-utils-1.7.0b3/setup.py
+-rw-r--r--   0        0        0     1513 2024-02-27 14:27:42.903591 fim-utils-1.7.0b3/test/al2s_test.py
+-rw-r--r--   0        0        0     1114 2024-01-04 15:38:10.589872 fim-utils-1.7.0b3/test/netam_test.py
+-rw-r--r--   0        0        0      326 2024-01-04 15:38:10.590054 fim-utils-1.7.0b3/test/ralph_test.py
+-rw-r--r--   0        0        0     9397 1970-01-01 00:00:00.000000 fim-utils-1.7.0b3/PKG-INFO
```

### Comparing `fim-utils-1.7.0b2/.gitignore` & `fim-utils-1.7.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/LICENSE` & `fim-utils-1.7.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/README.md` & `fim-utils-1.7.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/al2s/al2s_api.py` & `fim-utils-1.7.0b3/fimutil/al2s/al2s_api.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/al2s/arm.py` & `fim-utils-1.7.0b3/fimutil/al2s/arm.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/al2s/cloud_cfg.py` & `fim-utils-1.7.0b3/fimutil/al2s/cloud_cfg.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/netam/arm.py` & `fim-utils-1.7.0b3/fimutil/netam/arm.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/netam/nso.py` & `fim-utils-1.7.0b3/fimutil/netam/nso.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/netam/sr_pce.py` & `fim-utils-1.7.0b3/fimutil/netam/sr_pce.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/asset.py` & `fim-utils-1.7.0b3/fimutil/ralph/asset.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/dp_switch.py` & `fim-utils-1.7.0b3/fimutil/ralph/dp_switch.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/ethernetport.py` & `fim-utils-1.7.0b3/fimutil/ralph/ethernetport.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/fim_helper.py` & `fim-utils-1.7.0b3/fimutil/ralph/fim_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Tuple, List, Dict, Any, Set
 import logging
 import re
 from collections import defaultdict
 
 from fim.user.topology import SubstrateTopology
 from fim.user.node import Node, NodeType
@@ -305,14 +306,18 @@
     Optionally supply externally obtained postal address.
     """
     logging.info(f'Producing SubstrateTopology model for site {site.name}')
 
     loc = None
     if address is not None:
         loc = Location(postal=address)
+        loc.to_latlon()
+
+    if config and config.get(site.name) and config.get(site.name).get('location'):
+        loc = Location.from_json(json_string=json.dumps(config.get(site.name).get('location')))
 
     topo = SubstrateTopology()
 
     port_map = dict()
     # create workers with components
     for worker in site.workers:
         # {"Name": "lbnl-w1.fabric-testbed.net", "SN": "5B3BR53"} {"Model": "R7525", "RAM": "512G", "CPU": "2", "Core": 64, "Disk": "0.0 TB"}
@@ -508,15 +513,15 @@
 
     p4_name = p4_switch_name_id(real_switch_site.lower(),
                                 site.p4_switch.fields['IP'] if site.p4_switch.fields['IP'] else site.p4_switch.fields['SN'])
     logging.info(f'Adding P4 switch {p4_name}')
     p4 = topo.add_node(name=p4_name[0],
                        node_id=p4_name[1],
                        site=site.name, ntype=NodeType.Switch, stitch_node=False,
-                       capacities=Capacities(unit=1))
+                       capacities=Capacities(unit=1), management_ip=site.p4_switch.fields['IP'])
 
     p4_service_type = ServiceType.MPLS
     p4_ns = p4.add_network_service(name=p4.name + '-ns', node_id=p4.node_id + '-ns',
                                    nstype=p4_service_type, stitch_node=False)
 
     dp_to_p4_ports = []
```

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/fpga.py` & `fim-utils-1.7.0b3/fimutil/ralph/fpga.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/gpu.py` & `fim-utils-1.7.0b3/fimutil/ralph/gpu.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/model.py` & `fim-utils-1.7.0b3/fimutil/ralph/model.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/nvme.py` & `fim-utils-1.7.0b3/fimutil/ralph/nvme.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/p4_switch.py` & `fim-utils-1.7.0b3/fimutil/ralph/p4_switch.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/ralph_uri.py` & `fim-utils-1.7.0b3/fimutil/ralph/ralph_uri.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/site.py` & `fim-utils-1.7.0b3/fimutil/ralph/site.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/storage.py` & `fim-utils-1.7.0b3/fimutil/ralph/storage.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/ralph/worker_node.py` & `fim-utils-1.7.0b3/fimutil/ralph/worker_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
         ram = int(custom_fields_dict.get('usable_memory', '0'))//1024
         if ram > 0:
             self.model.fields['RAM'] = f'{ram}G'
         disk = custom_fields_dict.get('usable_disk')
         if disk:
             self.model.fields['Disk'] = f'{disk}G'
 
-        if self.config and self.config.get('ram_offset'):
-            ram_offset = self.config.get('ram_offset')
+        if self.config and self.config.get(self.site) and self.config.get(self.site).get('ram_offset'):
+            ram_offset = self.config.get(self.site).get('ram_offset')
             ram -= ram_offset
             if ram > 0:
                 self.model.fields['RAM'] = f'{ram}G'
 
         # override from config if present
         if self.config and self.config.get(self.site) and self.config.get(self.site).get('workers') and \
             self.config.get(self.site).get('workers').get(self.fields['Name']):
```

### Comparing `fim-utils-1.7.0b2/fimutil/utilities/generate_instance_flavors.py` & `fim-utils-1.7.0b3/fimutil/utilities/generate_instance_flavors.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/utilities/scan_al2s.py` & `fim-utils-1.7.0b3/fimutil/utilities/scan_al2s.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/utilities/scan_net.py` & `fim-utils-1.7.0b3/fimutil/utilities/scan_net.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/utilities/scan_site.py` & `fim-utils-1.7.0b3/fimutil/utilities/scan_site.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/fimutil/utilities/scan_worker.py` & `fim-utils-1.7.0b3/fimutil/utilities/scan_worker.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/pyproject.toml` & `fim-utils-1.7.0b3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License",
 		"Programming Language :: Python :: 3",
 		"Operating System :: OS Independent"]
 dynamic = ["version", "description"]
 requires-python = '>=3.9'
 dependencies = [
-	"fabric_fim >= 1.7.0b2",
+	"fabric_fim >= 1.7.0b3",
     "pyjq == 2.6.0",
 	"jsonpath_ng == 1.5.3",
 	]
 
 [tool.flit.module]
 name = "fimutil"
```

### Comparing `fim-utils-1.7.0b2/setup.py` & `fim-utils-1.7.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/test/al2s_test.py` & `fim-utils-1.7.0b3/test/al2s_test.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/test/netam_test.py` & `fim-utils-1.7.0b3/test/netam_test.py`

 * *Files identical despite different names*

### Comparing `fim-utils-1.7.0b2/PKG-INFO` & `fim-utils-1.7.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fim-utils
-Version: 1.7.0b2
+Version: 1.7.0b3
 Summary: This is a package of Information Model utilitied for FABRIC
 Author-email: Ilya Baldin <ibaldin@renci.org>, Xi Yang <xiyang@es.net>, Hussamuddin Nasir <nasir@netlab.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Dist: fabric_fim >= 1.7.0b2
+Requires-Dist: fabric_fim >= 1.7.0b3
 Requires-Dist: pyjq == 2.6.0
 Requires-Dist: jsonpath_ng == 1.5.3
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: flit ; extra == "test"
 Project-URL: Home, https://github.com/fabric-testbed/information-model-utils
 Provides-Extra: test
```

