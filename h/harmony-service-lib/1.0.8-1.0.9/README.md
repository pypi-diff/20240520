# Comparing `tmp/harmony-service-lib-1.0.8.tar.gz` & `tmp/harmony-service-lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony-service-lib-1.0.8.tar", last modified: Tue May  4 18:37:09 2021, max compression
+gzip compressed data, was "harmony-service-lib-1.0.9.tar", last modified: Wed Jul  7 19:25:26 2021, max compression
```

## Comparing `harmony-service-lib-1.0.8.tar` & `harmony-service-lib-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:37:09.795179 harmony-service-lib-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     9772 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7455 2021-05-04 18:37:09.795179 harmony-service-lib-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5774 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:37:09.795179 harmony-service-lib-1.0.8/harmony/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-05-04 18:37:08.000000 harmony-service-lib-1.0.8/harmony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31484 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7914 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/aws.py
--rw-r--r--   0 runner    (1001) docker     (121)    12348 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11742 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    17835 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/message.py
--rw-r--r--   0 runner    (1001) docker     (121)    20645 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/harmony/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 18:37:09.795179 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7455 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      541 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-05-04 18:37:09.000000 harmony-service-lib-1.0.8/harmony_service_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-04 18:37:09.795179 harmony-service-lib-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-05-04 18:36:59.000000 harmony-service-lib-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     9772 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6402 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5758 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/harmony/
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-07-07 19:25:24.000000 harmony-service-lib-1.0.9/harmony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31484 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7914 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/aws.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12348 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3143 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13070 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17835 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20645 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/harmony/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6402 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      323 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-07-07 19:25:26.000000 harmony-service-lib-1.0.9/harmony_service_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-07 19:25:26.704805 harmony-service-lib-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-07-07 19:25:15.000000 harmony-service-lib-1.0.9/setup.py
```

### Comparing `harmony-service-lib-1.0.8/LICENSE` & `harmony-service-lib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/PKG-INFO` & `harmony-service-lib-1.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,147 +1,150 @@
 Metadata-Version: 2.1
 Name: harmony-service-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
 Home-page: https://github.com/nasa/harmony-service-lib-py
 Author: NASA EOSDIS Harmony Team
 Author-email: patrick@element84.com
 License: License :: OSI Approved :: Apache Software License
-Description: # harmony-service-lib
-        
-        A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
-        
-        ## Installing
-        
-        ### Using pip
-        
-        Install the latest version of the package from PyPI using pip:
-        
-            $ pip install harmony-service-lib
-        
-        ### Other methods:
-        
-        The package is installable from source via
-        
-            $ pip install git+https://github.com/harmony/harmony-service-lib-py.git#egg=harmony-service-lib
-        
-        If using a local source tree, run the following in the source root directory instead:
-        
-            $ pip install -e .
-        
-        ## Usage
-        
-        Services that want to work with Harmony can make use of this library to ease
-        interop and upgrades.  To work with Harmony, services must:
-        
-        1. Receive incoming messages from Harmony.  Currently the CLI is the only
-        supported way to receive messages, though HTTP is likely to follow.  `harmony.cli`
-        provides helpers for setting up CLI parsing while being unobtrusive to non-Harmony
-        CLIs that may also need to exist.
-        2. Extend `harmony.BaseHarmonyAdapter` and implement the `#invoke` to
-        adapt the incoming Harmony message to a service call and adapt the service
-        result to call to one of the adapter's `#completed_with_*` methods. The adapter
-        class provides helper methods for retrieving data, staging results, and cleaning
-        up temporary files, though these can be overridden or ignored if a service
-        needs different behavior, e.g. if it operates on data in situ and does not
-        want to download the remote file.
-        
-        A full example of these two requirements with use of helpers can be found in
-        [example/example_service.py](example/example_service.py)
-        
-        ## Environment
-        
-        The following environment variables can be used to control the behavior of the
-        library and allow easier testing:
-        
-        REQUIRED:
-        
-        * `STAGING_BUCKET`: When using helpers to stage service output and pre-sign URLs, this
-               indicates the S3 bucket where data will be staged
-        * `STAGING_PATH`: When using helpers to stage output, this indicates the path within
-               `STAGING_BUCKET` under which data will be staged
-        * `ENV`: The name of the environment.  If 'dev' or 'test', callbacks to Harmony are
-               not made and data is not staged unless also using localstack
-        * `OAUTH_UID`, `OAUTH_PASSWORD`: Used to acquire a shared EDL token
-               needed for downloading granules from EDL token-aware data
-               sources. Services using data in S3 do not need to set this.
-        
-               NOTE: If `FALLBACK_AUTHN_ENABLED` is set to True (CAUTION!)
-               these credentials will be used to download data *as* the EDL
-               application user. This may cause problems with metrics and can
-               result in users getting data for which they've not approved a
-               EULA.
-        * `OAUTH_CLIENT_ID`: The Earthdata application client ID.
-        * `OAUTH_HOST`: Set to the correct Earthdata Login URL, depending on
-               where the service is being deployed. This should be the same
-               environment where the `OAUTH_*` credentials are valid. Defaults
-               to UAT.
-        * `OAUTH_REDIRECT_URI`: A valid redirect URI for the EDL application.
-        * `SHARED_SECRET_KEY`: The 32-byte encryption key shared between Harmony and backend services.
-               This is used to encrypt & decrypt the `accessToken` in the Harmony operation message.
-               In a production environment, this should be injected into the container running the service
-               Docker image. When running the service within Harmony, the Harmony infrastructure will
-               ensure that this environment variable is set with the shared secret key, and the Harmony
-               service library will read and use this key. Therefore, the service developer need not
-               be aware of this variable or its value.
-        
-        OPTIONAL:
-        
-        * `APP_NAME`: Defaults to first argument on commandline. Appears in log records.
-        * `AWS_DEFAULT_REGION`: (Default: `"us-west-2"`) The region in which S3 calls will be made
-        * `USE_LOCALSTACK`: (Development) If 'true' will perform S3 calls against localstack rather
-               than AWS
-        * `LOCALSTACK_HOST`: (Development) If `USE_LOCALSTACK` `true` and this is set, will
-               establish `boto` client connections for S3 & SQS operations using this hostname.
-        * `TEXT_LOGGER`: (Default: True) Setting this to true will cause all
-               log messages to use a text string format. By default log
-               messages will be formatted as JSON.
-        * `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
-               file's mtime is set to the current time whenever a successful attempt is made to to read the
-               message queue (whether or not a message is retrieved). This file can be used by a container's
-               health check command. The container is considered unhealthy if the mtime of the file is old -
-               where 'old' is configurable in the service container. If this variable is not set the path
-               defaults to '/tmp/health.txt'.
-        
-        OPTIONAL -- Use with CAUTION:
-        
-        * `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
-          uses the EDL application credentials. See CAUTION note above.
-        * `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
-        * `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
-        
-        ## Development Setup
-        
-        Prerequisites:
-          - Python 3.7+, ideally installed via a virtual environment such as `pyenv`
-          - A local copy of the code
-        
-        Install dependencies:
-        
-            $ make develop
-        
-        Run linter against production code:
-        
-            $ make lint
-        
-        Run tests:
-        
-            $ make test
-        
-        Build & publish the package:
-        
-            $ make publish
-        
-        ## Releasing
-        
-        GitHub release notes will automatically be generated based on pull request subjects.
-        Pull request subject lines should therefore concisely emphasize library
-        user-facing behavior and updates they should appear in the changelog.  If more
-        information is needed for release notes, note that in the PR content.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# harmony-service-lib
+
+A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
+
+## Installing
+
+### Using pip
+
+Install the latest version of the package from PyPI using pip:
+
+    $ pip install harmony-service-lib
+
+### Other methods:
+
+The package is installable from source via
+
+    $ pip install git+https://github.com/harmony/harmony-service-lib-py.git#egg=harmony-service-lib
+
+If using a local source tree, run the following in the source root directory instead:
+
+    $ pip install -e .
+
+## Usage
+
+Services that want to work with Harmony can make use of this library to ease
+interop and upgrades.  To work with Harmony, services must:
+
+1. Receive incoming messages from Harmony.  Currently the CLI is the only
+supported way to receive messages, though HTTP is likely to follow.  `harmony.cli`
+provides helpers for setting up CLI parsing while being unobtrusive to non-Harmony
+CLIs that may also need to exist.
+2. Extend `harmony.BaseHarmonyAdapter` and implement the `#invoke` to
+adapt the incoming Harmony message to a service call and adapt the service
+result to call to one of the adapter's `#completed_with_*` methods. The adapter
+class provides helper methods for retrieving data, staging results, and cleaning
+up temporary files, though these can be overridden or ignored if a service
+needs different behavior, e.g. if it operates on data in situ and does not
+want to download the remote file.
+
+A full example of these two requirements with use of helpers can be found in
+[example/example_service.py](example/example_service.py)
+
+## Environment
+
+The following environment variables can be used to control the behavior of the
+library and allow easier testing:
+
+REQUIRED:
+
+* `STAGING_BUCKET`: When using helpers to stage service output and pre-sign URLs, this
+       indicates the S3 bucket where data will be staged
+* `STAGING_PATH`: When using helpers to stage output, this indicates the path within
+       `STAGING_BUCKET` under which data will be staged
+* `ENV`: The name of the environment.  If 'dev' or 'test', callbacks to Harmony are
+       not made and data is not staged unless also using localstack
+* `OAUTH_UID`, `OAUTH_PASSWORD`: Used to acquire a shared EDL token
+       needed for downloading granules from EDL token-aware data
+       sources. Services using data in S3 do not need to set this.
+
+       NOTE: If `FALLBACK_AUTHN_ENABLED` is set to True (CAUTION!)
+       these credentials will be used to download data *as* the EDL
+       application user. This may cause problems with metrics and can
+       result in users getting data for which they've not approved a
+       EULA.
+* `OAUTH_CLIENT_ID`: The Earthdata application client ID.
+* `OAUTH_HOST`: Set to the correct Earthdata Login URL, depending on
+       where the service is being deployed. This should be the same
+       environment where the `OAUTH_*` credentials are valid. Defaults
+       to UAT.
+* `OAUTH_REDIRECT_URI`: A valid redirect URI for the EDL application.
+* `SHARED_SECRET_KEY`: The 32-byte encryption key shared between Harmony and backend services.
+       This is used to encrypt & decrypt the `accessToken` in the Harmony operation message.
+       In a production environment, this should be injected into the container running the service
+       Docker image. When running the service within Harmony, the Harmony infrastructure will
+       ensure that this environment variable is set with the shared secret key, and the Harmony
+       service library will read and use this key. Therefore, the service developer need not
+       be aware of this variable or its value.
+
+OPTIONAL:
+
+* `APP_NAME`: Defaults to first argument on commandline. Appears in log records.
+* `AWS_DEFAULT_REGION`: (Default: `"us-west-2"`) The region in which S3 calls will be made
+* `USE_LOCALSTACK`: (Development) If 'true' will perform S3 calls against localstack rather
+       than AWS
+* `LOCALSTACK_HOST`: (Development) If `USE_LOCALSTACK` `true` and this is set, will
+       establish `boto` client connections for S3 & SQS operations using this hostname.
+* `TEXT_LOGGER`: (Default: True) Setting this to true will cause all
+       log messages to use a text string format. By default log
+       messages will be formatted as JSON.
+* `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
+       file's mtime is set to the current time whenever a successful attempt is made to to read the
+       message queue (whether or not a message is retrieved). This file can be used by a container's
+       health check command. The container is considered unhealthy if the mtime of the file is old -
+       where 'old' is configurable in the service container. If this variable is not set the path
+       defaults to '/tmp/health.txt'.
+
+OPTIONAL -- Use with CAUTION:
+
+* `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
+  uses the EDL application credentials. See CAUTION note above.
+* `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
+* `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
+
+## Development Setup
+
+Prerequisites:
+  - Python 3.7+, ideally installed via a virtual environment
+  - A local copy of the code
+
+Install dependencies:
+
+    $ make install
+
+Run linter against production code:
+
+    $ make lint
+
+Run tests:
+
+    $ make test
+
+Build & publish the package:
+
+    $ make publish
+
+## Releasing
+
+GitHub release notes will automatically be generated based on pull request subjects.
+Pull request subject lines should therefore concisely emphasize library
+user-facing behavior and updates they should appear in the changelog.  If more
+information is needed for release notes, note that in the PR content.
+
+
```

### Comparing `harmony-service-lib-1.0.8/README.md` & `harmony-service-lib-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,20 @@
   uses the EDL application credentials. See CAUTION note above.
 * `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
 * `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
 
 ## Development Setup
 
 Prerequisites:
-  - Python 3.7+, ideally installed via a virtual environment such as `pyenv`
+  - Python 3.7+, ideally installed via a virtual environment
   - A local copy of the code
 
 Install dependencies:
 
-    $ make develop
+    $ make install
 
 Run linter against production code:
 
     $ make lint
 
 Run tests:
```

### Comparing `harmony-service-lib-1.0.8/harmony/adapter.py` & `harmony-service-lib-1.0.9/harmony/adapter.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/aws.py` & `harmony-service-lib-1.0.9/harmony/aws.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/cli.py` & `harmony-service-lib-1.0.9/harmony/cli.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/earthdata.py` & `harmony-service-lib-1.0.9/harmony/earthdata.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/exceptions.py` & `harmony-service-lib-1.0.9/harmony/exceptions.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/http.py` & `harmony-service-lib-1.0.9/harmony/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 from functools import lru_cache
 import json
 from urllib.parse import urlparse
 import datetime
 import sys
+import os
 import re
 
 import requests
 
 from harmony.earthdata import EarthdataAuth, EarthdataSession
 from harmony.exceptions import ForbiddenException
 from harmony.logging import build_logger
@@ -130,15 +131,15 @@
 
 @lru_cache(maxsize=128)
 def _earthdata_session():
     """Constructs an EarthdataSession for use to download one or more files."""
     return EarthdataSession()
 
 
-def _download(config, url: str, access_token: str, data, user_agent=None):
+def _download(config, url: str, access_token: str, data, user_agent=None, **kwargs_download_agent):
     """Implements the download functionality.
 
     Using the EarthdataSession and EarthdataAuth extensions to the
     `requests` module, this function will download the given url and
     perform any necessary Earthdata Login OAuth handshakes.
 
     Parameters
@@ -155,36 +156,39 @@
         when making an HTTP POST request. These data will be URL
         encoded to a query string containing a series of `key=value`
         pairs, separated by ampersands. If None (the default), the
         request will be sent with an HTTP GET request.
     user_agent : str
         The user agent that is requesting the download.
         E.g. harmony/0.0.0 (harmony-sit) harmony-service-lib/4.0 (gdal-subsetter)
+    kwargs_download_agent: dict
+        kwargs to be passed to the download agent
+        E.g. stream=True
 
     Returns
     -------
     requests.Response with the download result
 
     """
     headers = {}
     if user_agent is not None:
         headers['user-agent'] = user_agent
     auth = EarthdataAuth(config.oauth_uid, config.oauth_password, access_token)
     with _earthdata_session() as session:
         session.auth = auth
         if data is None:
-            return session.get(url, headers=headers, timeout=TIMEOUT)
+            return session.get(url, headers=headers, timeout=TIMEOUT, **kwargs_download_agent)
         else:
             # Including this header since the stdlib does by default,
             # but we've switched to `requests` which does not.
             headers['Content-Type'] = 'application/x-www-form-urlencoded'
             return session.post(url, headers=headers, data=data, timeout=TIMEOUT)
 
 
-def _download_with_fallback_authn(config, url: str, data, user_agent=None):
+def _download_with_fallback_authn(config, url: str, data, user_agent=None, **kwargs_download_agent):
     """Downloads the given url using Basic authentication as a fallback
     mechanism should the normal EDL Oauth handshake fail.
 
     This function requires the `edl_username` and `edl_password`
     attributes in the config object to be populated with valid
     credentials.
 
@@ -199,26 +203,29 @@
         when making an HTTP POST request. These data will be URL
         encoded to a query string containing a series of `key=value`
         pairs, separated by ampersands. If None (the default), the
         request will be sent with an HTTP GET request.
     user_agent : str
         The user agent that is requesting the download.
         E.g. harmony/0.0.0 (harmony-sit) harmony-service-lib/4.0 (gdal-subsetter)
+    kwargs_download_agent: dict
+        kwargs to be passed to the download agent
+        E.g. stream=True
 
     Returns
     -------
     requests.Response with the download result
 
     """
     headers = {}
     if user_agent is not None:
         headers['user-agent'] = user_agent
     auth = requests.auth.HTTPBasicAuth(config.edl_username, config.edl_password)
     if data is None:
-        return requests.get(url, headers=headers, timeout=TIMEOUT, auth=auth)
+        return requests.get(url, headers=headers, timeout=TIMEOUT, auth=auth, **kwargs_download_agent)
     else:
         return requests.post(url, headers=headers, data=data, timeout=TIMEOUT, auth=auth)
 
 
 def _log_download_performance(logger, url, duration_ms, file_size):
     """Logs a message tracking performance information related to a file download.
 
@@ -247,15 +254,16 @@
         'host': host,
         "path": url_path,
         "size": file_size
     }
     logger.info('timing.download.end', extra=extra_fields)
 
 
-def download(config, url: str, access_token: str, data, destination_file, user_agent=None):
+def download(config, url: str, access_token: str, data, destination_file,
+             user_agent=None, stream=True, buffer_size=1024*1024*16):
     """Downloads the given url using the provided EDL user access token
     and writes it to the provided file-like object.
 
     Exception cases:
     1. No user access token
     2. Invalid user access token
     3. Unable to authenticate the user with Earthdata Login
@@ -291,36 +299,53 @@
     Returns
     -------
     requests.Response with the download result
 
     Side-effects
     ------------
     Will write to provided destination_file
+    NOTE: streaming request is used to download the file,
+          and the chunksize is defaulted to 16MB based on the experiment with a large file of 1.8Gb
+          for optimized speed and memory consumption.
+          If you are experiencing some performance decay for high-throughput small-sized granules,
+          you may want to set stream=False.
     """
 
     response = None
     logger = build_logger(config)
     start_time = datetime.datetime.now()
     logger.info(f'timing.download.start {url}')
 
+    if (not stream) and buffer_size:
+        logger.warn(
+            f"In download paramters, buffer_size={buffer_size} will be ignored since stream is set to be {stream}."
+        )
+    elif stream and not isinstance(buffer_size, int):
+        raise Exception(f"In download parameters: buffer_size must be integer when stream={stream}.")
+
     if access_token is not None and _valid(config.oauth_host, config.oauth_client_id, access_token):
-        response = _download(config, url, access_token, data, user_agent)
+        response = _download(config, url, access_token, data, user_agent, stream=stream)
 
     if response is None or not response.ok:
         if config.fallback_authn_enabled:
             msg = ('No valid user access token in request or EDL OAuth authentication failed.'
                    'Fallback authentication enabled: retrying with Basic auth.')
             logger.warning(msg)
-            response = _download_with_fallback_authn(config, url, data, user_agent)
+            response = _download_with_fallback_authn(config, url, data, user_agent, stream=stream)
 
     if response.ok:
+        if not stream:
+            destination_file.write(response.content)
+            file_size = sys.getsizeof(response.content)
+        else:
+            for chunk in response.iter_content(chunk_size=buffer_size):
+                destination_file.write(chunk)
+            file_size = os.path.getsize(destination_file.name)
         time_diff = datetime.datetime.now() - start_time
         duration_ms = int(round(time_diff.total_seconds() * 1000))
-        destination_file.write(response.content)
-        file_size = sys.getsizeof(response.content)
         duration_logger = build_logger(config)
         _log_download_performance(duration_logger, url, duration_ms, file_size)
 
         return response
 
     if _is_eula_error(response.content):
         msg = _eula_error_message(response.content)
```

### Comparing `harmony-service-lib-1.0.8/harmony/logging.py` & `harmony-service-lib-1.0.9/harmony/logging.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/message.py` & `harmony-service-lib-1.0.9/harmony/message.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony/util.py` & `harmony-service-lib-1.0.9/harmony/util.py`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/harmony_service_lib.egg-info/PKG-INFO` & `harmony-service-lib-1.0.9/harmony_service_lib.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,147 +1,150 @@
 Metadata-Version: 2.1
 Name: harmony-service-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
 Home-page: https://github.com/nasa/harmony-service-lib-py
 Author: NASA EOSDIS Harmony Team
 Author-email: patrick@element84.com
 License: License :: OSI Approved :: Apache Software License
-Description: # harmony-service-lib
-        
-        A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
-        
-        ## Installing
-        
-        ### Using pip
-        
-        Install the latest version of the package from PyPI using pip:
-        
-            $ pip install harmony-service-lib
-        
-        ### Other methods:
-        
-        The package is installable from source via
-        
-            $ pip install git+https://github.com/harmony/harmony-service-lib-py.git#egg=harmony-service-lib
-        
-        If using a local source tree, run the following in the source root directory instead:
-        
-            $ pip install -e .
-        
-        ## Usage
-        
-        Services that want to work with Harmony can make use of this library to ease
-        interop and upgrades.  To work with Harmony, services must:
-        
-        1. Receive incoming messages from Harmony.  Currently the CLI is the only
-        supported way to receive messages, though HTTP is likely to follow.  `harmony.cli`
-        provides helpers for setting up CLI parsing while being unobtrusive to non-Harmony
-        CLIs that may also need to exist.
-        2. Extend `harmony.BaseHarmonyAdapter` and implement the `#invoke` to
-        adapt the incoming Harmony message to a service call and adapt the service
-        result to call to one of the adapter's `#completed_with_*` methods. The adapter
-        class provides helper methods for retrieving data, staging results, and cleaning
-        up temporary files, though these can be overridden or ignored if a service
-        needs different behavior, e.g. if it operates on data in situ and does not
-        want to download the remote file.
-        
-        A full example of these two requirements with use of helpers can be found in
-        [example/example_service.py](example/example_service.py)
-        
-        ## Environment
-        
-        The following environment variables can be used to control the behavior of the
-        library and allow easier testing:
-        
-        REQUIRED:
-        
-        * `STAGING_BUCKET`: When using helpers to stage service output and pre-sign URLs, this
-               indicates the S3 bucket where data will be staged
-        * `STAGING_PATH`: When using helpers to stage output, this indicates the path within
-               `STAGING_BUCKET` under which data will be staged
-        * `ENV`: The name of the environment.  If 'dev' or 'test', callbacks to Harmony are
-               not made and data is not staged unless also using localstack
-        * `OAUTH_UID`, `OAUTH_PASSWORD`: Used to acquire a shared EDL token
-               needed for downloading granules from EDL token-aware data
-               sources. Services using data in S3 do not need to set this.
-        
-               NOTE: If `FALLBACK_AUTHN_ENABLED` is set to True (CAUTION!)
-               these credentials will be used to download data *as* the EDL
-               application user. This may cause problems with metrics and can
-               result in users getting data for which they've not approved a
-               EULA.
-        * `OAUTH_CLIENT_ID`: The Earthdata application client ID.
-        * `OAUTH_HOST`: Set to the correct Earthdata Login URL, depending on
-               where the service is being deployed. This should be the same
-               environment where the `OAUTH_*` credentials are valid. Defaults
-               to UAT.
-        * `OAUTH_REDIRECT_URI`: A valid redirect URI for the EDL application.
-        * `SHARED_SECRET_KEY`: The 32-byte encryption key shared between Harmony and backend services.
-               This is used to encrypt & decrypt the `accessToken` in the Harmony operation message.
-               In a production environment, this should be injected into the container running the service
-               Docker image. When running the service within Harmony, the Harmony infrastructure will
-               ensure that this environment variable is set with the shared secret key, and the Harmony
-               service library will read and use this key. Therefore, the service developer need not
-               be aware of this variable or its value.
-        
-        OPTIONAL:
-        
-        * `APP_NAME`: Defaults to first argument on commandline. Appears in log records.
-        * `AWS_DEFAULT_REGION`: (Default: `"us-west-2"`) The region in which S3 calls will be made
-        * `USE_LOCALSTACK`: (Development) If 'true' will perform S3 calls against localstack rather
-               than AWS
-        * `LOCALSTACK_HOST`: (Development) If `USE_LOCALSTACK` `true` and this is set, will
-               establish `boto` client connections for S3 & SQS operations using this hostname.
-        * `TEXT_LOGGER`: (Default: True) Setting this to true will cause all
-               log messages to use a text string format. By default log
-               messages will be formatted as JSON.
-        * `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
-               file's mtime is set to the current time whenever a successful attempt is made to to read the
-               message queue (whether or not a message is retrieved). This file can be used by a container's
-               health check command. The container is considered unhealthy if the mtime of the file is old -
-               where 'old' is configurable in the service container. If this variable is not set the path
-               defaults to '/tmp/health.txt'.
-        
-        OPTIONAL -- Use with CAUTION:
-        
-        * `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
-          uses the EDL application credentials. See CAUTION note above.
-        * `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
-        * `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
-        
-        ## Development Setup
-        
-        Prerequisites:
-          - Python 3.7+, ideally installed via a virtual environment such as `pyenv`
-          - A local copy of the code
-        
-        Install dependencies:
-        
-            $ make develop
-        
-        Run linter against production code:
-        
-            $ make lint
-        
-        Run tests:
-        
-            $ make test
-        
-        Build & publish the package:
-        
-            $ make publish
-        
-        ## Releasing
-        
-        GitHub release notes will automatically be generated based on pull request subjects.
-        Pull request subject lines should therefore concisely emphasize library
-        user-facing behavior and updates they should appear in the changelog.  If more
-        information is needed for release notes, note that in the PR content.
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# harmony-service-lib
+
+A library for Python-based Harmony services to parse incoming messages, fetch data, stage data, and call back to Harmony
+
+## Installing
+
+### Using pip
+
+Install the latest version of the package from PyPI using pip:
+
+    $ pip install harmony-service-lib
+
+### Other methods:
+
+The package is installable from source via
+
+    $ pip install git+https://github.com/harmony/harmony-service-lib-py.git#egg=harmony-service-lib
+
+If using a local source tree, run the following in the source root directory instead:
+
+    $ pip install -e .
+
+## Usage
+
+Services that want to work with Harmony can make use of this library to ease
+interop and upgrades.  To work with Harmony, services must:
+
+1. Receive incoming messages from Harmony.  Currently the CLI is the only
+supported way to receive messages, though HTTP is likely to follow.  `harmony.cli`
+provides helpers for setting up CLI parsing while being unobtrusive to non-Harmony
+CLIs that may also need to exist.
+2. Extend `harmony.BaseHarmonyAdapter` and implement the `#invoke` to
+adapt the incoming Harmony message to a service call and adapt the service
+result to call to one of the adapter's `#completed_with_*` methods. The adapter
+class provides helper methods for retrieving data, staging results, and cleaning
+up temporary files, though these can be overridden or ignored if a service
+needs different behavior, e.g. if it operates on data in situ and does not
+want to download the remote file.
+
+A full example of these two requirements with use of helpers can be found in
+[example/example_service.py](example/example_service.py)
+
+## Environment
+
+The following environment variables can be used to control the behavior of the
+library and allow easier testing:
+
+REQUIRED:
+
+* `STAGING_BUCKET`: When using helpers to stage service output and pre-sign URLs, this
+       indicates the S3 bucket where data will be staged
+* `STAGING_PATH`: When using helpers to stage output, this indicates the path within
+       `STAGING_BUCKET` under which data will be staged
+* `ENV`: The name of the environment.  If 'dev' or 'test', callbacks to Harmony are
+       not made and data is not staged unless also using localstack
+* `OAUTH_UID`, `OAUTH_PASSWORD`: Used to acquire a shared EDL token
+       needed for downloading granules from EDL token-aware data
+       sources. Services using data in S3 do not need to set this.
+
+       NOTE: If `FALLBACK_AUTHN_ENABLED` is set to True (CAUTION!)
+       these credentials will be used to download data *as* the EDL
+       application user. This may cause problems with metrics and can
+       result in users getting data for which they've not approved a
+       EULA.
+* `OAUTH_CLIENT_ID`: The Earthdata application client ID.
+* `OAUTH_HOST`: Set to the correct Earthdata Login URL, depending on
+       where the service is being deployed. This should be the same
+       environment where the `OAUTH_*` credentials are valid. Defaults
+       to UAT.
+* `OAUTH_REDIRECT_URI`: A valid redirect URI for the EDL application.
+* `SHARED_SECRET_KEY`: The 32-byte encryption key shared between Harmony and backend services.
+       This is used to encrypt & decrypt the `accessToken` in the Harmony operation message.
+       In a production environment, this should be injected into the container running the service
+       Docker image. When running the service within Harmony, the Harmony infrastructure will
+       ensure that this environment variable is set with the shared secret key, and the Harmony
+       service library will read and use this key. Therefore, the service developer need not
+       be aware of this variable or its value.
+
+OPTIONAL:
+
+* `APP_NAME`: Defaults to first argument on commandline. Appears in log records.
+* `AWS_DEFAULT_REGION`: (Default: `"us-west-2"`) The region in which S3 calls will be made
+* `USE_LOCALSTACK`: (Development) If 'true' will perform S3 calls against localstack rather
+       than AWS
+* `LOCALSTACK_HOST`: (Development) If `USE_LOCALSTACK` `true` and this is set, will
+       establish `boto` client connections for S3 & SQS operations using this hostname.
+* `TEXT_LOGGER`: (Default: True) Setting this to true will cause all
+       log messages to use a text string format. By default log
+       messages will be formatted as JSON.
+* `HEALTH_CHECK_PATH`: Set this to the path where the health check file should be stored. This
+       file's mtime is set to the current time whenever a successful attempt is made to to read the
+       message queue (whether or not a message is retrieved). This file can be used by a container's
+       health check command. The container is considered unhealthy if the mtime of the file is old -
+       where 'old' is configurable in the service container. If this variable is not set the path
+       defaults to '/tmp/health.txt'.
+
+OPTIONAL -- Use with CAUTION:
+
+* `FALLBACK_AUTHN_ENABLED`: Default: False. Enable the fallback authentication that
+  uses the EDL application credentials. See CAUTION note above.
+* `EDL_USERNAME`: The Earthdata Login username used for fallback authn.
+* `EDL_PASSWORD`: The Earthdata Login password used for fallback authn.
+
+## Development Setup
+
+Prerequisites:
+  - Python 3.7+, ideally installed via a virtual environment
+  - A local copy of the code
+
+Install dependencies:
+
+    $ make install
+
+Run linter against production code:
+
+    $ make lint
+
+Run tests:
+
+    $ make test
+
+Build & publish the package:
+
+    $ make publish
+
+## Releasing
+
+GitHub release notes will automatically be generated based on pull request subjects.
+Pull request subject lines should therefore concisely emphasize library
+user-facing behavior and updates they should appear in the changelog.  If more
+information is needed for release notes, note that in the PR content.
+
+
```

### Comparing `harmony-service-lib-1.0.8/harmony_service_lib.egg-info/SOURCES.txt` & `harmony-service-lib-1.0.9/harmony_service_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harmony-service-lib-1.0.8/setup.py` & `harmony-service-lib-1.0.9/setup.py`

 * *Files identical despite different names*

