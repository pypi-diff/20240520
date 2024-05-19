# Comparing `tmp/iudex-0.5.5.tar.gz` & `tmp/iudex-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.5.5.tar", max compression
+gzip compressed data, was "iudex-0.6.0.tar", max compression
```

## Comparing `iudex-0.5.5.tar` & `iudex-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.5.5/LICENSE
--rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.5.5/README.md
--rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.5.5/iudex/__init__.py
--rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.5.5/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-17 01:17:53.127532 iudex-0.5.5/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.5.5/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1974 2024-05-14 23:55:03.479780 iudex-0.5.5/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     6043 2024-05-17 01:33:17.021670 iudex-0.5.5/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.5.5/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      608 2024-05-17 03:32:49.547700 iudex-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 iudex-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 21:03:01.210390 iudex-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-17 01:14:03.519309 iudex-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 01:39:19.649489 iudex-0.6.0/iudex/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-14 23:55:03.479188 iudex-0.6.0/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-19 23:25:11.000000 iudex-0.6.0/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 20:15:13.224407 iudex-0.6.0/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     2218 2024-05-19 23:24:45.000000 iudex-0.6.0/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     7874 2024-05-19 23:21:04.000000 iudex-0.6.0/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1517 2024-05-17 01:41:47.528945 iudex-0.6.0/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      608 2024-05-19 23:25:20.000000 iudex-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 iudex-0.6.0/PKG-INFO
```

### Comparing `iudex-0.5.5/LICENSE` & `iudex-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.5.5/README.md` & `iudex-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.5.5/iudex/instrumentation/README.md` & `iudex-0.6.0/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.5.5/iudex/instrumentation/attributes.py` & `iudex-0.6.0/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.5.5/iudex/instrumentation/fastapi.py` & `iudex-0.6.0/iudex/instrumentation/lambda.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 from typing import Optional, Union
 
-from fastapi import FastAPI
-from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
-
 from .instrumentation import _IudexConfig, IudexConfig
 
 
 def instrument(
-    app: FastAPI,
     service_name: Optional[str] = None,
     instance_id: Optional[str] = None,
     iudex_api_key: Optional[str] = None,
     log_level: Optional[Union[int, str]] = None,
     git_commit: Optional[str] = None,
     github_url: Optional[str] = None,
     env: Optional[str] = None,
     config: Optional[IudexConfig] = None,
 ):
-    """Auto-instruments FastAPI app to send OTel signals to Iudex.
-
-    Invoke this function in your FastAPI entrypoint.
+    """Auto-instruments app to send OTel signals to Iudex.
 
-    If you use Gunicorn, invoke it within a post_fork hook:
-    ```python
-    def post_fork(server, worker):
-        instrument(...)
-    ```
-    Per https://opentelemetry-python.readthedocs.io/en/latest/examples/fork-process-model/README.html.
+    Invoke this function in your Lambda entrypoint.
 
     Args:
-        app: FastAPI app to instrument.
         service_name: Name of the service, e.g. "billing_service", __name__.
             If not supplied, env var OTEL_SERVICE_NAME will be used.
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
         log_level: Logging level for the root logger.
         config: IudexConfig object with more granular options.
@@ -49,10 +37,9 @@
         "git_commit": git_commit,
         "github_url": github_url,
         "env": env,
     }
     iudex_config = _IudexConfig(**config)
 
     iudex_config.configure()
-    FastAPIInstrumentor().instrument_app(app)
 
     return iudex_config
```

### Comparing `iudex-0.5.5/iudex/instrumentation/instrumentation.py` & `iudex-0.6.0/iudex/instrumentation/instrumentation.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,41 +35,45 @@
     "CRITICAL": logging.CRITICAL,
     "NOTSET": logging.NOTSET,
 }
 DEFAULT_LOG_LEVEL = logging.INFO
 
 IUDEX_CONFIGURED = False
 
+
 class IudexConfig(TypedDict, total=False):
     iudex_api_key: Optional[str]
     service_name: Optional[str]
     instance_id: Optional[str]
     logs_endpoint: Optional[str]
     traces_endpoint: Optional[str]
     log_level: Optional[Union[str, int]]
     git_commit: Optional[str]
     github_url: Optional[str]
     env: Optional[str]
     attributes: Optional[Attributes]
 
-class _IudexConfig():
+
+class _IudexConfig:
     def __init__(
         self,
         **kwargs,
     ):
         self.iudex_api_key = kwargs["iudex_api_key"] or os.getenv("IUDEX_API_KEY")
         if not self.iudex_api_key:
             _logger.warning(
                 "Missing API key, no telemetry will be sent to Iudex. "
                 + "Provide the iudex_api_key parameter or set the IUDEX_API_KEY environment variable."
             )
             return
 
         self.service_name = (
-            kwargs["service_name"] or os.getenv(OTEL_SERVICE_NAME) or DEFAULT_SERVICE_NAME
+            kwargs["service_name"]
+            or os.getenv(OTEL_SERVICE_NAME)
+            or DEFAULT_SERVICE_NAME
         )
         self.instance_id = kwargs["instance_id"]
 
         self.logs_endpoint = (
             kwargs["logs_endpoint"]
             or os.getenv(OTEL_EXPORTER_OTLP_LOGS_ENDPOINT)
             or DEFAULT_IUDEX_LOGS_ENDPOINT
@@ -85,20 +89,22 @@
         if isinstance(log_level, str):
             log_level = LOG_LEVEL_ATOI.get(log_level.upper())
         self.log_level = log_level or DEFAULT_LOG_LEVEL
 
         self.git_commit = kwargs["git_commit"] or os.getenv("GIT_COMMIT")
         if not self.git_commit:
             try:
-                self.git_commit = subprocess.check_output(['git', 'rev-parse', 'HEAD']).strip()
+                self.git_commit = subprocess.check_output(
+                    ["git", "rev-parse", "HEAD"]
+                ).strip()
             except:
                 pass
 
         self.github_url = kwargs["github_url"] or os.getenv("GITHUB_URL")
-        
+
         self.env = kwargs["env"] or os.getenv("ENV") or os.getenv("ENVIRONMENT")
 
         self.attributes = kwargs.get("attributes", {})
 
     def configure(self):
         if not self.iudex_api_key:
             _logger.warning(
@@ -115,15 +121,17 @@
         attributes = {}
         attributes["service.name"] = self.service_name
         attributes["service.instance.id"] = self.instance_id
         attributes["git.commit"] = self.git_commit
         attributes["github.url"] = self.github_url
         attributes["env"] = self.env
         # clean attributes
-        attributes = {key: value for key, value in attributes.items() if value is not None}
+        attributes = {
+            key: value for key, value in attributes.items() if value is not None
+        }
 
         # add manual attributes
         attributes.update(self.attributes)
 
         # create resource
         resource = Resource.create(attributes)
 
@@ -145,14 +153,61 @@
         span_exporter = OTLPSpanExporter(endpoint=self.traces_endpoint, headers=headers)
         trace_provider.add_span_processor(BatchSpanProcessor(span_exporter))
         set_tracer_provider(trace_provider)
 
         IUDEX_CONFIGURED = True
 
 
+def instrument(
+    service_name: Optional[str] = None,
+    instance_id: Optional[str] = None,
+    iudex_api_key: Optional[str] = None,
+    log_level: Optional[Union[int, str]] = None,
+    git_commit: Optional[str] = None,
+    github_url: Optional[str] = None,
+    env: Optional[str] = None,
+    config: Optional[IudexConfig] = None,
+):
+    """Auto-instruments app to send OTel signals to Iudex.
+
+    Invoke this function in your Lambda entrypoint.
+
+    Args:
+        service_name: Name of the service, e.g. "billing_service", __name__.
+            If not supplied, env var OTEL_SERVICE_NAME will be used.
+        instance_id: ID of the service instance, e.g. container id, pod name.
+        iudex_api_key: Your Iudex API key.
+            If not supplied, env var IUDEX_API_KEY will be used.
+        log_level: Logging level for the root logger.
+        git_commit: Commit hash of the currently deployed code.
+            Used with github_url to deep link telemetry to source code.
+        github_url: URL of the GitHub repository.
+            Used with git_commit to deep link telemetry to source code.
+        env: Environment of the service, e.g. "production", "staging".
+        config: IudexConfig object with more granular options.
+            Will override all other args, so provide them to the object instead.
+    """
+    config = config or {
+        "iudex_api_key": iudex_api_key,
+        "service_name": service_name,
+        "instance_id": instance_id,
+        "logs_endpoint": None,
+        "traces_endpoint": None,
+        "log_level": log_level,
+        "git_commit": git_commit,
+        "github_url": github_url,
+        "env": env,
+    }
+    iudex_config = _IudexConfig(**config)
+
+    iudex_config.configure()
+
+    return iudex_config
+
+
 def configure_logger(
     logger_name: Optional[str] = None,
     log_level: Optional[Union[str, int]] = None,
 ):
     """Instruments a named logger.
 
     Useful for non-root loggers with propagate=False.
```

### Comparing `iudex-0.5.5/pyproject.toml` & `iudex-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.5.5"
+version = "0.6.0"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 opentelemetry-exporter-otlp-proto-http = "^1.20.0"
```

### Comparing `iudex-0.5.5/PKG-INFO` & `iudex-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.5.5
+Version: 0.6.0
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

