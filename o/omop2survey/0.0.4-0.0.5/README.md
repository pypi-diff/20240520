# Comparing `tmp/omop2survey-0.0.4.tar.gz` & `tmp/omop2survey-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2survey-0.0.4.tar", max compression
+gzip compressed data, was "omop2survey-0.0.5.tar", max compression
```

## Comparing `omop2survey-0.0.4.tar` & `omop2survey-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5296 2024-05-14 21:03:51.967987 omop2survey-0.0.4/README.md
--rw-r--r--   0        0        0     6148 2024-05-17 04:16:32.815544 omop2survey-0.0.4/omop2survey/.DS_Store
--rw-r--r--   0        0        0      323 2024-05-17 03:55:13.603705 omop2survey-0.0.4/omop2survey/__init__.py
--rw-r--r--   0        0        0     6059 2024-05-17 03:55:13.579601 omop2survey-0.0.4/omop2survey/codebooks.py
--rw-r--r--   0        0        0      571 2024-05-17 04:31:31.601715 omop2survey-0.0.4/omop2survey/hash_csv.py
--rw-r--r--   0        0        0     2801 2024-05-17 03:52:36.052302 omop2survey-0.0.4/omop2survey/pivot_data.py
--rw-r--r--   0        0        0      872 2024-05-17 03:49:20.928260 omop2survey-0.0.4/omop2survey/recode_missing.py
--rw-r--r--   0        0        0     7434 2024-05-17 03:55:13.607873 omop2survey-0.0.4/omop2survey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.0.4/omop2survey/survey_key.csv
--rw-r--r--   0        0        0       64 2024-05-17 04:31:33.436399 omop2survey-0.0.4/omop2survey/survey_key_hash.txt
--rw-r--r--   0        0        0      828 2024-05-17 04:39:02.850743 omop2survey-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 omop2survey-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5464 2024-05-19 23:44:34.164594 omop2survey-0.0.5/README.md
+-rw-r--r--   0        0        0     6148 2024-05-17 04:16:32.815544 omop2survey-0.0.5/omop2survey/.DS_Store
+-rw-r--r--   0        0        0      323 2024-05-17 04:52:20.337967 omop2survey-0.0.5/omop2survey/__init__.py
+-rw-r--r--   0        0        0     6058 2024-05-17 04:52:20.338391 omop2survey-0.0.5/omop2survey/codebooks.py
+-rw-r--r--   0        0        0      571 2024-05-17 04:52:20.338656 omop2survey-0.0.5/omop2survey/hash_csv.py
+-rw-r--r--   0        0        0     2800 2024-05-17 04:52:20.338900 omop2survey-0.0.5/omop2survey/pivot_data.py
+-rw-r--r--   0        0        0      872 2024-05-17 03:49:20.928260 omop2survey-0.0.5/omop2survey/recode_missing.py
+-rw-r--r--   0        0        0    10229 2024-05-20 00:05:36.987436 omop2survey-0.0.5/omop2survey/response_set.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omop2survey-0.0.5/omop2survey/survey_key.csv
+-rw-r--r--   0        0        0       64 2024-05-17 04:52:20.339780 omop2survey-0.0.5/omop2survey/survey_key_hash.txt
+-rw-r--r--   0        0        0      828 2024-05-19 23:32:17.602826 omop2survey-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 omop2survey-0.0.5/PKG-INFO
```

### Comparing `omop2survey-0.0.4/README.md` & `omop2survey-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 The **'omop2survey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
-## response_set.py
+The content of Python files in the package can be found below. For examples of how to use the package, see **example.py** for Python and **exampleR.Rmd** for R.
+
+### response_set.py
 
 >
 >**map_answers(input_data)**: Maps survey responses to corresponding numeric and text values, and handles survey responses that fall outside the predefined cases.
 > 
 > Parameters:
 > -  ***input_data***: DataFrame containing survey responses with columns question_concept_id and answer_concept_id. 
 > 
@@ -33,15 +35,15 @@
 > - ***score_name***: Name of the column where the score will be stored.
 > - ***na***: Boolean indicating whether to include participants with missing data in the calculations (na = True or na = False).
 > - ***method***: Specifies the method for score calculation (method = 'sum' or method = 'mean').
 > 
 > Returns: The original DataFrame with an additional column containing the calculated scores for each participant.
 > 
 
-## pivot_data.py
+### pivot_data.py
 
 >
 > **pivot(input_data, file_name)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
 >  The column names are prefixed with 'q' to denote question IDs. The resulting pivot table is saved to a CSV file and then uploaded to a cloud storage bucket using Google Cloud's gsutil tool.
 >
 > Parameters:
 > - ***input_data***: A pandas DataFrame containing the columns person_id, question_concept_id, and answer_numeric.
@@ -52,26 +54,28 @@
 >**pivot_text(input_data, file_name)**: Similar to pivot_data_numeric, but pivots text responses instead. The resulting pivot table is saved to a CSV file and then uploaded to a cloud storage bucket using Google Cloud's gsutil tool.
 >
 >Parameters:
 > - ***input_data***: A pandas DataFrame containing the columns person_id, question_concept_id, and answer_text.
 > - ***file_name***: Optional; the name of the file to which the pivot table will be saved. Defaults to 'pivot_t.csv'.
 >
 
-## recode_missing.py
+### recode_missing.py
 > 
 > **recode(input_data)**: Processes input data (either in file format or as a pandas DataFrame) to handle missing values according to a specified list of codes. It replaces a predefined set of numeric codes with pandas NA values to standardize the representation of missing data across the dataset. 
 > 
 > Parameters:
 > - ***input_data***: This can be either a path to a data file (CSV, TXT, or Excel) or a pandas DataFrame. The function adapts its behavior based on the type of input provided.
 >
 > Returns: A pandas DataFrame with the missing values recoded as pandas NA.
 
-## codebooks.py
+### codebooks.py
 >
 >**codebook(df)**: Processes input data to generate a structured HTML codebook, which includes a detailed listing of questions and responses formatted neatly. The function first cleans and deduplicates the data, then iteratively builds the formatted data, and finally writes it to an HTML file that is linked for download.
 >
 > Parameters:
 >
 > - ***input_data***: DataFrame to be processed into a codebook.
 > 
 > Returns: The HTML-formatted codebook and an IPython display link to the generated HTML file.
 > 
+
+
```

### Comparing `omop2survey-0.0.4/omop2survey/.DS_Store` & `omop2survey-0.0.5/omop2survey/.DS_Store`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.4/omop2survey/codebooks.py` & `omop2survey-0.0.5/omop2survey/codebooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
                     'answer_concept_id': row['answer_concept_id'],
                     'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
                     'answer': row['answer'],
                     'answer recoded as answer_text': row['answer_text']
                 })
 
     formatted_codebook_df = pd.DataFrame(formatted_data)
-
     current_time = datetime.now().strftime("%Y%m%d_%H%M%S")
 
     file_name = f'codebook_{current_time}.html'
     workspace_dir = os.path.join(os.getcwd(), 'workspace')
     os.makedirs(workspace_dir, exist_ok=True)
     file_path = os.path.join(workspace_dir, file_name)
```

### Comparing `omop2survey-0.0.4/omop2survey/hash_csv.py` & `omop2survey-0.0.5/omop2survey/hash_csv.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.4/omop2survey/pivot_data.py` & `omop2survey-0.0.5/omop2survey/pivot_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,11 +58,10 @@
                                 values='answer_text',
                                 aggfunc='first')
 
     pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
     workspace_dir = os.path.join(os.getcwd(), 'workspace')
     os.makedirs(workspace_dir, exist_ok=True)
     file_path = os.path.join(workspace_dir, file_name)
-
     pivot_df.to_csv(file_path)
 
     print(f"Pivoted dataset with text values saved successfully to: {file_path}")
```

### Comparing `omop2survey-0.0.4/omop2survey/recode_missing.py` & `omop2survey-0.0.5/omop2survey/recode_missing.py`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.4/omop2survey/response_set.py` & `omop2survey-0.0.5/omop2survey/response_set.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     file_path = os.path.join(current_dir, filename)
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"File path {file_path} does not exist.")
     return pd.read_csv(file_path)
 
 
-def map_items(input_data):
+def map_responses(input_data):
     special_cases = {
         903087: (-999, "Don't Know"),
         903096: (-998, "Skip"),
         903072: (-997, "Does Not Apply To Me"),
         903079: (-996, "Prefer Not To Answer"),
         903070: (-995, "Other"),
         903092: (-994, "Not Sure"),
@@ -178,7 +178,76 @@
     input_data[['answer_numeric', 'answer_text']] = result
 
     numeric_mask = pd.isna(input_data['answer_concept_id']) & input_data['answer'].apply(lambda x: str(x).isdigit())
     input_data.loc[numeric_mask, 'answer_numeric'] = input_data.loc[numeric_mask, 'answer'].astype(int)
     input_data.loc[numeric_mask, 'answer_text'] = input_data.loc[numeric_mask, 'answer'].astype(str)
 
     return input_data
+
+
+def map_items(input_data):
+    special_cases = {
+        903087: (-999, "Don't Know"),
+        903096: (-998, "Skip"),
+        903072: (-997, "Does Not Apply To Me"),
+        903079: (-996, "Prefer Not To Answer"),
+        903070: (-995, "Other"),
+        903092: (-994, "Not Sure"),
+        903095: (-993, "None"),
+        903103: (-992, "Unanswered"),
+        40192432: (-991, "I am not religious"),
+        40192487: (-990, "I do not believe in God (or a higher power)"),
+        40192520: (-989, "Does not apply to my neighborhood"),
+        903081: (-988, "Free Text"),
+        596889: (998, "Text"),
+        596883: (-994, "Not Sure"),
+        1332844: (-994, "Not Sure"),
+        903598: (-996, "Prefer Not To Answer"),
+        903596: (-996, "Prefer Not To Answer"),
+        903601: (-996, "Prefer Not To Answer"),
+        903607: (-996, "Prefer Not To Answer"),
+        903610: (-996, "Prefer Not To Answer"),
+        903604: (-996, "Prefer Not To Answer"),
+        43529089: (-997, "No Blood Related Daughters"),
+        43529086: (-997, "No Blood Related Siblings"),
+        43529092: (-997, "No Blood Related Sons"),
+        43529090: (-997, "No Daughters Related")
+    }
+
+    survey_data = load_survey_data()
+
+    mapping_numeric = survey_data.groupby('question_concept_id').apply(
+        lambda g: g.set_index('answer_concept_id')['answer_numeric'].to_dict()
+    ).to_dict()
+
+    mapping_text = survey_data.groupby('question_concept_id').apply(
+        lambda g: g.set_index('answer_concept_id')['answer_text'].str.strip().to_dict()
+    ).to_dict()
+
+    input_data['answer_numeric'] = pd.NA
+    input_data['answer_text'] = pd.NA
+
+    for answer_id, (num, text) in special_cases.items():
+        mask = input_data['answer_concept_id'] == answer_id
+        input_data.loc[mask, 'answer_numeric'] = num
+        input_data.loc[mask, 'answer_text'] = text
+
+    def apply_mappings(row):
+        if pd.notna(row['answer_numeric']) and pd.notna(row['answer_text']):
+            return row['answer_numeric'], row['answer_text']
+
+        question_id = row['question_concept_id']
+        answer_id = row['answer_concept_id']
+        numeric = mapping_numeric.get(question_id, {}).get(answer_id, pd.NA)
+        text = mapping_text.get(question_id, {}).get(answer_id, pd.NA)
+        return numeric, text
+
+    input_data[['answer_numeric', 'answer_text']] = input_data.apply(
+        lambda row: pd.Series(apply_mappings(row)), axis=1
+    )
+
+    numeric_mask = pd.isna(input_data['answer_concept_id']) & input_data['answer'].apply(lambda x: str(x).isdigit())
+    input_data.loc[numeric_mask, 'answer_numeric'] = input_data.loc[numeric_mask, 'answer'].astype(int)
+    input_data.loc[numeric_mask, 'answer_text'] = input_data.loc[numeric_mask, 'answer'].astype(str)
+
+    return input_data
+
```

### Comparing `omop2survey-0.0.4/omop2survey/survey_key.csv` & `omop2survey-0.0.5/omop2survey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omop2survey-0.0.4/pyproject.toml` & `omop2survey-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omop2survey"
-version = "0.0.4"
+version = "0.0.5"
 description = "The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omop2survey.git"
 license = "MIT"
 readme = "README.md"
 include = ["omop2survey/survey_key.csv"]
```

### Comparing `omop2survey-0.0.4/PKG-INFO` & `omop2survey-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omop2survey
-Version: 0.0.4
+Version: 0.0.5
 Summary: The 'omop2survey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2survey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,17 @@
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/elifdy/omop2survey.git
 Description-Content-Type: text/markdown
 
 
 The **'omop2survey'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
 
-## response_set.py
+The content of Python files in the package can be found below. For examples of how to use the package, see **example.py** for Python and **exampleR.Rmd** for R.
+
+### response_set.py
 
 >
 >**map_answers(input_data)**: Maps survey responses to corresponding numeric and text values, and handles survey responses that fall outside the predefined cases.
 > 
 > Parameters:
 > -  ***input_data***: DataFrame containing survey responses with columns question_concept_id and answer_concept_id. 
 > 
@@ -53,15 +55,15 @@
 > - ***score_name***: Name of the column where the score will be stored.
 > - ***na***: Boolean indicating whether to include participants with missing data in the calculations (na = True or na = False).
 > - ***method***: Specifies the method for score calculation (method = 'sum' or method = 'mean').
 > 
 > Returns: The original DataFrame with an additional column containing the calculated scores for each participant.
 > 
 
-## pivot_data.py
+### pivot_data.py
 
 >
 > **pivot(input_data, file_name)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
 >  The column names are prefixed with 'q' to denote question IDs. The resulting pivot table is saved to a CSV file and then uploaded to a cloud storage bucket using Google Cloud's gsutil tool.
 >
 > Parameters:
 > - ***input_data***: A pandas DataFrame containing the columns person_id, question_concept_id, and answer_numeric.
@@ -72,27 +74,29 @@
 >**pivot_text(input_data, file_name)**: Similar to pivot_data_numeric, but pivots text responses instead. The resulting pivot table is saved to a CSV file and then uploaded to a cloud storage bucket using Google Cloud's gsutil tool.
 >
 >Parameters:
 > - ***input_data***: A pandas DataFrame containing the columns person_id, question_concept_id, and answer_text.
 > - ***file_name***: Optional; the name of the file to which the pivot table will be saved. Defaults to 'pivot_t.csv'.
 >
 
-## recode_missing.py
+### recode_missing.py
 > 
 > **recode(input_data)**: Processes input data (either in file format or as a pandas DataFrame) to handle missing values according to a specified list of codes. It replaces a predefined set of numeric codes with pandas NA values to standardize the representation of missing data across the dataset. 
 > 
 > Parameters:
 > - ***input_data***: This can be either a path to a data file (CSV, TXT, or Excel) or a pandas DataFrame. The function adapts its behavior based on the type of input provided.
 >
 > Returns: A pandas DataFrame with the missing values recoded as pandas NA.
 
-## codebooks.py
+### codebooks.py
 >
 >**codebook(df)**: Processes input data to generate a structured HTML codebook, which includes a detailed listing of questions and responses formatted neatly. The function first cleans and deduplicates the data, then iteratively builds the formatted data, and finally writes it to an HTML file that is linked for download.
 >
 > Parameters:
 >
 > - ***input_data***: DataFrame to be processed into a codebook.
 > 
 > Returns: The HTML-formatted codebook and an IPython display link to the generated HTML file.
 > 
 
+
+
```

