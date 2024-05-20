# Comparing `tmp/wpp-bavapi-1.0.4.tar.gz` & `tmp/wpp_bavapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp-bavapi-1.0.4.tar", last modified: Tue Apr  9 12:46:19 2024, max compression
+gzip compressed data, was "wpp_bavapi-1.1.0.tar", last modified: Mon May 20 14:36:23 2024, max compression
```

## Comparing `wpp-bavapi-1.0.4.tar` & `wpp_bavapi-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.423018 wpp-bavapi-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-09 12:46:19.423018 wpp-bavapi-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.415018 wpp-bavapi-1.0.4/bavapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_batched.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.415018 wpp-bavapi-1.0.4/bavapi/_reference/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_reference/generate_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/_reference/int_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    62420 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21315 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.415018 wpp-bavapi-1.0.4/bavapi/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/parsing/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/parsing/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    64528 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/bavapi/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:46:19.423018 wpp-bavapi-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.419018 wpp-bavapi-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_batched.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 12:46:06.000000 wpp-bavapi-1.0.4/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:46:19.419018 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 12:46:19.000000 wpp-bavapi-1.0.4/wpp_bavapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:23.845574 wpp_bavapi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-20 14:36:23.845574 wpp_bavapi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:23.841574 wpp_bavapi-1.1.0/bavapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/_batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:23.841574 wpp_bavapi-1.1.0/bavapi/_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/_reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/_reference/generate_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/_reference/int_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62364 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21735 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:23.841574 wpp_bavapi-1.1.0/bavapi/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/parsing/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/parsing/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64529 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27260 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/bavapi/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:36:23.845574 wpp_bavapi-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:23.845574 wpp_bavapi-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-05-20 14:36:11.000000 wpp_bavapi-1.1.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:36:23.845574 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-20 14:36:23.000000 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-20 14:36:23.000000 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:36:23.000000 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 14:36:23.000000 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-20 14:36:23.000000 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 14:36:23.000000 wpp_bavapi-1.1.0/wpp_bavapi.egg-info/top_level.txt
```

### Comparing `wpp-bavapi-1.0.4/LICENSE` & `wpp_bavapi-1.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [2023] [WPPBAV]
+   Copyright [2024] [WPPBAV]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `wpp-bavapi-1.0.4/PKG-INFO` & `wpp_bavapi-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 1.0.4
+Version: 1.1.0
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://wppbav.github.io/bavapi-sdk-python/
 Project-URL: repository, https://github.com/wppbav/wpp-bavapi/
 Project-URL: api_reference, https://developer.wppbav.com/docs/2.x/intro
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
@@ -127,27 +127,29 @@
 | ... | ...       | ...                   | ...  | ...    | ... |
 
 ## Features
 
 - Support for all endpoints in the WPPBAV Fount API.
   - Extended support for the following endpoints:
     - `audiences`
+    - `audience-groups`
     - `brand-metrics`
     - `brand-metric-groups`
     - `brands`
     - `brandscape-data`
     - `categories`
     - `cities`
     - `collections`
     - `companies`
     - `countries`
     - `sectors`
     - `studies`
     - `years`
   - Other endpoints are available via the `raw_query` functions and methods.
+  - Extended support for Fount API Tools/TurboPitch endpoints.
 - Validates query parameters are of the correct types and provides type hints for better IDE support.
 - Retrieve multiple pages of data simultaneously, monitoring and preventing exceeding API rate limit.
 - Both synchronous and asynchronous APIs for accessing BAV data.
 
 ## Documentation
 
 Read more about `bavapi` in the [documentation](https://wppbav.github.io/bavapi-sdk-python/).
```

### Comparing `wpp-bavapi-1.0.4/README.md` & `wpp_bavapi-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,27 +73,29 @@
 | ... | ...       | ...                   | ...  | ...    | ... |
 
 ## Features
 
 - Support for all endpoints in the WPPBAV Fount API.
   - Extended support for the following endpoints:
     - `audiences`
+    - `audience-groups`
     - `brand-metrics`
     - `brand-metric-groups`
     - `brands`
     - `brandscape-data`
     - `categories`
     - `cities`
     - `collections`
     - `companies`
     - `countries`
     - `sectors`
     - `studies`
     - `years`
   - Other endpoints are available via the `raw_query` functions and methods.
+  - Extended support for Fount API Tools/TurboPitch endpoints.
 - Validates query parameters are of the correct types and provides type hints for better IDE support.
 - Retrieve multiple pages of data simultaneously, monitoring and preventing exceeding API rate limit.
 - Both synchronous and asynchronous APIs for accessing BAV data.
 
 ## Documentation
 
 Read more about `bavapi` in the [documentation](https://wppbav.github.io/bavapi-sdk-python/).
```

### Comparing `wpp-bavapi-1.0.4/bavapi/__init__.py` & `wpp_bavapi-1.1.0/bavapi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 >>> async with bavapi.Client("TOKEN") as bav:
 ...     result = await bav.brands(name="Facebook")
 """
 
 # pylint: disable=R0801
 
 from bavapi import filters
+from bavapi import tools
 from bavapi.client import Client
 from bavapi.exceptions import APIError, DataNotFoundError, RateLimitExceededError
 from bavapi.query import Query
 from bavapi.sync import (
     audiences,
+    audience_groups,
     brand_metric_groups,
     brand_metrics,
     brands,
     brandscape_data,
     categories,
     cities,
     collections,
@@ -47,14 +49,15 @@
     sectors,
     studies,
     years,
 )
 
 __all__ = (
     "audiences",
+    "audience_groups",
     "brand_metrics",
     "brand_metric_groups",
     "brands",
     "brandscape_data",
     "categories",
     "cities",
     "collections",
@@ -64,11 +67,12 @@
     "raw_query",
     "sectors",
     "studies",
     "years",
     "Client",
     "Query",
     "filters",
+    "tools",
     "APIError",
     "DataNotFoundError",
     "RateLimitExceededError",
 )
```

### Comparing `wpp-bavapi-1.0.4/bavapi/_batched.py` & `wpp_bavapi-1.1.0/bavapi/_batched.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/_fetcher.py` & `wpp_bavapi-1.1.0/bavapi/_fetcher.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/_jupyter.py` & `wpp_bavapi-1.1.0/bavapi/_jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/_reference/generate_reference.py` & `wpp_bavapi-1.1.0/bavapi/_reference/generate_reference.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/client.py` & `wpp_bavapi-1.1.0/bavapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     Type,
     TypeVar,
     Union,
     overload,
 )
 
 from bavapi import filters as _filters
+from bavapi.config import BASE_URL, USER_AGENT
 from bavapi.http import HTTPClient
 from bavapi.parsing.responses import parse_response
 from bavapi.query import Query
 from bavapi.typing import (
     CommonQueryParams,
     JSONDict,
     OptionalListOr,
@@ -63,17 +64,14 @@
 if TYPE_CHECKING:
     from types import TracebackType
 
     from pandas import DataFrame
 
 __all__ = ("Client",)
 
-BASE_URL: Final[str] = "https://fount.wppbav.com/api/v2/"
-USER_AGENT: Final[str] = "BAVAPI SDK Python"
-
 BRANDSCAPE_DEFAULTS: Final[List[str]] = ["study", "brand", "category", "audience"]
 CATEGORIES_DEFAULTS: Final[List[str]] = ["sector"]
 
 F = TypeVar("F", bound=_filters.FountFilters)
 
 OptionalFiltersOrMapping = Optional[_filters.FiltersOrMapping[F]]
 
@@ -794,15 +792,15 @@
         This endpoint requires at least one of the following combinations of filters:
 
         - Study + Audience + Brand + Category
         - Country + Year + Audience
         - Brand + Audience + Country + Year
 
         You should read these from left to right. A combination of "Study + Audience"
-        worksjust as well as "Study + Audience + Brand".
+        works just as well as "Study + Audience + Brand".
         However, "Category + Audience" will not.
 
         If you use Country or Year filters, you must use both filters together.
 
         An audience filter is also highly recommended, as otherwise the API will return
         data for all audiences (there are more than 100 standard audiences).
```

### Comparing `wpp-bavapi-1.0.4/bavapi/filters.py` & `wpp_bavapi-1.1.0/bavapi/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 >>> bavapi.brands("TOKEN", filters=bavapi.filters.CategoriesFilters(country_codes="UK"))
 
 The above example may work, but it is highly discouraged.
 """
 
 # pylint: disable=no-name-in-module, too-few-public-methods
 
+# import warnings
 from typing import Dict, Literal, Optional, Type, TypeVar, Union
 
 from pydantic import BaseModel, field_validator, model_validator
 
 from bavapi.parsing.params import parse_date
 from bavapi.typing import (
     DTValues,
@@ -51,14 +52,16 @@
     "StudiesFilters",
 )
 
 F = TypeVar("F", bound="FountFilters")
 
 FiltersOrMapping = Union[F, InputParamsMapping]
 
+# warnings.filterwarnings("default", category=DeprecationWarning, module="bavapi")
+
 
 class FountFilters(BaseModel):
     """Base class for Fount API Filters.
 
     Can be used with `raw_query` endpoints.
 
     Attributes
@@ -105,14 +108,22 @@
             `FountFilters` class or `None` if `filters` is `None`
             and no additional filters are passed.
         """
         new_filters: Dict[str, InputSequenceOrValues] = {
             k: v for k, v in addl_filters.items() if v
         }
 
+        # if addl_filters:
+        #     warnings.warn(
+        #         f"Using the {list(new_filters.keys())} function parameter(s) is deprecated. "
+        #         f"Use the `filters` parameter with a {cls.__name__} instance instead.",
+        #         DeprecationWarning,
+        #         2,
+        #     )
+
         if filters is None:
             if not new_filters:
                 return None
             return cls(**new_filters)  # type: ignore[arg-type]
 
         if isinstance(filters, FountFilters):
             if not new_filters:
```

### Comparing `wpp-bavapi-1.0.4/bavapi/http.py` & `wpp_bavapi-1.1.0/bavapi/http.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/parsing/params.py` & `wpp_bavapi-1.1.0/bavapi/parsing/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Functions to parse parameter values."""
 
 import datetime as dt
 from typing import Dict, Mapping, Sequence, TypeVar, Union, cast
 
-from bavapi.typing import BaseMutableParamsMapping, BaseMutableParamsMappingValues
+from bavapi.typing import MutableParamsMapping, SequenceOrValues
 
 T = TypeVar("T")
 
 
 def parse_date(value: Union[str, dt.datetime, dt.date]) -> str:
     """Parse date string or datetime value into a date string.
 
@@ -52,15 +52,17 @@
     -------
     dict[str, Any]
         Fount API parameter dictionary.
     """
     return {f"{param}[{k}]": v for k, v in data.items()}
 
 
-def list_to_str(mapping: BaseMutableParamsMapping) -> BaseMutableParamsMappingValues:
+def list_to_str(
+    mapping: MutableParamsMapping[SequenceOrValues[Union[T, str]]]
+) -> MutableParamsMapping[Union[T, str]]:
     """Convert any lists in a dictionary to a string with comma-separated elements.
 
     Parameters
     ----------
     mapping : ParamsMapping
         Dictionary with lists
 
@@ -69,8 +71,8 @@
     ParamsMappingValues
         Dictionary with lists converted to comma-separated strings
     """
     for key, value in mapping.items():
         if not isinstance(value, str) and isinstance(value, Sequence):
             mapping[key] = ",".join(str(i) for i in value)
 
-    return cast(BaseMutableParamsMappingValues, mapping)
+    return cast(MutableParamsMapping[Union[T, str]], mapping)
```

### Comparing `wpp-bavapi-1.0.4/bavapi/parsing/responses.py` & `wpp_bavapi-1.1.0/bavapi/parsing/responses.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/query.py` & `wpp_bavapi-1.1.0/bavapi/query.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/bavapi/sync.py` & `wpp_bavapi-1.1.0/bavapi/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,15 +749,15 @@
     This endpoint requires at least one of the following combinations of parameters:
 
     - Study + Audience + Brand + Category
     - Country + Year + Audience
     - Brand + Audience + Country + Year
 
     You should read these from left to right. A combination of "Study + Audience"
-    worksjust as well as "Study + Audience + Brand".
+    works just as well as "Study + Audience + Brand".
     However, "Category + Audience" will not.
 
     If you use Country or Year filters, you must use both filters together.
 
     An audience filter is also highly recommended, as otherwise the API will return
     data for all audiences (there are more than 100 standard audiences).
```

### Comparing `wpp-bavapi-1.0.4/bavapi/typing.py` & `wpp_bavapi-1.1.0/bavapi/typing.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/pyproject.toml` & `wpp_bavapi-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wpp-bavapi"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
     { name = "Ignacio Maiz Vilches", email = "ignacio.maiz@bavgroup.com" },
 ]
 description = "Python consumer for the WPPBAV Fount API."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `wpp-bavapi-1.0.4/tests/test_client.py` & `wpp_bavapi-1.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_fetcher.py` & `wpp_bavapi-1.1.0/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_filters.py` & `wpp_bavapi-1.1.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_helpers.py` & `wpp_bavapi-1.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_http.py` & `wpp_bavapi-1.1.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_jupyter.py` & `wpp_bavapi-1.1.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_query.py` & `wpp_bavapi-1.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/tests/test_sync.py` & `wpp_bavapi-1.1.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `wpp-bavapi-1.0.4/wpp_bavapi.egg-info/PKG-INFO` & `wpp_bavapi-1.1.0/wpp_bavapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpp-bavapi
-Version: 1.0.4
+Version: 1.1.0
 Summary: Python consumer for the WPPBAV Fount API.
 Author-email: Ignacio Maiz Vilches <ignacio.maiz@bavgroup.com>
 License: Apache 2.0
 Project-URL: homepage, https://wppbav.github.io/bavapi-sdk-python/
 Project-URL: repository, https://github.com/wppbav/wpp-bavapi/
 Project-URL: api_reference, https://developer.wppbav.com/docs/2.x/intro
 Keywords: wpp-bavapi,bavapi,bavgroup,bav,brandasset,brandassetvaluator,wppbav,wpp,fount
@@ -127,27 +127,29 @@
 | ... | ...       | ...                   | ...  | ...    | ... |
 
 ## Features
 
 - Support for all endpoints in the WPPBAV Fount API.
   - Extended support for the following endpoints:
     - `audiences`
+    - `audience-groups`
     - `brand-metrics`
     - `brand-metric-groups`
     - `brands`
     - `brandscape-data`
     - `categories`
     - `cities`
     - `collections`
     - `companies`
     - `countries`
     - `sectors`
     - `studies`
     - `years`
   - Other endpoints are available via the `raw_query` functions and methods.
+  - Extended support for Fount API Tools/TurboPitch endpoints.
 - Validates query parameters are of the correct types and provides type hints for better IDE support.
 - Retrieve multiple pages of data simultaneously, monitoring and preventing exceeding API rate limit.
 - Both synchronous and asynchronous APIs for accessing BAV data.
 
 ## Documentation
 
 Read more about `bavapi` in the [documentation](https://wppbav.github.io/bavapi-sdk-python/).
```

### Comparing `wpp-bavapi-1.0.4/wpp_bavapi.egg-info/SOURCES.txt` & `wpp_bavapi-1.1.0/wpp_bavapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 README.md
 pyproject.toml
 bavapi/__init__.py
 bavapi/_batched.py
 bavapi/_fetcher.py
 bavapi/_jupyter.py
 bavapi/client.py
+bavapi/config.py
 bavapi/exceptions.py
 bavapi/filters.py
 bavapi/http.py
 bavapi/py.typed
 bavapi/query.py
 bavapi/sync.py
+bavapi/tools.py
 bavapi/typing.py
 bavapi/_reference/__init__.py
 bavapi/_reference/generate_reference.py
 bavapi/_reference/int_enum.py
 bavapi/parsing/__init__.py
 bavapi/parsing/params.py
 bavapi/parsing/responses.py
@@ -25,13 +27,14 @@
 tests/test_filters.py
 tests/test_helpers.py
 tests/test_http.py
 tests/test_integration.py
 tests/test_jupyter.py
 tests/test_query.py
 tests/test_sync.py
+tests/test_tools.py
 wpp_bavapi.egg-info/PKG-INFO
 wpp_bavapi.egg-info/SOURCES.txt
 wpp_bavapi.egg-info/dependency_links.txt
 wpp_bavapi.egg-info/entry_points.txt
 wpp_bavapi.egg-info/requires.txt
 wpp_bavapi.egg-info/top_level.txt
```

