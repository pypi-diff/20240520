# Comparing `tmp/abeewayconfig-0.2.2.tar.gz` & `tmp/abeewayconfig-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.2.tar", last modified: Mon May 20 13:22:43 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.2.1.tar", last modified: Mon May 20 13:47:51 2024, max compression
```

## Comparing `abeewayconfig-0.2.2.tar` & `abeewayconfig-0.2.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/
--rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2/LICENSE
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1414 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1051 2024-05-16 14:51:58.000000 abeewayconfig-0.2.2/README.md
--rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/setup.cfg
--rw-r--r--   0 lucas     (1001) lucas     (1001)      753 2024-05-20 13:22:06.000000 abeewayconfig-0.2.2/setup.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/src/
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     2248 2024-05-20 13:12:46.000000 abeewayconfig-0.2.2/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     2261 2024-05-20 13:16:13.000000 abeewayconfig-0.2.2/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4788 2024-05-20 13:14:44.000000 abeewayconfig-0.2.2/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:22:43.778250 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1414 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)      434 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       12 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-20 13:22:43.000000 abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:47:51.354914 abeewayconfig-0.2.2.1/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2.1/LICENSE
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1416 2024-05-20 13:47:51.351580 abeewayconfig-0.2.2.1/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1051 2024-05-16 14:51:58.000000 abeewayconfig-0.2.2.1/README.md
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-20 13:47:51.354914 abeewayconfig-0.2.2.1/setup.cfg
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      755 2024-05-20 13:47:48.000000 abeewayconfig-0.2.2.1/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:47:51.351580 abeewayconfig-0.2.2.1/src/
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:47:51.351580 abeewayconfig-0.2.2.1/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     2248 2024-05-20 13:12:46.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     2263 2024-05-20 13:43:18.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4788 2024-05-20 13:14:44.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-20 13:47:51.351580 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1416 2024-05-20 13:47:51.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      434 2024-05-20 13:47:51.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-20 13:47:51.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-20 13:47:51.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       12 2024-05-20 13:47:51.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-20 13:47:51.000000 abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.2/LICENSE` & `abeewayconfig-0.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2/PKG-INFO` & `abeewayconfig-0.2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `abeewayconfig-0.2.2/README.md` & `abeewayconfig-0.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2/setup.py` & `abeewayconfig-0.2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.2",
+    version="0.2.2.1",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
```

### Comparing `abeewayconfig-0.2.2/src/AbeewayConfig/Config.py` & `abeewayconfig-0.2.2.1/src/AbeewayConfig/Config.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.2.1/src/AbeewayConfig/Device.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             ser.write(b'system buzzer 6\r')
             ser.close()
 
     # This doesn't actually talk to the device directly, rather it just grabs the value from a string
     # Might move it back to the main module
     def get_config_value_from_dev(config_name: str, parameter: int) -> int:
         if parameter is not None:
-            match_line = re.search(r".* %s\s*=\s*(-?\d+)" % parameter, config_name)
+            match_line = re.search(r".*\s+%s\s*=\s*(-?\d+)" % parameter, config_name)
             if match_line is not None:
                 return int(match_line.group(1))
 
     def config_show_at_device(serial_port: str, br: int) -> str:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             ser.write(b'config show\r')
```

### Comparing `abeewayconfig-0.2.2/src/AbeewayConfig/abeewayconfig.py` & `abeewayconfig-0.2.2.1/src/AbeewayConfig/abeewayconfig.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.2.1/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.2.1/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

