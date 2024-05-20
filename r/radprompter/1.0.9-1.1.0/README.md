# Comparing `tmp/radprompter-1.0.9.tar.gz` & `tmp/radprompter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.0.9.tar` & `radprompter-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.9/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.9/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.9/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.9/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.9/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.9/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.9/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.9/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.0.9/pyproject.toml
--rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.0.9/radprompter/__init__.py
--rw-r--r--   0        0        0       21 2024-05-19 20:35:14.195029 radprompter-1.0.9/radprompter/__version__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.9/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.9/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.9/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.0.9/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     7035 2024-05-19 20:35:03.508905 radprompter-1.0.9/radprompter/radprompter.py
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.9/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.9/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.9/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.9/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 19:37:48.126029 radprompter-1.0.9/tutorials/.DS_Store
--rw-r--r--   0        0        0    16762 2024-05-19 18:51:21.283638 radprompter-1.0.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.0.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    17583 2024-05-19 19:52:03.804859 radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
--rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.toml
--rw-r--r--   0        0        0    19012 2024-05-19 19:51:58.516551 radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
--rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
--rw-r--r--   0        0        0    26892 2024-05-19 19:51:53.847964 radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.toml
--rw-r--r--   0        0        0    35817 2024-05-19 20:35:17.292967 radprompter-1.0.9/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     3277 2024-05-19 20:19:42.275696 radprompter-1.0.9/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.9/tutorials/README.md
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.1.0/.DS_Store
+-rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.1.0/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.1.0/Plan.md
+-rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.1.0/README.md
+-rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.1.0/demo.ipynb
+-rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.1.0/demo_no_CoT.ipynb
+-rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.1.0/demo_prompt_no_CoT.toml
+-rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.1.0/radprompter/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-19 20:38:38.191128 radprompter-1.1.0/radprompter/__version__.py
+-rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.1.0/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.1.0/radprompter/clients/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.0/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.1.0/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     7054 2024-05-19 20:37:23.343879 radprompter-1.1.0/radprompter/radprompter.py
+-rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.1.0/sample_prompt.toml
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.0/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.0/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.0/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0     6148 2024-05-19 19:37:48.126029 radprompter-1.1.0/tutorials/.DS_Store
+-rw-r--r--   0        0        0    16762 2024-05-19 18:51:21.283638 radprompter-1.1.0/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.0/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    17583 2024-05-19 19:52:03.804859 radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
+-rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.toml
+-rw-r--r--   0        0        0    19012 2024-05-19 19:51:58.516551 radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
+-rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
+-rw-r--r--   0        0        0    26892 2024-05-19 19:51:53.847964 radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.toml
+-rw-r--r--   0        0        0    28952 2024-05-19 20:38:21.626249 radprompter-1.1.0/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     3275 2024-05-19 20:37:55.612863 radprompter-1.1.0/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.1.0/tutorials/README.md
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.1.0/PKG-INFO
```

### Comparing `radprompter-1.0.9/.DS_Store` & `radprompter-1.1.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/.gitignore` & `radprompter-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/LICENSE` & `radprompter-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/demo.ipynb` & `radprompter-1.1.0/demo.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/demo_no_CoT.ipynb` & `radprompter-1.1.0/demo_no_CoT.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/demo_prompt_no_CoT.toml` & `radprompter-1.1.0/demo_prompt_no_CoT.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/pyproject.toml` & `radprompter-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/radprompter/clients/clients.py` & `radprompter-1.1.0/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/radprompter/prompts/prompts.py` & `radprompter-1.1.0/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/radprompter/radprompter.py` & `radprompter-1.1.0/radprompter/radprompter.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             f.write("-"*20)
             f.write("\n")
             f.write(self.prompt.raw_data)
             
             f.close()
             
     def sanitize_json(self, variable_name="all"):
-        df = pd.read_csv(self.output_file)
+        df = pd.read_csv(self.output_file, index_col='index')
 
         if variable_name == "all":
             for schema in self.prompt.schemas.schemas:
                 if schema["type"] == "select":
                     column_name = f"{schema['variable_name']}_response"
                     options = schema["options"]
                     df[column_name] = df[column_name].apply(lambda x: self._sanitize_response(x, options))
```

### Comparing `radprompter-1.0.9/sample_prompt.toml` & `radprompter-1.1.0/sample_prompt.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/sample_reports/sample_report_1.txt` & `radprompter-1.1.0/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/sample_reports/sample_report_2.txt` & `radprompter-1.1.0/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/sample_reports/sample_report_3.txt` & `radprompter-1.1.0/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/.DS_Store` & `radprompter-1.1.0/tutorials/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.1.0/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb` & `radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.toml` & `radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb` & `radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml` & `radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb` & `radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.toml` & `radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.9/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml` & `radprompter-1.1.0/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 }
 </json>
 """
 
 assistant_response_template = """
 <json>
 {
-  "{{variable_name}}" : \""""
+  "{{variable_name}}" : """
 
 [CONSTRUCTOR]
 system = "rdp(system_prompt)"
 user = "rdp(user_prompt_intro + user_prompt_no_cot)"
 response_templates = "rdp(assistant_response_template)"
 stop_tags = "</json>"
```

### Comparing `radprompter-1.0.9/PKG-INFO` & `radprompter-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: openai
 Project-URL: Home, https://github.com/BardiaKh/RadPrompter
```

