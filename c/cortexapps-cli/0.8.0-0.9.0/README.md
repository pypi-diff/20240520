# Comparing `tmp/cortexapps_cli-0.8.0.tar.gz` & `tmp/cortexapps_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortexapps_cli-0.8.0.tar", max compression
+gzip compressed data, was "cortexapps_cli-0.9.0.tar", max compression
```

## Comparing `cortexapps_cli-0.8.0.tar` & `cortexapps_cli-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-11-19 21:02:18.104396 cortexapps_cli-0.8.0/LICENSE
--rw-r--r--   0        0        0     1072 2023-11-19 21:02:18.104396 cortexapps_cli-0.8.0/README.pypi.md
--rw-r--r--   0        0        0        0 2023-11-19 21:02:18.104396 cortexapps_cli-0.8.0/cortexapps_cli/__init__.py
--rwxr-xr-x   0        0        0   138522 2023-11-19 21:02:18.104396 cortexapps_cli-0.8.0/cortexapps_cli/cortex.py
--rw-r--r--   0        0        0     1107 2023-11-19 21:02:28.824527 cortexapps_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 cortexapps_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-11-21 22:45:01.916333 cortexapps_cli-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1072 2023-11-21 22:45:01.916333 cortexapps_cli-0.9.0/README.pypi.md
+-rw-r--r--   0        0        0        0 2023-11-21 22:45:01.916333 cortexapps_cli-0.9.0/cortexapps_cli/__init__.py
+-rwxr-xr-x   0        0        0   139109 2023-11-21 22:45:01.916333 cortexapps_cli-0.9.0/cortexapps_cli/cortex.py
+-rw-r--r--   0        0        0     1107 2023-11-21 22:45:14.136423 cortexapps_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1766 1970-01-01 00:00:00.000000 cortexapps_cli-0.9.0/PKG-INFO
```

### Comparing `cortexapps_cli-0.8.0/LICENSE` & `cortexapps_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cortexapps_cli-0.8.0/README.pypi.md` & `cortexapps_cli-0.9.0/README.pypi.md`

 * *Files identical despite different names*

### Comparing `cortexapps_cli-0.8.0/cortexapps_cli/cortex.py` & `cortexapps_cli-0.9.0/cortexapps_cli/cortex.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,20 +116,31 @@
 def get_config(config, args, argv, parser, replace_string):
     check_config_file(args.config, replace_string)
 
     config_parser = configparser.ConfigParser()
     config_parser.read(args.config)
     tenant_config = config_parser[args.tenant]
     api_key = tenant_config.get('api_key')
+
+    # https://github.com/cortexapps/cli/issues/20
+    # Deal with case where user may have added key with quotes.
+    # Don't want to do a global replace in case there is a quote in the key, so
+    # only remove if found at begining or end of the string.
+    api_key = api_key.lstrip('\"')
+    api_key = api_key.rstrip('\"')
+    api_key = api_key.lstrip("\'")
+    api_key = api_key.rstrip("\'")
+
     if api_key == replace_string:
         print("Config file " + args.config + " has not been updated to include your Cortex API key.")
         print("Add your key to the file and then retry your command.")
         sys.exit(2)
     config.update({"url": tenant_config.get('base_url', 'https://api.getcortexapp.com')})
     config.update({"api_key": api_key})
+    config.update({"config_file": args.config})
 
     config.update({"debug": args.debug})
     config.update({"noObfuscate": args.noObfuscate})
 
     if args.cliAlias != None:
         key = args.tenant + '.aliases'
         argv.remove("-a")
@@ -543,15 +554,17 @@
         if config['noObfuscate'] != True:
             data['request_headers']['Authorization'] = "Bearer <OBFUSCATED>"
         json_data = json.dumps(data)
         print(json_data, file=sys.stderr)
 
 def exit(r, method, expected_rc=200):
     if r.status_code != expected_rc:
-        print(r.text)
+        sys.stderr.write(r.reason + "\n")
+        if r.status_code == 401:
+            sys.stderr.write("\nCheck your api_key in " + config['config_file'] + ".\n")
         debug_json(r, method)
         sys.exit(r.status_code)
     else:
         debug_json(r, method)
         print(r.text)
 
 def api_key(headers):
```

### Comparing `cortexapps_cli-0.8.0/pyproject.toml` & `cortexapps_cli-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cortexapps-cli"
 # version will be incremented via command line as part of github actions build
-version = "v0.8.0"
+version = "v0.9.0"
 description = "Command Line Interface for cortexapps"
 license = "MIT"
 authors = [
     "Cortex Apps <cortexapps@cortex.io>",
 ]
 readme = "README.pypi.md"
 packages = [{include = "cortexapps_cli"}]
```

### Comparing `cortexapps_cli-0.8.0/PKG-INFO` & `cortexapps_cli-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortexapps-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command Line Interface for cortexapps
 License: MIT
 Author: Cortex Apps
 Author-email: cortexapps@cortex.io
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

