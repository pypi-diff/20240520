# Comparing `tmp/rdatapp-0.5.tar.gz` & `tmp/rdatapp-0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdatapp-0.5.tar", last modified: Sun May 19 01:39:34 2024, max compression
+gzip compressed data, was "rdatapp-0.6a0.tar", last modified: Mon May 20 11:06:22 2024, max compression
```

## Comparing `rdatapp-0.5.tar` & `rdatapp-0.6a0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:39:34.661285 rdatapp-0.5/
--rw-r--r--   0 ifozmen    (501) staff       (20)      569 2024-05-19 01:39:34.661167 rdatapp-0.5/PKG-INFO
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:39:34.660401 rdatapp-0.5/rdatapp/
--rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.5/rdatapp/__init__.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1407 2024-05-19 01:08:24.000000 rdatapp-0.5/rdatapp/categorical_encoder.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1067 2024-05-18 22:01:35.000000 rdatapp-0.5/rdatapp/data_type_converter.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1170 2024-05-18 22:04:22.000000 rdatapp-0.5/rdatapp/datetime_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      624 2024-05-18 22:04:31.000000 rdatapp-0.5/rdatapp/feature_engineer.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     2245 2024-05-18 21:48:09.000000 rdatapp-0.5/rdatapp/missing_value_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)      844 2024-05-18 22:01:04.000000 rdatapp-0.5/rdatapp/outlier_handler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1145 2024-05-18 21:56:43.000000 rdatapp-0.5/rdatapp/scaler.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     3316 2024-05-19 01:24:37.000000 rdatapp-0.5/rdatapp/test.py
--rw-r--r--   0 ifozmen    (501) staff       (20)     1212 2024-05-18 21:57:57.000000 rdatapp-0.5/rdatapp/text_cleaner.py
-drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-19 01:39:34.660987 rdatapp-0.5/rdatapp.egg-info/
--rw-r--r--   0 ifozmen    (501) staff       (20)      569 2024-05-19 01:39:34.000000 rdatapp-0.5/rdatapp.egg-info/PKG-INFO
--rw-r--r--   0 ifozmen    (501) staff       (20)      418 2024-05-19 01:39:34.000000 rdatapp-0.5/rdatapp.egg-info/SOURCES.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-19 01:39:34.000000 rdatapp-0.5/rdatapp.egg-info/dependency_links.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-19 01:39:34.000000 rdatapp-0.5/rdatapp.egg-info/requires.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-19 01:39:34.000000 rdatapp-0.5/rdatapp.egg-info/top_level.txt
--rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-19 01:39:34.661329 rdatapp-0.5/setup.cfg
--rw-rw-r--   0 ifozmen    (501) staff       (20)      821 2024-05-19 01:39:26.000000 rdatapp-0.5/setup.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:06:22.604677 rdatapp-0.6a0/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-20 11:06:22.604488 rdatapp-0.6a0/PKG-INFO
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:06:22.603396 rdatapp-0.6a0/rdatapp/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      651 2024-05-19 01:23:55.000000 rdatapp-0.6a0/rdatapp/__init__.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1823 2024-05-20 10:38:30.000000 rdatapp-0.6a0/rdatapp/categorical_encoder.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1404 2024-05-20 10:39:16.000000 rdatapp-0.6a0/rdatapp/data_type_converter.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1474 2024-05-20 10:39:41.000000 rdatapp-0.6a0/rdatapp/datetime_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)      969 2024-05-20 10:42:18.000000 rdatapp-0.6a0/rdatapp/feature_engineer.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     2638 2024-05-20 10:44:02.000000 rdatapp-0.6a0/rdatapp/missing_value_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1155 2024-05-20 10:45:07.000000 rdatapp-0.6a0/rdatapp/outlier_handler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1464 2024-05-20 10:45:34.000000 rdatapp-0.6a0/rdatapp/scaler.py
+-rw-r--r--   0 ifozmen    (501) staff       (20)     1389 2024-05-20 10:46:15.000000 rdatapp-0.6a0/rdatapp/text_cleaner.py
+drwxr-xr-x   0 ifozmen    (501) staff       (20)        0 2024-05-20 11:06:22.604247 rdatapp-0.6a0/rdatapp.egg-info/
+-rw-r--r--   0 ifozmen    (501) staff       (20)      571 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/PKG-INFO
+-rw-r--r--   0 ifozmen    (501) staff       (20)      402 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/SOURCES.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        1 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/dependency_links.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       31 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/requires.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)        8 2024-05-20 11:06:22.000000 rdatapp-0.6a0/rdatapp.egg-info/top_level.txt
+-rw-r--r--   0 ifozmen    (501) staff       (20)       38 2024-05-20 11:06:22.604767 rdatapp-0.6a0/setup.cfg
+-rw-rw-r--   0 ifozmen    (501) staff       (20)      822 2024-05-20 11:06:15.000000 rdatapp-0.6a0/setup.py
```

### Comparing `rdatapp-0.5/PKG-INFO` & `rdatapp-0.6a0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.5
+Version: 0.6a0
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: izzettin furkan özmen, ismail cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rdatapp-0.5/rdatapp/__init__.py` & `rdatapp-0.6a0/rdatapp/__init__.py`

 * *Files identical despite different names*

### Comparing `rdatapp-0.5/rdatapp/categorical_encoder.py` & `rdatapp-0.6a0/rdatapp/categorical_encoder.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,37 +3,44 @@
 from sklearn.preprocessing import OneHotEncoder, LabelEncoder
 
 class CategoricalEncoder:
     @staticmethod
     def one_hot_encode(df, column):
         """
         One-hot encodes a categorical column in a DataFrame.
+        
+        This method converts a categorical column into a new DataFrame with binary columns 
+        for each category and then concatenates it to the original DataFrame, dropping the original column.
 
         Parameters:
         df (pandas.DataFrame): The DataFrame containing the categorical column.
         column (str): The name of the categorical column to be one-hot encoded.
 
         Returns:
-        pandas.DataFrame: The DataFrame with the categorical column one-hot encoded and the original column dropped.
+        pandas.DataFrame: The DataFrame with the one-hot encoded column and the original column removed.
         """
         encoder = OneHotEncoder(sparse_output=False)
         encoded = encoder.fit_transform(df[[column]])
         encoded_df = pd.DataFrame(encoded, columns=encoder.get_feature_names_out([column]))
         return pd.concat([df, encoded_df], axis=1).drop(columns=[column])
 
     @staticmethod
     def label_encode(df, column):
         """
-        Encodes the specified column in the given DataFrame using label encoding.
+        Label encodes a categorical column in a DataFrame.
+
+        This method converts each category in a column into a numeric label. This is useful 
+        for converting categorical data into a format suitable for machine learning algorithms 
+        that require numerical input.
 
         Parameters:
-        - df (pandas.DataFrame): The DataFrame containing the column to be encoded.
-        - column (str): The name of the column to be encoded.
+        df (pandas.DataFrame): The DataFrame containing the column to be label encoded.
+        column (str): The name of the column to be label encoded.
 
         Returns:
-        - df (pandas.DataFrame): The DataFrame with the encoded column.
+        pandas.DataFrame: The DataFrame with the label encoded column.
         """
         encoder = LabelEncoder()
         df[column] = encoder.fit_transform(df[column])
         return df
```

### Comparing `rdatapp-0.5/rdatapp/data_type_converter.py` & `rdatapp-0.6a0/rdatapp/data_type_converter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import pandas as pd
 
 class DataTypeConverter:
     @staticmethod
     def to_numeric(df, column):
         """
         Convert the values in a specific column of a DataFrame to numeric type.
+        
+        This method attempts to convert all values in the specified column to a numeric type. 
+        Non-numeric values will be set as NaN.
 
         Parameters:
         df (pandas.DataFrame): The DataFrame containing the column to be converted.
         column (str): The name of the column to be converted.
 
         Returns:
         pandas.DataFrame: The DataFrame with the converted column.
-
         """
         df[column] = pd.to_numeric(df[column], errors='coerce')
         return df
 
     @staticmethod
     def to_categorical(df, column):
         """
         Convert a column in a DataFrame to categorical data type.
+        
+        This method changes the data type of the specified column to 'category', 
+        which can help reduce memory usage and improve performance for categorical data.
 
         Parameters:
         df (pandas.DataFrame): The DataFrame containing the column to be converted.
         column (str): The name of the column to be converted.
 
         Returns:
         pandas.DataFrame: The DataFrame with the specified column converted to categorical data type.
         """
         df[column] = df[column].astype('category')
-        return df
+        return df
```

### Comparing `rdatapp-0.5/rdatapp/datetime_handler.py` & `rdatapp-0.6a0/rdatapp/datetime_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import pandas as pd
 
 class DateTimeHandler:
     @staticmethod
     def to_datetime(df, column):
         """
         Converts a column in a DataFrame to datetime format.
-        
+
+        This method attempts to convert all values in the specified column to datetime format. 
+        Any values that cannot be converted will be set as NaT (Not a Time).
+
         Args:
             df (pandas.DataFrame): The DataFrame containing the column to be converted.
             column (str): The name of the column to be converted.
-            
+
         Returns:
-            pandas.DataFrame: The DataFrame with the converted column.
+            pandas.DataFrame: The DataFrame with the column converted to datetime format.
         """
         df[column] = pd.to_datetime(df[column], errors='coerce')
         return df
 
     @staticmethod
     def extract_date_parts(df, column):
         """
         Extracts year, month, and day from a datetime column in a DataFrame.
 
+        This method creates new columns for the year, month, and day extracted from 
+        the specified datetime column.
+
         Args:
             df (pandas.DataFrame): The DataFrame containing the datetime column.
             column (str): The name of the datetime column.
 
         Returns:
             pandas.DataFrame: The DataFrame with additional columns for year, month, and day.
-
         """
         df[f'{column}_year'] = df[column].dt.year
         df[f'{column}_month'] = df[column].dt.month
         df[f'{column}_day'] = df[column].dt.day
-        return df
+        return df
```

### Comparing `rdatapp-0.5/rdatapp/feature_engineer.py` & `rdatapp-0.6a0/rdatapp/feature_engineer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 class FeatureEngineer:
     @staticmethod
     def create_new_feature(df, column, func):
         """
         Creates a new feature in the given DataFrame by applying the specified function to the specified column.
+        
+        This method applies a given function to each element of a specified column, creating a new column 
+        with the results.
 
         Args:
             df (pandas.DataFrame): The DataFrame to modify.
             column (str): The name of the column to apply the function to.
-            func (callable): The function to apply to the column.
+            func (callable): The function to apply to the column. This function should take a single 
+                             argument and return a single value.
 
         Returns:
-            pandas.DataFrame: The modified DataFrame with the new feature added.
+            pandas.DataFrame: The modified DataFrame with the new feature added as a new column. 
+                              The new column will be named as '{column}_new'.
         """
         df[f'{column}_new'] = df[column].apply(func)
-        return df
+        return df
```

### Comparing `rdatapp-0.5/rdatapp/missing_value_handler.py` & `rdatapp-0.6a0/rdatapp/missing_value_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,60 +2,67 @@
 
 class MissingValueHandler:
     @staticmethod
     def impute_mean(df, column):
         """
         Imputes missing values in a DataFrame column with the mean value of the column.
 
+        This method fills missing values in the specified column using the mean of that column.
+
         Parameters:
         - df (pandas.DataFrame): The DataFrame containing the column to be imputed.
         - column (str): The name of the column to be imputed.
 
         Returns:
-        - df (pandas.DataFrame): The DataFrame with the imputed column.
-
+        - pandas.DataFrame: The DataFrame with the imputed column.
         """
         df[column] = df[column].fillna(df[column].mean())
         return df
 
     @staticmethod
     def impute_median(df, column):
         """
         Imputes missing values in a specific column of a DataFrame with the median value of that column.
-        
+
+        This method fills missing values in the specified column using the median of that column.
+
         Parameters:
             df (pandas.DataFrame): The DataFrame containing the column with missing values.
             column (str): The name of the column to impute missing values.
-            
+
         Returns:
             pandas.DataFrame: The DataFrame with missing values imputed using the median value of the column.
         """
         df[column] = df[column].fillna(df[column].median())
         return df
 
     @staticmethod
     def impute_constant(df, column, value):
         """
         Imputes missing values in a specific column of a DataFrame with a constant value.
 
-        Args:
+        This method fills missing values in the specified column using a provided constant value.
+
+        Parameters:
             df (pandas.DataFrame): The DataFrame containing the column with missing values.
             column (str): The name of the column to impute.
             value: The constant value to fill the missing values with.
 
         Returns:
             pandas.DataFrame: The DataFrame with the missing values imputed.
         """
         df[column] = df[column].fillna(value)
         return df
 
     @staticmethod
     def delete_missing(df, column):
         """
-        Delete rows with missing values in the specified column.
+        Deletes rows with missing values in the specified column.
+
+        This method removes all rows from the DataFrame that contain missing values in the specified column.
 
         Parameters:
         - df (pandas.DataFrame): The input DataFrame.
         - column (str): The name of the column to check for missing values.
 
         Returns:
         - pandas.DataFrame: The DataFrame with rows containing missing values in the specified column removed.
```

### Comparing `rdatapp-0.5/rdatapp/text_cleaner.py` & `rdatapp-0.6a0/rdatapp/text_cleaner.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,28 @@
         It initializes the stop words set with the English stopwords and creates
         a WordNetLemmatizer object for lemmatization.
         """
         self.stop_words = set(stopwords.words('english'))
         self.lemmatizer = WordNetLemmatizer()
 
     def clean_text(self, text):
-            """
-            Cleans the given text by converting it to lowercase, removing punctuation,
-            removing stop words, and lemmatizing the words.
+        """
+        Cleans the given text by converting it to lowercase, removing punctuation,
+        removing stop words, and lemmatizing the words.
+
+        This method performs several text preprocessing steps:
+        1. Converts the text to lowercase.
+        2. Removes punctuation.
+        3. Removes English stop words.
+        4. Lemmatizes the words in the text.
 
-            Args:
-                text (str): The text to be cleaned.
+        Args:
+            text (str): The text to be cleaned.
 
-            Returns:
-                str: The cleaned text.
-            """
-            text = text.lower()
-            text = re.sub(r'[^\w\s]', '', text)
-            text = ' '.join([word for word in text.split() if word not in self.stop_words])
-            text = ' '.join([self.lemmatizer.lemmatize(word) for word in text.split()])
-            return text
+        Returns:
+            str: The cleaned text.
+        """
+        text = text.lower()
+        text = re.sub(r'[^\w\s]', '', text)
+        text = ' '.join([word for word in text.split() if word not in self.stop_words])
+        text = ' '.join([self.lemmatizer.lemmatize(word) for word in text.split()])
+        return text
```

### Comparing `rdatapp-0.5/rdatapp.egg-info/PKG-INFO` & `rdatapp-0.6a0/rdatapp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdatapp
-Version: 0.5
+Version: 0.6a0
 Summary: A recoded data preprocessing library for handling various data cleaning and transformation tasks. The library includes classes for text cleaning, missing value imputation, one-hot encoding and more.
 Home-page: https://github.com/Beegash/Recoded-Data-Processing-Library
 Author: izzettin furkan özmen, ismail cifci
 Author-email: izzettinfurkan.ozmen@stu.fsm.edu.tr, ismail.cifci@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `rdatapp-0.5/setup.py` & `rdatapp-0.6a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rdatapp',
-    version='0.5',
+    version='0.6a',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
     ],
```

