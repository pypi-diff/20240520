# Comparing `tmp/FlowVisor-0.1.9.tar.gz` & `tmp/FlowVisor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.9.tar", last modified: Mon May 13 10:33:57 2024, max compression
+gzip compressed data, was "FlowVisor-0.2.0.tar", last modified: Mon May 20 18:19:30 2024, max compression
```

## Comparing `FlowVisor-0.1.9.tar` & `FlowVisor-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-13 10:33:57.000000 FlowVisor-0.1.9/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.9/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.9/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.9/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.9/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.9/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.9/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.9/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    14240 2024-05-13 10:16:16.000000 FlowVisor-0.1.9/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2214 2024-05-13 09:29:39.000000 FlowVisor-0.1.9/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8113 2024-05-13 10:09:22.000000 FlowVisor-0.1.9/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8460 2024-05-13 10:20:06.000000 FlowVisor-0.1.9/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.1.9/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.9/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.9/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2474 2024-05-13 09:18:43.000000 FlowVisor-0.1.9/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.9/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.9/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-13 10:33:57.061928 FlowVisor-0.1.9/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.9/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.369689 FlowVisor-0.2.0/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.365689 FlowVisor-0.2.0/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-20 18:19:30.000000 FlowVisor-0.2.0/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.0/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-20 18:19:30.369689 FlowVisor-0.2.0/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.0/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.365689 FlowVisor-0.2.0/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.0/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-20 18:19:30.365689 FlowVisor-0.2.0/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.0/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.2.0/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.0/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1172 2024-05-20 18:19:00.000000 FlowVisor-0.2.0/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    14811 2024-05-20 18:08:31.000000 FlowVisor-0.2.0/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.0/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7861 2024-05-13 12:26:30.000000 FlowVisor-0.2.0/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.0/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.0/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.0/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.0/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.0/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.0/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.0/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-20 18:19:30.369689 FlowVisor-0.2.0/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.0/setup.py
```

### Comparing `FlowVisor-0.1.9/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.2.0/FlowVisor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.9
+Version: 0.2.0
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
@@ -15,16 +15,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <br />
-  <!-- <img src="" alt="FlowVisorLogo" width="30%"/> -->
-  <h1>FlowVisor</h1>
+  <img src="https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/logo.png" alt="FlowVisor" width="60%"/>
   <p>
     Visualize the flow of your python code.
   </p>
 </div>
 
 <!-- Badges -->
 <div align="center">
```

### Comparing `FlowVisor-0.1.9/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.2.0/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/LICENSE` & `FlowVisor-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/PKG-INFO` & `FlowVisor-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.9
+Version: 0.2.0
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
@@ -15,16 +15,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <br />
-  <!-- <img src="" alt="FlowVisorLogo" width="30%"/> -->
-  <h1>FlowVisor</h1>
+  <img src="https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/logo.png" alt="FlowVisor" width="60%"/>
   <p>
     Visualize the flow of your python code.
   </p>
 </div>
 
 <!-- Badges -->
 <div align="center">
```

### Comparing `FlowVisor-0.1.9/README.md` & `FlowVisor-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 <div align="center">
   <br />
-  <!-- <img src="" alt="FlowVisorLogo" width="30%"/> -->
-  <h1>FlowVisor</h1>
+  <img src="https://raw.githubusercontent.com/cophilot/FlowVisor/main/assets/logo.png" alt="FlowVisor" width="60%"/>
   <p>
     Visualize the flow of your python code.
   </p>
 </div>
 
 <!-- Badges -->
 <div align="center">
```

### Comparing `FlowVisor-0.1.9/flowvisor/cli/add_vis.py` & `FlowVisor-0.2.0/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/flowvisor/cli/remove_vis.py` & `FlowVisor-0.2.0/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/flowvisor/cli/vis_file.py` & `FlowVisor-0.2.0/flowvisor/cli/vis_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 import os
 import sys
 
 from flowvisor.flowvisor import FlowVisor
 
-def generate_graph(file_path):
-    FlowVisor.generate_graph(file_path)
+
+def generate_graph(file_path, verify=False, verify_file=None):
+    if verify_file is not None:
+        FlowVisor.generate_graph(file_path, verify, verify_file)
+    else:
+        FlowVisor.generate_graph(file_path, verify)
+
+    out_file = FlowVisor.CONFIG.output_file
+    print(f"Flow graph generated at {out_file}")
+
 
 def main():
-    print("This script will generate a flow graph from a file that was exported by FlowVisor.")
+    print(
+        "This script will generate a flow graph from a file that was exported by FlowVisor."
+    )
     print("Visit https://github.com/cophilot/FlowVisor#cli for more information.")
     # check if the path is provided as an argument
     args = sys.argv
+
+    if len(args) < 2:
+        print("No file path provided!")
+
+    file_path = args[1]
+
+    if not os.path.exists(file_path):
+        print("Invalid file path!")
+        sys.exit(1)
+
+    verify = False
+    verify_file = None
+
     for index, arg in enumerate(args):
-        if arg == "-file" or arg == "-f":
-            file_path = args[index + 1]
-            if os.path.exists(file_path):
-                generate_graph(file_path)
-                return
-
-    while True:
-        file_path = input("Enter the file you want to generate the flow graph from: ")
-        if not os.path.exists(file_path):
-            print("Invalid file")
-            continue
-        break
-    generate_graph(file_path)
+        if arg == "-verify" or arg == "-v":
+            verify = True
+            if len(args) > index + 1:
+                verify_file = args[index + 1]
+
+    generate_graph(file_path, verify, verify_file)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `FlowVisor-0.1.9/flowvisor/flowvisor.py` & `FlowVisor-0.2.0/flowvisor/flowvisor.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     ROOTS: List[FunctionNode] = []
     STACK: List[FunctionNode] = []
     CONFIG = FlowVisorConfig()
 
     EXCLUDE_FUNCTIONS = []
     VERIFIER_MODE = False
 
+    SYS_INFO = None
+
     @staticmethod
     def add_function_node(func):
         """
         Adds a function node to the list of nodes if it does not exist.
         """
         func_id = function_to_id(func)
         for node in FlowVisor.NODES:
@@ -208,15 +210,17 @@
         """
         Draws some metadata on the graph.
         """
         with Cluster("Metadata", graph_attr={"bgcolor": "#FFFFFF"}):
             if verify_text is not None:
                 Custom(verify_text, blank_image, width="2", height="0.1")
             if FlowVisor.CONFIG.show_system_info:
-                sys_info = utils.get_sys_info()
+                sys_info = FlowVisor.SYS_INFO
+                if sys_info is None:
+                    sys_info = utils.get_sys_info()
                 text = ""
                 for key, value in sys_info.items():
                     text += f"{key}: {value}\n"
                 Custom(text, blank_image, width="6", height="1")
             if FlowVisor.CONFIG.show_timestamp:
                 timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                 Custom(str(timestamp), blank_image, width="3", height="0.2")
@@ -286,59 +290,76 @@
         Saves the flow to a file.
         """
         if FlowVisor.VERIFIER_MODE:
             Logger.log("Can not export in verifier mode!")
             return
 
         nodes_dict = FlowVisor.get_nodes_as_dict()
+        settings = FlowVisor.CONFIG.to_dict()
+        sys_info = utils.get_sys_info()
+
+        data = {"data": nodes_dict, "settings": settings, "sys-info": sys_info}
+
         if export_type == "json":
             if not file.endswith(".json"):
                 file += ".json"
             with open(file, "w", encoding="utf-8") as f:
-                json.dump(nodes_dict, f, indent=4)
+                json.dump(data, f, indent=4)
         if export_type == "pickle":
             if not file.endswith(".pickle"):
                 file += ".pickle"
             with open(file, "wb") as f:
-                pickle.dump(nodes_dict, f)
+                pickle.dump(data, f)
 
     @staticmethod
     def generate_graph(
         file: str = "", verify=False, verify_file_name="flowvisor_verifier.json"
     ):
         """
         Generates the graph from a file.
         """
         if not os.path.exists(file):
             Logger.log(f"File {file} does not exist!")
             return
         mode = "pickle"
         if file.endswith(".json"):
             mode = "json"
+
         if mode == "json":
             with open(file, "r", encoding="utf-8") as f:
-                raw_nodes = json.load(f)
+                raw_data = json.load(f)
         else:
             with open(file, "rb") as f:
-                raw_nodes = pickle.load(f)
+                raw_data = pickle.load(f)
+
+        if "data" in raw_data:
+            raw_nodes = raw_data["data"]
+        else:
+            raw_nodes = raw_data
+
+        if "settings" in raw_data:
+            FlowVisor.CONFIG = FlowVisorConfig.from_dict(raw_data["settings"])
+
+        if "sys-info" in raw_data:
+            FlowVisor.SYS_INFO = raw_data["sys-info"]
 
         for n in raw_nodes:
             node = FunctionNode.from_dict(n)
             FlowVisor.NODES.append(node)
         for node in FlowVisor.NODES:
             node.resolve_children_ids(FlowVisor.NODES)
 
         FlowVisor.graph(verify, verify_file_name)
 
     @staticmethod
     def draw_function_node(func_node: FunctionNode):
         """
         Draws the function node.
         """
-        time_value = TimeValue(FlowVisor.NODES, FlowVisor.CONFIG, FlowVisor.ROOTS)
+        time_value = TimeValue(FlowVisor.NODES, FlowVisor.CONFIG)
 
         node = func_node.get_as_diagram_node(time_value, FlowVisor.CONFIG)
         for child in func_node.children:
             _ = node >> child.get_as_diagram_node(time_value, FlowVisor.CONFIG)
 
     @staticmethod
     def is_function_excluded(func):
```

### Comparing `FlowVisor-0.1.9/flowvisor/flowvisor_config.py` & `FlowVisor-0.2.0/flowvisor/flowvisor_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,20 @@
                 + utils.get_time_as_string(self.advanced_overhead_reduction)
                 + "\n"
             )
         s += "Exclusive Time Mode: " + str(self.exclusive_time_mode) + "\n"
         s += "Use Average Time: " + str(self.use_avg_time) + "\n"
         return s
 
+    def to_dict(self):
+        """
+        Convert the FlowVisorConfig object to a dictionary
+        """
+        return self.__dict__
+
     @staticmethod
     def from_dict(config_dict: dict):
         """
         Create a FlowVisorConfig object from a dictionary
         """
         config = FlowVisorConfig()
         for key in config_dict:
```

### Comparing `FlowVisor-0.1.9/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.2.0/flowvisor/flowvisor_verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,19 +185,19 @@
             print_warning = False
 
             if not FlowVisorVerifier.is_function_verified(entry, node_time, threshold):
                 is_verified = False
                 print_warning = True
 
             time_delta_direction = "more"
-            time_delta_direction_arrow = "📈"
+            time_delta_direction_arrow = "🔼"
             if time_delta < 0:
                 time_delta *= -1
                 time_delta_direction = "less"
-                time_delta_direction_arrow = "📉"
+                time_delta_direction_arrow = "🔽"
 
             Logger.log(
                 f"  Function '{node.file_function_name()}' took {utils.get_time_as_string(time_delta)} {time_delta_direction} than expected ({time_delta_percentage * 100}%) {time_delta_direction_arrow}{'🚨' if print_warning else ''}"
             )
 
         if is_verified:
             Logger.log("All functions are verified! ✅")
@@ -206,28 +206,20 @@
         return is_verified
 
     @staticmethod
     def is_function_verified(entry, node_time, threshold):
         max_value = entry["max"]
         min_value = entry["min"]
         mean_time = entry["time"]
-        interval = max_value - min_value
 
-        offset_interval = interval * threshold
-        offset_meean = mean_time * threshold
+        if min_value <= node_time and node_time <= max_value:
+            return True
 
-        if offset_interval > offset_meean:
-            return (
-                min_value - offset_interval <= node_time
-                and node_time <= max_value + offset_interval
-            )
-        return (
-            mean_time - offset_meean <= node_time
-            and node_time <= mean_time + offset_meean
-        )
+        offset = mean_time * threshold
+        return mean_time - offset <= node_time and node_time <= mean_time + offset
 
     @staticmethod
     def read_existing_file(file_name: str):
         """
         Read the existing verifier file
 
         Args:
```

### Comparing `FlowVisor-0.1.9/flowvisor/function_node.py` & `FlowVisor-0.2.0/flowvisor/function_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,13 +272,14 @@
         """
         node = FunctionNode(None)
         node.id = d["id"]
         node.uuid = d["uuid"]
         node.name = d["name"]
         node.file_path = d["file_path"]
         node.file_name = d["file_name"]
+        node.called = d["called"]
         node.children_ids = [child["uuid"] for child in d["children"]]
         ex_time = d["exclusive_time"]
         in_time = d["inclusive_time"]
         node.set_time(in_time)
         node.child_time = in_time - ex_time
         return node
```

### Comparing `FlowVisor-0.1.9/flowvisor/logger.py` & `FlowVisor-0.2.0/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/flowvisor/sankey.py` & `FlowVisor-0.2.0/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/flowvisor/time_tracker.py` & `FlowVisor-0.2.0/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/flowvisor/time_value.py` & `FlowVisor-0.2.0/flowvisor/time_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,18 @@
     A data structure to store the time values of a flowvisor
     """
 
     def __init__(
         self,
         nodes: List[any],
         config: FlowVisorConfig,
-        roots: List[any],
     ):
         self.max_time = TimeValue.get_max_time(nodes, config)
         self.max_avg_time = TimeValue.get_avg_max_time(nodes, config)
-        self.total_time = TimeValue.get_total_time(nodes, config, roots)
+        self.total_time = TimeValue.get_total_time(nodes)
         self.mean_time = TimeValue.get_mean_time(nodes, config)
         self.mean_avg_time = TimeValue.get_mean_avg_time(nodes, config)
 
     @staticmethod
     def get_max_time(nodes: List[any], config: FlowVisorConfig):
         """
         Returns the highest time.
@@ -44,25 +43,21 @@
         for node in nodes:
             node_time = node.get_avg_time(config.exclusive_time_mode)
             if node_time > highest_time:
                 highest_time = node_time
         return highest_time
 
     @staticmethod
-    def get_total_time(nodes: List[any], config: FlowVisorConfig, roots: List[any]):
+    def get_total_time(nodes: List[any]):
         """
         Returns the total time.
         """
         total_time = 0
-        n = nodes
-        if not config.exclusive_time_mode:
-            n = roots
-
-        for node in n:
-            total_time += node.get_time(config.exclusive_time_mode)
+        for node in nodes:
+            total_time += node.get_time(True)
 
         return total_time
 
     @staticmethod
     def get_mean_time(nodes: List[any], config: FlowVisorConfig):
         """
         Returns the mean time.
```

### Comparing `FlowVisor-0.1.9/flowvisor/utils.py` & `FlowVisor-0.2.0/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.9/setup.py` & `FlowVisor-0.2.0/setup.py`

 * *Files identical despite different names*

