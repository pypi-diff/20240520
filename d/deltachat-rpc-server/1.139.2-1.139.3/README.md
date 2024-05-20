# Comparing `tmp/deltachat-rpc-server-1.139.2.tar.gz` & `tmp/deltachat-rpc-server-1.139.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-rpc-server-1.139.2.tar", last modified: Sat May 18 21:49:22 2024, max compression
+gzip compressed data, was "deltachat-rpc-server-1.139.3.tar", last modified: Mon May 20 19:18:26 2024, max compression
```

## Comparing `deltachat-rpc-server-1.139.2.tar` & `deltachat-rpc-server-1.139.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.2/PKG-INFO
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.2/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.2/setup.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.2/src/deltachat_rpc_server/__init__.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.3/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.3/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.3/setup.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 deltachat-rpc-server-1.139.3/src/deltachat_rpc_server/__init__.py
```

### Comparing `deltachat-rpc-server-1.139.2/PKG-INFO` & `deltachat-rpc-server-1.139.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-server
-Version: 1.139.2
+Version: 1.139.3
 Summary: Delta Chat JSON-RPC server
 Description-Content-Type: text/markdown
 
 # Delta Chat RPC server
 
 This program provides a [JSON-RPC 2.0](https://www.jsonrpc.org/specification) interface to DeltaChat
 over standard I/O.
```

### Comparing `deltachat-rpc-server-1.139.2/setup.py` & `deltachat-rpc-server-1.139.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 "download",
                 "--no-input",
                 "--timeout",
                 "1000",
                 "--platform",
                 "musllinux_1_1_" + platform.machine(),
                 "--only-binary=:all:",
-                "deltachat-rpc-server==1.139.2",
+                "deltachat-rpc-server==1.139.3",
             ],
             cwd=tmpdir,
         )
 
         wheel_path = next(Path(tmpdir).glob("*.whl"))
         with ZipFile(wheel_path, "r") as wheel:
             exe_path = wheel.extract("deltachat_rpc_server/deltachat-rpc-server", "src")
```

