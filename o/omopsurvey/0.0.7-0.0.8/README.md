# Comparing `tmp/omopsurvey-0.0.7.tar.gz` & `tmp/omopsurvey-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omopsurvey-0.0.7.tar", max compression
+gzip compressed data, was "omopsurvey-0.0.8.tar", max compression
```

## Comparing `omopsurvey-0.0.7.tar` & `omopsurvey-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5295 2024-05-14 20:29:44.829203 omopsurvey-0.0.7/README.md
--rw-r--r--   0        0        0      273 2024-05-13 21:25:29.218835 omopsurvey-0.0.7/omopsurvey/__init__.py
--rw-r--r--   0        0        0     4118 2024-05-14 19:34:35.623448 omopsurvey-0.0.7/omopsurvey/codebooks.py
--rw-r--r--   0        0        0     1567 2024-05-14 19:38:37.534134 omopsurvey-0.0.7/omopsurvey/pivot_data.py
--rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omopsurvey-0.0.7/omopsurvey/recode_missing.py
--rw-r--r--   0        0        0     7436 2024-05-14 07:33:20.872482 omopsurvey-0.0.7/omopsurvey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.7/omopsurvey/survey_key.csv
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.7/omopsurvey/tests/codebook_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.7/omopsurvey/tests/map_responses_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.7/omopsurvey/tests/pivot_data_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.7/omopsurvey/tests/recode_missing_test.py
--rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.7/omopsurvey/vignettes/example_basics.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.7/omopsurvey/vignettes/example_healthcare.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.7/omopsurvey/vignettes/example_sdoh.ipynb
--rw-r--r--   0        0        0      722 2024-05-14 20:33:43.916066 omopsurvey-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     6310 1970-01-01 00:00:00.000000 omopsurvey-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     5295 2024-05-14 20:29:44.829203 omopsurvey-0.0.8/README.md
+-rw-r--r--   0        0        0      273 2024-05-13 21:25:29.218835 omopsurvey-0.0.8/omopsurvey/__init__.py
+-rw-r--r--   0        0        0     4077 2024-05-14 20:57:26.446629 omopsurvey-0.0.8/omopsurvey/codebooks.py
+-rw-r--r--   0        0        0     1567 2024-05-14 19:38:37.534134 omopsurvey-0.0.8/omopsurvey/pivot_data.py
+-rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omopsurvey-0.0.8/omopsurvey/recode_missing.py
+-rw-r--r--   0        0        0     7436 2024-05-14 07:33:20.872482 omopsurvey-0.0.8/omopsurvey/response_set.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.8/omopsurvey/survey_key.csv
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.8/omopsurvey/tests/codebook_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.8/omopsurvey/tests/map_responses_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.8/omopsurvey/tests/pivot_data_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.8/omopsurvey/tests/recode_missing_test.py
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.8/omopsurvey/vignettes/example_basics.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.8/omopsurvey/vignettes/example_healthcare.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.8/omopsurvey/vignettes/example_sdoh.ipynb
+-rw-r--r--   0        0        0      723 2024-05-19 22:29:57.070543 omopsurvey-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6312 1970-01-01 00:00:00.000000 omopsurvey-0.0.8/PKG-INFO
```

### Comparing `omopsurvey-0.0.7/README.md` & `omopsurvey-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/codebooks.py` & `omopsurvey-0.0.8/omopsurvey/codebooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
                     'answer_concept_id': row['answer_concept_id'],
                     'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
                     'answer': row['answer'],
                     'answer recoded as answer_text': row['answer_text']
                 })
 
     formatted_codebook_df = pd.DataFrame(formatted_data)
-    display(HTML(formatted_codebook_df))
 
     current_time = datetime.now().strftime("%Y%m%d_%H%M%S")
 
     file_name = f'codebook_{current_time}.html'
     file_path = os.path.join(os.getcwd(), file_name)
     temp = formatted_codebook_df.to_html(index=False, escape=False)
     with open(file_path, 'w') as f:
```

### Comparing `omopsurvey-0.0.7/omopsurvey/pivot_data.py` & `omopsurvey-0.0.8/omopsurvey/pivot_data.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/recode_missing.py` & `omopsurvey-0.0.8/omopsurvey/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/response_set.py` & `omopsurvey-0.0.8/omopsurvey/response_set.py`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/survey_key.csv` & `omopsurvey-0.0.8/omopsurvey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/vignettes/example_basics.ipynb` & `omopsurvey-0.0.8/omopsurvey/vignettes/example_basics.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/vignettes/example_healthcare.ipynb` & `omopsurvey-0.0.8/omopsurvey/vignettes/example_healthcare.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/omopsurvey/vignettes/example_sdoh.ipynb` & `omopsurvey-0.0.8/omopsurvey/vignettes/example_sdoh.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.7/pyproject.toml` & `omopsurvey-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "omopsurvey"
-version = "0.0.7"
+version = "0.0.8"
 description = "The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
-repository = "https://github.com/elifdy/omopsurvey.git"
+repository = "https://github.com/elifdy/omop2survey.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2.2"
 tabulate = "^0.9.0"
```

### Comparing `omopsurvey-0.0.7/PKG-INFO` & `omopsurvey-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: omopsurvey
-Version: 0.0.7
+Version: 0.0.8
 Summary: The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
-Home-page: https://github.com/elifdy/omopsurvey.git
+Home-page: https://github.com/elifdy/omop2survey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Project-URL: Repository, https://github.com/elifdy/omopsurvey.git
+Project-URL: Repository, https://github.com/elifdy/omop2survey.git
 Description-Content-Type: text/markdown
 
 
 The **'omopsurvey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
 ## response_set.py
```

