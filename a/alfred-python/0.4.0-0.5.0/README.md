# Comparing `tmp/alfred_python-0.4.0.tar.gz` & `tmp/alfred_python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_python-0.4.0.tar", last modified: Tue May 14 23:43:37 2024, max compression
+gzip compressed data, was "alfred_python-0.5.0.tar", last modified: Mon May 20 21:07:54 2024, max compression
```

## Comparing `alfred_python-0.4.0.tar` & `alfred_python-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 23:43:29.000000 alfred_python-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-14 23:43:37.518888 alfred_python-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-14 23:43:29.000000 alfred_python-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-14 23:43:29.000000 alfred_python-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:43:37.518888 alfred_python-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.510888 alfred_python-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.510888 alfred_python-0.4.0/src/alfred/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.510888 alfred_python-0.4.0/src/alfred/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/base/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/http/typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/data_points/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/data_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/data_points/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/data_points/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/files/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/files/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/typed.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/jobs/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.514888 alfred_python-0.4.0/src/alfred/rest/sessions/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/rest/sessions/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/src/alfred/typings/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/typings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/typings/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/src/alfred/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-14 23:43:29.000000 alfred_python-0.4.0/src/alfred/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:43:37.518888 alfred_python-0.4.0/src/alfred_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 23:43:37.000000 alfred_python-0.4.0/src/alfred_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.872689 alfred_python-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 21:07:46.000000 alfred_python-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-05-20 21:07:54.872689 alfred_python-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14758 2024-05-20 21:07:46.000000 alfred_python-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.864689 alfred_python-0.5.0/alfred/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.864689 alfred_python-0.5.0/alfred/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/base/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.864689 alfred_python-0.5.0/alfred/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.864689 alfred_python-0.5.0/alfred/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/http/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.864689 alfred_python-0.5.0/alfred/realtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/realtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.864689 alfred_python-0.5.0/alfred/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.868689 alfred_python-0.5.0/alfred/rest/data_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/data_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/data_points/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/data_points/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.868689 alfred_python-0.5.0/alfred/rest/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/files/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/files/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.868689 alfred_python-0.5.0/alfred/rest/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/jobs/typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/jobs/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.868689 alfred_python-0.5.0/alfred/rest/sessions/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/rest/sessions/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.868689 alfred_python-0.5.0/alfred/typings/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/typings/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.868689 alfred_python-0.5.0/alfred/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-20 21:07:46.000000 alfred_python-0.5.0/alfred/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:07:54.872689 alfred_python-0.5.0/alfred_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-05-20 21:07:54.000000 alfred_python-0.5.0/alfred_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-20 21:07:54.000000 alfred_python-0.5.0/alfred_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:07:54.000000 alfred_python-0.5.0/alfred_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 21:07:54.000000 alfred_python-0.5.0/alfred_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 21:07:54.000000 alfred_python-0.5.0/alfred_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-20 21:07:46.000000 alfred_python-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:07:54.872689 alfred_python-0.5.0/setup.cfg
```

### Comparing `alfred_python-0.4.0/LICENSE` & `alfred_python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred_python-0.4.0/PKG-INFO` & `alfred_python-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,24 @@
-Metadata-Version: 2.1
-Name: alfred-python
-Version: 0.4.0
-Summary: Python library designed to simplify and streamline interactions with the Alfred API
-Author-email: Tagshelf LLC <support@tagshelf.com>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: homepage, https://github.com/tagshelfsrl/alfred-python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydantic>=2.0
-Requires-Dist: pydantic-settings>=2.0
-Requires-Dist: requests>=2.30
-
 # Overview
 
 Welcome to the `alfred-python` SDK, the official Python library for interfacing with Alfred, your intelligent process automation platform. This SDK provides a simple and efficient way to integrate Alfred's capabilities into your Python applications.
 
 ## Prerequisites
 
 - Python v3.8+
 
 ## Usage
 
 Check out this simple example to get up and running:
 
 ```python
 from alfred.rest import AlfredClient
-from alfred.base.config import Configuration
+from alfred.base import Configuration
 
-config = Configuration.v1()
+config = Configuration.default()
 auth_config = {"api_key": "AXXXXXXXXXXXXXXXXXXXXXX"}
 
 client = AlfredClient(config, auth_config)
 
 values = client.data_points.get_values("XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXX")
 print(values)
 ```
@@ -202,14 +167,97 @@
 - `PUT`: Updates a resource in a way that it can be repeatedly updated without changing the outcome beyond the initial application.
 - `DELETE`: Removes a resource and subsequent deletions of the same resource are redundant.
 - `HEAD`: Fetches metadata about a resource without side-effects.
 - `OPTIONS`: Retrieves supported communication options for a given URL or server without causing any side effects.
 
 For non-idempotent methods like POST and PATCH, the SDK does not perform retries by default because doing so could potentially result in unwanted side effects or duplicate operations. If you need to enable retries for these methods under specific circumstances, please handle them cautiously in your application logic.
 
+## Real-time Events
+
+The `alfred-python` library provides a way to listen to events emitted by Alfred IPA in real-time through a websockets implementation. This feature is particularly useful when you need to monitor the progress of a Job, File, or any other event that occurs within the Alfred platform. To see more information visit our [official documentation](https://docs.tagshelf.dev).
+
+### Getting started
+
+To get started, you need to create an instance of the `AlfredRealTimeClient` class.
+
+```python
+from alfred import AlfredRealTimeClient
+from alfred.base import Configuration
+from alfred import AuthConfiguration
+
+config = Configuration.default()
+
+auth_config = AuthConfiguration({
+    "api_key": "AXXXXXXXXXXXXXXXXXXXXXX"
+})
+
+client = AlfredRealTimeClient(config, auth_config, verbose=True)
+```
+
+### File Events
+These events are specifically designed to respond to a variety of actions or status changes related to Files. To see more details about File events, visit our [official documentation](https://docs.tagshelf.dev/event-api/fileevents).
+```python
+# Listen to all File events
+client.on_file_event(lambda data: print(data))
+```
+
+### Job Events
+Alfred performs asynchronous document classification, extraction, and indexing on a variety of file types. The events detailed here offer insights into how a Job progresses, fails, retries, or completes its tasks. To see more details about Job events, visit our [official documentation](https://docs.tagshelf.dev/event-api/jobevents).
+
+```python
+# Listen to all Job events
+client.on_job_event(lambda data: print(data))
+```
+
+### Specific Events
+
+This enables you to select a specific event you wish to monitor from the list of supported events.
+It's particularly useful when you want to listen to a specific event instead of all events of a particular type.
+
+Here's an example of how to listen to a specific event:
+
+```python
+from alfred.base import FileEvent, JobEvent
+
+# Listen to the specific File Done event
+client.on(FileEvent.FILE_DONE_EVENT.value, lambda data: print(data))
+
+# Listen to the specific Job Finished event
+client.on(JobEvent.JOB_FINISHED_EVENT.value, lambda data: print(data))
+```
+
+Here is a list of all supported events:
+
+| Event Type | Event Name | Description |
+| --- | --- | --- |
+| FileEvent | `FILE_ADD_TO_JOB_EVENT` | Triggered when a file is added to a job for processing. |
+| FileEvent | `FILE_CATEGORY_CREATE_EVENT` | Occurs when a new category is created for a file. |
+| FileEvent | `FILE_CATEGORY_DELETE_EVENT` | Signals the deletion of a file's category. |
+| FileEvent | `FILE_CHANGE_TAG_EVENT` | Indicates a change in the tag associated with a file. |
+| FileEvent | `FILE_DONE_EVENT` | Marks the completion of file processing. |
+| FileEvent | `FILE_EXTRACTED_DATA_CREATE_EVENT` | Triggered when new data is extracted from a file. |
+| FileEvent | `FILE_EXTRACTED_DATA_DELETE_EVENT` | Occurs when extracted data from a file is deleted. |
+| FileEvent | `FILE_FAILED_EVENT` | Indicates a failure in file processing. |
+| FileEvent | `FILE_MOVE_EVENT` | Signals the movement of a file within the system. |
+| FileEvent | `FILE_MOVE_TO_PENDING_EVENT` | Triggered when a file is moved to a pending state. |
+| FileEvent | `FILE_MOVE_TO_RECYCLE_BIN_EVENT` | Indicates movement of a file to the recycle bin. |
+| FileEvent | `FILE_PROPERTY_CREATE_EVENT` | Reflects the creation of a file property. |
+| FileEvent | `FILE_PROPERTY_DELETE_EVENT` | Signals the deletion of a file property. |
+| FileEvent | `FILE_REMOVE_TAG_EVENT` | Signals the removal of a tag from a file. |
+| FileEvent | `FILE_STATUS_UPDATE_EVENT` | Indicates an update in the file's status. |
+| FileEvent | `FILE_UPDATE_EVENT` | Triggered when a file is updated in any manner. |
+| JobEvent | `JOB_CREATE_EVENT` | Triggered when a new job is instantiated for file operations. |
+| JobEvent | `JOB_EXCEEDED_RETRIES_EVENT` | Fires when job exceeds maximum retry attempts for a stage. |
+| JobEvent | `JOB_FAILED_EVENT` | Occurs when a job halts due to an unrecoverable error. |
+| JobEvent | `JOB_FINISHED_EVENT` | Triggered when job successfully completes all workflow stages. |
+| JobEvent | `JOB_INVALID_EVENT` | Fires when job fails initial validation of input files or parameters. |
+| JobEvent | `JOB_RETRY_EVENT` | Triggered when job retries a stage after a recoverable failure. |
+| JobEvent | `JOB_STAGE_UPDATE_EVENT` | Occurs when job transitions from one workflow stage to another. |
+| JobEvent | `JOB_START_EVENT` | Triggered when job begins its workflow and state machine. |
+
 ## Development Setup
 
 ### Setting up the development environment
 
 To contribute to `alfred-python`, you'll need to set up a Python development environment. We recommend using Conda, a popular package and environment management system. Here’s how to set it up:
 
 1. **Install Conda**: If you do not have Conda installed, you can download and install it from [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (a minimal installer) or [Anaconda](https://www.anaconda.com/products/distribution) (a full-featured distribution).
```

### Comparing `alfred_python-0.4.0/pyproject.toml` & `alfred_python-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alfred-python"
-version = "0.4.0"
+version = "0.5.0"
 authors = [{ name = "Tagshelf LLC", email = "support@tagshelf.com" }]
 description = "Python library designed to simplify and streamline interactions with the Alfred API"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "pydantic >= 2.0",
   "pydantic-settings >= 2.0",
   "requests >= 2.30",
+  "python-socketio >= 5.11",
+  "websocket-client >= 1.8"
 ]
 
 [project.urls]
 homepage = "https://github.com/tagshelfsrl/alfred-python"
 
 [tool.setuptools.packages.find]
-where = ["src"]
 include = ["alfred", "alfred.*"]
```

### Comparing `alfred_python-0.4.0/src/alfred/base/config.py` & `alfred_python-0.5.0/alfred/base/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Native imports
 from typing import TypedDict, Optional, Text
 
 
 class ConfigurationDict(TypedDict):
     base_url: Text
+    realtime_url: Text
     version: int
 
 
 class OverridesDict(TypedDict):
     base_url: Optional[Text]
 
 
 class Configuration:
     @staticmethod
     def default() -> ConfigurationDict:
         """
-        Returns default client configuration. Currently targets Alfred V1.
+        Returns default client configuration. Currently, targets Alfred V1.
         """
         return Configuration.v1()
 
     @staticmethod
     def v1(overrides: Optional[OverridesDict] = None) -> ConfigurationDict:
         """
         Returns client configuration for Alfred V1.
         """
         overrides = overrides or {}
         return {
             "version": 1,
             "base_url": overrides.get("base_url", "https://app.tagshelf.com"),
+            "realtime_url": overrides.get("realtime_url", "https://sockets.tagshelf.io"),
         }
```

### Comparing `alfred_python-0.4.0/src/alfred/http/http_client.py` & `alfred_python-0.5.0/alfred/http/http_client.py`

 * *Files identical despite different names*

### Comparing `alfred_python-0.4.0/src/alfred/http/typed.py` & `alfred_python-0.5.0/alfred/http/typed.py`

 * *Files identical despite different names*

### Comparing `alfred_python-0.4.0/src/alfred/rest/__init__.py` & `alfred_python-0.5.0/alfred/rest/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Native imports
 from typing import Optional
 
 # Project imports
-from src.alfred.base.config import ConfigurationDict
-from src.alfred.http.http_client import HttpClient
-from src.alfred.http.typed import AuthConfiguration, HttpConfiguration
-from src.alfred.rest.data_points import DataPointsBase, DataPointsFactory
-from src.alfred.rest.sessions import SessionsBase, SessionsFactory
-from src.alfred.rest.jobs import JobsBase, JobsFactory
-from src.alfred.rest.files import FilesBase, FilesFactory
+from alfred.base.config import ConfigurationDict
+from alfred.http.http_client import HttpClient
+from alfred.http.typed import AuthConfiguration, HttpConfiguration
+from alfred.rest.data_points import DataPointsBase, DataPointsFactory
+from alfred.rest.sessions import SessionsBase, SessionsFactory
+from alfred.rest.jobs import JobsBase, JobsFactory
+from alfred.rest.files import FilesBase, FilesFactory
 
 
 class AlfredClient:
     __DEFAULT_HTTP_CONFIG: HttpConfiguration = {
         "max_retries": 3,
         "pool_connections": True,
         "timeout": 5,
```

### Comparing `alfred_python-0.4.0/src/alfred/rest/data_points/v1.py` & `alfred_python-0.5.0/alfred/rest/data_points/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Native imports
 from typing import Text
 
 # Project imports
-from src.alfred.http.http_client import HttpClient
-from src.alfred.rest.data_points.base import DataPointsBase
+from alfred.http.http_client import HttpClient
+from alfred.rest.data_points.base import DataPointsBase
 
 
 class DataPoints(DataPointsBase):
     def __init__(self, http_client: HttpClient):
         self.http_client = http_client
 
     def get_values(self, file_id: Text):
```

### Comparing `alfred_python-0.4.0/src/alfred/rest/files/base.py` & `alfred_python-0.5.0/alfred/rest/files/base.py`

 * *Files identical despite different names*

### Comparing `alfred_python-0.4.0/src/alfred/rest/files/typed.py` & `alfred_python-0.5.0/alfred/rest/files/typed.py`

 * *Files identical despite different names*

### Comparing `alfred_python-0.4.0/src/alfred/rest/files/v1.py` & `alfred_python-0.5.0/alfred/rest/files/v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Native imports
 import os
 import json
 from typing import Text
-from io import BufferedReader
 from urllib.parse import unquote
 
 # Project imports
-from src.alfred.rest.files.typed import *  # pylint: disable=W0401, W0614
-from src.alfred.http.http_client import HttpClient
-from src.alfred.base.exceptions import AlfredMissingArgument
+from alfred.rest.files.typed import *  # pylint: disable=W0401, W0614
+from alfred.http.http_client import HttpClient
+from alfred.base.exceptions import AlfredMissingArgument
 from .base import FilesBase
 from .typed import FileDetailsResponse
 
 
 class Files(FilesBase):
     def __init__(self, http_client: HttpClient):
         self.http_client = http_client
```

### Comparing `alfred_python-0.4.0/src/alfred/rest/jobs/v1.py` & `alfred_python-0.5.0/alfred/rest/jobs/v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Native imports
 from typing import Text
 
 # Project imports
-from src.alfred.rest.jobs.typed import CreateJobDict
-from src.alfred.http.http_client import HttpClient
-from src.alfred.rest.jobs.base import JobsBase
+from alfred.rest.jobs.typed import CreateJobDict
+from alfred.http.http_client import HttpClient
+from alfred.rest.jobs.base import JobsBase
 
 
 class Jobs(JobsBase):
     def __init__(self, http_client: HttpClient):
         self.http_client = http_client
 
     def create(self, job: CreateJobDict):
```

### Comparing `alfred_python-0.4.0/src/alfred/rest/sessions/v1.py` & `alfred_python-0.5.0/alfred/rest/sessions/v1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Native imports
 from typing import Text
 
 # Project imports
-from src.alfred.http.http_client import HttpClient
-from src.alfred.rest.sessions.base import SessionsBase
+from alfred.http.http_client import HttpClient
+from alfred.rest.sessions.base import SessionsBase
 
 
 class Sessions(SessionsBase):
     def __init__(self, http_client: HttpClient):
         self.http_client = http_client
 
     def create(self):
```

### Comparing `alfred_python-0.4.0/src/alfred/utils/logging.py` & `alfred_python-0.5.0/alfred/utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import logging
 import socket
 from logging.handlers import SysLogHandler
 from typing import Union
 
 # Project imports
-from src.alfred.typings import LoggingOptions
+from alfred.typings import LoggingOptions
 
 
 def setup_logger(options: LoggingOptions):
     """
     Set up a custom logger with JSON formatting and handler
     based on application environment.
     """
```

### Comparing `alfred_python-0.4.0/src/alfred_python.egg-info/PKG-INFO` & `alfred_python-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python library designed to simplify and streamline interactions with the Alfred API
 Author-email: Tagshelf LLC <support@tagshelf.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,14 +28,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: requests>=2.30
+Requires-Dist: python-socketio>=5.11
+Requires-Dist: websocket-client>=1.8
 
 # Overview
 
 Welcome to the `alfred-python` SDK, the official Python library for interfacing with Alfred, your intelligent process automation platform. This SDK provides a simple and efficient way to integrate Alfred's capabilities into your Python applications.
 
 ## Prerequisites
 
@@ -43,17 +45,17 @@
 
 ## Usage
 
 Check out this simple example to get up and running:
 
 ```python
 from alfred.rest import AlfredClient
-from alfred.base.config import Configuration
+from alfred.base import Configuration
 
-config = Configuration.v1()
+config = Configuration.default()
 auth_config = {"api_key": "AXXXXXXXXXXXXXXXXXXXXXX"}
 
 client = AlfredClient(config, auth_config)
 
 values = client.data_points.get_values("XXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXX")
 print(values)
 ```
@@ -202,14 +204,97 @@
 - `PUT`: Updates a resource in a way that it can be repeatedly updated without changing the outcome beyond the initial application.
 - `DELETE`: Removes a resource and subsequent deletions of the same resource are redundant.
 - `HEAD`: Fetches metadata about a resource without side-effects.
 - `OPTIONS`: Retrieves supported communication options for a given URL or server without causing any side effects.
 
 For non-idempotent methods like POST and PATCH, the SDK does not perform retries by default because doing so could potentially result in unwanted side effects or duplicate operations. If you need to enable retries for these methods under specific circumstances, please handle them cautiously in your application logic.
 
+## Real-time Events
+
+The `alfred-python` library provides a way to listen to events emitted by Alfred IPA in real-time through a websockets implementation. This feature is particularly useful when you need to monitor the progress of a Job, File, or any other event that occurs within the Alfred platform. To see more information visit our [official documentation](https://docs.tagshelf.dev).
+
+### Getting started
+
+To get started, you need to create an instance of the `AlfredRealTimeClient` class.
+
+```python
+from alfred import AlfredRealTimeClient
+from alfred.base import Configuration
+from alfred import AuthConfiguration
+
+config = Configuration.default()
+
+auth_config = AuthConfiguration({
+    "api_key": "AXXXXXXXXXXXXXXXXXXXXXX"
+})
+
+client = AlfredRealTimeClient(config, auth_config, verbose=True)
+```
+
+### File Events
+These events are specifically designed to respond to a variety of actions or status changes related to Files. To see more details about File events, visit our [official documentation](https://docs.tagshelf.dev/event-api/fileevents).
+```python
+# Listen to all File events
+client.on_file_event(lambda data: print(data))
+```
+
+### Job Events
+Alfred performs asynchronous document classification, extraction, and indexing on a variety of file types. The events detailed here offer insights into how a Job progresses, fails, retries, or completes its tasks. To see more details about Job events, visit our [official documentation](https://docs.tagshelf.dev/event-api/jobevents).
+
+```python
+# Listen to all Job events
+client.on_job_event(lambda data: print(data))
+```
+
+### Specific Events
+
+This enables you to select a specific event you wish to monitor from the list of supported events.
+It's particularly useful when you want to listen to a specific event instead of all events of a particular type.
+
+Here's an example of how to listen to a specific event:
+
+```python
+from alfred.base import FileEvent, JobEvent
+
+# Listen to the specific File Done event
+client.on(FileEvent.FILE_DONE_EVENT.value, lambda data: print(data))
+
+# Listen to the specific Job Finished event
+client.on(JobEvent.JOB_FINISHED_EVENT.value, lambda data: print(data))
+```
+
+Here is a list of all supported events:
+
+| Event Type | Event Name | Description |
+| --- | --- | --- |
+| FileEvent | `FILE_ADD_TO_JOB_EVENT` | Triggered when a file is added to a job for processing. |
+| FileEvent | `FILE_CATEGORY_CREATE_EVENT` | Occurs when a new category is created for a file. |
+| FileEvent | `FILE_CATEGORY_DELETE_EVENT` | Signals the deletion of a file's category. |
+| FileEvent | `FILE_CHANGE_TAG_EVENT` | Indicates a change in the tag associated with a file. |
+| FileEvent | `FILE_DONE_EVENT` | Marks the completion of file processing. |
+| FileEvent | `FILE_EXTRACTED_DATA_CREATE_EVENT` | Triggered when new data is extracted from a file. |
+| FileEvent | `FILE_EXTRACTED_DATA_DELETE_EVENT` | Occurs when extracted data from a file is deleted. |
+| FileEvent | `FILE_FAILED_EVENT` | Indicates a failure in file processing. |
+| FileEvent | `FILE_MOVE_EVENT` | Signals the movement of a file within the system. |
+| FileEvent | `FILE_MOVE_TO_PENDING_EVENT` | Triggered when a file is moved to a pending state. |
+| FileEvent | `FILE_MOVE_TO_RECYCLE_BIN_EVENT` | Indicates movement of a file to the recycle bin. |
+| FileEvent | `FILE_PROPERTY_CREATE_EVENT` | Reflects the creation of a file property. |
+| FileEvent | `FILE_PROPERTY_DELETE_EVENT` | Signals the deletion of a file property. |
+| FileEvent | `FILE_REMOVE_TAG_EVENT` | Signals the removal of a tag from a file. |
+| FileEvent | `FILE_STATUS_UPDATE_EVENT` | Indicates an update in the file's status. |
+| FileEvent | `FILE_UPDATE_EVENT` | Triggered when a file is updated in any manner. |
+| JobEvent | `JOB_CREATE_EVENT` | Triggered when a new job is instantiated for file operations. |
+| JobEvent | `JOB_EXCEEDED_RETRIES_EVENT` | Fires when job exceeds maximum retry attempts for a stage. |
+| JobEvent | `JOB_FAILED_EVENT` | Occurs when a job halts due to an unrecoverable error. |
+| JobEvent | `JOB_FINISHED_EVENT` | Triggered when job successfully completes all workflow stages. |
+| JobEvent | `JOB_INVALID_EVENT` | Fires when job fails initial validation of input files or parameters. |
+| JobEvent | `JOB_RETRY_EVENT` | Triggered when job retries a stage after a recoverable failure. |
+| JobEvent | `JOB_STAGE_UPDATE_EVENT` | Occurs when job transitions from one workflow stage to another. |
+| JobEvent | `JOB_START_EVENT` | Triggered when job begins its workflow and state machine. |
+
 ## Development Setup
 
 ### Setting up the development environment
 
 To contribute to `alfred-python`, you'll need to set up a Python development environment. We recommend using Conda, a popular package and environment management system. Here’s how to set it up:
 
 1. **Install Conda**: If you do not have Conda installed, you can download and install it from [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (a minimal installer) or [Anaconda](https://www.anaconda.com/products/distribution) (a full-featured distribution).
```

### Comparing `alfred_python-0.4.0/src/alfred_python.egg-info/SOURCES.txt` & `alfred_python-0.5.0/alfred_python.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 LICENSE
 README.md
 pyproject.toml
-src/alfred/__init__.py
-src/alfred/base/__init__.py
-src/alfred/base/config.py
-src/alfred/base/constants.py
-src/alfred/base/exceptions.py
-src/alfred/http/__init__.py
-src/alfred/http/http_client.py
-src/alfred/http/typed.py
-src/alfred/rest/__init__.py
-src/alfred/rest/data_points/__init__.py
-src/alfred/rest/data_points/base.py
-src/alfred/rest/data_points/v1.py
-src/alfred/rest/files/__init__.py
-src/alfred/rest/files/base.py
-src/alfred/rest/files/typed.py
-src/alfred/rest/files/v1.py
-src/alfred/rest/jobs/__init__.py
-src/alfred/rest/jobs/base.py
-src/alfred/rest/jobs/typed.py
-src/alfred/rest/jobs/v1.py
-src/alfred/rest/sessions/__init__.py
-src/alfred/rest/sessions/base.py
-src/alfred/rest/sessions/v1.py
-src/alfred/typings/__init__.py
-src/alfred/typings/misc.py
-src/alfred/utils/__init__.py
-src/alfred/utils/logging.py
-src/alfred_python.egg-info/PKG-INFO
-src/alfred_python.egg-info/SOURCES.txt
-src/alfred_python.egg-info/dependency_links.txt
-src/alfred_python.egg-info/requires.txt
-src/alfred_python.egg-info/top_level.txt
+alfred/__init__.py
+alfred/base/__init__.py
+alfred/base/config.py
+alfred/base/constants.py
+alfred/base/exceptions.py
+alfred/exceptions/__init__.py
+alfred/http/__init__.py
+alfred/http/http_client.py
+alfred/http/typed.py
+alfred/realtime/__init__.py
+alfred/rest/__init__.py
+alfred/rest/data_points/__init__.py
+alfred/rest/data_points/base.py
+alfred/rest/data_points/v1.py
+alfred/rest/files/__init__.py
+alfred/rest/files/base.py
+alfred/rest/files/typed.py
+alfred/rest/files/v1.py
+alfred/rest/jobs/__init__.py
+alfred/rest/jobs/base.py
+alfred/rest/jobs/typed.py
+alfred/rest/jobs/v1.py
+alfred/rest/sessions/__init__.py
+alfred/rest/sessions/base.py
+alfred/rest/sessions/v1.py
+alfred/typings/__init__.py
+alfred/typings/misc.py
+alfred/utils/__init__.py
+alfred/utils/logging.py
+alfred_python.egg-info/PKG-INFO
+alfred_python.egg-info/SOURCES.txt
+alfred_python.egg-info/dependency_links.txt
+alfred_python.egg-info/requires.txt
+alfred_python.egg-info/top_level.txt
```

