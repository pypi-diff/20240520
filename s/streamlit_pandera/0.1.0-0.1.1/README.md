# Comparing `tmp/streamlit_pandera-0.1.0.tar.gz` & `tmp/streamlit_pandera-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_pandera-0.1.0.tar", max compression
+gzip compressed data, was "streamlit_pandera-0.1.1.tar", max compression
```

## Comparing `streamlit_pandera-0.1.0.tar` & `streamlit_pandera-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-05-15 22:07:51.676223 streamlit_pandera-0.1.0/LICENSE
--rw-r--r--   0        0        0     2239 2024-05-19 03:43:52.219286 streamlit_pandera-0.1.0/README.md
--rw-r--r--   0        0        0      692 2024-05-19 02:34:06.468115 streamlit_pandera-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4158 2024-05-19 03:06:59.362779 streamlit_pandera-0.1.0/streamlit_pandera/validate_file.py
--rw-r--r--   0        0        0     3514 2024-05-18 20:44:07.622489 streamlit_pandera-0.1.0/streamlit_pandera/validator.py
--rw-r--r--   0        0        0     3134 1970-01-01 00:00:00.000000 streamlit_pandera-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-19 16:50:18.345405 streamlit_pandera-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2367 2024-05-19 16:50:18.345405 streamlit_pandera-0.1.1/README.md
+-rw-r--r--   0        0        0      704 2024-05-19 16:50:18.349405 streamlit_pandera-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4130 2024-05-19 16:50:18.349405 streamlit_pandera-0.1.1/streamlit_pandera/validate_file.py
+-rw-r--r--   0        0        0     3514 2024-05-19 16:50:18.349405 streamlit_pandera-0.1.1/streamlit_pandera/validator.py
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 streamlit_pandera-0.1.1/PKG-INFO
```

### Comparing `streamlit_pandera-0.1.0/LICENSE` & `streamlit_pandera-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_pandera-0.1.0/README.md` & `streamlit_pandera-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Welcome to Streamlit-Panderas!
 
 
 [![Test](https://github.com/resilientinfrastructure/streamlit-panderas/actions/workflows/e2e.yml/badge.svg)](https://github.com/resilientinfrastructure/streamlit-panderas/actions/workflows/e2e.yml)
 
-Streamlit-Panderas is your go-to tool for clean data ingestion, seamlessly integrating Streamlit and Panderas to make your data processing tasks a breeze.
+Streamlit-Panderas is your go-to tool for clean data ingestion and validation, seamlessly integrating Streamlit and Panderas to make your data processing tasks a breeze.
 
 ## Features
 
 - **Easy Data Ingestion:** Select your file format (CSV or JSON) and provide a URL to a Panderas schema.
 - **Streamlined Validation:** With just a few clicks, submit your selections and validate your data effortlessly.
 
 
@@ -20,17 +20,17 @@
 ```
 
 ## Usage instructions
 
 ```python
 import streamlit as st
 
-from streamlit_pandera.validate_file  import run
+from streamlit_pandera.validate_file  import run_validate_file
 
-validated_df = run()
+validated_df = run_validate_file()
 
 st.write(validated_df)
 ```
 
 
 ## Instructions
 
@@ -42,15 +42,15 @@
 
 ### Step 3: Submit and Validate
 Hit that submit button and let Streamlit-Panderas work its magic! Your data will be validated against the specified schema in no time.
 
 
 [Go to Demo](https://youtu.be/9Ry_A9LgrbQ)
 
-
+[![Video](http://img.youtube.com/vi/9Ry_A9LgrbQ/0.jpg)](https://youtu.be/9Ry_A9LgrbQ)
 
 
 ## Run Tests
 To ensure everything is functioning smoothly, run the tests using the following commands:
 
 ```bash
 poetry install
```

### Comparing `streamlit_pandera-0.1.0/pyproject.toml` & `streamlit_pandera-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit_pandera"
-version = "0.1.0"
+version = "0.1.1"
 description = "Clean Data Validation Tool integrates Streamlit and Panderas"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 streamlit = "^1.34.0"
@@ -19,12 +19,13 @@
 pytest-rerunfailures = "12.0"
 pandera = { version = "^0.7.2", extras = ["io"] }
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pytest = "*"
 pylint = "^3.2.0"
+twine = "*"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `streamlit_pandera-0.1.0/streamlit_pandera/validate_file.py` & `streamlit_pandera-0.1.1/streamlit_pandera/validate_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 if st.session_state["file_format"] == "Unassigned":
                     st.session_state["file_format"] = "csv"
                 return
             except:
                 st.error("Invalid URL! Please enter a valid URL.")
                 return
 
-def run():
+def run_validate_file():
     st.set_page_config(
         page_title="Clean Data Home",
         page_icon="📊",
     )
     st.write("# Clean Data Validation Tool! 📊")
     set_selectbox()
     set_format_type_form()
@@ -118,11 +118,8 @@
         uploaded_file = st.file_uploader("Choose a file")
         if uploaded_file is not None:
             dataframe = validator.run_validation(uploaded_file=uploaded_file)
             st.dataframe(dataframe)
             st.balloons()
             return uploaded_file
 
-# if __name__ == "__main__":
-#     run()
-
```

### Comparing `streamlit_pandera-0.1.0/streamlit_pandera/validator.py` & `streamlit_pandera-0.1.1/streamlit_pandera/validator.py`

 * *Files identical despite different names*

### Comparing `streamlit_pandera-0.1.0/PKG-INFO` & `streamlit_pandera-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_pandera
-Version: 0.1.0
+Version: 0.1.1
 Summary: Clean Data Validation Tool integrates Streamlit and Panderas
 Author: Manrique Vargas
 Author-email: machomaxg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 
 # Welcome to Streamlit-Panderas!
 
 
 [![Test](https://github.com/resilientinfrastructure/streamlit-panderas/actions/workflows/e2e.yml/badge.svg)](https://github.com/resilientinfrastructure/streamlit-panderas/actions/workflows/e2e.yml)
 
-Streamlit-Panderas is your go-to tool for clean data ingestion, seamlessly integrating Streamlit and Panderas to make your data processing tasks a breeze.
+Streamlit-Panderas is your go-to tool for clean data ingestion and validation, seamlessly integrating Streamlit and Panderas to make your data processing tasks a breeze.
 
 ## Features
 
 - **Easy Data Ingestion:** Select your file format (CSV or JSON) and provide a URL to a Panderas schema.
 - **Streamlined Validation:** With just a few clicks, submit your selections and validate your data effortlessly.
 
 
@@ -44,17 +44,17 @@
 ```
 
 ## Usage instructions
 
 ```python
 import streamlit as st
 
-from streamlit_pandera.validate_file  import run
+from streamlit_pandera.validate_file  import run_validate_file
 
-validated_df = run()
+validated_df = run_validate_file()
 
 st.write(validated_df)
 ```
 
 
 ## Instructions
 
@@ -66,15 +66,15 @@
 
 ### Step 3: Submit and Validate
 Hit that submit button and let Streamlit-Panderas work its magic! Your data will be validated against the specified schema in no time.
 
 
 [Go to Demo](https://youtu.be/9Ry_A9LgrbQ)
 
-
+[![Video](http://img.youtube.com/vi/9Ry_A9LgrbQ/0.jpg)](https://youtu.be/9Ry_A9LgrbQ)
 
 
 ## Run Tests
 To ensure everything is functioning smoothly, run the tests using the following commands:
 
 ```bash
 poetry install
```

