# Comparing `tmp/ucam_observe-0.1.4.tar.gz` & `tmp/ucam_observe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucam_observe-0.1.4.tar", max compression
+gzip compressed data, was "ucam_observe-0.2.0.tar", max compression
```

## Comparing `ucam_observe-0.1.4.tar` & `ucam_observe-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2807 2024-05-16 20:03:12.153112 ucam_observe-0.1.4/README.md
--rw-r--r--   0        0        0     1927 2024-05-17 14:42:05.515283 ucam_observe-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      231 2024-05-16 22:09:02.870367 ucam_observe-0.1.4/ucam_observe/__init__.py
--rw-r--r--   0        0        0      243 2024-05-15 15:57:57.344997 ucam_observe-0.1.4/ucam_observe/django.py
--rw-r--r--   0        0        0     1296 2024-05-17 14:42:05.515283 ucam_observe-0.1.4/ucam_observe/gunicorn.py
--rw-r--r--   0        0        0     4840 2024-05-17 12:36:45.416469 ucam_observe-0.1.4/ucam_observe/logging_config.py
--rw-r--r--   0        0        0     3564 1970-01-01 00:00:00.000000 ucam_observe-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2821 2024-05-17 19:19:28.581765 ucam_observe-0.2.0/README.md
+-rw-r--r--   0        0        0     1927 2024-05-17 19:15:58.703949 ucam_observe-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-05-17 19:03:31.697492 ucam_observe-0.2.0/ucam_observe/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-15 15:59:18.796561 ucam_observe-0.2.0/ucam_observe/django.py
+-rw-r--r--   0        0        0     1580 2024-05-17 19:18:05.805049 ucam_observe-0.2.0/ucam_observe/gunicorn.py
+-rw-r--r--   0        0        0     5915 2024-05-20 11:42:36.602630 ucam_observe-0.2.0/ucam_observe/logging_config.py
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 ucam_observe-0.2.0/PKG-INFO
```

### Comparing `ucam_observe-0.1.4/README.md` & `ucam_observe-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,20 +36,19 @@
 ## Include Gunicorn structlog configuration in your project
 
 ### Adapt Gunicorn configuration
 In the root of your project, create/amend a gunicorn.conf.py. Add the following code to the file.
 
 ```py
 from ucam_observe.gunicorn import (  # noqa F401 used by gunicorn as magic variable
-    logconfig_dict,
-    loglevel,
+    logconfig_dict
 )
 ```
 
-**Be sure not to set loglevel via the CLI.**
+**Be sure not to set any log config values via the CLI or config files.**
 
 ### Environment Configuration
 
 #### Log Level
 
 Set the `LOG_LEVEL` environment variable to control the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL). This setting adjusts the verbosity of the log outputs:
```

### Comparing `ucam_observe-0.1.4/pyproject.toml` & `ucam_observe-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ucam_observe"
-version = "0.1.4"
+version = "0.2.0"
 description = "Python library to aid consistent configuration of logging, metrics (future) and tracing (further in future). Packaging and wiring existing open tooling to work effortlessly on UIS DevOps managed cloud infrastructure."
 license = "MIT"
 readme = "README.md"
 authors = []
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `ucam_observe-0.1.4/ucam_observe/gunicorn.py` & `ucam_observe-0.2.0/ucam_observe/gunicorn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-from ucam_observe.logging_config import get_dict_config_formatters, get_log_level
+from ucam_observe.logging_config import (
+    get_chosen_formatter_key,
+    get_chosen_handler_keys,
+    get_dict_config_formatters,
+    get_dict_config_handlers,
+    get_log_level_name,
+)
 
 logconfig_dict = {
     "formatters": get_dict_config_formatters(),
+    "root": {
+        "handlers": get_chosen_handler_keys(),
+        "level": get_log_level_name(),
+    },
     "handlers": {
         "console": {
             "class": "logging.StreamHandler",
-            "formatter": "json",
+            "formatter": get_chosen_formatter_key(),
             "stream": "ext://sys.stdout",
         },
         "error_console": {
             "class": "logging.StreamHandler",
-            "formatter": "json",
+            "formatter": get_chosen_formatter_key(),
             "stream": "ext://sys.stderr",
         },
+        **get_dict_config_handlers(),
     },
     "loggers": {
         "gunicorn.error": {
-            "level": "INFO",
+            "level": get_log_level_name(),
             "handlers": ["error_console"],
             # Whilst True is the default in CONFIG_DEFAULTS within structlog, these default
             # settings cause duplicate logs (the default settings are only applied when
             # logconfig_dict is specified and is not empty), presumably because other
             # settings cause gunicorn to programmatically add stdout/err to these existing
             # handlers.
             "propagate": False,
             "qualname": "gunicorn.error",
         },
         "gunicorn.access": {
-            "level": "INFO",
+            "level": get_log_level_name(),
             "handlers": ["console"],
             "propagate": False,
             "qualname": "gunicorn.access",
         },
     },
 }
-
-loglevel = get_log_level().lower()
```

### Comparing `ucam_observe-0.1.4/ucam_observe/logging_config.py` & `ucam_observe-0.2.0/ucam_observe/logging_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,44 @@
+import logging
 import os
 import re
 from logging.config import dictConfig
 
 import structlog
 
 
-def get_log_level():
+def get_log_level_name():
     """Retrieve log level from environment variables."""
-    return os.getenv("LOG_LEVEL", "INFO").upper()
+    VALID_LEVELS = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+
+    input_upper = os.getenv("LOG_LEVEL", "INFO").upper()
+
+    if input_upper not in VALID_LEVELS:
+        raise RuntimeError(f"{input_upper} not from valid choices {VALID_LEVELS}")
+
+    return input_upper
+
+
+def get_log_level_int():
+    return logging.getLevelName(get_log_level_name())
 
 
 def get_console_logging_status():
     """Retrieve console logging status from environment variables."""
     return os.getenv("CONSOLE_LOGGING", "False").lower() in ("true", "1")
 
 
+def get_chosen_formatter_key():
+    return "developer_console" if get_console_logging_status() else "json"
+
+
+def get_chosen_handler_keys():
+    return [get_chosen_formatter_key()]
+
+
 def _add_gcp_log_severity(logger, method_name, event_dict):  # pragma: no cover
     """
     Add the log level to the event dict under the "severity" key.
 
     This is used as a structlog log processor, and is necessary as severity is used by GCP instead
     of level.
 
@@ -69,91 +89,105 @@
         # We want the log even if this code fails
         except:  # noqa E722 rare occasion where we do want to carry on if this block fails
             pass
 
     return event_dict
 
 
-def _set_process_id(_, __, event_dict):
-    event_dict["process_id"] = os.getpid()
-    return event_dict
+def get_common_structlog_processors():
+    # This configuration is used by logs that originate from both standard python loggers and
+    # structlog loggers
+    return [
+        structlog.contextvars.merge_contextvars,
+        structlog.stdlib.add_log_level,
+        structlog.stdlib.add_logger_name,
+        structlog.processors.TimeStamper(fmt="iso"),
+        _add_gcp_log_severity,
+        _gunicorn_combined_logformat,
+        structlog.processors.CallsiteParameterAdder(
+            {
+                structlog.processors.CallsiteParameter.FILENAME,
+                structlog.processors.CallsiteParameter.FUNC_NAME,
+                structlog.processors.CallsiteParameter.LINENO,
+                structlog.processors.CallsiteParameter.PROCESS,
+                structlog.processors.CallsiteParameter.THREAD,
+            }
+        ),
+        structlog.stdlib.PositionalArgumentsFormatter(),
+        structlog.processors.StackInfoRenderer(),
+        structlog.processors.format_exc_info,
+        structlog.processors.UnicodeDecoder(),
+    ]
 
 
 def get_dict_config_formatters():
     return {
         "developer_console": {
             "()": "structlog.stdlib.ProcessorFormatter",
             "processor": structlog.dev.ConsoleRenderer(colors=True),
+            "foreign_pre_chain": get_common_structlog_processors(),
         },
         "json": {
             "()": "structlog.stdlib.ProcessorFormatter",
             "processor": structlog.processors.JSONRenderer(),
-            "foreign_pre_chain": [
-                structlog.stdlib.add_log_level,
-                structlog.stdlib.add_logger_name,
-                structlog.processors.TimeStamper(fmt="iso"),
-                _add_gcp_log_severity,
-                _gunicorn_combined_logformat,
-                _set_process_id,
-            ],
+            "foreign_pre_chain": get_common_structlog_processors(),
+        },
+    }
+
+
+def get_dict_config_handlers():
+    return {
+        "developer_console": {
+            "class": "logging.StreamHandler",
+            "formatter": "developer_console",
+        },
+        "json": {
+            "class": "logging.StreamHandler",
+            "formatter": "json",
         },
     }
 
 
 def get_dict_config():
     return {
         "version": 1,
         "disable_existing_loggers": True,
         "formatters": get_dict_config_formatters(),
-        "handlers": {
-            "developer_console": {
-                "class": "logging.StreamHandler",
-                "formatter": "developer_console",
-            },
-            "json": {
-                "class": "logging.StreamHandler",
-                "formatter": "json",
-            },
-        },
+        "handlers": get_dict_config_handlers(),
         "loggers": {
+            # This is potentially overridden by gunicorn
             "": {
-                "handlers": ["developer_console" if get_console_logging_status() else "json"],
-                "level": get_log_level(),
-                "propagate": True,
+                "handlers": get_chosen_handler_keys(),
+                "level": get_log_level_name(),
             },
         },
     }
 
 
 def configure_structlog():
+    # This configuration is just used by logs that are generated by structlog loggers
     structlog.configure(
         processors=[
-            structlog.contextvars.merge_contextvars,
-            structlog.stdlib.filter_by_level,
-            structlog.processors.TimeStamper(fmt="iso"),
-            structlog.stdlib.add_logger_name,
-            structlog.stdlib.PositionalArgumentsFormatter(),
-            structlog.processors.StackInfoRenderer(),
-            structlog.processors.format_exc_info,
-            structlog.processors.UnicodeDecoder(),
+            *get_common_structlog_processors(),
             structlog.stdlib.ProcessorFormatter.wrap_for_formatter,
         ],
+        wrapper_class=structlog.make_filtering_bound_logger(get_log_level_int()),
         logger_factory=structlog.stdlib.LoggerFactory(),
         cache_logger_on_first_use=True,
     )
 
 
 def configure_logging(force_reset=False):
     """Configure structured logging for both Python logging and structlog."""
 
     global configure_logging_run
     if not force_reset and configure_logging_run:
         return
 
     configure_logging_run = True
 
-    configure_structlog()
-
     dictConfig(get_dict_config())
 
+    configure_structlog()
+
 
 configure_logging_run = False
```

### Comparing `ucam_observe-0.1.4/PKG-INFO` & `ucam_observe-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucam_observe
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python library to aid consistent configuration of logging, metrics (future) and tracing (further in future). Packaging and wiring existing open tooling to work effortlessly on UIS DevOps managed cloud infrastructure.
 License: MIT
 Requires-Python: >=3.9.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -52,20 +52,19 @@
 ## Include Gunicorn structlog configuration in your project
 
 ### Adapt Gunicorn configuration
 In the root of your project, create/amend a gunicorn.conf.py. Add the following code to the file.
 
 ```py
 from ucam_observe.gunicorn import (  # noqa F401 used by gunicorn as magic variable
-    logconfig_dict,
-    loglevel,
+    logconfig_dict
 )
 ```
 
-**Be sure not to set loglevel via the CLI.**
+**Be sure not to set any log config values via the CLI or config files.**
 
 ### Environment Configuration
 
 #### Log Level
 
 Set the `LOG_LEVEL` environment variable to control the logging level (e.g., DEBUG, INFO, WARNING, ERROR, CRITICAL). This setting adjusts the verbosity of the log outputs:
```

