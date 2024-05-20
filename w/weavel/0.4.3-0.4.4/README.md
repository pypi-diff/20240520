# Comparing `tmp/weavel-0.4.3.tar.gz` & `tmp/weavel-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weavel-0.4.3.tar", last modified: Thu May 16 08:44:49 2024, max compression
+gzip compressed data, was "weavel-0.4.4.tar", last modified: Mon May 20 06:18:22 2024, max compression
```

## Comparing `weavel-0.4.3.tar` & `weavel-0.4.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.451751 weavel-0.4.3/
--rw-r--r--   0 jypark     (501) staff       (20)        0 2024-01-15 02:29:57.000000 weavel-0.4.3/LICENSE
--rw-r--r--   0 jypark     (501) staff       (20)      406 2024-05-16 08:44:49.451597 weavel-0.4.3/PKG-INFO
--rw-r--r--   0 jypark     (501) staff       (20)       15 2024-02-08 04:16:27.000000 weavel-0.4.3/README.md
--rw-r--r--   0 jypark     (501) staff       (20)       38 2024-05-16 08:44:49.451801 weavel-0.4.3/setup.cfg
--rw-r--r--   0 jypark     (501) staff       (20)     1244 2024-05-16 06:20:33.000000 weavel-0.4.3/setup.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.441623 weavel-0.4.3/testapp/
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.442563 weavel-0.4.3/testapp/daily_dialog/
--rw-r--r--   0 jypark     (501) staff       (20)     9480 2024-02-06 10:50:36.000000 weavel-0.4.3/testapp/daily_dialog/run_qa_extractor.py
--rw-r--r--   0 jypark     (501) staff       (20)     8672 2024-02-06 10:50:37.000000 weavel-0.4.3/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py
--rw-r--r--   0 jypark     (501) staff       (20)     4110 2024-02-06 12:05:08.000000 weavel-0.4.3/testapp/daily_dialog/save_to_db.py
--rw-r--r--   0 jypark     (501) staff       (20)     1678 2024-05-16 06:35:48.000000 weavel-0.4.3/testapp/demo.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.443589 weavel-0.4.3/testapp/py_files/
--rw-r--r--   0 jypark     (501) staff       (20)     1065 2024-01-24 05:01:55.000000 weavel-0.4.3/testapp/py_files/duplicate_log_test.py
--rw-r--r--   0 jypark     (501) staff       (20)     1892 2024-01-30 03:05:12.000000 weavel-0.4.3/testapp/py_files/poe_test.py
--rw-r--r--   0 jypark     (501) staff       (20)     1068 2024-01-24 07:27:52.000000 weavel-0.4.3/testapp/py_files/save_mock_data.py
--rw-r--r--   0 jypark     (501) staff       (20)     1160 2024-01-24 11:29:54.000000 weavel-0.4.3/testapp/py_files/save_mock_retention_data.py
--rw-r--r--   0 jypark     (501) staff       (20)    43795 2024-03-22 07:15:41.000000 weavel-0.4.3/testapp/test.py
--rw-r--r--   0 jypark     (501) staff       (20)      278 2024-04-05 04:45:14.000000 weavel-0.4.3/testapp/test_identify.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.440219 weavel-0.4.3/venv/
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.447260 weavel-0.4.3/venv/bin/
--rwxr-xr-x   0 jypark     (501) staff       (20)     8236 2024-02-02 10:25:14.000000 weavel-0.4.3/venv/bin/pwiz.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      648 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2html.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      770 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2html4.py
--rwxr-xr-x   0 jypark     (501) staff       (20)     1105 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2html5.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      847 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2latex.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      670 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2man.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      836 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2odt.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      642 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      655 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      691 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2s5.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      927 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      656 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rst2xml.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      724 2024-01-15 02:43:20.000000 weavel-0.4.3/venv/bin/rstpep2html.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.448956 weavel-0.4.3/weavel/
--rw-r--r--   0 jypark     (501) staff       (20)      107 2024-05-16 06:20:37.000000 weavel-0.4.3/weavel/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     6063 2024-02-08 04:18:02.000000 weavel-0.4.3/weavel/_api_client.py
--rw-r--r--   0 jypark     (501) staff       (20)     1692 2024-04-05 02:11:37.000000 weavel-0.4.3/weavel/_buffer_storage.py
--rw-r--r--   0 jypark     (501) staff       (20)      211 2024-03-22 06:53:42.000000 weavel-0.4.3/weavel/_constants.py
--rw-r--r--   0 jypark     (501) staff       (20)    11046 2024-05-16 06:35:28.000000 weavel-0.4.3/weavel/_worker.py
--rw-r--r--   0 jypark     (501) staff       (20)     5957 2024-05-16 06:20:02.000000 weavel-0.4.3/weavel/client.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.450444 weavel-0.4.3/weavel/poe/
--rw-r--r--   0 jypark     (501) staff       (20)       58 2024-01-30 04:23:45.000000 weavel-0.4.3/weavel/poe/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     1749 2024-03-22 06:53:42.000000 weavel-0.4.3/weavel/poe/_poe_buffer_storage.py
--rw-r--r--   0 jypark     (501) staff       (20)     4768 2024-05-10 09:30:15.000000 weavel-0.4.3/weavel/poe/_poe_worker.py
--rw-r--r--   0 jypark     (501) staff       (20)     1300 2024-05-10 09:38:47.000000 weavel-0.4.3/weavel/poe/poe_client.py
--rw-r--r--   0 jypark     (501) staff       (20)     2736 2024-05-16 06:38:11.000000 weavel-0.4.3/weavel/types.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.451184 weavel-0.4.3/weavel/utils/
--rw-r--r--   0 jypark     (501) staff       (20)       43 2024-01-15 06:20:46.000000 weavel-0.4.3/weavel/utils/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     1134 2024-01-15 05:54:15.000000 weavel-0.4.3/weavel/utils/crypto.py
--rw-r--r--   0 jypark     (501) staff       (20)      679 2024-01-15 11:33:18.000000 weavel-0.4.3/weavel/utils/logger.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-16 08:44:49.449500 weavel-0.4.3/weavel.egg-info/
--rw-r--r--   0 jypark     (501) staff       (20)      406 2024-05-16 08:44:49.000000 weavel-0.4.3/weavel.egg-info/PKG-INFO
--rw-r--r--   0 jypark     (501) staff       (20)     1115 2024-05-16 08:44:49.000000 weavel-0.4.3/weavel.egg-info/SOURCES.txt
--rw-r--r--   0 jypark     (501) staff       (20)        1 2024-05-16 08:44:49.000000 weavel-0.4.3/weavel.egg-info/dependency_links.txt
--rw-r--r--   0 jypark     (501) staff       (20)      184 2024-05-16 08:44:49.000000 weavel-0.4.3/weavel.egg-info/requires.txt
--rw-r--r--   0 jypark     (501) staff       (20)       20 2024-05-16 08:44:49.000000 weavel-0.4.3/weavel.egg-info/top_level.txt
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.560458 weavel-0.4.4/
+-rw-r--r--   0 jypark     (501) staff       (20)        0 2024-01-15 02:29:57.000000 weavel-0.4.4/LICENSE
+-rw-r--r--   0 jypark     (501) staff       (20)      406 2024-05-20 06:18:22.560263 weavel-0.4.4/PKG-INFO
+-rw-r--r--   0 jypark     (501) staff       (20)       15 2024-02-08 04:16:27.000000 weavel-0.4.4/README.md
+-rw-r--r--   0 jypark     (501) staff       (20)       38 2024-05-20 06:18:22.560551 weavel-0.4.4/setup.cfg
+-rw-r--r--   0 jypark     (501) staff       (20)     1244 2024-05-20 06:17:55.000000 weavel-0.4.4/setup.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.545612 weavel-0.4.4/testapp/
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.546951 weavel-0.4.4/testapp/daily_dialog/
+-rw-r--r--   0 jypark     (501) staff       (20)     9480 2024-02-06 10:50:36.000000 weavel-0.4.4/testapp/daily_dialog/run_qa_extractor.py
+-rw-r--r--   0 jypark     (501) staff       (20)     8672 2024-02-06 10:50:37.000000 weavel-0.4.4/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py
+-rw-r--r--   0 jypark     (501) staff       (20)     4110 2024-02-06 12:05:08.000000 weavel-0.4.4/testapp/daily_dialog/save_to_db.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1881 2024-05-16 13:06:56.000000 weavel-0.4.4/testapp/demo.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.548835 weavel-0.4.4/testapp/py_files/
+-rw-r--r--   0 jypark     (501) staff       (20)     1065 2024-01-24 05:01:55.000000 weavel-0.4.4/testapp/py_files/duplicate_log_test.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1892 2024-01-30 03:05:12.000000 weavel-0.4.4/testapp/py_files/poe_test.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1068 2024-01-24 07:27:52.000000 weavel-0.4.4/testapp/py_files/save_mock_data.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1160 2024-01-24 11:29:54.000000 weavel-0.4.4/testapp/py_files/save_mock_retention_data.py
+-rw-r--r--   0 jypark     (501) staff       (20)    43795 2024-03-22 07:15:41.000000 weavel-0.4.4/testapp/test.py
+-rw-r--r--   0 jypark     (501) staff       (20)      278 2024-04-05 04:45:14.000000 weavel-0.4.4/testapp/test_identify.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.543042 weavel-0.4.4/venv/
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.552678 weavel-0.4.4/venv/bin/
+-rwxr-xr-x   0 jypark     (501) staff       (20)     8236 2024-02-02 10:25:14.000000 weavel-0.4.4/venv/bin/pwiz.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      648 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2html.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      770 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)     1105 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      847 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      670 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2man.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      836 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      642 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      655 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      691 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      927 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      656 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 jypark     (501) staff       (20)      724 2024-01-15 02:43:20.000000 weavel-0.4.4/venv/bin/rstpep2html.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.555568 weavel-0.4.4/weavel/
+-rw-r--r--   0 jypark     (501) staff       (20)      107 2024-05-20 06:17:55.000000 weavel-0.4.4/weavel/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     6063 2024-02-08 04:18:02.000000 weavel-0.4.4/weavel/_api_client.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1692 2024-04-05 02:11:37.000000 weavel-0.4.4/weavel/_buffer_storage.py
+-rw-r--r--   0 jypark     (501) staff       (20)      211 2024-03-22 06:53:42.000000 weavel-0.4.4/weavel/_constants.py
+-rw-r--r--   0 jypark     (501) staff       (20)    12130 2024-05-20 06:17:55.000000 weavel-0.4.4/weavel/_worker.py
+-rw-r--r--   0 jypark     (501) staff       (20)     6566 2024-05-20 06:17:55.000000 weavel-0.4.4/weavel/client.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.558626 weavel-0.4.4/weavel/poe/
+-rw-r--r--   0 jypark     (501) staff       (20)       58 2024-01-30 04:23:45.000000 weavel-0.4.4/weavel/poe/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1749 2024-03-22 06:53:42.000000 weavel-0.4.4/weavel/poe/_poe_buffer_storage.py
+-rw-r--r--   0 jypark     (501) staff       (20)     4768 2024-05-10 09:30:15.000000 weavel-0.4.4/weavel/poe/_poe_worker.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1300 2024-05-10 09:38:47.000000 weavel-0.4.4/weavel/poe/poe_client.py
+-rw-r--r--   0 jypark     (501) staff       (20)     2675 2024-05-20 06:17:55.000000 weavel-0.4.4/weavel/types.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.559818 weavel-0.4.4/weavel/utils/
+-rw-r--r--   0 jypark     (501) staff       (20)       43 2024-01-15 06:20:46.000000 weavel-0.4.4/weavel/utils/__init__.py
+-rw-r--r--   0 jypark     (501) staff       (20)     1134 2024-01-15 05:54:15.000000 weavel-0.4.4/weavel/utils/crypto.py
+-rw-r--r--   0 jypark     (501) staff       (20)      679 2024-01-15 11:33:18.000000 weavel-0.4.4/weavel/utils/logger.py
+drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-05-20 06:18:22.556551 weavel-0.4.4/weavel.egg-info/
+-rw-r--r--   0 jypark     (501) staff       (20)      406 2024-05-20 06:18:22.000000 weavel-0.4.4/weavel.egg-info/PKG-INFO
+-rw-r--r--   0 jypark     (501) staff       (20)     1115 2024-05-20 06:18:22.000000 weavel-0.4.4/weavel.egg-info/SOURCES.txt
+-rw-r--r--   0 jypark     (501) staff       (20)        1 2024-05-20 06:18:22.000000 weavel-0.4.4/weavel.egg-info/dependency_links.txt
+-rw-r--r--   0 jypark     (501) staff       (20)      184 2024-05-20 06:18:22.000000 weavel-0.4.4/weavel.egg-info/requires.txt
+-rw-r--r--   0 jypark     (501) staff       (20)       20 2024-05-20 06:18:22.000000 weavel-0.4.4/weavel.egg-info/top_level.txt
```

### Comparing `weavel-0.4.3/setup.py` & `weavel-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read README.md for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="weavel",
-    version="0.4.3",
+    version="0.4.4",
     packages=find_namespace_packages(),
     entry_points={},
     description="Weavel, natural language analysis Dashboard for LLM Agent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="weavel",
     url="https://github.com/weavel-ai/weavel-python",
```

### Comparing `weavel-0.4.3/testapp/daily_dialog/run_qa_extractor.py` & `weavel-0.4.4/testapp/daily_dialog/run_qa_extractor.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py` & `weavel-0.4.4/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/daily_dialog/save_to_db.py` & `weavel-0.4.4/testapp/daily_dialog/save_to_db.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/demo.py` & `weavel-0.4.4/testapp/demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 
 # trace: Trace = client.open_trace(user_identifier, trace_id='3714d452-ad29-4811-9ee0-8aec1771eaf8') # -> trace_id
 
 # trace_id='3714d452-ad29-4811-9ee0-8aec1771eaf8'
 trace_id='3714d452-ad29-4811-9ee0-8aec1771eaf8'
 trace: Trace = client.resume_trace(user_identifier, trace_id=trace_id)
 
-client.track(user_identifier, "paid", {"amount": "100"})
-client.track(user_identifier, "test", {}, trace_id)
+# client.track(user_identifier, "paid", {"amount": "100"})
+# client.track(user_identifier, "test", {}, trace_id)
 
-client.track(user_identifier, "test", {}, "new_trace_id")
-trace: Trace = client.open_trace(user_identifier, "new_trace_id")
+# client.track(user_identifier, "test", {}, "new_trace_id")
+# trace: Trace = client.open_trace(user_identifier, "new_trace_id")
 
+trace.log_message("assistant", "hello!", metadata={"test_key": "test_value1"}, trace_data_id="test_trace_data_id")
+
+client.log_message_metadata("test_trace_data_id", {"test_key": "test_value2"})
 
 # res = "I can assist you with a variety of tasks. I can help answer questions, provide information, give suggestions, assist with research, set reminders, manage your schedule, make reservations, provide translations, and much more. Just let me know what you need help with!"
 
 # # print(res.choices[0].message.content)
 
 # trace.log_message("assistant", res)
```

### Comparing `weavel-0.4.3/testapp/py_files/duplicate_log_test.py` & `weavel-0.4.4/testapp/py_files/duplicate_log_test.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/py_files/poe_test.py` & `weavel-0.4.4/testapp/py_files/poe_test.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/py_files/save_mock_data.py` & `weavel-0.4.4/testapp/py_files/save_mock_data.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/py_files/save_mock_retention_data.py` & `weavel-0.4.4/testapp/py_files/save_mock_retention_data.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/testapp/test.py` & `weavel-0.4.4/testapp/test.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/pwiz.py` & `weavel-0.4.4/venv/bin/pwiz.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2html.py` & `weavel-0.4.4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2html4.py` & `weavel-0.4.4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2html5.py` & `weavel-0.4.4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2latex.py` & `weavel-0.4.4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2man.py` & `weavel-0.4.4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2odt.py` & `weavel-0.4.4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2odt_prepstyles.py` & `weavel-0.4.4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2pseudoxml.py` & `weavel-0.4.4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2s5.py` & `weavel-0.4.4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2xetex.py` & `weavel-0.4.4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rst2xml.py` & `weavel-0.4.4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/venv/bin/rstpep2html.py` & `weavel-0.4.4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/_api_client.py` & `weavel-0.4.4/weavel/_api_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/_buffer_storage.py` & `weavel-0.4.4/weavel/_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/_worker.py` & `weavel-0.4.4/weavel/_worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from concurrent.futures import Future, ThreadPoolExecutor
 
 from weavel.types import (
     TraceDataRole,
     OpenTraceBody,
     CaptureTraceDataBody,
     CaptureTrackEventBody,
+    CaptureTraceDataMetadataBody,
     SaveUserIdentityBody
 )
 from weavel._constants import BACKEND_SERVER_URL
 from weavel._buffer_storage import BufferStorage
 from weavel._api_client import APIClient
 from weavel.utils import logger
 
@@ -118,115 +119,144 @@
             timestamp=str(datetime.now(timezone.utc).isoformat()),
             trace_id=trace_id,
         )
         self.buffer_storage.push(request)
 
         return
 
+    def log_message_metadata(
+        self,
+        trace_data_id: str,
+        metadata: Dict[str, str],
+        timestamp: Optional[datetime] = None,
+    ):
+        if timestamp is None:
+            timestamp = datetime.now(timezone.utc)
+        elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
+            timestamp = timestamp.astimezone(timezone.utc)
+            
+        request = CaptureTraceDataMetadataBody(
+            trace_data_id=trace_data_id,
+            metadata=metadata,
+            timestamp=timestamp,
+        )
+        self.buffer_storage.push(request)
+        return
+
     def log_user_message(
         self,
         user_id: str,
         trace_id: str,
         content: str,
-        unit_name: Optional[str] = None,
         timestamp: Optional[datetime] = None,
+        trace_data_id: Optional[str] = None,
+        unit_name: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
     ):
         """Log the "user_message" type data to the trace.
 
         Args:
             trace_id: The trace identifier.
             content: The data content.
-            unit_name: The unit name.
             timestamp: The timestamp.
+            trace_data_id: The trace data identifier.
+            unit_name: The unit name.
             metadata: The metadata.
         """
         if timestamp is None:
             timestamp = datetime.now(timezone.utc)
         elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
             timestamp = timestamp.astimezone(timezone.utc)
             
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
             role=TraceDataRole.user,
             content=content,
+            timestamp=timestamp.isoformat(),
+            trace_data_id=trace_data_id,
             unit_name=unit_name,
             metadata=metadata,
-            timestamp=timestamp.isoformat(),
         )
         self.buffer_storage.push(request)
         return
 
     def log_assistant_message(
         self,
         user_id: str,
         trace_id: str,
         content: str,
-        unit_name: Optional[str] = None,
         timestamp: Optional[datetime] = None,
+        trace_data_id: Optional[str] = None,
+        unit_name: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
     ):
         """Log the "llm_background_message" type data to the trace.
 
         Args:
             trace_id: The trace identifier.
             content: The data content.
-            unit_name: The unit name.
             timestamp: The timestamp.
+            trace_data_id: The trace data identifier.
+            unit_name: The unit name.
             metadata: The metadata.
         """
         if timestamp is None:
             timestamp = datetime.now(timezone.utc)
         elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
             timestamp = timestamp.astimezone(timezone.utc)
             
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
             role=TraceDataRole.assisatant,
             content=content,
+            timestamp=timestamp.isoformat(),
+            trace_data_id=trace_data_id,
             unit_name=unit_name,
             metadata=metadata,
-            timestamp=timestamp.isoformat(),
         )
         self.buffer_storage.push(request)
         return
 
     def log_inner_step(
         self,
         user_id: str,
         trace_id: str,
         content: str,
-        unit_name: Optional[str] = None,
         timestamp: Optional[datetime] = None,
+        trace_data_id: Optional[str] = None,
+        unit_name: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
+        
     ):
         """Log the "inner_step" type data to the trace.
 
         Args:
             trace_id: The trace identifier.
             content: The data content.
-            unit_name: The unit name.
             timestamp: The timestamp.
+            trace_data_id: The trace data identifier.
+            unit_name: The unit name.
             metadata: The metadata.
         """
         if timestamp is None:
             timestamp = datetime.now(timezone.utc)
         elif timestamp.tzinfo is None or timestamp.tzinfo.utcoffset(timestamp) is None:
             timestamp = timestamp.astimezone(timezone.utc)
             
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
             role=TraceDataRole.inner_step,
             content=content,
+            timestamp=timestamp.isoformat(),
+            trace_data_id=trace_data_id,
             unit_name=unit_name,
             metadata=metadata,
-            timestamp=timestamp.isoformat(),
         )
         self.buffer_storage.push(request)
         return
 
     def send_requests(
         self,
         requests: List[
```

### Comparing `weavel-0.4.3/weavel/client.py` & `weavel-0.4.4/weavel/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,59 +24,63 @@
 
     def log_message(
         self,
         # pylint: disable=redefined-builtin
         type: Literal["user", "assistant"],
         content: str,
         timestamp: Optional[datetime] = None,
+        trace_data_id: Optional[str] = None,
         unit_name: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
     ):
         """
         Logs a message with the specified type, content, timestamp, unit name, and metadata.
 
         Args:
             type (Literal["user", "assistant"]): The type of the message. Must be either "user" or "assistant".
             content (str): The content of the message.
             timestamp (Optional[datetime], optional): The timestamp of the message. Defaults to None.
+            trace_data_id (Optional[str], optional): The trace data ID associated with the message. Defaults to None.
             unit_name (Optional[str], optional): The unit name associated with the message. Defaults to None.
             metadata (Optional[Dict[str, str]], optional): Additional metadata for the message. Defaults to None.
 
         Raises:
             ValueError: If an invalid message type is provided.
         """
         if type == "user":
             self.worker.log_user_message(
-                self.user_id, self.trace_id, content, unit_name, timestamp, metadata
+                self.user_id, self.trace_id, content, timestamp, trace_data_id, unit_name, metadata
             )
         elif type == "assistant":
             self.worker.log_assistant_message(
-                self.user_id, self.trace_id, content, unit_name, timestamp, metadata
+                self.user_id, self.trace_id, content, timestamp, trace_data_id, unit_name, metadata
             )
         else:
             raise ValueError("Invalid message type.")
 
     def log_inner_step(
         self,
         content: str,
         timestamp: Optional[datetime] = None,
+        trace_data_id: Optional[str] = None,
         unit_name: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
     ):
         """
         Logs an inner step in the worker.
 
         Args:
             content (str): The content of the inner step.
             timestamp (Optional[datetime], optional): The timestamp of the inner step. Defaults to None.
+            trace_data_id (Optional[str], optional): The trace data ID of the inner step. Defaults to None.
             unit_name (Optional[str], optional): The unit name of the inner step. Defaults to None.
             metadata (Optional[Dict[str, str]], optional): Additional metadata for the inner step. Defaults to None.
         """
         self.worker.log_inner_step(
-            self.user_id, self.trace_id, content, unit_name, timestamp, metadata
+            self.user_id, self.trace_id, content, timestamp, trace_data_id, unit_name, metadata
         )
 
 
 class WeavelClient:
     """Client for interacting with the Weavel service.
 
     This class provides methods for creating and managing traces, tracking user actions,
@@ -151,14 +155,18 @@
             event_name (str): The name of the track event.
             properties (Dict): The properties of the track event.
             trace_id (str, optional): The ID of the trace associated with the track event.
 
         """
         self._worker.log_track_event(user_id, event_name, properties, trace_id)
         
+    def log_message_metadata(self, trace_data_id: str, metadata: Dict[str, str], timestamp: Optional[datetime] = None):
+        """Add metadata to a message."""
+        self._worker.log_message_metadata(trace_data_id, metadata, timestamp)
+        
     def identify(self, user_id: str, properties: Dict[str, Any]):
         """Identify a user with the specified properties.
         
         You can save any user information you know about a user for user_id, such as their email, name, or phone number in dict format.
         Properties will be updated for every call.
         """
```

### Comparing `weavel-0.4.3/weavel/poe/_poe_buffer_storage.py` & `weavel-0.4.4/weavel/poe/_poe_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/poe/_poe_worker.py` & `weavel-0.4.4/weavel/poe/_poe_worker.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/poe/poe_client.py` & `weavel-0.4.4/weavel/poe/poe_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/types.py` & `weavel-0.4.4/weavel/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,24 +29,14 @@
 class TraceDataRole(str, Enum):
     system = "system"
     user = "user"
     assisatant = "assistant"
     inner_step = "inner_step"
     # retrieved_content = "retrieved_content"
 
-
-class BackgroundTaskType(str, Enum):
-    open_trace = "open_trace"
-    capture_trace_data = "capture_trace_data"
-    capture_track_event = "capture_track_event"
-    create_semantic_event = "create_semantic_event"
-    extract_keywords = "extract_keywords"
-    save_user_identity = "save_user_identity"
-
-
 class OpenTraceBody(WeavelObject):
     """Start Trace body."""
 
     type: Literal["open_trace"] = "open_trace"
     user_id: str
     trace_id: str
     timestamp: Optional[str] = None
@@ -68,17 +58,24 @@
     """Capture Trace Data body."""
 
     type: Literal["capture_trace_data"] = "capture_trace_data"
     user_id: str
     trace_id: str
     role: str
     content: str
+    timestamp: Optional[str] = None
+    trace_data_id: Optional[str] = None
     unit_name: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
-    timestamp: Optional[str] = None
+
+class CaptureTraceDataMetadataBody(WeavelObject):
+    type: Literal["capture_trace_data_metadata"] = "capture_trace_data_metadata"
+    trace_data_id: str
+    metadata: Dict[str, Any]
+    timestamp: str
 
 class SaveUserIdentityBody(WeavelObject):
     """Save user identity body."""
     type: Literal["save_user_identity"] = "save_user_identity"
     user_id: str
     properties: Dict[str, Any]
     timestamp: Optional[str] = None
```

### Comparing `weavel-0.4.3/weavel/utils/crypto.py` & `weavel-0.4.4/weavel/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel/utils/logger.py` & `weavel-0.4.4/weavel/utils/logger.py`

 * *Files identical despite different names*

### Comparing `weavel-0.4.3/weavel.egg-info/SOURCES.txt` & `weavel-0.4.4/weavel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

