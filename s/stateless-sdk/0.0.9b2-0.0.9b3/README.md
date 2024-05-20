# Comparing `tmp/stateless-sdk-0.0.9b2.tar.gz` & `tmp/stateless-sdk-0.0.9b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stateless-sdk-0.0.9b2.tar", last modified: Fri Feb  2 23:16:56 2024, max compression
+gzip compressed data, was "stateless-sdk-0.0.9b3.tar", last modified: Fri Feb  2 23:31:30 2024, max compression
```

## Comparing `stateless-sdk-0.0.9b2.tar` & `stateless-sdk-0.0.9b3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:56.177936 stateless-sdk-0.0.9b2/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-02 23:16:56.177936 stateless-sdk-0.0.9b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 23:16:56.177936 stateless-sdk-0.0.9b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:56.169936 stateless-sdk-0.0.9b2/stateless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:56.173936 stateless-sdk-0.0.9b2/stateless/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:56.173936 stateless-sdk-0.0.9b2/stateless/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/offerings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/commands/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:56.173936 stateless-sdk-0.0.9b2/stateless/cli/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/offerings.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-02 23:16:48.000000 stateless-sdk-0.0.9b2/stateless/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:16:56.177936 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-02 23:16:56.000000 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-02 23:16:56.000000 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 23:16:56.000000 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-02 23:16:56.000000 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-02 23:16:56.000000 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-02 23:16:56.000000 stateless-sdk-0.0.9b2/stateless_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:30.081063 stateless-sdk-0.0.9b3/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-02 23:31:30.077063 stateless-sdk-0.0.9b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 23:31:30.081063 stateless-sdk-0.0.9b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:30.073063 stateless-sdk-0.0.9b3/stateless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:30.073063 stateless-sdk-0.0.9b3/stateless/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:30.077063 stateless-sdk-0.0.9b3/stateless/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/offerings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/commands/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:30.077063 stateless-sdk-0.0.9b3/stateless/cli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/offerings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-02 23:31:22.000000 stateless-sdk-0.0.9b3/stateless/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 23:31:30.077063 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-02 23:31:30.000000 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-02 23:31:30.000000 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 23:31:30.000000 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-02 23:31:30.000000 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-02 23:31:30.000000 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-02 23:31:30.000000 stateless-sdk-0.0.9b3/stateless_sdk.egg-info/top_level.txt
```

### Comparing `stateless-sdk-0.0.9b2/PKG-INFO` & `stateless-sdk-0.0.9b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stateless-sdk
-Version: 0.0.9b2
+Version: 0.0.9b3
 Summary: A CLI for interacting with the Stateless Gateway
 Author-email: blockjoe <joe@stateless.solutions>
 Description-Content-Type: text/markdown
 Requires-Dist: typer~=0.9.0
 Requires-Dist: pydantic~=2.4.2
 Requires-Dist: httpx~=0.24.1
 Requires-Dist: rich~=13.6.0
```

### Comparing `stateless-sdk-0.0.9b2/pyproject.toml` & `stateless-sdk-0.0.9b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stateless-sdk"
-version = "0.0.9-beta2" # Keep this in sync with __version__ in stateless/main.py
+version = "0.0.9-beta3" # Keep this in sync with __version__ in stateless/main.py
 authors = [{name = "blockjoe", email = "joe@stateless.solutions"}]
 description = "A CLI for interacting with the Stateless Gateway"
 dependencies = [
     "typer~=0.9.0",
     "pydantic~=2.4.2",
     "httpx~=0.24.1",
     "rich~=13.6.0",
```

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/api_keys.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/api_keys.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/buckets.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/buckets.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,34 +62,41 @@
         items = [
             (
                 bucket["id"],
                 bucket["name"],
                 bucket["chain"]["name"],
                 "\n".join(
                     [
-                        f"{offering['provider']['name']}"
+                        f"{offering['provider']['name']} "
+                        + " ".join(
+                            [
+                                f"{region}[{count}]"
+                                for region, count in {
+                                    entrypoint["region"]["name"]: len(
+                                        [
+                                            ep
+                                            for ep in offering["entrypoints"]
+                                            if ep["region"]["name"]
+                                            == entrypoint["region"]["name"]
+                                        ]
+                                    )
+                                    for offering in bucket["offerings"]
+                                    for entrypoint in offering["entrypoints"]
+                                }.items()
+                            ]
+                        )
                         for offering in bucket["offerings"]
                     ]
                 ),
-                "\n".join(
-                    [
-                        f"{entrypoint['region']['name']} [{len(offering['entrypoints'])}]"
-                        for offering in bucket["offerings"]
-                        for entrypoint in offering["entrypoints"]
-                    ]
-                )
-                if any(offering["entrypoints"] for offering in bucket["offerings"])
-                else "No entrypoints in this bucket",
                 f"https://api.stateless.solutions/{get_route_by_chain_id(int(bucket['chain_id']))}/v1/{bucket['id']}",
             )
             for bucket in buckets
         ]
-        BucketsManager._print_table(
-            items, ["ID", "Name", "Chain", "Offerings", "Entrypoints per Region", "URL"]
-        )
+
+        BucketsManager._print_table(items, ["ID", "Name", "Chain", "Offerings", "URL"])
 
         if len(buckets) < limit or offset + limit >= total:
             console.print("End of buckets list.")
             break
 
         navigate = inquirer.list_input(
             "Navigate pages", choices=["Next", "Previous", "Exit"], carousel=True
```

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/chains.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/chains.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/entrypoints.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/entrypoints.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/offerings.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/offerings.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/providers.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/providers.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/regions.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/regions.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/commands/users.py` & `stateless-sdk-0.0.9b3/stateless/cli/commands/users.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/accounts.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/accounts.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/api_keys.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/api_keys.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/billing.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/billing.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/buckets.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/buckets.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/chains.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/chains.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/entrypoints.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/entrypoints.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/models/offerings.py` & `stateless-sdk-0.0.9b3/stateless/cli/models/offerings.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/routes.py` & `stateless-sdk-0.0.9b3/stateless/cli/routes.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/cli/utils.py` & `stateless-sdk-0.0.9b3/stateless/cli/utils.py`

 * *Files identical despite different names*

### Comparing `stateless-sdk-0.0.9b2/stateless/main.py` & `stateless-sdk-0.0.9b3/stateless/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   / ____| |      | |     | |                / ____| |    |_   _|
  | (___ | |_ __ _| |_ ___| | ___  ___ ___  | |    | |      | |  
   \___ \| __/ _` | __/ _ \ |/ _ \/ __/ __| | |    | |      | |  
   ____) | || (_| | ||  __/ |  __/\__ \__ \ | |____| |____ _| |_ 
  |_____/ \__\__,_|\__\___|_|\___||___/___/  \_____|______|_____|                                                        
 """  # noqa: W291
 
-__version__ = "0.0.9-beta2"  # Keep this in sync with pyproject.toml
+__version__ = "0.0.9-beta3"  # Keep this in sync with pyproject.toml
 
 
 def version_callback(value: bool):
     if value:
         print(f"Stateless CLI Version: {__version__}")
         raise Exit()
```

### Comparing `stateless-sdk-0.0.9b2/stateless_sdk.egg-info/PKG-INFO` & `stateless-sdk-0.0.9b3/stateless_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stateless-sdk
-Version: 0.0.9b2
+Version: 0.0.9b3
 Summary: A CLI for interacting with the Stateless Gateway
 Author-email: blockjoe <joe@stateless.solutions>
 Description-Content-Type: text/markdown
 Requires-Dist: typer~=0.9.0
 Requires-Dist: pydantic~=2.4.2
 Requires-Dist: httpx~=0.24.1
 Requires-Dist: rich~=13.6.0
```

### Comparing `stateless-sdk-0.0.9b2/stateless_sdk.egg-info/SOURCES.txt` & `stateless-sdk-0.0.9b3/stateless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

