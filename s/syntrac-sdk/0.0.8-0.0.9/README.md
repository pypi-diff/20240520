# Comparing `tmp/syntrac_sdk-0.0.8.tar.gz` & `tmp/syntrac_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_sdk-0.0.8.tar", max compression
+gzip compressed data, was "syntrac_sdk-0.0.9.tar", max compression
```

## Comparing `syntrac_sdk-0.0.8.tar` & `syntrac_sdk-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      395 2024-05-14 12:30:48.102957 syntrac_sdk-0.0.8/README.md
--rw-r--r--   0        0        0     2072 2024-05-14 12:30:48.124836 syntrac_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-14 12:30:48.105917 syntrac_sdk-0.0.8/syntrac/sdk/.DS_Store
--rw-r--r--   0        0        0     6417 2024-05-14 12:30:48.106063 syntrac_sdk-0.0.8/syntrac/sdk/__init__.py
--rw-r--r--   0        0        0      358 2024-05-14 12:30:48.107769 syntrac_sdk-0.0.8/syntrac/sdk/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-05-14 12:30:48.108356 syntrac_sdk-0.0.8/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2024-05-14 12:30:48.108821 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__init__.py
--rw-r--r--   0        0        0      491 2024-05-14 12:30:48.109245 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3126 2024-05-14 12:30:48.109542 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc
--rw-r--r--   0        0        0    10195 2024-05-14 12:30:48.109740 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     9276 2024-05-14 12:30:48.110033 syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1571 2024-05-14 12:30:48.110356 syntrac_sdk-0.0.8/syntrac/sdk/decorators/helper.py
--rw-r--r--   0        0        0     7917 2024-05-14 12:30:48.110510 syntrac_sdk-0.0.8/syntrac/sdk/decorators/task.py
--rw-r--r--   0        0        0     7099 2024-05-14 12:30:48.110724 syntrac_sdk-0.0.8/syntrac/sdk/decorators/workflow.py
--rw-r--r--   0        0        0     2650 2024-05-14 12:30:48.110901 syntrac_sdk-0.0.8/syntrac/sdk/fetcher.py
--rw-r--r--   0        0        0      465 2024-05-14 12:30:48.111145 syntrac_sdk-0.0.8/syntrac/sdk/instruments.py
--rw-r--r--   0        0        0        0 2024-05-14 12:30:48.111345 syntrac_sdk-0.0.8/syntrac/sdk/metrics/__init__.py
--rw-r--r--   0        0        0      202 2024-05-14 12:30:48.111991 syntrac_sdk-0.0.8/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3362 2024-05-14 12:30:48.112212 syntrac_sdk-0.0.8/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2109 2024-05-14 12:30:48.112451 syntrac_sdk-0.0.8/syntrac/sdk/metrics/metrics.py
--rw-r--r--   0        0        0     2721 2024-05-14 12:30:48.112861 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__init__.py
--rw-r--r--   0        0        0     2638 2024-05-14 12:30:48.113182 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      225 2024-05-14 12:30:48.113319 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     7791 2024-05-14 12:30:48.113644 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__init__.py
--rw-r--r--   0        0        0    10408 2024-05-14 12:30:48.113862 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      607 2024-05-14 12:30:48.114183 syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/version.py
--rw-r--r--   0        0        0     2424 2024-05-14 12:30:48.114441 syntrac_sdk-0.0.8/syntrac/sdk/telemetry.py
--rw-r--r--   0        0        0     6148 2024-05-14 12:30:48.114817 syntrac_sdk-0.0.8/syntrac/sdk/tracing/.DS_Store
--rw-r--r--   0        0        0      302 2024-05-14 12:30:48.114945 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      650 2024-05-14 12:30:48.115162 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1969 2024-05-14 12:30:48.115395 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0     4806 2024-05-14 12:30:48.115527 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc
--rw-r--r--   0        0        0      877 2024-05-14 12:30:48.115774 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0      818 2024-05-14 12:30:48.116022 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
--rw-r--r--   0        0        0     2748 2024-05-14 12:30:48.116171 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc
--rw-r--r--   0        0        0    27176 2024-05-14 12:30:48.116356 syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-05-14 12:30:48.116607 syntrac_sdk-0.0.8/syntrac/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0     2509 2024-05-14 12:30:48.116737 syntrac_sdk-0.0.8/syntrac/sdk/tracing/context.py
--rw-r--r--   0        0        0      297 2024-05-14 12:30:48.116963 syntrac_sdk-0.0.8/syntrac/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0      322 2024-05-14 12:30:48.117283 syntrac_sdk-0.0.8/syntrac/sdk/tracing/context_passing.py
--rw-r--r--   0        0        0     1880 2024-05-14 12:30:48.117414 syntrac_sdk-0.0.8/syntrac/sdk/tracing/span_from_context.py
--rw-r--r--   0        0        0    22336 2024-05-14 12:30:48.117769 syntrac_sdk-0.0.8/syntrac/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      878 2024-05-14 12:30:48.118042 syntrac_sdk-0.0.8/syntrac/sdk/utils/__init__.py
--rw-r--r--   0        0        0     2171 2024-05-14 12:30:48.118253 syntrac_sdk-0.0.8/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2112 2024-05-14 12:30:48.118486 syntrac_sdk-0.0.8/syntrac/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-05-14 12:30:48.118610 syntrac_sdk-0.0.8/syntrac/sdk/version.py
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      395 2024-05-15 01:09:25.739307 syntrac_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0     2072 2024-05-15 01:09:25.775645 syntrac_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-15 01:09:25.742532 syntrac_sdk-0.0.9/syntrac/sdk/.DS_Store
+-rw-r--r--   0        0        0     6417 2024-05-15 01:09:25.742757 syntrac_sdk-0.0.9/syntrac/sdk/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-15 01:09:25.747695 syntrac_sdk-0.0.9/syntrac/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-05-15 01:09:25.748293 syntrac_sdk-0.0.9/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2024-05-15 01:09:25.748590 syntrac_sdk-0.0.9/syntrac/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-15 01:09:25.751244 syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3126 2024-05-15 01:09:25.756204 syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc
+-rw-r--r--   0        0        0    10195 2024-05-15 01:09:25.757879 syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     9276 2024-05-15 01:09:25.758161 syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1571 2024-05-15 01:09:25.758488 syntrac_sdk-0.0.9/syntrac/sdk/decorators/helper.py
+-rw-r--r--   0        0        0     7917 2024-05-15 01:09:25.758695 syntrac_sdk-0.0.9/syntrac/sdk/decorators/task.py
+-rw-r--r--   0        0        0     7099 2024-05-15 01:09:25.759183 syntrac_sdk-0.0.9/syntrac/sdk/decorators/workflow.py
+-rw-r--r--   0        0        0     2650 2024-05-15 01:09:25.759533 syntrac_sdk-0.0.9/syntrac/sdk/fetcher.py
+-rw-r--r--   0        0        0      465 2024-05-15 01:09:25.759815 syntrac_sdk-0.0.9/syntrac/sdk/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:09:25.760114 syntrac_sdk-0.0.9/syntrac/sdk/metrics/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-15 01:09:25.760722 syntrac_sdk-0.0.9/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3362 2024-05-15 01:09:25.761006 syntrac_sdk-0.0.9/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2109 2024-05-15 01:09:25.761286 syntrac_sdk-0.0.9/syntrac/sdk/metrics/metrics.py
+-rw-r--r--   0        0        0     2721 2024-05-15 01:09:25.761785 syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/__init__.py
+-rw-r--r--   0        0        0     2638 2024-05-15 01:09:25.762407 syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      225 2024-05-15 01:09:25.762727 syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     7791 2024-05-15 01:09:25.763361 syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/trace_exporter/__init__.py
+-rw-r--r--   0        0        0    10408 2024-05-15 01:09:25.763677 syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      607 2024-05-15 01:09:25.763892 syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/version.py
+-rw-r--r--   0        0        0     2424 2024-05-15 01:09:25.764208 syntrac_sdk-0.0.9/syntrac/sdk/telemetry.py
+-rw-r--r--   0        0        0     6148 2024-05-15 01:09:25.764559 syntrac_sdk-0.0.9/syntrac/sdk/tracing/.DS_Store
+-rw-r--r--   0        0        0      302 2024-05-15 01:09:25.764715 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      650 2024-05-15 01:09:25.765185 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1969 2024-05-15 01:09:25.765497 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0     4806 2024-05-15 01:09:25.765648 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2024-05-15 01:09:25.766071 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0      818 2024-05-15 01:09:25.766429 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc
+-rw-r--r--   0        0        0     2748 2024-05-15 01:09:25.766579 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc
+-rw-r--r--   0        0        0    27176 2024-05-15 01:09:25.766792 syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-05-15 01:09:25.767108 syntrac_sdk-0.0.9/syntrac/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0     2509 2024-05-15 01:09:25.767260 syntrac_sdk-0.0.9/syntrac/sdk/tracing/context.py
+-rw-r--r--   0        0        0      297 2024-05-15 01:09:25.767498 syntrac_sdk-0.0.9/syntrac/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0      322 2024-05-15 01:09:25.767902 syntrac_sdk-0.0.9/syntrac/sdk/tracing/context_passing.py
+-rw-r--r--   0        0        0     1880 2024-05-15 01:09:25.768039 syntrac_sdk-0.0.9/syntrac/sdk/tracing/span_from_context.py
+-rw-r--r--   0        0        0    22833 2024-05-15 01:09:25.768398 syntrac_sdk-0.0.9/syntrac/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      878 2024-05-15 01:09:25.768812 syntrac_sdk-0.0.9/syntrac/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2024-05-15 01:09:25.769273 syntrac_sdk-0.0.9/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2112 2024-05-15 01:09:25.769517 syntrac_sdk-0.0.9/syntrac/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-05-15 01:09:25.769648 syntrac_sdk-0.0.9/syntrac/sdk/version.py
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.9/PKG-INFO
```

### Comparing `syntrac_sdk-0.0.8/pyproject.toml` & `syntrac_sdk-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-sdk"
-version = "0.0.8"
+version = "0.0.9"
 description = "Syntrac Software Development Kit (SDK) for Python"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac"
 documentation = "https://syntrac.com/docs/openllmetry"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/.DS_Store` & `syntrac_sdk-0.0.9/syntrac/sdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/__init__.py` & `syntrac_sdk-0.0.9/syntrac/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/helper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/decorators/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/decorators/helper.py` & `syntrac_sdk-0.0.9/syntrac/sdk/decorators/helper.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/decorators/task.py` & `syntrac_sdk-0.0.9/syntrac/sdk/decorators/task.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/decorators/workflow.py` & `syntrac_sdk-0.0.9/syntrac/sdk/decorators/workflow.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/fetcher.py` & `syntrac_sdk-0.0.9/syntrac/sdk/fetcher.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/metrics/metrics.py` & `syntrac_sdk-0.0.9/syntrac/sdk/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__init__.py` & `syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__init__.py` & `syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/otlp/json/version.py` & `syntrac_sdk-0.0.9/syntrac/sdk/otlp/json/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/telemetry.py` & `syntrac_sdk-0.0.9/syntrac/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/.DS_Store` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/context_passing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/span_from_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/content_allow_list.py` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/context.py` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/context.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/span_from_context.py` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/span_from_context.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/tracing/tracing.py` & `syntrac_sdk-0.0.9/syntrac/sdk/tracing/tracing.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 
 class TracerWrapper(object):
     resource_attributes: dict = {}
     enable_content_tracing: bool = True
     endpoint: Optional[str] = None
     headers: Dict[str, str] = {}
+    create_new_provider: bool = False
     __resource: Resource
     __tracer_provider: TracerProvider
     __spans_processor: SpanProcessor
     __spans_processor_original_on_start: Optional[Callable] = None
     __spans_exporter: SpanExporter
     __content_allow_list: ContentAllowList
 
@@ -70,14 +71,15 @@
             obj = cls.instance = super(TracerWrapper, cls).__new__(cls)
             if not TracerWrapper.endpoint:
                 return obj
 
             obj.__resource = Resource(attributes=TracerWrapper.resource_attributes)
             obj.__tracer_provider = init_tracer_provider(
                 resource=obj.__resource
+                create_new_provider=create_new_provider
             )
             if processor:
                 Telemetry().capture("tracer:init", {"processor": "custom"})
                 obj.__spans_processor = processor
                 obj.__spans_processor_original_on_start = processor.on_start
             else:
                 if exporter:
@@ -270,14 +272,16 @@
 
         return cls.instance
 
     def exit_handler(self):
         self.flush()
 
     def _span_processor_on_start(self, span, parent_context):
+        print(Fore.RED + "span starting.")
+        print(Fore.RESET)
         set_workflow_name_from_context(span)
 
         association_properties: Any = get_association_properties()
         if association_properties is not None:
             for key, value in association_properties.items():
                 span.set_attribute(
                     f"{SpanAttributes.SYNTRAC_ASSOCIATION_PROPERTIES}.{key}", value
@@ -339,27 +343,33 @@
         {
             "api_endpoint": api_endpoint,
         },
     )
     return OTLPSpanExporter(endpoint=f"{api_endpoint}/v1/traces", headers=headers)
 
 
-def init_tracer_provider(resource: Resource) -> TracerProvider:
+def init_tracer_provider(resource: Resource, create_new_provider: bool = False) -> TracerProvider:
     provider: Optional[TracerProvider] = None
     default_provider: TracerProvider = get_tracer_provider()
 
-    if isinstance(default_provider, ProxyTracerProvider):
+    if isinstance(default_provider, ProxyTracerProvider) or (create_new_provider is True):
+        print(Fore.RED + "Create new trace provider.")
+        print(Fore.RESET)
         provider = TracerProvider(resource=resource)
         trace.set_tracer_provider(provider)
     elif not hasattr(default_provider, "add_span_processor"):
+        print(Fore.RED + "Cannot add span processor to default provider.")
+        print(Fore.RESET)
         logging.error(
             "Cannot add span processor to the default provider since it doesn't support it"
         )
         return
     else:
+        print(Fore.RED + "Using default trace provider.")
+        print(Fore.RESET)
         provider = default_provider
 
     return provider
 
 
 def init_instrumentations():
     init_openai_instrumentor()
```

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/utils/__init__.py` & `syntrac_sdk-0.0.9/syntrac/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.9/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/syntrac/sdk/utils/in_memory_span_exporter.py` & `syntrac_sdk-0.0.9/syntrac/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.8/PKG-INFO` & `syntrac_sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Syntrac Software Development Kit (SDK) for Python
 Home-page: https://github.com/syntracAI/syntrac
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

