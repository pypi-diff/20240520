# Comparing `tmp/airbyte_source_iterable-0.5.1.dev202405182050.tar.gz` & `tmp/airbyte_source_iterable-0.5.1.dev202405190244.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_iterable-0.5.1.dev202405182050.tar", max compression
+gzip compressed data, was "airbyte_source_iterable-0.5.1.dev202405190244.tar", max compression
```

## Comparing `airbyte_source_iterable-0.5.1.dev202405182050.tar` & `airbyte_source_iterable-0.5.1.dev202405190244.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4542 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/README.md
--rw-r--r--   0        0        0      887 2024-05-18 20:50:51.764643 airbyte_source_iterable-0.5.1.dev202405182050/pyproject.toml
--rw-r--r--   0        0        0       65 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/__init__.py
--rw-r--r--   0        0        0     1374 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/components.py
--rw-r--r--   0        0        0    13996 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/run.py
--rw-r--r--   0        0        0     2494 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/campaigns.json
--rw-r--r--   0        0        0      168 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/campaigns_metrics.json
--rw-r--r--   0        0        0      605 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/channels.json
--rw-r--r--   0        0        0     1755 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_bounce.json
--rw-r--r--   0        0        0     2749 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_click.json
--rw-r--r--   0        0        0     1704 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_complaint.json
--rw-r--r--   0        0        0     2257 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_open.json
--rw-r--r--   0        0        0     5994 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_send.json
--rw-r--r--   0        0        0     6124 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_send_skip.json
--rw-r--r--   0        0        0     1773 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_subscribe.json
--rw-r--r--   0        0        0     2665 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_unsubscribe.json
--rw-r--r--   0        0        0     1193 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/events.json
--rw-r--r--   0        0        0      307 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/list_users.json
--rw-r--r--   0        0        0      521 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/lists.json
--rw-r--r--   0        0        0      437 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/message_types.json
--rw-r--r--   0        0        0      158 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/metadata.json
--rw-r--r--   0        0        0     1156 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/templates.json
--rw-r--r--   0        0        0    14569 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/users.json
--rw-r--r--   0        0        0     6482 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/slice_generators.py
--rw-r--r--   0        0        0     4537 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/source.py
--rw-r--r--   0        0        0     1009 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/spec.json
--rw-r--r--   0        0        0    19468 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/streams.py
--rw-r--r--   0        0        0      649 2024-05-17 23:09:36.000000 airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/utils.py
--rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 airbyte_source_iterable-0.5.1.dev202405182050/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/README.md
+-rw-r--r--   0        0        0      887 2024-05-19 02:44:32.061132 airbyte_source_iterable-0.5.1.dev202405190244/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/__init__.py
+-rw-r--r--   0        0        0     1374 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/components.py
+-rw-r--r--   0        0        0    13996 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/run.py
+-rw-r--r--   0        0        0     2494 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/campaigns.json
+-rw-r--r--   0        0        0      168 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/campaigns_metrics.json
+-rw-r--r--   0        0        0      605 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/channels.json
+-rw-r--r--   0        0        0     1755 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_bounce.json
+-rw-r--r--   0        0        0     2749 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_click.json
+-rw-r--r--   0        0        0     1704 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_complaint.json
+-rw-r--r--   0        0        0     2257 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_open.json
+-rw-r--r--   0        0        0     5994 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_send.json
+-rw-r--r--   0        0        0     6124 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_send_skip.json
+-rw-r--r--   0        0        0     1773 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_subscribe.json
+-rw-r--r--   0        0        0     2665 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_unsubscribe.json
+-rw-r--r--   0        0        0     1193 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/events.json
+-rw-r--r--   0        0        0      307 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/list_users.json
+-rw-r--r--   0        0        0      521 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/lists.json
+-rw-r--r--   0        0        0      437 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/message_types.json
+-rw-r--r--   0        0        0      158 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/metadata.json
+-rw-r--r--   0        0        0     1156 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/templates.json
+-rw-r--r--   0        0        0    14569 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/users.json
+-rw-r--r--   0        0        0     6482 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/slice_generators.py
+-rw-r--r--   0        0        0     4537 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/source.py
+-rw-r--r--   0        0        0     1009 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/spec.json
+-rw-r--r--   0        0        0    19468 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/streams.py
+-rw-r--r--   0        0        0      649 2024-05-19 02:40:58.989436 airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/utils.py
+-rw-r--r--   0        0        0     5378 1970-01-01 00:00:00.000000 airbyte_source_iterable-0.5.1.dev202405190244/PKG-INFO
```

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/README.md` & `airbyte_source_iterable-0.5.1.dev202405190244/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/pyproject.toml` & `airbyte_source_iterable-0.5.1.dev202405190244/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.1.dev202405182050"
+version = "0.5.1.dev202405190244"
 name = "airbyte-source-iterable"
 description = "Source implementation for Iterable."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/components.py` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/manifest.yaml` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/campaigns.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/channels.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/channels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_bounce.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_bounce.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_click.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_click.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_complaint.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_complaint.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_open.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_open.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_send.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_send.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_send_skip.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_send_skip.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_subscribe.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_subscribe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/email_unsubscribe.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/email_unsubscribe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/events.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/lists.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/templates.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/schemas/users.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/slice_generators.py` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/slice_generators.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/source.py` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/spec.json` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/streams.py` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/source_iterable/utils.py` & `airbyte_source_iterable-0.5.1.dev202405190244/source_iterable/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_iterable-0.5.1.dev202405182050/PKG-INFO` & `airbyte_source_iterable-0.5.1.dev202405190244/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-iterable
-Version: 0.5.1.dev202405182050
+Version: 0.5.1.dev202405190244
 Summary: Source implementation for Iterable.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

