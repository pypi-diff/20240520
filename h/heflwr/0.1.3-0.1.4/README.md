# Comparing `tmp/heflwr-0.1.3.tar.gz` & `tmp/heflwr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflwr-0.1.3.tar", last modified: Wed May 15 12:54:57 2024, max compression
+gzip compressed data, was "heflwr-0.1.4.tar", last modified: Mon May 20 06:34:44 2024, max compression
```

## Comparing `heflwr-0.1.3.tar` & `heflwr-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.479993 heflwr-0.1.3/
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      552 2024-05-15 12:54:57.478993 heflwr-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-14 16:05:22.000000 heflwr-0.1.3/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-15 12:54:57.479993 heflwr-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-05-15 12:54:23.000000 heflwr-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.424346 heflwr-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.439346 heflwr-0.1.3/src/heflwr/
--rw-rw-rw-   0        0        0      104 2024-05-15 12:54:23.000000 heflwr-0.1.3/src/heflwr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.456993 heflwr-0.1.3/src/heflwr/fed/
--rw-rw-rw-   0        0        0       87 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/__init__.py
--rw-rw-rw-   0        0        0     6687 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/aggregate.py
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/he_client_manager.py
--rw-rw-rw-   0        0        0     4746 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/fed/hetero_aggregate.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.457993 heflwr-0.1.3/src/heflwr/log/
--rw-rw-rw-   0        0        0       22 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/log/__init__.py
--rw-rw-rw-   0        0        0     3458 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/log/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.458994 heflwr-0.1.3/src/heflwr/monitor/
--rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.463993 heflwr-0.1.3/src/heflwr/monitor/process_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/__init__.py
--rw-rw-rw-   0        0        0     5522 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5541 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5356 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/process_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.468993 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/__init__.py
--rw-rw-rw-   0        0        0     4938 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5299 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5025 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/thread_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.471993 heflwr-0.1.3/src/heflwr/monitor/utils/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/utils/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/utils/network.py
--rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/monitor/utils/power.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.475993 heflwr-0.1.3/src/heflwr/nn/
--rw-rw-rw-   0        0        0      153 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/__init__.py
--rw-rw-rw-   0        0        0      351 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/scaler.py
--rw-rw-rw-   0        0        0     9696 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/ssconv2d.py
--rw-rw-rw-   0        0        0     9284 2024-05-14 16:05:22.000000 heflwr-0.1.3/src/heflwr/nn/sslinear.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.452993 heflwr-0.1.3/src/heflwr.egg-info/
--rw-rw-rw-   0        0        0      552 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 12:54:57.000000 heflwr-0.1.3/src/heflwr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 12:54:57.476993 heflwr-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.828838 heflwr-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      552 2024-05-20 06:34:44.828838 heflwr-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-14 16:05:22.000000 heflwr-0.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:34:44.828838 heflwr-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-05-20 06:33:33.000000 heflwr-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.719585 heflwr-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.735432 heflwr-0.1.4/src/heflwr/
+-rw-rw-rw-   0        0        0      104 2024-05-15 12:54:23.000000 heflwr-0.1.4/src/heflwr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.751134 heflwr-0.1.4/src/heflwr/fed/
+-rw-rw-rw-   0        0        0       94 2024-05-20 06:25:41.000000 heflwr-0.1.4/src/heflwr/fed/__init__.py
+-rw-rw-rw-   0        0        0     6687 2024-05-19 16:30:24.000000 heflwr-0.1.4/src/heflwr/fed/aggregate.py
+-rw-rw-rw-   0        0        0     4796 2024-05-20 06:33:33.000000 heflwr-0.1.4/src/heflwr/fed/heflwr_aggregate.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/fed/heflwr_client_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.766957 heflwr-0.1.4/src/heflwr/log/
+-rw-rw-rw-   0        0        0       22 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/log/__init__.py
+-rw-rw-rw-   0        0        0     3458 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/log/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.766957 heflwr-0.1.4/src/heflwr/monitor/
+-rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.781421 heflwr-0.1.4/src/heflwr/monitor/process_monitor/
+-rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/__init__.py
+-rw-rw-rw-   0        0        0     5522 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5541 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5356 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.797045 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/
+-rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/__init__.py
+-rw-rw-rw-   0        0        0     4938 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5299 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5025 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.812876 heflwr-0.1.4/src/heflwr/monitor/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/utils/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/utils/network.py
+-rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/utils/power.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.828838 heflwr-0.1.4/src/heflwr/nn/
+-rw-rw-rw-   0        0        0      153 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/nn/__init__.py
+-rw-rw-rw-   0        0        0      359 2024-05-19 19:11:39.000000 heflwr-0.1.4/src/heflwr/nn/scaler.py
+-rw-rw-rw-   0        0        0     3832 2024-05-19 19:19:04.000000 heflwr-0.1.4/src/heflwr/nn/ssbatchnorm2d.py
+-rw-rw-rw-   0        0        0     9704 2024-05-19 19:11:39.000000 heflwr-0.1.4/src/heflwr/nn/ssconv2d.py
+-rw-rw-rw-   0        0        0     9292 2024-05-19 19:11:39.000000 heflwr-0.1.4/src/heflwr/nn/sslinear.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.751134 heflwr-0.1.4/src/heflwr.egg-info/
+-rw-rw-rw-   0        0        0      552 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.828838 heflwr-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.4/tests/test.py
```

### Comparing `heflwr-0.1.3/LICENSE` & `heflwr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/PKG-INFO` & `heflwr-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflwr
-Version: 0.1.3
+Version: 0.1.4
 Summary: 「HeFlwr」is a federated learning package for heterogeneous devices.
 Home-page: https://github.com/QVQZZZ/HeFlwr
 Author: Zhu Yaolin
 Author-email: zhuyaolinluck@qq.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `heflwr-0.1.3/setup.py` & `heflwr-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.rst", encoding="UTF-8") as f:
         return f.read()
 
 
 setup(
     name="heflwr",
-    version="0.1.3",
+    version="0.1.4",
     description="「HeFlwr」is a federated learning package for heterogeneous devices.",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author="Zhu Yaolin",
     author_email="zhuyaolinluck@qq.com",
     long_description=readme(),
     long_description_content_type='text/x-rst',
```

### Comparing `heflwr-0.1.3/src/heflwr/fed/aggregate.py` & `heflwr-0.1.4/src/heflwr/fed/aggregate.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/fed/hetero_aggregate.py` & `heflwr-0.1.4/src/heflwr/fed/heflwr_aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch
 import torch.nn as nn
 from flwr.common.parameter import parameters_to_ndarrays, ndarrays_to_parameters
 from flwr.common.typing import Parameters, FitRes
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_layer
-from ..nn import SSLinear, SSConv2d
+from ..nn import SUPPORT_LAYER
 from ..log.logger import logger
 
 
 def extract(parameters: Parameters, client_net: nn.Module, server_net: nn.Module) -> Parameters:
     """
     Extracts the parameters of a client model (`client_net`) from the global server model (`server_net`)
     based on a given `Parameters` object.
@@ -31,16 +31,18 @@
     """
     with torch.no_grad():
         tensor_list: List[torch.Tensor] = [torch.Tensor(_) for _ in parameters_to_ndarrays(parameters)]
         global_dict = {name: tensor for name, tensor in zip(server_net.state_dict().keys(), tensor_list)}
         server_net.load_state_dict(global_dict)
 
         for layer, father_layer in zip(client_net.modules(), server_net.modules()):
-            if hasattr(layer, 'reset_parameters_from_father_layer'):
+            if isinstance(layer, SUPPORT_LAYER):
                 layer.reset_parameters_from_father_layer(father_layer)
+            else:
+                logger.debug(f"Can't extract {layer}, ignore it.")
 
         array_list: List[np.ndarray] = [_.numpy() for _ in list(client_net.parameters())]
         parameters = ndarrays_to_parameters(array_list)
     return parameters
 
 
 def merge(results: List[Tuple[ClientProxy, FitRes]], client_nets: List[nn.Module], server_net: nn.Module) -> Parameters:
@@ -72,15 +74,15 @@
             parameters_list.append(tensor_parameters)
 
         for client_net, parameters in zip(client_nets, parameters_list):
             client_dict = {name: tensor for name, tensor in zip(client_net.state_dict().keys(), parameters)}
             client_net.load_state_dict(client_dict)
 
         for layer_name, layer in dict(server_net.named_modules()).items():
-            if isinstance(layer, Union[SSConv2d, SSLinear]):
+            if isinstance(layer, SUPPORT_LAYER):
                 client_layers = [dict(client_net.named_modules())[layer_name] for client_net in client_nets]
                 aggregate_layer(layer, client_layers, num_examples_list)
             else:
                 logger.debug(f"Can't merge {layer}, ignore it.")
 
         array_list: List[np.ndarray] = [_.numpy() for _ in list(server_net.parameters())]
         parameters = ndarrays_to_parameters(array_list)
```

### Comparing `heflwr-0.1.3/src/heflwr/log/logger.py` & `heflwr-0.1.4/src/heflwr/log/logger.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/process_monitor/file_monitor.py` & `heflwr-0.1.4/src/heflwr/monitor/process_monitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/process_monitor/prometheus_monitor.py` & `heflwr-0.1.4/src/heflwr/monitor/process_monitor/prometheus_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/process_monitor/remote_monitor.py` & `heflwr-0.1.4/src/heflwr/monitor/process_monitor/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/thread_monitor/file_monitor.py` & `heflwr-0.1.4/src/heflwr/monitor/thread_monitor/file_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/thread_monitor/prometheus_monitor.py` & `heflwr-0.1.4/src/heflwr/monitor/thread_monitor/prometheus_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/thread_monitor/remote_monitor.py` & `heflwr-0.1.4/src/heflwr/monitor/thread_monitor/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/utils/network.py` & `heflwr-0.1.4/src/heflwr/monitor/utils/network.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/monitor/utils/power.py` & `heflwr-0.1.4/src/heflwr/monitor/utils/power.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.3/src/heflwr/nn/ssconv2d.py` & `heflwr-0.1.4/src/heflwr/nn/ssconv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Layer_Range = Union[Interval, Intervals]
 
 
 class SSConv2d(nn.Conv2d):
     def __init__(self: Self, in_channels: int, out_channels: int, kernel_size: Union[int, Tuple[int, int]],
                  stride: Union[int, Tuple[int, int]] = 1, padding: Union[int, Tuple[int, int]] = 0,
                  dilation: Union[int, Tuple[int, int]] = 1, groups: int = 1, bias: bool = True,
-                 in_channels_ranges: Layer_Range = ('0', '1'), out_channels_ranges: Layer_Range = ('0', '1')):
+                 in_channels_ranges: Layer_Range = ('0', '1'), out_channels_ranges: Layer_Range = ('0', '1')) -> None:
 
         # if in_channels_ranges/out_channels_ranges belong to Interval, then convert into Intervals.
         if isinstance(in_channels_ranges[0], str):
             in_channels_ranges = [in_channels_ranges]
         if isinstance(out_channels_ranges[0], str):
             out_channels_ranges = [out_channels_ranges]
```

### Comparing `heflwr-0.1.3/src/heflwr/nn/sslinear.py` & `heflwr-0.1.4/src/heflwr/nn/sslinear.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Intervals = List[Tuple[str, str]]
 Layer_Range = Union[Interval, Intervals]
 
 
 class SSLinear(nn.Linear):
     def __init__(self: Self, in_features: int, out_features: int, bias: bool = True,
                  in_features_ranges: Layer_Range = ('0', '1'),
-                 out_features_ranges: Layer_Range = ('0', '1')):
+                 out_features_ranges: Layer_Range = ('0', '1')) -> None:
 
         # if in_channels_ranges/out_channels_ranges belong to Interval, then convert into Intervals.
         if isinstance(in_features_ranges[0], str):
             in_features_ranges = [in_features_ranges]
         if isinstance(out_features_ranges[0], str):
             out_features_ranges = [out_features_ranges]
```

### Comparing `heflwr-0.1.3/src/heflwr.egg-info/PKG-INFO` & `heflwr-0.1.4/src/heflwr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflwr
-Version: 0.1.3
+Version: 0.1.4
 Summary: 「HeFlwr」is a federated learning package for heterogeneous devices.
 Home-page: https://github.com/QVQZZZ/HeFlwr
 Author: Zhu Yaolin
 Author-email: zhuyaolinluck@qq.com
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `heflwr-0.1.3/src/heflwr.egg-info/SOURCES.txt` & `heflwr-0.1.4/src/heflwr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 src/heflwr/__init__.py
 src/heflwr.egg-info/PKG-INFO
 src/heflwr.egg-info/SOURCES.txt
 src/heflwr.egg-info/dependency_links.txt
 src/heflwr.egg-info/top_level.txt
 src/heflwr/fed/__init__.py
 src/heflwr/fed/aggregate.py
-src/heflwr/fed/he_client_manager.py
-src/heflwr/fed/hetero_aggregate.py
+src/heflwr/fed/heflwr_aggregate.py
+src/heflwr/fed/heflwr_client_manager.py
 src/heflwr/log/__init__.py
 src/heflwr/log/logger.py
 src/heflwr/monitor/__init__.py
 src/heflwr/monitor/process_monitor/__init__.py
 src/heflwr/monitor/process_monitor/file_monitor.py
 src/heflwr/monitor/process_monitor/prometheus_monitor.py
 src/heflwr/monitor/process_monitor/remote_monitor.py
@@ -23,10 +23,11 @@
 src/heflwr/monitor/thread_monitor/prometheus_monitor.py
 src/heflwr/monitor/thread_monitor/remote_monitor.py
 src/heflwr/monitor/utils/__init__.py
 src/heflwr/monitor/utils/network.py
 src/heflwr/monitor/utils/power.py
 src/heflwr/nn/__init__.py
 src/heflwr/nn/scaler.py
+src/heflwr/nn/ssbatchnorm2d.py
 src/heflwr/nn/ssconv2d.py
 src/heflwr/nn/sslinear.py
 tests/test.py
```

