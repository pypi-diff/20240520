# Comparing `tmp/pypomes_logging-0.0.8.tar.gz` & `tmp/pypomes_logging-0.0.9.tar.gz`

## Comparing `pypomes_logging-0.0.8.tar` & `pypomes_logging-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0    13127 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0    13131 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.9/PKG-INFO
```

### Comparing `pypomes_logging-0.0.8/src/pypomes_logging/__init__.py` & `pypomes_logging-0.0.9/src/pypomes_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.8/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.0.9/src/pypomes_logging/logging_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from flask import Request, Response, send_file
 from logging import NOTSET, DEBUG, INFO, WARNING, ERROR, CRITICAL  # 0, 10, 20, 30, 40, 50
 from io import BytesIO
 from pathlib import Path
 from typing import Final, Literal, TextIO
 
 from pypomes_core import (
-    APP_PREFIX, DATETIME_FORMAT_INV, TEMP_DIR, DATETIME_FORMAT_COMPACT,
+    APP_PREFIX, DATETIME_FORMAT_INV, TEMP_FOLDER, DATETIME_FORMAT_COMPACT,
     env_get_str, env_get_path, datetime_parse
 )
 from pypomes_http import http_get_parameters
 
 
 def __get_logging_level(level: Literal["debug", "info", "warning", "error", "critical"]) -> int:
     """
@@ -42,15 +42,15 @@
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID", f"{APP_PREFIX}")
 LOGGING_FORMAT: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FORMAT",
                                          "{asctime} {levelname:1.1} {thread:5d} "
                                          "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
 LOGGING_STYLE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_STYLE", "{")
 
 LOGGING_FILE_PATH: Final[Path] = env_get_path(f"{APP_PREFIX}_LOGGING_FILE_PATH",
-                                              TEMP_DIR / f"{APP_PREFIX}.log")
+                                              TEMP_FOLDER / f"{APP_PREFIX}.log")
 LOGGING_FILE_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_MODE", "a")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
 # define the logging severity level
 # noinspection PyTypeChecker
@@ -110,15 +110,15 @@
                 # noinspection PyTypeChecker
                 msg_level: int = CRITICAL if len(items) < 2 else __get_logging_level(items[2])
                 # 'not log_level' works for both values 'NOTSET' and 'None'
                 if not log_level or msg_level >= log_level:
                     if len(items) > 1 and (log_from or log_to):
                         timestamp: datetime = datetime_parse(f"{items[0]} {items[1]}")
                         if not timestamp or \
-                           ((not log_from or timestamp >= log_from) and \
+                           ((not log_from or timestamp >= log_from) and
                             (not log_to or timestamp <= log_to)):
                             result.write(line.encode())
                     else:
                         result.write(line.encode())
                 line = f.readline()
 
     return result
```

### Comparing `pypomes_logging-0.0.8/LICENSE` & `pypomes_logging-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.8/pyproject.toml` & `pypomes_logging-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=1.0.3",
+    "pypomes_core>=1.0.5",
     "pypomes_http>=0.1.6",
     "python-dateutil>=2.8.2",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_logging-0.0.8/PKG-INFO` & `pypomes_logging-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_logging
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.0.3
+Requires-Dist: pypomes-core>=1.0.5
 Requires-Dist: pypomes-http>=0.1.6
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

