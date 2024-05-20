# Comparing `tmp/esp-idf-size-1.3.0.tar.gz` & `tmp/esp-idf-size-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-_1j2ui7g/esp-idf-size-1.3.0.tar", last modified: Mon Apr 15 11:27:38 2024, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-size/esp-idf-size/dist/.tmp-49074yuv/esp-idf-size-1.4.0.tar", last modified: Mon May 20 11:31:53 2024, max compression
```

## Comparing `esp-idf-size-1.3.0.tar` & `esp-idf-size-1.4.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32c61.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32h2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32h4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32p4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s3.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)    57441 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size/ng/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/format_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16584 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/mapfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    51323 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/esp_idf_size/ng/memorymap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/esp_idf_size.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:27:38.000000 esp-idf-size-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-15 11:27:28.000000 esp-idf-size-1.3.0/test/test_idf_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32c2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32c5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32c6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32c61.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32h2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32h4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32p4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32s2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32s3.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57441 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size/ng/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68603 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/format_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/format_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/format_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/format_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/format_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/mapfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61948 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/esp_idf_size/ng/memorymap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/esp_idf_size.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:31:53.000000 esp-idf-size-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 11:31:43.000000 esp-idf-size-1.4.0/test/test_idf_size.py
```

### Comparing `esp-idf-size-1.3.0/LICENSE` & `esp-idf-size-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/PKG-INFO` & `esp-idf-size-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 1.3.0
+Version: 1.4.0
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32.yaml` & `esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32p4.yaml` & `esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32p4.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s2.yaml` & `esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32s2.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/chip_info/esp32s3.yaml` & `esp-idf-size-1.4.0/esp_idf_size/chip_info/esp32s3.yaml`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/core.py` & `esp-idf-size-1.4.0/esp_idf_size/core.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/format_csv.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/format_csv.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/format_json.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/format_json.py`

 * *Files identical despite different names*

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/format_table.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/format_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     table = Table(title='Memory Type Usage Summary')
     table.add_column('Memory Type/Section', overflow='fold')
     table.add_column(r'Used \[bytes]', overflow='fold', justify='right')
     table.add_column(r'Used \[%]', overflow='fold', justify='right')
     table.add_column(r'Remain \[bytes]', overflow='fold', justify='right')
     table.add_column(r'Total \[bytes]', overflow='fold', justify='right')
 
+    memorymap.trim(memmap, args)
+
     # Extend memory types and sections for percentage and remain info
     for mem_type_name, mem_type_info in memmap['memory_types'].items():
         if mem_type_info['size']:
             mem_type_info['pct'] = mem_type_info['used'] / mem_type_info['size'] * 100
         else:
             mem_type_info['pct'] = 0
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/format_tree.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/format_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 from . import log, memorymap
 from .format_table import color_diff, color_size
 
 
 def show(memmap: Dict[str, Any], args: Namespace) -> None:
 
+    memorymap.trim(memmap, args)
     memorymap.sort(memmap, args)
+
     tree = Tree('Memory Types')
     for mem_type_name, mem_type_info in memmap['memory_types'].items():
         size = color_size(mem_type_info['size'], mem_type_info['size_diff'], args.diff)
         used = color_diff(mem_type_info['used'], mem_type_info['used_diff'], args.diff)
         mem_type_tree = tree.add(f'{mem_type_name} {used} / {size}',
                                  style='dark_orange', guide_style='dark_orange')
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/log.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
 from typing import IO, Any
 
 from rich.console import Console
 
@@ -39,16 +39,16 @@
 
 def set_console(file: IO[str]=sys.stdout, quiet: bool=False, no_color: bool=False,
                 force_terminal: bool=None, debug: bool=False) -> None:
     global console_stderr
     global console_stdout
     global debug_on
 
-    console_stderr = Console(stderr=True, quiet=quiet, no_color=no_color, force_terminal=force_terminal)
-    width = None
-    if file is not sys.stdout:
-        # https://rich.readthedocs.io/en/stable/console.html#file-output
-        # Don't limit the output to console width if it dosn't go into stdout
-        width = 10000
+    # https://rich.readthedocs.io/en/stable/console.html#file-output
+    # Don't limit the output to console width. Rich console doesn't allow to set unlimited
+    # terminal width, so set it here to large enough size, that could be considered
+    # as unlimited.
+    width = 10000
+    console_stderr = Console(stderr=True, width=width, quiet=quiet, no_color=no_color, force_terminal=force_terminal)
     console_stdout = Console(file=file, width=width, quiet=quiet, no_color=no_color, force_terminal=force_terminal)
 
     debug_on = debug
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/main.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 #!/usr/bin/env python
 
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import os
 import sys
+from typing import Any, Optional, Sequence, Union
 
 from . import (format_csv, format_json, format_raw, format_table, format_tree,
                log, memorymap)
 
 
+class ToggleAction(argparse.Action):
+    def __call__(self,
+                 parser: argparse.ArgumentParser,
+                 namespace: argparse.Namespace,
+                 values: Union[str, Sequence[Any], None],
+                 option_string: Optional[str] = None) -> None:
+        setattr(namespace, self.dest, option_string and not option_string.startswith('--no-'))
+
+
 def main() -> None:
     parser = argparse.ArgumentParser(prog='esp_idf_size.ng',
                                      description='This tool displays firmware size information for project built by ESP-IDF')
 
     parser.add_argument('input_file',
                         metavar='MAP_FILE',
                         help='Path to the link map file generated by the ESP-IDF build system.')
@@ -37,26 +47,30 @@
                         action='store_true',
                         help='Print per-file sizes.')
 
     parser.add_argument('--diff',
                         metavar='MAP_FILE',
                         help='Compare sizes with another project.')
 
-    parser.add_argument('--no-abbrev',
-                        action='store_true',
-                        help='Do not abbreviate section and file names.')
-
     parser.add_argument('--show-unused',
                         action='store_true',
                         help='Show unused memory types and sections.')
 
     parser.add_argument('--show-unchanged',
                         action='store_true',
                         help='Show unchanged items for --diff operation.')
 
+    parser.add_argument('--lto', '--no-lto',
+                        dest='use_dwarf',
+                        action=ToggleAction,
+                        nargs=0,
+                        help=('Enable or disable usage of DWARF debugging information to identify '
+                              'archives for symbols without archive. Intended to be used if LTO is enabled. '
+                              'If not specified, detect LTO usage from sdkconfig.json, if available.'))
+
     parser.add_argument('-d', '--debug',
                         action='store_true',
                         help=('Print debug information. Messages are printed to stderr.'))
 
     parser.add_argument('-o', '--output-file',
                         metavar='OUTPUT_FILE',
                         help=('Print output to the specified file instead of stdout.'))
@@ -88,36 +102,61 @@
 
     parser.add_argument('--force-terminal',
                         action='store_true',
                         default=bool(os.environ.get('ESP_IDF_SIZE_FORCE_TERMINAL')) or None,
                         help=('Enable terminal control codes even if out is not attached to terminal. '
                               'This option is ignored if used along with the "--output-file" option.'))
 
+    # mutually exclusive options
+    # --no-abbrev used along with --unify doesn't make sense, because
+    # all entries(sections, archives, ...) are using already abbreviated names
+    group = parser.add_mutually_exclusive_group()
+    group.add_argument('--no-abbrev',
+                       action='store_true',
+                       help='Do not abbreviate section and file names.')
+
+    group.add_argument('--unify',
+                       action='store_true',
+                       help=('Use abbreviated names with aggregated size information. '
+                             'For example .dram0.bss and .dram1.bss sections will be reported '
+                             'under one .bss section. Archives, object files and symbols will be '
+                             'aggregated too. This can be useful for the --diff option when '
+                             'comparing project built with different esp-idf versions.'))
+
     ofile = sys.stdout
     try:
         args = parser.parse_args()
 
         if args.output_file:
             args.force_terminal = False
             ofile = open(args.output_file, 'w')
 
         log.set_console(ofile, args.quiet, args.no_color, args.force_terminal, args.debug)
 
         args.abbrev = not args.no_abbrev
-        load_symbols = True if args.archive_details or args.format == 'raw' else False
+        load_symbols = args.archive_details or args.format == 'raw'
 
-        memmap = memorymap.get(args.input_file, load_symbols)
+        if args.use_dwarf:
+            # We need DWARF only for detailed outputs like archives
+            args.use_dwarf = any((args.archive_details, args.archives, args.files, args.format == 'raw'))
+
+        memmap = memorymap.get(args.input_file, load_symbols, args.use_dwarf)
+        if not args.show_unused:
+            memorymap.remove_unused(memmap)
         if args.diff:
-            memmap_ref = memorymap.get(args.diff, load_symbols)
+            memmap_ref = memorymap.get(args.diff, load_symbols, args.use_dwarf)
+            if not args.show_unused:
+                memorymap.remove_unused(memmap_ref)
             memmap = memorymap.diff(memmap, memmap_ref)
             if memmap['target'] != memmap['target_diff']:
                 log.warn((f'The target of the reference and other project is '
                           f'{memmap["target"]} and {memmap["target_diff"]}, respectively.'))
 
-        memorymap.trim(memmap, args)
+        if args.unify:
+            memorymap.unify(memmap)
 
         if args.format in ['table', 'text']:
             format_table.show(memmap, args)
         elif args.format == 'json2':
             format_json.show(memmap, args)
         elif args.format == 'raw':
             format_raw.show(memmap, args)
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/mapfile.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/mapfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import re
 from typing import Any, Dict, List, Tuple
 
 from . import log
 
@@ -29,15 +29,15 @@
 
         return lines
 
     def _get_memory_regions(self) -> List[Dict[str, Any]]:
         regions: List[Dict[str, Any]] = []
         found = False
         header = False
-        for ln, line in enumerate(self.lines[self.line_idx:]):
+        for ln, line in enumerate(self.lines[self.line_idx:], start=self.line_idx):
             if line.startswith('Linker script and memory map'):
                 break
 
             if not found:
                 if line.startswith('Memory Configuration'):
                     found = True
                 continue
@@ -83,15 +83,15 @@
         # For back-compatible with cmake in idf version before 5.0
         RE_TARGET_CMAKEv4x = re.compile(r'project_elf_src_(\S*)\.c.obj')
         # For back-compatible with make
         RE_TARGET_MAKE = re.compile(r'^LOAD .*?/xtensa-(esp[^-]+)-elf/')
 
         target = ''
         found = False
-        for ln, line in enumerate(self.lines[self.line_idx:]):
+        for ln, line in enumerate(self.lines[self.line_idx:], start=self.line_idx):
             if line.startswith('Cross Reference Table'):
                 # We have reached end of the "Linker script and memory map" section.
                 log.warn(f'cannot find target in linker map file')
                 break
 
             elif not found:
                 # Continue here till we find the beginning of linker scripts section.
@@ -212,15 +212,15 @@
 
         output_sections: List[Dict[str, Any]] = []
         output_section: Dict[str, Any] = {}
         input_section: Dict[str, Any] = {}
         in_output_section = False
         in_input_section = False
         found = False
-        for ln, line in enumerate(self.lines[self.line_idx:]):
+        for ln, line in enumerate(self.lines[self.line_idx:], start=self.line_idx):
             if line.startswith('Cross Reference Table'):
                 # We have reached end of the "Linker script and memory map" section.
                 break
 
             elif not found:
                 # Continue here till we find the beginning of linker scripts section.
                 if line.startswith('Linker script and memory map'):
@@ -237,21 +237,34 @@
                     in_output_section = False
                     in_input_section = False
                     output_section = {}
                     input_section = {}
 
                 elif output_section['address'] is None:
                     # Missing address and length key means that the output section info
-                    # is splitted on two lines. Fill in the missing address and length here.
+                    # is split on two lines or it's an empty output section without
+                    # address and size like
+                    # .xt.prop
+                    #  *(.xt.prop .xt.prop.* .gnu.linkonce.prop.*)
+                    # By default zero the missing address and length to handle the
+                    # empty output section.
+
+                    output_section['address'] = 0
+                    output_section['size'] = 0
+
                     splitted = line.split()
-                    if len(splitted) != 2:
-                        log.die((f'unexpected output section continuous line "{line}" at line {ln + 1} in '
-                                 f'"Linker script and memory map" section in "{self.fn}" map file'))
-                    output_section['address'] = int(splitted[0], 0)
-                    output_section['size'] = int(splitted[1], 0)
+                    if len(splitted) == 2:
+                        try:
+                            address = int(splitted[0], 0)
+                            size = int(splitted[1], 0)
+                            # Output section has address and length on the second line.
+                            output_section['address'] = address
+                            output_section['size'] = size
+                        except ValueError:
+                            pass
 
                 elif line.startswith(('.', 'COMMON')):
                     # New input section
                     in_input_section = True
                     if input_section:
                         add_input_section(output_section, input_section)
                     input_section = {
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size/ng/memorymap.py` & `esp-idf-size-1.4.0/esp_idf_size/ng/memorymap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# SPDX-FileCopyrightText: 2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2023-2024 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import copy
 import json
 import os
 from argparse import Namespace
+from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional
 
 import yaml
-from elftools.common.exceptions import ELFError
-from elftools.elf.constants import SH_FLAGS
-from elftools.elf.elffile import ELFFile
-from elftools.elf.sections import Symbol
 
 from . import log, mapfile
+from .elf import (SHF_ALLOC, SHT_PROGBITS, STT_FUNC, STT_OBJECT, Elf,
+                  Elf_Exception, Elf_Shdr, Elf_Sym)
 
 
-def get(input_fn: str, load_symbols: bool=False) -> Dict[str, Any]:
+def get(input_fn: str, load_symbols: bool=False, use_dwarf: Optional[bool]=None) -> Dict[str, Any]:
     """
     This is the main function, which returns a dictionary representing
     the whole memory map for a given project. It's converted by formatting
     functions to a requested format(table, json, cvs).
 
     Memory types are defined in chip info yaml files. These define the memory
     partitioning and all memory is divided into these memory types.
@@ -88,36 +87,50 @@
         'project_path': '',
         'project_path_diff': '',
         'memory_types': {},
     }
 
     proj_desc = elf_fn = map_fn = elf = target = None
 
-    # Try to guess project description file path based on map file.
-    proj_desc_fn = _get_project_description_fn(input_fn)
+    map_fn = os.path.abspath(input_fn)
+
+    memory_map['project_path'] = map_fn
+
+    dirname = os.path.dirname(map_fn)
 
     # Load project description if available.
-    proj_desc = _get_project_description(proj_desc_fn)
+    proj_desc_fn = os.path.join(dirname, 'project_description.json')
+    proj_desc = _load_json_file(proj_desc_fn)
+
+    if use_dwarf is None:
+        # DWARF usage is not explicitly set, try to look into sdkconfig
+        # if LTO was enabled.
+        sdkconfig_fn = os.path.join(dirname, 'config', 'sdkconfig.json')
+        sdkconfig = _load_json_file(sdkconfig_fn)
+        if sdkconfig is not None:
+            use_dwarf = sdkconfig.get('COMPILER_LTO_LINKTIME', False)
+        else:
+            use_dwarf = False
 
     if proj_desc:
-        memory_map['project_path'] = proj_desc['project_path']
         target = proj_desc['target']
-        elf_fn = os.path.join(proj_desc['build_dir'], proj_desc['app_elf'])
-        map_fn = os.path.join(proj_desc['build_dir'], proj_desc['project_name'] + '.map')
-    else:
-        map_fn = input_fn
+        elf_fn = os.path.join(dirname, proj_desc['app_elf'])
 
     if elf_fn and os.path.isfile(elf_fn):
         elf = _load_elf_file(elf_fn)
     else:
         log.debug(f'elf file is not available')
 
     # Parse linker map file memory regions, target and output sections
     map_file = mapfile.MapFile(map_fn)
 
+    if use_dwarf:
+        # Try to expand input sections without archive based on DWARF info.
+        _expand_input_sections(map_file, proj_desc, elf)
+
     if not target:
         # Target from project_description.json is not available, use target detected in map file.
         target = map_file.target
 
     if not target:
         log.die(f'cannot determine chip target')
 
@@ -151,15 +164,15 @@
         for osec in map_sections_filtered:
             for isec in osec['input_sections']:
                 isec['symbols'] = []
 
     # Split output sections according to splitted memory regions
     map_sections_splitted = _split_map_sections(map_sections_filtered, memory_regions_splitted)
 
-    # Add archives info into sections. Archives contain objects and objects contains symbols.
+    # Add archives info into sections. Archives contain objects and objects contain symbols.
     _add_archives_to_sections(map_sections_splitted)
 
     # Generate the overall memory map representation
     memory_map['memory_types'] = _get_mem_type_map(memory_types, memory_regions_splitted, map_sections_splitted)
 
     log.debug(f'memory map', memory_map)
 
@@ -279,14 +292,70 @@
                             symbol_info_diff['size'] = 0
                             symbol_info_diff['size_diff'] = 0 - symbol_info_ref['size']
 
     log.debug(f'memory map diff', memory_map_diff)
     return memory_map_diff
 
 
+def unify(memory_map: Dict[str, Any]) -> None:
+    """
+    Aggregate size information based on the abbreviated names.
+    For example .dram0.bss and .dram1.bss sections will be reported
+    under one .bss section. Archives, object files and symbols will be
+    aggregated too. This can be useful for the --diff option when
+    comparing project built with different esp-idf versions.
+    """
+
+    # Level nodes in the memory map have different children key identifier.
+    # This maps each level to sublevel name.
+    level_map: Dict[str, Optional[str]] = {
+        'sections': 'archives',
+        'archives': 'object_files',
+        'object_files': 'symbols',
+        'symbols': None,  # Leaf node, no children
+    }
+
+    def unify_items(original: Dict[str, Any], unified: Dict[str, Any], level: str) -> None:
+        # Generic function which unifies all memory map levels
+        for original_item_name, original_item_info in original.items():
+            original_item_name_abbrev = original_item_info['abbrev_name']
+            sublevel = level_map[level]
+            unified_item_info = unified.get(original_item_name_abbrev)
+            if unified_item_info is None:
+                unified_item_info = {
+                    'abbrev_name': original_item_info['abbrev_name'],
+                    'size': original_item_info['size'],
+                    'size_diff': original_item_info['size_diff'],
+                    sublevel: {},
+                }
+                unified[original_item_name_abbrev] = unified_item_info
+            else:
+                unified_item_info['size'] += original_item_info['size']
+                unified_item_info['size_diff'] += original_item_info['size_diff']
+
+            if sublevel is None:
+                # We reached the leaf(symbols) node
+                continue
+            # Unify children nodes
+            unify_items(original_item_info[sublevel], unified_item_info[sublevel], sublevel)
+
+    # Create copy of memory_types without sections, which will be filled
+    # with aggregated size information.
+    memory_types_unified: Dict[str, Any] = {k: copy.copy(v) for k, v in memory_map['memory_types'].items()}
+    for mem_type_unified_info in memory_types_unified.values():
+        mem_type_unified_info['sections'] = {}
+
+    # Go through sections, archives, object files and symbols and aggregate
+    # them based on the abbreviated name.
+    for mem_type_name, mem_type_info in memory_map['memory_types'].items():
+        unify_items(mem_type_info['sections'], memory_types_unified[mem_type_name]['sections'], 'sections')
+
+    memory_map['memory_types'] = memory_types_unified
+
+
 def walk(memory_map: Dict[str, Any], depth: str='all') -> Generator:
     """Generator which yields tuple for memory type tree entries."""
     for mem_type_name, mem_type_info in memory_map['memory_types'].items():
         if depth == 'types':
             yield (mem_type_name, mem_type_info,
                    None, None,
                    None, None,
@@ -321,19 +390,29 @@
                         yield (mem_type_name, mem_type_info,
                                section_name, section_info,
                                archive_name, archive_info,
                                object_file_name, object_file_info,
                                symbol_name, symbol_info)
 
 
+def remove_unused(memory_map: Dict[str, Any]) -> None:
+    # Remove memory types which are not used
+    memory_map['memory_types'] = {k: v for k, v in memory_map['memory_types'].items() if v['used']}
+
+    # Remove sections, which do not have any archive. For example .iram0.text_end is defined
+    # to mark the end of IRAM code segment and contains just an alignment.
+    for mem_type_name, mem_type_info in memory_map['memory_types'].items():
+        mem_type_info['sections'] = {k: v for k, v in mem_type_info['sections'].items() if v['archives']}
+
+
 def trim(memory_map: Dict[str, Any], args: Namespace) -> None:
-    """Trim the memory map tree based on command line arguments. This removes
-    unused memory types and sections and trims the dept of the tree if e.g.
-    --archives is specified. It also removes all entries for the diff command if
-    they were not changed."""
+    """Trim the memory map tree based on command line arguments. This trims the
+    dept of the tree if e.g. --archives is specified. It also removes all entries
+    for the diff command if they were not changed."""
+
     def changed(diff: int) -> bool:
         if not args.diff or args.show_unchanged:
             return True
         return True if diff else False
 
     ARCHIVE_DETAILS, ARCHIVES, OBJECTS, ALL = range(4)
 
@@ -342,27 +421,18 @@
     elif args.archives:
         depth = ARCHIVES
     elif args.files:
         depth = OBJECTS
     else:
         depth = ALL
 
-    if not args.show_unused:
-        memory_map['memory_types'] = {k: v for k, v in memory_map['memory_types'].items()
-                                      if v['used'] + abs(v['used_diff'])}
-
     memory_map['memory_types'] = {k: v for k, v in memory_map['memory_types'].items()
                                   if changed(v['used_diff'])}
 
     for mem_type_name, mem_type_info in memory_map['memory_types'].items():
-        if not args.show_unused:
-            # Remove sections, which do not have any archive. For example .iram0.text_end is defined
-            # to mark the end of IRAM code segment and contains just an alignment.
-            mem_type_info['sections'] = {k: v for k, v in mem_type_info['sections'].items()
-                                         if v['archives']}
         mem_type_info['sections'] = {k: v for k, v in mem_type_info['sections'].items()
                                      if changed(v['size_diff'])}
 
         for section_name, section_info in mem_type_info['sections'].items():
             if depth == ARCHIVE_DETAILS:
                 section_info['archives'] = {k: v for k, v in section_info['archives'].items()
                                             if v['abbrev_name'] == args.archive_details and
@@ -445,14 +515,22 @@
 
         for mem_type_name, mem_type_info in entry_info['memory_types'].items():
             mem_type_info['sections'] = sort_dict_by_key(mem_type_info['sections'], sort_key, reverse)
 
     return entries
 
 
+def rem_summary_unchanged(entries: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
+    if not args.diff or args.show_unchanged:
+        return entries
+
+    entries = {k: v for k, v in entries.items() if v['size_diff']}
+    return entries
+
+
 def get_symbols_summary(memory_map: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
     symbols: Dict[str, Any] = {}
 
     mem_types = _get_summary_memory_types(memory_map)
     found = False
 
     for (mem_type_name, mem_type_info,
@@ -463,14 +541,16 @@
 
         if archive_info['abbrev_name'] != args.archive_details:
             continue
 
         found = True
 
         symbol_name_full = ':'.join([archive_name, object_file_name, symbol_name])
+        if args.unify:
+            symbol_name_full = symbol_info['abbrev_name']
         if symbol_name_full not in symbols:
             symbol: Dict[str, Any] = {
                 'abbrev_name': symbol_name,
                 'size': 0,
                 'size_diff': 0,
                 'memory_types': copy.deepcopy(mem_types),
             }
@@ -488,29 +568,31 @@
         symbol_mem_type['sections'][section_name]['size_diff'] = size
         symbol_mem_type['size_diff'] += size
         symbol['size_diff'] += size
 
     if not found:
         log.die(f'Archive "{args.archive_details}" not found.')
 
-    return symbols
+    return rem_summary_unchanged(symbols, args)
 
 
 def get_object_files_summary(memory_map: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
     object_files: Dict[str, Any] = {}
 
     mem_types = _get_summary_memory_types(memory_map)
 
     for (mem_type_name, mem_type_info,
          section_name, section_info,
          archive_name, archive_info,
          object_file_name, object_file_info,
          _, _) in walk(memory_map, depth='objects'):
 
         object_file_name_full = ':'.join([archive_name, object_file_name])
+        if args.unify:
+            object_file_name_full = object_file_info['abbrev_name']
         if object_file_name_full not in object_files:
             object_file: Dict[str, Any] = {
                 'abbrev_name': os.path.basename(object_file_name),
                 'size': 0,
                 'size_diff': 0,
                 'memory_types': copy.deepcopy(mem_types),
             }
@@ -525,15 +607,15 @@
         object_file['size'] += size
 
         size = object_file_info['size_diff']
         object_file_mem_type['sections'][section_name]['size_diff'] = size
         object_file_mem_type['size_diff'] += size
         object_file['size_diff'] += size
 
-    return object_files
+    return rem_summary_unchanged(object_files, args)
 
 
 def get_archives_summary(memory_map: Dict[str, Any], args: Namespace) -> Dict[str, Any]:
     archives: Dict[str, Any] = {}
 
     mem_types = _get_summary_memory_types(memory_map)
 
@@ -561,15 +643,15 @@
         archive['size'] += size
 
         size = archive_info['size_diff']
         archive_mem_type['sections'][section_name]['size_diff'] = size
         archive_mem_type['size_diff'] += size
         archive['size_diff'] += size
 
-    return archives
+    return rem_summary_unchanged(archives, args)
 
 
 def _filter_memory_regions(memory_regions: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
     memory_regions_filtered: List[Dict[str, Any]] = []
 
     for mem_reg in memory_regions:
         if mem_reg['name'] == '*default*':
@@ -638,15 +720,15 @@
             if not mem_reg_length:
                 break
 
     log.debug(f'memory regions splitted', memory_regions_splitted)
     return memory_regions_splitted
 
 
-def _filter_map_sections(sections: List[Dict[str, Any]], elf_sections: Optional[Dict[str, Any]]) -> List[Dict[str, Any]]:
+def _filter_map_sections(sections: List[Dict[str, Any]], elf_sections: Optional[Dict[str, Elf_Shdr]]) -> List[Dict[str, Any]]:
     sections_filtered: List[Dict[str, Any]] = []
     for section in sections:
         if not section['size']:
             # Remove empty sections.
             continue
 
         if section['name'].endswith(('dummy', 'reserved_for_iram')):
@@ -778,70 +860,53 @@
 
 
 def _abbrev(section_name: str) -> str:
     splitted = section_name.split('.')
     return f'.{splitted[-1]}'
 
 
-def _get_project_description_fn(fn: str) -> str:
-    dirname = os.path.dirname(fn)
-    fn = os.path.join(dirname, 'project_description.json')
-    return fn
-
-
-def _get_project_description(fn: str) -> Optional[Dict[str, Any]]:
-    proj_desc = None
+def _load_json_file(fn: str) -> Optional[Dict[str, Any]]:
+    data = None
     try:
         with open(fn, 'r') as f:
-            proj_desc = json.load(f)
+            data = json.load(f)
     except (OSError, ValueError) as e:
-        log.debug(f'project_description.json is not available: {e}')
+        log.debug(f'{fn} is not available: {e}')
 
-    log.debug('project_description.json', proj_desc)
-    return proj_desc
+    return data
 
 
-def _load_elf_file(fn: str) -> Optional[ELFFile]:
+def _load_elf_file(fn: str) -> Optional[Elf]:
     try:
-        elf = ELFFile.load_from_path(fn)
+        elf = Elf(fn)
     except (OSError, ValueError) as e:
         log.die(f'cannot read project ELF file: {e}')
-    except ELFError as e:
+    except Elf_Exception as e:
         log.die(f'cannot parse ELF file sections: {e}')
 
     log.debug(f'elf file {fn}')
     return elf
 
 
-def _add_symbols_to_sections(elf: Optional[ELFFile], osections: List[Dict[str, Any]]) -> None:
+def _add_symbols_to_sections(elf: Optional[Elf], osections: List[Dict[str, Any]]) -> None:
     if not elf:
         # ELF is not available. Use input section names as symbols.
         for osec in osections:
             for isec in osec['input_sections']:
                 isec['symbols'] = [{
                     'name': isec['name'],
                     'address': isec['address'],
                     'size': isec['size'],
                 }]
         return
 
     # Get dictionary of symbols from ELF for STT_FUNC and STT_OBJECT and sort it based
     # on symbol address.
-    symbols: List[Symbol] = []
-    for section in elf.iter_sections():
-        if section.header['sh_type'] != 'SHT_SYMTAB':
-            continue
-        symtab = elf.get_section_by_name(section.name)
-        for symbol in symtab.iter_symbols():
-            if symbol['st_info']['type'] not in ['STT_FUNC', 'STT_OBJECT'] or not symbol['st_size']:
-                # Skip uninteresting symbols
-                continue
-            symbols.append(symbol)
-
-    symbols = [s for s in sorted(symbols, key=lambda s: s['st_value'] or 0)]  # or 0 help mypy
+    symbols: List[Elf_Sym] = [s for s in sorted(elf.symbols, key=lambda s: s.st_value or 0)
+                              if s.type in (STT_FUNC, STT_OBJECT) and s.st_size]  # or 0 help mypy
 
     # Get list of input sections, sorted by address, and add symbols list to each
     # input section.
     isections: List[Dict[str, Any]] = []
     for osec in osections:
         for isec in osec['input_sections']:
             isec['symbols'] = []
@@ -849,16 +914,16 @@
 
     isections = [s for s in sorted(isections, key=lambda s: s.get('address', 0))]  # s.get used to help mypy
 
     # Add ELF symbols into input sections
     isec = isections.pop(0)
     for symbol in symbols:
         sym_name = symbol.name
-        sym_addr = symbol['st_value']
-        sym_size = symbol['st_size']
+        sym_addr = symbol.st_value
+        sym_size = symbol.st_size
         while sym_addr >= isec['address'] + isec['size']:
             if not isections:
                 # Sanity check that we found input section for symbol
                 log.die(f'cannot find input section for symbol {sym_name}({sym_addr})')
 
             if not isec['symbols']:
                 # Input section does not have any ELF symbols assigned.
@@ -889,62 +954,61 @@
 
         if sym_addr < isec['address']:
             # Symbol is not part of the current input section. It must be
             # ROM mappend symbol.
             continue
 
         # Append '()' to function symbol
-        if symbol['st_info']['type'] == 'STT_FUNC':
+        if symbol.type == STT_FUNC:
             sym_name += '()'
 
         isec['symbols'].append({
             'name': sym_name,
             'address': sym_addr,
             'size': sym_size,
         })
 
     log.debug(f'linker map output sections filtered with symbols', osections)
 
 
-def _get_elf_sections_headers(elf: Optional[ELFFile]) -> Optional[Dict[str, Any]]:
+def _get_elf_sections_headers(elf: Optional[Elf]) -> Optional[Dict[str, Elf_Shdr]]:
     if not elf:
         return None
 
-    hdrs: Dict[str, Any] = {}
-    sections_headers = {s.name: dict(s.header) for s in elf.iter_sections()}
+    hdrs: Dict[str, Elf_Shdr] = {}
 
-    for name, info in sections_headers.items():
-        if info['sh_size'] == 0:
+    for shdr in elf.shdrs:
+        if shdr.sh_size == 0:
             # Section has zero memory size, so skip it
             continue
-        if not info['sh_flags'] & SH_FLAGS.SHF_ALLOC:
+        if not shdr.sh_flags & SHF_ALLOC:
             # Section doesn't occupy memory during app execution, so skip it
             continue
-        hdrs[name] = info
+        hdrs[shdr.name] = shdr
 
-    log.debug('elf section headers', hdrs)
+    log.debug('elf section headers', hdrs.keys())
 
     return hdrs
 
 
-def _get_image_size(elf_sections: Optional[Dict[str, Any]], sections: List[Dict[str, Any]]) -> int:
+def _get_image_size(elf_sections: Optional[Dict[str, Elf_Shdr]], sections: List[Dict[str, Any]]) -> int:
     size = 0
     if not elf_sections:
         # ELF information not available
         for sec in sections:
             # NOLOAD(SHT_NOBITS) sections are not part of the image
             if sec['name'].endswith(('.bss', 'noinit')):
                 continue
             size += sec['size']
         return size
 
     for name, info in elf_sections.items():
-        if info['sh_type'] != 'SHT_PROGBITS':
+        if info.sh_type != SHT_PROGBITS:
             continue
-        size += info['sh_size']
+        size += info.sh_size
 
     return size
 
 
 def _add_archives_to_sections(sections: List[Dict[str, Any]]) -> None:
     for section in sections:
         archives: Dict[str, Any] = {}
@@ -986,14 +1050,164 @@
 
         section['abbrev_name'] = _abbrev(section['name'])
         section['archives'] = archives
 
     log.debug('sections with archives', sections)
 
 
+def _expand_input_sections(map_file: mapfile.MapFile, proj_desc: Optional[Dict[str, Any]], elf: Optional[Elf]) -> None:
+    # Based on information in .debug_info section, try to find components for input sections without
+    # archive. These are generated when object file is directly linked or when LTO is used. With LTO enabled,
+    # object files from several archives may be merged into one artificial object file, which is used by compiler
+    # for optimization. Meaning linker has no information about archives and hence this info is also missing in
+    # the link map file. Instead the link map file contains artificially created object file by compiler.
+    if proj_desc is None:
+        log.warn('ignoring DWARF information because project description information is not available')
+        return
+    if elf is None:
+        log.warn('ignoring DWARF information because ELF file is not available')
+        return
+
+    def find_symbol_component(sym: Elf_Sym, components: List[Dict[str, Any]]) -> Optional[Dict[str, Any]]:
+        # Find component to which the symbol belongs to
+        for component in components:
+            # NOTE: Elf_Sym is dynamically extended with cu_path and archive_path attribute and mypy doesn't like it
+            if sym.cu_path.startswith(component['component_path']):  # type: ignore
+                # The components list is sorted based on component_path length, from longest to shortest.
+                # The longest possible match was found, so return. There is no need to search further.
+                return component
+
+        return None
+
+    def add_archives_to_symbols(symbols: Dict[int, Elf_Sym], components: List[Dict[str, Any]]) -> None:
+        # Based on CU path and information in project_description.json try to assign
+        # each symbol into archive. Symbols without CU info were already removed from
+        # the list.
+        for sym in symbols.values():
+            component = find_symbol_component(sym, components)
+            if component is None:
+                continue
+
+            # Add archive to symbol
+            sym.archive_path = component['archive_relpath']  # type: ignore
+
+    # Get symbols with CU name info if available
+    symbols: Dict[int, Elf_Sym] = elf.add_cus_to_symbols()
+
+    # Remove symbols with zero size and symbols for which we don't have CU name
+    symbols = {k: v for k, v in symbols.items() if v.st_size and v.cu_name}
+
+    # Get list of components with archive file, removing CONFIG_ONLY components
+    components = [comp for comp in proj_desc['build_component_info'].values() if comp['file']]
+
+    # Add component_path and relative, to build directory, archive path to components in posix form
+    build_dir_path = Path(proj_desc['build_dir']).as_posix()
+    for comp in components:
+        comp['component_path'] = Path(comp['dir']).as_posix()
+        comp['archive_relpath'] = Path(comp['file']).relative_to(build_dir_path).as_posix()
+
+    # Sort components in descending order based on their paths, from longest to shortest.
+    components = [comp for comp in sorted(components, key=lambda c: len(c['component_path']), reverse=True)]
+
+    # Add CU path to symbols posix form
+    for sym in symbols.values():
+        sym.cu_path = Path(str(sym.cu_name)).as_posix()  # type: ignore
+
+    # Add 'archive_path' attribute to each symbol if available.
+    # The native path form created in the two steps above are used
+    # to quickly find if symbol's CU is within component's directory.
+    add_archives_to_symbols(symbols, components)
+
+    # Remove symbols without archive information
+    symbols = {k: v for k, v in symbols.items() if hasattr(v, 'archive_path')}
+
+    # Sort symbols based on their addresses
+    symbols = {k: v for k, v in sorted(symbols.items(), key=lambda item: item[0])}
+
+    for osec in map_file.sections:
+        isecs_new: List[Dict[str, Any]] = []
+        for isec in osec['input_sections']:
+            if isec['archive'] != '(exe)':
+                # We have proper archive info, so just use the input section as is
+                isecs_new.append(isec)
+                continue
+            # Go through symbols, for which we have CU names, and create new input
+            # sections.
+            for addr, sym in symbols.items():
+                if addr < isec['address']:
+                    # Symbol is not part of this input section
+                    continue
+                elif addr == isec['address'] and isec['size']:
+                    # Symbol starts at the same address as input section.
+                    # Create new input section covered by the symbol, insert it
+                    # into isecs_new and adjust isec address and size.
+                    # Do this only if there is some size left, because
+                    # previous symbol may have covered the rest of the input section.
+                    isec_new = {
+                        'name': sym.name,
+                        'address': sym.st_value,
+                        'size': sym.st_size,
+                        'archive': sym.archive_path,  # type: ignore
+                        'object_file': Path(str(sym.cu_name)).name,
+                        'fill': 0,
+                    }
+                    isecs_new.append(isec_new)
+                    isec['address'] += sym.st_size
+                    isec['size'] -= sym.st_size
+
+                elif addr < isec['address'] + isec['size']:
+                    # There is a gap between isec address and symbol address, for which
+                    # we have no symbol with CU info. Create copy of the original
+                    # isec with reduced size and keep it in the artificial '(exe)' archive.
+                    # The gap may be because of align, maybe we can account it into previous
+                    # symbol if it doesn't cross some threshold?
+                    isec_new = {
+                        'name': isec['name'],
+                        'address': isec['address'],
+                        'size': sym.st_value - isec['address'],
+                        'archive': '(exe)',
+                        'object_file': isec['object_file'],
+                        'fill': 0,
+                    }
+                    isecs_new.append(isec_new)
+                    isec['address'] += isec_new['size']
+                    isec['size'] -= isec_new['size']
+
+                    # Now add new isec for symbol as if it would have the same
+                    # address as input section.
+                    isec_new = {
+                        'name': sym.name,
+                        'address': sym.st_value,
+                        'size': sym.st_size,
+                        'archive': sym.archive_path,  # type: ignore
+                        'object_file': Path(str(sym.cu_name)).name,
+                        'fill': 0,
+                    }
+                    isecs_new.append(isec_new)
+                    isec['address'] += sym.st_size
+                    isec['size'] -= sym.st_size
+                else:
+                    # No other symbols fit into this input section
+                    if isec['size'] or not isecs_new:
+                        # There is some part(tail) of the original input section, which
+                        # was not covered by any symbol. Or no symbol fits into this
+                        # input section at all and isecs_new is empty.
+                        isecs_new.append(isec)
+                    else:
+                        # Whole input section was covered by symbols. If it had filling,
+                        # account it into the lastly added input section.
+                        isecs_new[-1]['fill'] = isec['fill']
+                    break
+
+        # Finally assign expanded input sections into the output section
+        osec['input_sections'] = isecs_new
+
+    log.debug(f'linker map output sections expanded', map_file.sections)
+
+
 def _get_memory_types(target: str) -> Dict[str, Any]:
     # Load memory types from yml file
     memory_types: Dict[str, Any] = {}
     try:
         directory = os.path.dirname(__file__)
         fn = os.path.join(directory, '..', 'chip_info', target + '.yaml')
         with open(fn, 'r') as f:
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size.egg-info/PKG-INFO` & `esp-idf-size-1.4.0/esp_idf_size.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-size
-Version: 1.3.0
+Version: 1.4.0
 Summary: Firmware size analysis for ESP-IDF
 Home-page: https://github.com/espressif/esp-idf-size
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,project,size
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-size-1.3.0/esp_idf_size.egg-info/SOURCES.txt` & `esp-idf-size-1.4.0/esp_idf_size.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 esp_idf_size/chip_info/esp32h2.yaml
 esp_idf_size/chip_info/esp32h4.yaml
 esp_idf_size/chip_info/esp32p4.yaml
 esp_idf_size/chip_info/esp32s2.yaml
 esp_idf_size/chip_info/esp32s3.yaml
 esp_idf_size/ng/__init__.py
 esp_idf_size/ng/__main__.py
+esp_idf_size/ng/elf.py
 esp_idf_size/ng/format_csv.py
 esp_idf_size/ng/format_json.py
 esp_idf_size/ng/format_raw.py
 esp_idf_size/ng/format_table.py
 esp_idf_size/ng/format_tree.py
 esp_idf_size/ng/log.py
 esp_idf_size/ng/main.py
```

### Comparing `esp-idf-size-1.3.0/setup.py` & `esp-idf-size-1.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: 2024 Espressif Systems (Shanghai) CO LTD
+# SPDX-License-Identifier: Apache-2.0
 import os.path
 
 from setuptools import find_packages, setup
 
 
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
@@ -33,16 +35,15 @@
     long_description_content_type='text/markdown',
     long_description=get_long_description(),
     url='https://github.com/espressif/esp-idf-size',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'pyyaml',
-        'rich',
-        'pyelftools'],
+        'rich'],
     extras_require={
         'dev': [
             'pre-commit',
             'coverage',
             'jsonschema',
             'pytest',
             'commitizen',
```

### Comparing `esp-idf-size-1.3.0/test/test_idf_size.py` & `esp-idf-size-1.4.0/test/test_idf_size.py`

 * *Files identical despite different names*

