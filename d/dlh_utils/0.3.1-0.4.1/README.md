# Comparing `tmp/dlh_utils-0.3.1.tar.gz` & `tmp/dlh_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlh_utils-0.3.1.tar", max compression
+gzip compressed data, was "dlh_utils-0.4.1.tar", max compression
```

## Comparing `dlh_utils-0.3.1.tar` & `dlh_utils-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0     2743 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/LICENSE
--rw-r--r--   0        0        0     3220 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/README.md
--rw-r--r--   0        0        0      378 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/__init__.py
--rw-r--r--   0        0        0      141 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/_version.py
--rwxr-xr-x   0        0        0    74673 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/dataframes.py
--rw-r--r--   0        0        0    15780 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/flags.py
--rwxr-xr-x   0        0        0    41020 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/linkage.py
--rw-r--r--   0        0        0    15273 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/profiling.py
--rw-r--r--   0        0        0     6442 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/sessions.py
--rw-r--r--   0        0        0    47883 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/standardisation.py
--rwxr-xr-x   0        0        0        0 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/__init__.py
--rwxr-xr-x   0        0        0      904 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/conftest.py
--rw-r--r--   0        0        0    27443 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_dataframes.py
--rw-r--r--   0        0        0    21704 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_flags.py
--rw-r--r--   0        0        0    22391 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_linkage.py
--rw-r--r--   0        0        0    31733 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_standardisation.py
--rw-r--r--   0        0        0    30872 2023-04-26 10:09:02.632761 dlh_utils-0.3.1/dlh_utils/utilities.py
--rw-r--r--   0        0        0      829 2023-04-26 10:09:02.632761 dlh_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 dlh_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2743 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3604 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/README.md
+-rw-r--r--   0        0        0      378 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/_version.py
+-rwxr-xr-x   0        0        0    74547 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/dataframes.py
+-rwxr-xr-x   0        0        0    25027 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/disco.py
+-rw-r--r--   0        0        0    15718 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/flags.py
+-rwxr-xr-x   0        0        0    19248 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/formatting.py
+-rwxr-xr-x   0        0        0    38701 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/linkage.py
+-rw-r--r--   0        0        0    15274 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/profiling.py
+-rw-r--r--   0        0        0     6530 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/sessions.py
+-rw-r--r--   0        0        0    49576 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/standardisation.py
+-rwxr-xr-x   0        0        0        0 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/__init__.py
+-rwxr-xr-x   0        0        0      873 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/conftest.py
+-rw-r--r--   0        0        0    31807 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_dataframes.py
+-rw-r--r--   0        0        0    16281 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_flags.py
+-rwxr-xr-x   0        0        0    17592 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_formatting.py
+-rw-r--r--   0        0        0    34901 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_linkage.py
+-rwxr-xr-x   0        0        0     3933 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_profiling.py
+-rw-r--r--   0        0        0    43788 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_standardisation.py
+-rwxr-xr-x   0        0        0     5721 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/tests/test_utilities.py
+-rw-r--r--   0        0        0    31670 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/dlh_utils/utilities.py
+-rw-r--r--   0        0        0      779 2024-05-20 07:53:13.295427 dlh_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4650 1970-01-01 00:00:00.000000 dlh_utils-0.4.1/PKG-INFO
```

### Comparing `dlh_utils-0.3.1/LICENSE` & `dlh_utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlh_utils-0.3.1/README.md` & `dlh_utils-0.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,21 @@
 ```sh
 pip3 install -U dlh_utils
 ```
 
 ## Demo
 For a worked demonstration notebook of these functions being applied within a data linkage context, head over to our [separate demo repository](https://github.com/anthonye93/dlh_utils_demo)
 
+## Contributing
+
+This repository adheres to pep8 coding standards. These can be automatically checked for when you're making new commits by the repository's pre-commit hooks. To get this working:
+* `pip install` both 'flake8' and 'pre-commit'
+* install the git hook scripts `pre-commit install`
+* When adding new git commits, the pre-commit hooks will now run and make suggestions needed to adhere to pep8 code standards
+
 ## Common issues
 
 ### When using the jaro/jaro_winkler functions the error "no module called Jellyfish found" is thrown
 
 These functions are dependent on the Jellyfish package and this may not be installed on the executors used in your spark session.
 Try submitting Jellyfish to your sparkcontext via addPyFile() or by setting the following environmental variables in your CDSW engine settings (ONS only):
 
@@ -60,8 +67,8 @@
 
 ## Thanks
 
 Thanks to all those in the Data Linkage Hub, Data Engineering and Methodology at ONS that have contributed towards this repository.
 
 ## Any questions?
 
-If you need any additional help, or have any feedback on the package, please contact Jenna Hart (Jenna.Hart@ons.gov.uk) or the Data Linkage Hub at Linkage.Hub@ons.gov.uk . 
+If you need any additional help, or have any feedback on the package, please contact the Data Linkage Hub at Linkage.Hub@ons.gov.uk .
```

### Comparing `dlh_utils-0.3.1/dlh_utils/dataframes.py` & `dlh_utils-0.4.1/dlh_utils/dataframes.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     regex : string, default = None
       This parameter takes a string value in
       regex format and selects columns from the
       dataframe if the column title matches
       the conditions of the regex string.
 
     drop_duplicates : bool, default = True
-      This parameter drops duplicated columns.
+      This parameter drops duplicated rows.
 
     Returns
     -------
     dataframe
       Dataframe with columns limited to those
       specified by the parameters.
 
@@ -270,32 +270,32 @@
      |    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
      |  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|
      +--------+----------+-------+----------+---+--------+
 
     """
 
     if startswith is not None:
-        df = df.drop(*
-                     [x for x in df.columns if x.startswith(startswith)]
-                     )
+        df = df.drop(
+            * [x for x in df.columns if x.startswith(startswith)]
+        )
 
     if endswith is not None:
-        df = df.drop(*
-                     [x for x in df.columns if x.endswith(endswith)]
-                     )
+        df = df.drop(
+            * [x for x in df.columns if x.endswith(endswith)]
+        )
 
     if contains is not None:
-        df = df.drop(*
-                     [x for x in df.columns if contains in x]
-                     )
+        df = df.drop(
+            * [x for x in df.columns if contains in x]
+        )
 
     if regex is not None:
-        df = df.drop(*
-                     [x for x in df.columns if re.search(regex, x)]
-                     )
+        df = df.drop(
+            * [x for x in df.columns if re.search(regex, x)]
+        )
 
     if subset is not None:
         if not isinstance(subset, list):
             subset = [subset]
         df = df.drop(*subset)
 
     if drop_duplicates:
@@ -483,15 +483,15 @@
 
         df = (df
               .where(F.col(column).rlike(on))
               .select(*[x for x in df.columns if x != column],
                       F.explode(F.split(F.col(column), on))
                       .alias(column))
               .unionByName((df
-                           .where((F.col(column).rlike(on) == False)
+                           .where(~(F.col(column).rlike(on))
                                   | (F.col(column).rlike(on).isNull()))))
               )
 
     if retain is True:
 
         if flag is None:
 
@@ -504,15 +504,15 @@
                   )
 
         else:
 
             df = (df
                   .where(F.col(column).rlike(on))
                   .withColumn(flag, F.lit(True))
-                  .select(*[x for x in df.columns+[flag] if x != column],
+                  .select(*[x for x in df.columns + [flag] if x != column],
                           F.explode(F.split(F.col(column), on))
                           .alias(column))
                   .unionByName(df.withColumn(flag, F.lit(False)))
                   )
 
     if drop_duplicates is True:
         df = df.dropDuplicates()
@@ -732,15 +732,15 @@
 
     """
 
     if not isinstance(exclude, list):
         exclude = [exclude]
 
     old = [x for x in df.columns if x not in exclude]
-    new = [x+suffix for x in old]
+    new = [x + suffix for x in old]
 
     rename = dict(zip(old, new))
 
     for old, new in rename.items():
         df = df.withColumnRenamed(old, new)
 
     return df
@@ -1088,55 +1088,55 @@
     if mode == 'countDistinct':
 
         df = df.fillna("<<<>>>", subset=window)
 
         if alias is not None:
             if drop_na is True:
                 df = (df
-                      .dropDuplicates(subset=window+[target])
+                      .dropDuplicates(subset=window + [target])
                       .dropna(subset=[target])
-                      .select(*window+[target],
+                      .select(*window + [target],
                               F.count(target)
                               .over(window_spec)
                               .alias(alias))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
             else:
                 df = (df
-                      .dropDuplicates(subset=window+[target])
-                      .select(*window+[target],
+                      .dropDuplicates(subset=window + [target])
+                      .select(*window + [target],
                               F.count(target)
                               .over(window_spec)
                               .alias(alias))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
 
         else:
             if drop_na is True:
                 df = (df
-                      .dropDuplicates(subset=window+[target])
+                      .dropDuplicates(subset=window + [target])
                       .dropna(subset=[target])
-                      .select(*window+[target],
+                      .select(*window + [target],
                               F.count(target)
                               .over(window_spec))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
             else:
                 df = (df
-                      .dropDuplicates(subset=window+[target])
-                      .select(*window+[target],
+                      .dropDuplicates(subset=window + [target])
+                      .select(*window + [target],
                               F.count(target)
                               .over(window_spec))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
@@ -1157,15 +1157,15 @@
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
                           on=window,
                           how='left_anti')
                     )
 
             df = (union_all(df_1, df_2)
-                  .select(window+[alias])
+                  .select(window + [alias])
                   .dropDuplicates()
                   .join(df,
                         on=window,
                         how='right')
                   )
 
         else:
@@ -1198,28 +1198,28 @@
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.max(target)
                             .over(window_spec)
                             .alias(alias))
-                    .select(window+[alias])
+                    .select(window + [alias])
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
                           on=window,
                           how='left_anti')
                     .select(window)
                     )
 
             df = (union_all(df_1, df_2)
-                  .select(window+[alias])
+                  .select(window + [alias])
                   .dropDuplicates()
                   .join(df,
                         on=window,
                         how='right')
                   )
 
         else:
@@ -1260,28 +1260,28 @@
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.sum(target)
                             .over(window_spec)
                             .alias(alias))
-                    .select(window+[alias])
+                    .select(window + [alias])
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
                           on=window,
                           how='left_anti')
                     .select(window)
                     )
 
             df = (union_all(df_1, df_2)
-                  .select(window+[alias])
+                  .select(window + [alias])
                   .dropDuplicates()
                   .join(df,
                         on=window,
                         how='right')
                   )
 
         else:
@@ -1427,15 +1427,16 @@
     +---+---+----------+-------+----------+---+--------+
     |  3|  4|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  5|  1|      null|Simpson|2021-01-12|  F|ET74 2SP|
     |  1|  2|       Jay|Simpson|1983-05-12|  M|ET74 2SP|
     |  4|  5|     Marie|Simpson|2014-05-09|  F|ET74 2SP|
     |  2|  3|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|
     +---+---+----------+-------+----------+---+--------+
-
+    The records are grouped by ID, and then the minimum age for each record
+    is returned. Therefore, the age '6' for ID '3' is removed.
 
     See Also
     --------
     standardisation.fill_nulls()
     """
 
     if not isinstance(filter_window, list):
@@ -1457,45 +1458,34 @@
             df = (window(df, filter_window, target, mode, alias='count')
                   .where(F.col('count') != value)
                   .drop('count')
                   )
 
     if mode in ['min', 'max']:
 
-        if condition:
-
-            df = window(df, filter_window, target, mode, alias='value')
-
-            df = st.fill_nulls(df, fill='<<<>>>', subset=['value']+[target])
+        dt_target = [dtype for name, dtype in df.dtypes if name == target][0]
+        df = window(df, filter_window, target, mode, alias='value')
+        df = st.fill_nulls(df, fill='<<<>>>', subset=['value'] + [target])
 
+        if condition:
             df = (df
                   .where(F.col(target) == F.col('value'))
                   .drop('value')
                   )
-
-            df = (st.standardise_null(df=df,
-                                      replace="^<<<>>>$",
-                                      subset=target)
-                  )
-
         else:
-
-            df = window(df, filter_window, target, mode, alias='value')
-
-            df = st.fill_nulls(df, fill='<<<>>>', subset=['value']+[target])
-
             df = (df
                   .where(F.col(target) != F.col('value'))
                   .drop('value')
                   )
 
-            df = (st.standardise_null(df=df,
-                                      replace="^<<<>>>$",
-                                      subset=target)
-                  )
+        df = (st.standardise_null(df=df,
+                                  replace="^<<<>>>$",
+                                  subset=target)
+              )
+        df = df.withColumn(target, F.col(target).cast(dt_target))
 
     return df
 
 ###############################################################################
 
 
 def literal_column(df, col_name, literal):
@@ -1568,15 +1558,15 @@
       Subset of columns being coalesced together
       into a single column, if subset = None then
       subset = all columns in dataframe.
     output_col : string, default = 'coalesced_col'
       Name of the output column for results of
       the coalesced columns.
     drop : boolean, default = False
-      If drop = True, the columns that were coalesced 
+      If drop = True, the columns that were coalesced
       will be dropped from the dataframe.
 
     Returns
     -------
     dataframe
       Dataframe with coalesced columns results
       appended to original dataframe in the
@@ -1751,15 +1741,15 @@
             df = (df.
                   withColumn(out_col, F.col(split_col)
                              .getItem(index)))
 
         if index < 0:
             df = (df
                   .withColumn(out_col, F.reverse(F.col(split_col))
-                              .getItem(abs(index)-1)))
+                              .getItem(abs(index) - 1)))
 
     return df
 
 #############################################################################
 
 
 def clone_column(df, target, clone):
@@ -1987,15 +1977,15 @@
         df = df.where(F.col(threshold_column) <= val)
     return df
 
 ###############################################################################
 
 
 def date_diff(df, col_name1, col_name2, diff='Difference',
-              in_date_format='dd-mm-yyyy', units='days', absolute=True):
+              in_date_format='dd-MM-yyyy', units='days', absolute=True):
     """
     date_diff finds the number of days/months/years between two date columns
     by subtracting the dates in the second column from the dates in the first.
     Note, using just months is currently inaccurate as all months are assumed
     to have 31 days.
 
     Parameters
@@ -2007,15 +1997,15 @@
       dates.
     col_name2 : string
       Name of second column with values representing
       dates.
     diff : string, default = 'Difference'
       Name of the column in which the difference between
       dates will be shown.
-    in_date_format : string, default = 'dd-mm-yyyy'
+    in_date_format : string, default = 'dd-MM-yyyy'
       User must specify the format of how the dates are entered
       in both colName1 and colName2 and use this argument to
       do so.
     units : {'days','months','years'}
       units of how the difference in the two date columns
       will be represented in the 'diff' arg column.
     absolute : bool, default = True
@@ -2070,19 +2060,19 @@
 
     """
 
     df = df.withColumn(diff, F.unix_timestamp(F.col(col_name1), in_date_format)
                        - F.unix_timestamp(F.col(col_name2), in_date_format))
 
     if units == 'days':
-        df = df.withColumn(diff, (F.col(diff)/86400))
+        df = df.withColumn(diff, (F.col(diff) / 86400))
         df = df.withColumn(diff, F.round(diff, 2))
     elif units == 'months':
         # months value is slightly inaccurate as it assumes every month is a 31 day month
-        df = df.withColumn(diff, F.col(diff)/(31*86400))
+        df = df.withColumn(diff, F.col(diff) / (31 * 86400))
         df = df.withColumn(diff, F.round(diff, 2))
     elif units == 'years':
-        df = df.withColumn(diff, F.col(diff)/(86400*365))
+        df = df.withColumn(diff, F.col(diff) / (86400 * 365))
         df = df.withColumn(diff, F.round(diff, 2))
     if absolute is True:
         df = df.withColumn(diff, F.abs((F.col(diff))))
     return df
```

### Comparing `dlh_utils-0.3.1/dlh_utils/flags.py` & `dlh_utils-0.4.1/dlh_utils/flags.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pyspark.sql.types import IntegerType
 import pyspark.sql.functions as F
 import pandas as pd
 
 ###############################################################################
 
 
-def flag(df, ref_col, condition = None, condition_value=None, condition_col=None,
+def flag(df, ref_col, condition=None, condition_value=None, condition_col=None,
          alias=None, prefix='FLAG', fill_null=None):
     """
     Adds True or False flags to supplied dataframe that can then be used for
     quality checks.
 
     Conditions can be set in comparison to columns or specific values
     (e.g. == column, ==1).  Conditions covered are equals, not equals,
@@ -176,37 +176,34 @@
         df = df.withColumn(alias,
                            (F.col(ref_col).isNull()) | (
                                F.isnan(F.col(ref_col)))
                            )
 
     if condition == 'isNotNull':
         df = df.withColumn(alias,
-                           (F.col(ref_col).isNotNull()) & (
-                               F.isnan(F.col(ref_col)) == False)
+                           (F.col(ref_col).isNotNull()) & ~(
+                               F.isnan(F.col(ref_col)))
                            )
-   
+
     if condition == 'regex':
         df = df.withColumn(alias,
-                          (F.col(ref_col).rlike(condition_value)
-                          ))
+                           (F.col(ref_col).rlike(condition_value))
+                           )
 
     if fill_null is not None:
         df = (df
               .withColumn(alias,
                           F.when(F.col(alias).isNull(),
                                  fill_null)
                           .otherwise(F.col(alias)))
               )
 
     return df
 ###############################################################################
 
-# Potential to imporve with automated identifiaction of flag columns
-# e.g. through prefix or regex - as used in flag_check())
-
 
 def flag_summary(df, flags=None, pandas=False):
     """
     Produces summary table of boolean flag columns.
 
     Produces a summary of True/False counts and percentages.
     Option to output as pandas or spark dataframe (default
@@ -269,26 +266,25 @@
 
     flags_out = []
 
     for col in flags:
 
         flags_out.append((df
                           .select(col)
-                         .where(F.col(col) == True)
-
+                          .where(F.col(col) == F.lit(True))
                           .count()
                           ))
 
     out = pd.DataFrame({
         'flag': flags,
         'true': flags_out,
-        'false': [rows-x for x in flags_out],
+        'false': [rows - x for x in flags_out],
         'rows': rows,
-        'percent_true': [(x/rows)*100 for x in flags_out],
-        'percent_false': [100-((x/rows)*100) for x in flags_out]
+        'percent_true': [(x / rows) * 100 for x in flags_out],
+        'percent_false': [100 - ((x / rows) * 100) for x in flags_out]
     })
 
     out = out[[
         'flag',
         'true',
         'false',
         'rows',
@@ -303,15 +299,15 @@
                .coalesce(1))
 
     return out
 
 ###############################################################################
 
 
-def flag_check(df, prefix='FLAG_', flags=None,  mode='master', summary=False):
+def flag_check(df, prefix='FLAG_', flags=None, mode='master', summary=False):
     """
     Reads flag columns and counts True/ Fail values.
 
     Adds flag count column (counting TRUE/Fail values) and overall
     fail column (TRUE/FALSE and flag TRUE/Fail). If any rows in the flag count
     column are greater than 0, the overall fail value for this row will be True so
     this is quickly highlighted to the user.
@@ -398,51 +394,51 @@
 
     df = df.withColumn('flag_count', F.lit(0))
 
     for flag in flags:
 
         df = (df
               .withColumn('flag_count',
-                          F.when(F.col(flag) == True,
-                                 F.col('flag_count')+1)
+                          F.when(F.col(flag),
+                                 F.col('flag_count') + F.lit(1))
                           .otherwise(F.col('flag_count')))
               )
 
     df = df.withColumn("FAIL",
                        reduce(add, [F.col(flag).cast(IntegerType())
                                     for flag in flags]))
     df = df.withColumn('FAIL', F.col('FAIL') > 0)
 
     if summary is True:
 
-        summary_df = flag_summary(df, flags+['FAIL'], pandas=False)
+        summary_df = flag_summary(df, flags + ['FAIL'], pandas=False)
 
         if mode == 'master':
             return (df,
                     summary_df)
 
         if mode == 'split':
-            return ((df.where(F.col('Fail') == False)),
-                    (df.where(F.col('Fail') == True)),
+            return ((df.where(F.col('FAIL') == F.lit(False))),
+                    (df.where(F.col('FAIL') == F.lit(True))),
                     summary_df)
 
         if mode == 'pass':
-            return (df.where(F.col('Fail') == False),
+            return (df.where(F.col('FAIL') == F.lit(False)),
                     summary_df)
 
         if mode == 'fail':
-            return (df.where(F.col('Fail') == True),
+            return (df.where(F.col('FAIL') == F.lit(True)),
                     summary_df)
 
     else:
         if mode == 'master':
             return df
 
         if mode == 'split':
-            return ((df.where(F.col('Fail') == False)),
-                    (df.where(F.col('Fail') == True)))
+            return ((df.where(F.col('FAIL') == F.lit(False))),
+                    (df.where(F.col('FAIL') == F.lit(True))))
 
         if mode == 'pass':
-            return df.where(F.col('Fail') == False)
+            return df.where(F.col('FAIL') == F.lit(False))
 
         if mode == 'fail':
-            return df.where(F.col('Fail') == True)
+            return df.where(F.col('FAIL') == F.lit(True))
```

### Comparing `dlh_utils-0.3.1/dlh_utils/linkage.py` & `dlh_utils-0.4.1/dlh_utils/linkage.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,68 +8,84 @@
 import py4j
 from pyspark.sql import SparkSession, Window
 import pyspark.sql.functions as F
 from pyspark.sql.types import StringType, FloatType
 from graphframes import GraphFrame
 from dlh_utils import dataframes as da
 from dlh_utils import utilities as ut
+from difflib import SequenceMatcher
 
 ###############################################################################
 
-# phonetic encoders
+# Phonetic Encoders
 
 
 def alpha_name(df, input_col, output_col):
     """
-    Orders string columns alphabetically, also setting them to UPPER CASE.
+    Orders each field of a string column alphabetically, also setting to UPPER CASE.
+    If input_col contains a Null, this will remain in output_col
 
     Parameters
     ----------
-    df: dataframe
+    df: Spark dataframe
     input_col: string
       name of column to be sorted alphabetically
     output_col: string
       name of column to be output
 
     Returns
     -------
     a dataframe with output_col appended
 
+    Raises
+    ------
+    Exception if input_col not string type
+
     Example
     --------
 
     > df.show()
     +---+--------+
     | ID|Forename|
     +---+--------+
     |  1|   Homer|
     |  2|   Marge|
     |  3|    Bart|
     |  4|    Lisa|
     |  5|  Maggie|
+    |  6|    null|
     +---+--------+
 
     > alpha_name(df,'Forename','alphaname').show()
     +---+--------+---------+
     | ID|Forename|alphaname|
     +---+--------+---------+
     |  1|   Homer|    EHMOR|
     |  2|   Marge|    AEGMR|
     |  3|    Bart|     ABRT|
     |  4|    Lisa|     AILS|
     |  5|  Maggie|   AEGGIM|
+    |  6|    null|     null|
     +---+--------+---------+
 
     """
-    df = df.withColumn('name_array', (F.split(F.upper(F.col(input_col)), '')))\
-           .withColumn('sorted_name_array', F.array_sort(F.col('name_array')))\
-           .withColumn(output_col, F.concat_ws('', F.col('sorted_name_array')))\
-           .drop('name_array', 'sorted_name_array')
+
+    # input validation
+    if df.schema[input_col].dataType.typeName() != 'string':
+        raise TypeError(f'Column: {input_col} is not of type string')
+
+    # concat removes any null values. conditional replacement only when not null added
+    # to avoid unwanted removal of null
+    df = df.withColumn(output_col,
+                       F.when(F.col(input_col).isNull(),F.col(input_col)).otherwise(
+                           F.concat_ws('',F.array_sort(F.split(F.upper(F.col(input_col)),'')))))
+
     return df
 
+
 ###############################################################################
 
 
 def metaphone(df, input_col, output_col):
     """
     Generates the metaphone phonetic encoding of a string.
 
@@ -153,16 +169,16 @@
     +---+--------+----------------+
 
     """
     df = df.withColumn(output_col, F.soundex(input_col))
     return df
 
 ###############################################################################
-# string comparators
 
+# String Comparators
 
 def std_lev_score(string1, string2):
     """
     Applies the standardised levenshtein string similarity function to two
     strings to return a score between 0 and 1.
 
     This function works at the column level, and so needs to either be applied
@@ -220,16 +236,16 @@
         CEN.Postcode_cen == CCS.Postcode_ccs]
 
     links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS,
                                           id_l = 'Resident_ID_cen', id_r = 'Resident_ID_ccs',
                                           matchkeys = MK, out_dir = '/some_path/links')
     """
 
-    return (1 - ((F.levenshtein(string1, string2)) /
-                 F.greatest(F.length(string1), F.length(string2))))
+    return (1 - ((F.levenshtein(string1, string2))
+                 / F.greatest(F.length(string1), F.length(string2))))
 
 ###############################################################################
 
 
 @F.udf(FloatType())
 def jaro(string1, string2):
     """
@@ -364,17 +380,75 @@
 
     """
 
     return jellyfish.jaro_winkler_similarity(
         string1, string2) if string1 is not None and string2 is not None else None
 
 ###############################################################################
-# linkage methods
 
 
+@F.udf(FloatType())
+def difflib_sequence_matcher(string1, string2):
+    """
+    Applies the difflib.SequenceMatcher ratio() function to get the distance between two
+    strings and calculates a score between 0 and 1 (1.0 if the sequences are identical,
+    0.0 if they do not have anything in common).
+
+    This function works at the column level, and so needs to either be applied to two
+    forename columns in an already-linked dataset, or as a join condition in a matchkey.
+
+    Parameters
+    ----------
+    string1: str
+        string to be compared to string2
+    string2: str
+        string to be compared to string1
+
+    Returns
+    -------
+    float
+        similarity score between 0 and 1
+
+    Example
+    --------
+
+    >df.show()
+    +---+---------+----------+
+    | ID| Forename|Forename_2|
+    +---+---------+----------+
+    |  1|    David|     Emily|
+    |  2|  Idrissa|     Emily|
+    |  3|   Edward|     Emily|
+    |  4|   Gordon|     Emily|
+    |  5|     Emma|     Emily|
+    +---+---------+----------+
+
+    >df = df.withColumn('sequence_matcher', difflib_sequence_matcher(F.col('Forename'),\
+                                                                    F.col('Forename_2')))
+    +---+---------+----------+----------------+
+    | ID| Forename|Forename_2|sequence_matcher|
+    +---+---------+----------+----------------+
+    |  1|    David|     Emily|             0.2|
+    |  2|  Idrissa|     Emily|      0.16666667|
+    |  3|   Edward|     Emily|      0.18181819|
+    |  4|   Gordon|     Emily|             0.0|
+    |  5|     Emma|     Emily|      0.44444445|
+    +---+---------+----------+----------------+
+
+    """
+
+    if string1 is None or string2 is None:
+        return None
+
+    return SequenceMatcher(a=string1, b=string2).ratio()
+
+###############################################################################
+
+# Linkage Methods
+
 def blocking(df1, df2, blocks, id_vars):
     """
     Combines two spark dataframes, based on a set of defined blocking criteria,
     to create a new dataframe of unique record pairs.
 
     Parameters
     ----------
@@ -546,18 +620,18 @@
         df = df.join(cluster, on=id_1, how='left').sort(
             'Cluster_Number').drop('component')
 
         return df
 
     except py4j.protocol.Py4JJavaError:
         print("""WARNING: A graphframes wrapper package installation has not been found!
-        If you have not already done so, you will need to submit graphframes' JAR file 
+        If you have not already done so, you will need to submit graphframes' JAR file
         dependency to your spark context. This can be found here:
         \nhttps://repos.spark-packages.org/graphframes/graphframes/0.6.0-spark2.3-s_2.11/
-        graphframes-0.6.0-spark2.3-s_2.11.jar\nOnce downloaded, 
+        graphframes-0.6.0-spark2.3-s_2.11.jar\nOnce downloaded,
         this can be submitted to your spark context via:
         spark.conf.set('spark.jars', path_to_jar_file) or by starting a sparksession from the
         sessions module of dlh_utils
         """)
 
 ###############################################################################
 
@@ -661,32 +735,32 @@
     '''
     mk_order = pd.DataFrame({
         'mks': mks,
         'supplied_order': [mk_n for mk_n, mk
                            in enumerate(mks)]
     })
 
-    mks = chunk_list(mks, chunk)
+    mks = ut.chunk_list(mks, chunk)
 
     mk_counts = pd.DataFrame(columns=[
         'supplied_order',
         'count'
     ])
 
-    chunk_n = 0-chunk
+    chunk_n = 0 - chunk
 
     for mk_chunk in mks:
 
         chunk_n += chunk
 
         df = da.union_all(*[
             (mk_dropna(df_l, mk).join(mk_dropna(df_r, mk),
                                       on=mk,
                                       how='inner')
-             .withColumn('supplied_order', F.lit(mk_n+chunk_n))
+             .withColumn('supplied_order', F.lit(mk_n + chunk_n))
              .select('supplied_order')
              )
             for mk_n, mk in enumerate(mk_chunk)
         ])
 
         df = (df
               .groupBy('supplied_order')
@@ -768,22 +842,14 @@
     df = da.filter_window(df, id_l, id_r, 'count', 1)
 
     return df
 
 ###############################################################################
 
 
-def chunk_list(_list, _num):
-    '''splits a list into a specified number of chunks'''
-    return [_list[i * _num:(i + 1) * _num]
-            for i in range((len(_list) + _num - 1) // _num)]
-
-###############################################################################
-
-
 def matchkey_dataframe(mks):
     """
     Creates dataframe of matchkeys and descriptions
 
     Takes a list of matchkeys. Assigns numbers to matchkeys based on order in list
     provided. Adds description of each matchkey from string manipulation of join
     condition.
@@ -856,15 +922,15 @@
 def assert_unique(df, column):
     '''
     Asserts whether a dataframe contains only one instance of each
     unique identifier, specified by the col argument.
     '''
 
     if not isinstance(column, list):
-        col = [col]
+        column = [column]
 
     assert df.count() == df.dropDuplicates(subset=column).count()
 
 ###############################################################################
 
 
 def matchkey_counts(linked_df):
@@ -916,27 +982,23 @@
       left dataframe to be joined.
     df_r : dataframe
       right dataframe to be joined.
     id_l : string
       variable name of column containing left unique identifier
     id_r : string
       variable name of column containing right unique identifier
-    suffix_l : string
-      suffix to be applied to left dataframe
-    suffix_r : string
-      suffix to be applied to right dataframe
     n_ids : int, default = 100
       The number of identifier pairs sampled for each matchkey
     Returns
     -------
     dataframe
       Dataframe of deterministic linkage samples by matchkey.
     Raises
     -------
-    None at present. 
+    None at present.
 
     See Also
     --------
     dataframes.union_all()
     """
 
     mks = sorted([x[0] for x in
@@ -963,194 +1025,27 @@
                  .sort('matchkey', id_l)
                  )
 
     lead_columns = ['matchkey', id_l, id_r]
     end_columns = ['description']
 
     review_df = (review_df
-                 .select(lead_columns +
-                         sorted([x for x in review_df.columns
-                                 if x not in
-                                 lead_columns+end_columns])
+                 .select(lead_columns
+                         + sorted([x for x in review_df.columns
+                                   if x not in
+                                   lead_columns + end_columns])
                          + end_columns)
                  )
 
     return review_df
 
-###################################################################
-
-
-def demographics(*args, df, identifier,):
-    """
-    Produces demographics count of dataframe for groups specified.
-
-    Used to get counts of, for example number of persons in age
-    groups, to allow comparison of counts in raw data to counts in
-    linked data. Produces output used in demographics_compare()
-
-    Parameters
-    ----------
-    *args : str or list of str
-      Variable column titles to be included in group counts
-    df : dataframe
-      the dataframe for which demographics are calculated
-      number and description
-    identifier : string
-      Reference to column containing unique identifier
-
-    Returns
-    -------
-    dataframe
-      Dataframe of demograhic metrics.
-
-    Raises
-    -------
-      None at present.
-
-    See Also
-    --------
-    dataframes.union_all()
-    """
-
-    total_count = (df
-                   .select(identifier)
-                   .dropDuplicates()
-                   ).count()
-
-    df = da.union_all(*[
-        (df
-         .select(identifier, col)
-         .dropDuplicates()
-         .groupBy(col)
-         .agg(F.count(F.col(identifier)).alias('count'))
-         .fillna('not_provided')
-         .withColumn('variable', F.lit(col))
-         .withColumnRenamed(col, 'value')
-         )
-        for col in args
-    ])
-
-    df = (df
-          .withColumn('total_count', F.lit(total_count))
-          .select('variable', 'value', 'count', 'total_count')
-          .sort(['variable', 'value'])
-          ).coalesce(1)
-
-    return df
-
-####################################################################
-
-
-def demographics_compare(df_raw, df_linked):
-    """
-    Compares raw and linked outputs produced by demographics() to
-    highlight bias in linked data.
-
-    Determines the expected counts in linked data per demographic
-    group, from match rates and counts in raw data. Produces positive
-    or negative discrepency metric, highlighting under or
-    over-representation of each group in the linked data, versus the
-    raw data.
-
-    Parameters
-    ----------
-    df_raw : dataframe
-      output of demographics() for raw data
-    df_linked : dataframe
-      output of demographics() for linked data
-
-    Returns
-    -------
-    dataframe
-      Dataframe of demographic comparison metrics.
-
-    Raises
-    -------
-      None at present.
-    """
-
-    df_raw = (da.suffix_columns(df_raw,
-                                '_raw',
-                                exclude=['variable',
-                                         'value']))
-
-    df_linked = (da.suffix_columns(df_linked,
-                                   '_linked',
-                                   exclude=['variable',
-                                            'value']))
-
-    df = (df_raw
-          .join(df_linked,
-                on=['variable', 'value'],
-                how='full')
-          )
-
-    df = df.fillna(0, subset=['count_linked', 'count_raw'])
-
-    total_count_linked = int((df
-                             .select('total_count_linked')
-                             .dropna()
-                             .dropDuplicates()
-                             .toPandas()
-                              )['total_count_linked'][0])
-    df = df.withColumn('total_count_linked',
-                       F.lit(total_count_linked))
-
-    total_count_raw = int((df
-                           .select('total_count_raw')
-                           .dropna()
-                           .dropDuplicates()
-                           .toPandas()
-                           )['total_count_raw'][0])
-    df = df.withColumn('total_count_raw',
-                       F.lit(total_count_raw))
-
-    df = (df
-          .withColumn('match_rate',
-                      F.col('total_count_linked')
-                      / F.col('total_count_raw')
-                      )
-          )
-
-    df = (df
-          .withColumn('proportional_count',
-                      (F.col('match_rate')*F.col('count_raw'))
-                      .cast('int')
-                      )
-          )
-
-    df = (df
-          .withColumn('proportional_discrepency',
-                      (F.col('count_linked')-F.col('proportional_count'))
-                      / F.col('proportional_count'))
-          )
-
-    df = (df
-          .sort(['variable', 'value'])
-          ).coalesce(1)
-
-    return df
-
-###############################################################################
-
-
-def matchkeys_drop_duplicates(mks):
-    '''
-    Removes duplicates from generated matchkeys
-    '''
-    out = pd.DataFrame({'mks': mks})
-    out['mks_str'] = [str(x) for x in out['mks']]
-    out = out.drop_duplicates(subset=['mks_str'])
-    out = list(out['mks'])
-
-    return out
-
 ############################################################################
 
 
+'''
 def deduplicate(df, record_id, mks, checkpoint=False):
     """
     Matches a dataframe to itself on a specified set of matchkeys. Returns
     either the unique records in your data, or the identified duplicates.
 
     Parameters
     ----------
@@ -1185,17 +1080,14 @@
 
     > CCS = linkage.deduplicate(df = CCS, record_id = 'Resident_ID', mks = deduplicate_keys)[0]
 
     > CCS.count()
     10487
     """
 
-    # get active spark session
-    spark = SparkSession.builder.getOrCreate()
-
     # check to see if matchkeys are passed as a list of lists
     if any(isinstance(matchkey, list) for matchkey in mks) is False:
         mks = [mks]
 
     df2 = da.suffix_columns(df, suffix='_2')
 
     for count, matchkey in enumerate(mks, 1):
@@ -1230,19 +1122,19 @@
     duplicates = duplicates.selectExpr(f"{record_id}_min AS {record_id}",
                                        f"{record_id}_max AS {record_id}_2",
                                        "matchkey")
 
     duplicates = duplicates.drop_duplicates([f"{record_id}", f"{record_id}_2"])
 
     unique = df.join(duplicates, how="left_anti",
-                     on=(df[f"{record_id}"] == duplicates[f"{record_id}"]) |
-                     (df[f"{record_id}"] == duplicates[f"{record_id}_2"]))
+                     on=(df[f"{record_id}"] == duplicates[f"{record_id}"])
+                     | (df[f"{record_id}"] == duplicates[f"{record_id}_2"]))
 
     return unique, duplicates
-
+'''
 ############################################################################
 
 
 def deterministic_linkage(df_l, df_r, id_l, id_r, matchkeys, out_dir):
     '''
     Performs determistic linkage of two dataframes given a list of matchkeys /
     join conditions. Returns a dataframe of the linked identifers of left and
@@ -1314,16 +1206,18 @@
     |C1075168650487354680|C5417150230708747120|       1|
     |C1111234343783150025|C6146302309226089123|       1|
     |C1338540771296365051|C8521797154702755129|       1|
     |C1604818046072784138|C3975523078369491788|       1|
     +--------------------+--------------------+--------+
     '''
 
+    use_parquet = out_dir is not None
+
     # control for file path format
-    if out_dir[-1] == "/":
+    if use_parquet and out_dir[-1] == "/":
         out_dir = out_dir[:-1]
 
     # count of unique ids in left df
     df_l_count = (df_l
                   .select(id_l)
                   .drop_duplicates()
                   ).count()
@@ -1334,52 +1228,71 @@
                   ).count()
     # initial count of matches
     count = 0
 
     for index, matchkey in enumerate(matchkeys, 1):
 
         if index == 1:
+            match_data = matchkey_join(
+                df_l, df_r, id_l, id_r, matchkey, index
+            )
             # writes first matchkey to parquet
-            ut.write_format(matchkey_join(
-                df_l, df_r, id_l, id_r, matchkey, index),
-                'parquet',
-                f"{out_dir}/linked_identifiers",
-                mode='overwrite')
+            if use_parquet:
+                ut.write_format(
+                    match_data,
+                    'parquet',
+                    f"{out_dir}/linked_identifiers",
+                    mode='overwrite'
+                )
+            else:
+                out_df = match_data
 
         else:
             # reads previous matches
             # used in left anti join to ignore matched records
-            matches = ut.read_format('parquet',
-                                     f"{out_dir}/linked_identifiers")
+            if use_parquet:
+                matches = ut.read_format('parquet',
+                                         f"{out_dir}/linked_identifiers")
+            else:
+                matches = out_df
 
             last_count = count
             count = matches.count()
 
-            print("\nMATCHKEY", index-1)
-            print("matches on matchkey: ", count-last_count)
+            print("\nMATCHKEY", index - 1)
+            print("matches on matchkey: ", count - last_count)
             print("total matches: ", count)
-            print("left residual: ", df_l_count-count)
-            print("right residual: ", df_r_count-count)
+            print("left residual: ", df_l_count - count)
+            print("right residual: ", df_r_count - count)
 
             # appends subsequent matches to initial parquet
-            ut.write_format(matchkey_join(
+            match_data = matchkey_join(
                 df_l.join(matches, id_l, 'left_anti'),
                 df_r.join(matches, id_r, 'left_anti'),
-                id_l, id_r, matchkey, index),
-                'parquet',
-                f"{out_dir}/linked_identifiers",
-                mode='append')
+                id_l, id_r, matchkey, index
+            )
+            if use_parquet:
+                ut.write_format(
+                    match_data,
+                    'parquet',
+                    f"{out_dir}/linked_identifiers",
+                    mode='append'
+                )
+            else:
+                out_df = out_df.union(match_data)
 
     # reads and returns final matches
-    matches = ut.read_format('parquet',
-                             f"{out_dir}/linked_identifiers")
+    if use_parquet:
+        matches = ut.read_format('parquet', f"{out_dir}/linked_identifiers")
+    else:
+        matches = out_df
 
     last_count = count
     count = matches.count()
 
     print("\nMATCHKEY", index)
-    print("matches on matchkey: ", count-last_count)
+    print("matches on matchkey: ", count - last_count)
     print("total matches: ", count)
-    print("left residual: ", df_l_count-count)
-    print("right residual: ", df_r_count-count)
+    print("left residual: ", df_l_count - count)
+    print("right residual: ", df_r_count - count)
 
     return matches
```

### Comparing `dlh_utils-0.3.1/dlh_utils/profiling.py` & `dlh_utils-0.4.1/dlh_utils/profiling.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
 
 def df_describe(df, output_mode='pandas', approx_distinct=False, rsd=0.05):
     '''
     Produces a dataframe containing descriptive metrics on each variable within a
     specified dataframe, including:
     * the variable type
-    * the maximum value length
-    * the minimum value length
+    * the maximum and minimum value length
     * the maximum and minimum lengths before/after decimal places for float variables
     * the number and percentage of distinct values
     * the number and percentage of null and non-null values
 
     Parameters
     ----------
     df: dataframe
@@ -227,31 +226,31 @@
         max_l_bp_df,
         min_l_bp_df,
         max_l_ap_df,
         min_l_ap_df,
     ).toPandas()
 
     describe_df = describe_df.transpose().reset_index()
-    describe_df.columns = ['variable']+list(describe_df[describe_df['index'] == 'summary']
-                                            .reset_index(drop=True).transpose()[0])[1:]
+    describe_df.columns = ['variable'] + list(describe_df[describe_df['index'] == 'summary']
+                                              .reset_index(drop=True).transpose()[0])[1:]
     describe_df = describe_df[describe_df['variable'] != 'summary']
 
     describe_df = describe_df.rename(columns={'count': 'not_null'})
 
     describe_df['row_count'] = count
     describe_df['null'] = describe_df['row_count'] - \
         describe_df['not_null'].astype(int)
     for variable in [
         'distinct',
         'null',
         'not_null',
         'empty',
     ]:
-        describe_df['percent_'+variable] = (
-            describe_df[variable].astype(int)/describe_df['row_count'])*100
+        describe_df['percent_' + variable] = (
+            describe_df[variable].astype(int) / describe_df['row_count']) * 100
     describe_df['type'] = [types[x] for x in describe_df['variable']]
 
     describe_df = describe_df.reset_index(drop=True)
     describe_df['min'] = [y if describe_df['type'][x] != 'string' else None
                           for x, y in enumerate(describe_df['min'])]
 
     describe_df = describe_df.reset_index(drop=True)
@@ -341,22 +340,22 @@
                    .withColumn("count",
                                F.count(col)
                                .over(Window.partitionBy(col)))).dropDuplicates().persist()
 
         high = (grouped
                 .sort('count', ascending=False)
                 .limit(limit)
-                .withColumnRenamed('count', col+'_count')
+                .withColumnRenamed('count', col + '_count')
                 .toPandas()
                 )
 
         low = (grouped
                .sort('count', ascending=True)
                .limit(limit)
-               .withColumnRenamed('count', col+'_count')
+               .withColumnRenamed('count', col + '_count')
                .toPandas()
                )
 
         grouped.unpersist()
 
         return (high, low)
 
@@ -366,19 +365,19 @@
 
     def make_limit(df, limit):
 
         count = df.shape[0]
 
         if count < limit:
 
-            dif = limit-count
+            dif = limit - count
 
             dif_df = pd.DataFrame({
-                0: ['']*dif,
-                1: [0]*dif
+                0: [''] * dif,
+                1: [0] * dif
             })[[0, 1]]
 
             dif_df.columns = list(df)
 
             df = (df
                   .append(dif_df)
                   .reset_index(drop=True)
```

### Comparing `dlh_utils-0.3.1/dlh_utils/sessions.py` & `dlh_utils-0.4.1/dlh_utils/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 generating a Spark UI link to monitor session progress.
 '''
 import os
 from IPython.core.display import display, HTML
 from pyspark.sql import SparkSession
 import graphframes_jars as graphframes
 
+##################################################################################
+
 
 def getOrCreateSparkSession(appName='DE_DL',
                             size='large',
                             showConsoleProgress='false',
                             shufflePartitions=200,
                             defaultParallelism=200,
                             memory='10g',
@@ -51,20 +53,20 @@
 
     Raises
     -------
       None at present.
     """
     # obtain spark UI url parameters
     url = 'spark-' + str(os.environ['CDSW_ENGINE_ID']) + \
-        '.'+str(os.environ['CDSW_DOMAIN'])
+        '.' + str(os.environ['CDSW_DOMAIN'])
     spark_ui = display(HTML(f'<a href=http://{url}s>Spark UI</a>'))
 
     try:
 
-      # get graphframes jar path to configure session with
+        # get graphframes jar path to configure session with
         graphframes_path = graphframes.__file__
         graphframes_path = graphframes_path.rsplit('/', 1)[0]
 
         for file in os.listdir(graphframes_path):
             if file.endswith(".jar"):
                 # Get the latest jar file
                 jar_path = os.path.join(graphframes_path, file)
```

### Comparing `dlh_utils-0.3.1/dlh_utils/standardisation.py` & `dlh_utils-0.4.1/dlh_utils/standardisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 '''
 Functions used to standardise and clean data prior to linkage.
 '''
 import pyspark.sql.functions as F
-from pyspark.sql.types import IntegerType
+from pyspark.sql.types import IntegerType, StringType, StructType, StructField
+from pyspark.sql import SparkSession
 from dlh_utils import dataframes as da
 
 ###############################################################################
 
+
 def cast_type(df, subset=None, types='string'):
     """
     Casts specific dataframe columns to a specified type.
 
     The function can either take a subset of columns or if no subset is defined
     it takes all the columns and converts their datatypes into the datatype
     specified by the user.
@@ -189,16 +191,15 @@
     None at present.
 
     See Also
     --------
     dataframes.concat()
     """
 
-    out = df.where((F.col(first_name).contains(sep) == False)
-                   | (F.col(first_name).isNull()))
+    out = df.where(~(F.col(first_name).contains(sep)) | (F.col(first_name).isNull()))
     df = df.where(F.col(first_name).contains(sep))
 
     df = da.concat(df, 'align_forenames', sep, [
         first_name,
         middle_name
     ])
 
@@ -318,15 +319,15 @@
         'SAN',
         'BA'
     ]
 
     surname_prefix_regex = "|".join([f"(?<=\\b{prefix})[ -]"
                                      for prefix in prefixes])
 
-    surname_regex = surname_regex+"|"+surname_prefix_regex
+    surname_regex = surname_regex + "|" + surname_prefix_regex
 
     if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         df = df.withColumn(col, F.regexp_replace(F.col(col),
@@ -609,14 +610,15 @@
                   )
 
     return df
 
 
 #################################################################
 
+
 def max_white_space(df, limit, subset=None):
     """
     Sets maximum number of whitespaces in a row.
 
     Any whitespace above the limit e.g. 3 subsequent whitespaces
     when the limit is 2 will be changed to the limit value within
     the string.
@@ -756,15 +758,15 @@
 
     if subset is None:
         subset = df.columns
 
     if not isinstance(subset, list):
         subset = [subset]
 
-    number_hyphens = "-"*limit
+    number_hyphens = "-" * limit
 
     for col in subset:
 
         df = (df
               .withColumn('space_count',
                           F.length(
                               F.regexp_replace(F.col(col), "[^-]",
@@ -1077,37 +1079,47 @@
               )
 
     return df
 
 ##############################################################################
 
 
-def replace(df, subset, replace_dict):
+def replace(df, subset, replace_dict, use_join=False, use_regex=False):
     """
     Replaces specific string values in given column(s) with specified values.
 
     Parameters
     ----------
     df : dataframe
       Dataframe to which the function is applied.
     subset : string or list of strings
       The subset is the column(s) on which the function is applied.
       If None the function applies to the whole dataframe.
     replace_dict: dictionary
       Dictionary given needs to be in the format of
       value_to_be_replaced:value_to_replace_with.
+    use_join : Boolean, default = False
+      Set this to True for higher performance if you have a large
+      number of key-value pairs (e.g. industrial classifications).
+      NOTE: You cannot use this mode to replace None values.
+      Call replace() separately with use_join=False if you need to
+      replace the None values.
+    use_regex : Boolean, default = False
+      Use regular expression matching. By default replacements are
+      only done if the whole value matches the dictionary key exactly.
+      If use_regex is True, use_join must be set to False.
 
     Returns
     -------
     dataframe
       Dataframe with replaced values as specified.
 
     Raises
     -------
-    None at present.
+    ValueError if use_join and use_regex are both passed in as True.
 
     Example
     -------
     > df.show()
 
     +---+--------+----------+-------+----------+---+--------+
     | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|
@@ -1130,67 +1142,98 @@
     |  3|Turbo man|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  3|Turbo man|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  4|     Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|
     |  5|   Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|
     +---+---------+----------+-------+----------+---+--------+
     """
 
+    if use_join and use_regex:
+        raise ValueError("Can't call replace() with True values for both use_join and use_regex.")
+    if use_join:
+        for k, i in replace_dict.items():
+            if k is None or i is None:
+                raise ValueError("Join mode (use_join=True) is not compatible with the use of None\
+                                 in the replace dictionary. Set use_join=True to use None values.")
+
     if not isinstance(subset, list):
         subset = [subset]
 
-    for col in subset:
-
-        for before, after in replace_dict.items():
-            df = (df
-                  .withColumn(col, F.when(F.col(col).like(before), after)
-                              .otherwise(F.col(col)))
-                  )
+    if use_join:
+        spark = SparkSession.builder.getOrCreate()
+        schema = StructType([
+            StructField("_replace_dict_element_before", StringType(), True),
+            StructField("_replace_dict_element_after", StringType(), True)])
+        replace_df = spark.createDataFrame(replace_dict.items(), schema)
+        for col in subset:
+            df = df.join(
+                replace_df,
+                df[col] == replace_df["_replace_dict_element_before"],
+                how="left"
+            )
+            df = df.withColumn(
+                col,
+                F.coalesce(df["_replace_dict_element_after"], df[col])
+            )
+            df = df.drop("_replace_dict_element_before", "_replace_dict_element_after")
+    else:
+        for col in subset:
+            for before, after in replace_dict.items():
+                if use_regex:
+                    df = (df
+                          .withColumn(col, F.when(F.col(col).rlike(before), after)
+                                      .otherwise(F.col(col)))
+                          )
+                else:
+                    df = (df
+                          .withColumn(col, F.when(F.col(col).like(before), after)
+                                      .otherwise(F.col(col)))
+                          )
 
     return df
 
 ##############################################################################
 
 
 def standardise_date(df, col_name, in_date_format='dd-MM-yyyy',
                      out_date_format='yyyy-MM-dd',null_counts=False):
     """
     Changes the date format of a specified date column.
-    
+
     Also has an optional argument null_counts. If set to False, the function
-    only returns the dataframe with specified date values altered. 
-    However, if set to True, will also return a tuple, displaying a count of 
-    nulls in the dataframe before and after the function has been applied.  
+    only returns the dataframe with specified date values altered.
+    However, if set to True, will also return a tuple, displaying a count of
+    nulls in the dataframe before and after the function has been applied.
     This is because the standardise_date function will make a date
-    value null if its format differs from the in_date_format. 
+    value null if its format differs from the in_date_format.
 
     Parameters
     ----------
     df : dataframe
       Dataframe to which the function is applied.
     col_name: string
       The column in the dataframe to which the function is being
       applied.
-    in_date_format: default = 'dd-mm-yyyy', string
+    in_date_format: default = 'dd-MM-yyyy', string
       This is the current date format of the the column.
-    out_date_format: default = 'yyyy-mm-dd', string
+    out_date_format: default = 'yyyy-MM-dd', string
       This is the date format to which the column values will be
       changed.
     null_counts: default = False, bool
       If set to True provides a tuple, where the first part displays
-      the df null count before the function has been applied, and the 
-      second part is the df null count after the function has been 
-      applied. 
+      the df null count before the function has been applied, and the
+      second part is the df null count after the function has been
+      applied.
 
     Returns
     -------
     If null_counts = False:
     dataframe
       Dataframe with specified date column values altered
       to new specified format.
-    
+
     If null_counts = True:
     dataframe as described above,
     Tuple
       showing null counts before and after standardise_date
       has been applied to df
 
     Raises
@@ -1221,58 +1264,58 @@
     |  1|   Homer|       Jay|Simpson|12/05/1983|  M|ET74 2SP|
     |  2|   Marge|    Juliet|Simpson|19/03/1983|  F|ET74 2SP|
     |  3|    Bart|     Jo-Jo|Simpson|01/04/2012|  M|ET74 2SP|
     |  3|    Bart|     Jo-Jo|Simpson|01/04/2012|  M|ET74 2SP|
     |  4|    Lisa|     Marie|Simpson|09/05/2014|  F|ET74 2SP|
     |  5|  Maggie|      null|Simpson|12/01/2021|  F|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
-    
+
     Example using null_counts:
     > df.show()
-    
+
     +----------+
     |      date|
     +----------+
     |1990/07/19|
     |2020/09/01|
     |1998/03/21|
     |1999/11/02|
     |2005-12-24|
     +----------+
-    
+
     >df,nulls = standardise_date(df,'date','yyyy/MM/dd','yyyy.MM.dd',True)
-    
+
     >df.show()
     +----------+
     |      date|
     +----------+
     |1990.07.19|
     |2020.09.01|
     |1998.03.21|
     |1999.11.02|
     |      null|
     +----------+
-    
+
     >nulls
     (0, 1)
-     
+
     """
     if null_counts:
         null_before = df.where(F.col(col_name).isNull()).count()
 
     df = df.withColumn(col_name, F.unix_timestamp(F.col(col_name), in_date_format))
     df = df.withColumn(col_name, F.from_unixtime(F.col(col_name), out_date_format))
 
     if null_counts:
         null_after = df.where(F.col(col_name).isNull()).count()
 
         return df,(null_before,null_after)
 
     else:
-      return df
+        return df
 
 ##############################################################################
 
 
 def fill_nulls(df, fill, subset=None):
     """
     Fills null and NaN with specified value
@@ -1334,16 +1377,15 @@
 
     if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
         df = (df
               .withColumn(col, F.when(
-                  (F.col(col).isNull())
-                  | (F.isnan(F.col(col))), fill)
+                  (F.col(col).isNull()) | (F.isnan(F.col(col))), fill)
                   .otherwise(F.col(col)))
               )
 
     return df
 
 ################################################################################
 
@@ -1380,37 +1422,37 @@
     Raises
     -------
     None at present.
 
     Example
     -------
     > df.show()
-    +---+--------+----------+-------+----------+---+--------+
-    | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|
-    +---+--------+----------+-------+----------+---+--------+
-    |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|
-    |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
-    |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|
-    |  5|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|
-    +---+--------+----------+-------+----------+---+--------+
+    +---+--------+-------+----------+---+
+    | ID|Forename|Surname|       DoB|Sex|
+    +---+--------+-------+----------+---+
+    |  1|   Homer|Simpson|1983-05-12|  M|
+    |  2|   Marge|Simpson|1983-03-19|  F|
+    |  3|    Bart|Simpson|2012-04-01|  M|
+    |  3|    Bart|Simpson|2012-04-01|  M|
+    |  4|    Lisa|Simpson|2014-05-09|  F|
+    |  5|  Maggie|Simpson|2021-01-12|  F|
+    +---+--------+-------+----------+---+
 
     > dates = ['2022-11-03','2020-12-25']
     > age_at(df,'DoB','yyyy-MM-dd',*dates).show()
-    +---+--------+----------+-------+----------+---+--------+---------------------+---------------------+
-    | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|DoB_age_at_2022-11-03|DoB_age_at_2020-12-25|
-    +---+--------+----------+-------+----------+---+--------+---------------------+---------------------+
-    |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|                   39|                   37|
-    |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|                   39|                   37|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|                   10|                    8|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|                   10|                    8|
-    |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|                    8|                    6|
-    |  5|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|                    1|                    0|
-    +---+--------+----------+-------+----------+---+--------+---------------------+---------------------+
+    +---+--------+-------+----------+---+---------------------+---------------------+
+    | ID|Forename|Surname|       DoB|Sex|DoB_age_at_2022-11-03|DoB_age_at_2020-12-25|
+    +---+--------+-------+----------+---+---------------------+---------------------+
+    |  1|   Homer|Simpson|1983-05-12|  M|                   39|                   37|
+    |  2|   Marge|Simpson|1983-03-19|  F|                   39|                   37|
+    |  3|    Bart|Simpson|2012-04-01|  M|                   10|                    8|
+    |  3|    Bart|Simpson|2012-04-01|  M|                   10|                    8|
+    |  4|    Lisa|Simpson|2014-05-09|  F|                    8|                    6|
+    |  5|  Maggie|Simpson|2021-01-12|  F|                    1|                    0|
+    +---+--------+-------+----------+---+---------------------+---------------------+
 
     """
 
     df = df.withColumn(
         f"{reference_col}_fmt", F.unix_timestamp(F.col(reference_col), in_date_format)
     ).withColumn(
         f"{reference_col}_fmt",
@@ -1421,15 +1463,14 @@
 
         df = df.withColumn(
             f"{reference_col}_age_at_{age_at_date}",
             (
                 F.months_between(
                     F.lit(age_at_date),
                     F.col(f"{reference_col}_fmt"),
-                )
-                / F.lit(12)
+                ) / F.lit(12)
             ).cast(IntegerType()),
         )
-        
+
     df = df.drop(f"{reference_col}_fmt")
-        
+
     return df
```

### Comparing `dlh_utils-0.3.1/dlh_utils/tests/test_dataframes.py` & `dlh_utils-0.4.1/dlh_utils/tests/test_dataframes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,29 @@
 '''
-Pytesting on Dataframes functions
+Pytesting on Dataframes functions.
 '''
 
-import pyspark
 from pyspark.sql import SparkSession
 import pyspark.sql.functions as F
-from pyspark.sql.types import StructType,StructField,StringType,IntegerType,LongType
+from pyspark.sql.types import StructType,StructField,StringType,LongType,DoubleType
 import pandas as pd
-import chispa
 from chispa import assert_df_equality
 import pytest
 from dlh_utils.dataframes import explode,drop_columns,select,cut_off,\
-drop_nulls,union_all,rename_columns,prefix_columns,suffix_columns,split,\
-clone_column,substring,filter_window,concat,coalesced,window,literal_column
+    drop_nulls,union_all,rename_columns,prefix_columns,suffix_columns,split,\
+    clone_column,substring,filter_window,concat,coalesced,window,literal_column,\
+    date_diff,index_select
 
 pytestmark = pytest.mark.usefixtures("spark")
 
-
-@pytest.fixture(scope="session")
-def spark(request):
-    """fixture for creating a spark context
-    Args:
-        request: pytest.FixtureRequest object
-    """
-    spark = (
-        SparkSession.builder.appName("dataframe_testing")
-        .config("spark.executor.memory", "5g")
-        .config("spark.yarn.excecutor.memoryOverhead", "2g")
-        .getOrCreate()
-    )
-    request.addfinalizer(lambda: spark.stop())
-    return spark
-
 #############################################################################
 
 
 class TestExplode(object):
+    """Test of explode function."""
     def test_expected(self, spark):
 
         test_df = spark.createDataFrame(
             (pd.DataFrame({"check": ["iagsigajs"], "before1": ["a_b_c"]}))
         ).select("check", "before1")
 
         intended_df = spark.createDataFrame(
@@ -50,21 +34,22 @@
                         "before1": ["b", "c", "a"],
                     }
                 )
             )
         ).select("check", "before1")
 
         result_df = explode(test_df, "before1", "_")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,ignore_row_order=True)
 
 
 #############################################################################
 
 
 class TestConcat(object):
+    """Test of concat function"""
     def test_expected(self, spark):
 
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "firstname": [None, "Claire", "Josh", "Bob"],
@@ -77,45 +62,51 @@
                             "Josh_Smith",
                             "Bob_Greg_Evans",
                         ],
                     }
                 )
             )
         )
+
+        # Pandas replaces None with NaN in a numeric column. Convert back to Null:
+        test_df = test_df.replace(float('nan'), None)
+
         intended_schema = StructType(
             [
                 StructField("firstname", StringType(), True),
                 StructField("middlename", StringType(), True),
                 StructField("lastname", StringType(), True),
-                StructField("numeric", IntegerType(), True),
+                StructField("numeric", DoubleType(), True),
                 StructField("after", StringType(), True),
                 StructField("fullname", StringType(), True),
             ]
         )
         intended_data = [
-            [None, "Maria", "Jones", 1, "Maria_Jones", "Maria_Jones"],
-            ["Claire", None, None, None, "Claire", "Claire"],
+            [None, "Maria", "Jones", 1.0, "Maria_Jones", "Maria_Jones"],
+            ["Claire", None, None, 2.0, "Claire", "Claire"],
             ["Josh", "", "Smith", None, "Josh_Smith", "Josh_Smith"],
-            ["Bob", "Greg", "Evans", 4, "Bob_Greg_Evans", "Bob_Greg_Evans"],
+            ["Bob", "Greg", "Evans", 4.0, "Bob_Greg_Evans", "Bob_Greg_Evans"],
         ]
 
         intended_df = spark.createDataFrame(intended_data, intended_schema)
 
         result_df = concat(
             test_df,
             "fullname",
             sep="_",
             columns=["firstname", "middlename", "lastname"],
         )
 
+        assert_df_equality(intended_df, result_df, ignore_row_order=True, ignore_column_order=True)
 
 ##############################################################################
 
 
 class TestDropColumns(object):
+    """Test of drop_columns function"""
     def test_expected(self, spark):
 
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "col1": ["ONE", "TWO", "THREE"],
@@ -130,15 +121,15 @@
             (
                 pd.DataFrame(
                     {"col2": ["one", "three", "two"], "extra": ["One", "Three", "Two"]}
                 )
             )
         )
         result_df = drop_columns(test_df, subset="col1")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 ##############################################################################
 
 
 class TestSelect(object):
     def test_expected(self, spark):
@@ -165,35 +156,34 @@
                         "firstLetter": ["r", "a", "j", "c"],
                         "first": ["x", "2", "4", "3"],
                     }
                 )
             )
         )
         result_df = select(test_df, startswith="first")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 ##########################################################################
 class TestCoalesced(object):
     def test_expected(self, spark):
 
-        test_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
-                    {
-                        "extra": [None, None, None, "FO+ UR", None],
-                        "lower": ["one", None, "one", "four", None],
-                        "lowerNulls": ["one", "two", None, "four", None],
-                        "upperNulls": ["ONE", "TWO", None, "FOU  R", None],
-                        "value": [1, 2, 3, 4, 5],
-                    }
-                )
-            )
+        pdf = pd.DataFrame(
+            {
+                "extra": [None, None, None, "FO+ UR", None],
+                "lower": ["one", None, "one", "four", None],
+                "lowerNulls": ["one", "two", None, "four", None],
+                "upperNulls": ["ONE", "TWO", None, "FOU  R", None],
+                "value": [1, 2, 3, 4, 5],
+            }
         )
 
+        pdf = pdf[["extra", "lower", "lowerNulls", "upperNulls", "value"]]
+        test_df = spark.createDataFrame((pdf))
+
         intended_schema = StructType(
             [
                 StructField("extra", StringType(), True),
                 StructField("lower", StringType(), True),
                 StructField("lowerNulls", StringType(), True),
                 StructField("upperNulls", StringType(), True),
                 StructField("value", LongType(), True),
@@ -206,54 +196,51 @@
             [None, "one", None, None, 3, "one"],
             ["FO+ UR", "four", "four", "FOU  R", 4, "FO+ UR"],
             [None, None, None, None, 5, "5"],
         ]
         intended_df = spark.createDataFrame(intended_data, intended_schema)
 
         result_df = coalesced(test_df)
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True, ignore_column_order=True)
 
     def test_expected_with_drop(self, spark):
-
-        test_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
-                    {
-                        "lower": ["one", None, "one", "four", None],
-                        "value": [1, 2, 3, 4, 5],
-                        "extra": [None, None, None, "FO+ UR", None],
-                        "lowerNulls": ["one", "two", None, "four", None],
-                        "upperNulls": ["ONE", "TWO", None, "FOU  R", None],
-                    }
-                )
-            )
+        pdf = pd.DataFrame(
+            {
+                "lower": ["one", None, "one", "four", None],
+                "value": [1, 2, 3, 4, 5],
+                "extra": [None, None, None, "FO+ UR", None],
+                "lowerNulls": ["one", "two", None, "four", None],
+                "upperNulls": ["ONE", "TWO", None, "FOU  R", None],
+            }
         )
+        pdf = pdf[["lower", "value", "extra", "lowerNulls", "upperNulls"]]
 
-        intended_schema = StructType(
+        test_df2 = spark.createDataFrame((pdf))
+
+        intended_schema2 = StructType(
             [
                 StructField("coalesced_col", StringType(), True),
             ]
         )
-        intended_data = [
+        intended_data2 = [
             ["one"],
-            ["two"],
+            ["2"],
             ["one"],
-            ["FO+ UR"],
+            ["four"],
             ["5"]
         ]
-        intended_df = spark.createDataFrame(intended_data, intended_schema)
-
-        result_df = coalesced(test_df, drop=True)
-        assert_df_equality(intended_df, result_df)
+        intended_df2 = spark.createDataFrame(intended_data2, intended_schema2)
 
+        result_df2 = coalesced(test_df2, drop=True)
+        assert_df_equality(intended_df2, result_df2, ignore_row_order=True,
+                           ignore_column_order=True)
 
 
 #################################################################
 
-
 class TestCutOff(object):
     def test_expected(self, spark):
 
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {"strings": ["1", "2", "3", "4", "5"], "ints": [1, 2, 3, 4, 5]}
@@ -263,15 +250,15 @@
 
         intended_df = spark.createDataFrame(
             (pd.DataFrame({"strings": ["3", "4", "5"], "ints": [3, 4, 5]}))
         )
 
         # cutOff does not remove null values when the val is an Int type
         result_df = cut_off(test_df, threshold_column="ints", val=3, mode=">=")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
         test_df_2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "col1": [
                             None,
@@ -286,15 +273,36 @@
         ).withColumn("col1", F.to_date("col1", "dd-MM-yyyy"))
 
         intended_df_2 = spark.createDataFrame(
             (pd.DataFrame({"col1": ["18-05-1997"]}))
         ).withColumn("col1", F.to_date("col1", "dd-MM-yyyy"))
 
         result_df_2 = cut_off(test_df_2, "col1", "1997-01-15", ">=")
-        assert_df_equality(intended_df_2, result_df_2)
+        assert_df_equality(intended_df_2, result_df_2, ignore_row_order=True)
+
+        intended_df_3 = spark.createDataFrame(
+            (pd.DataFrame({"strings": ["4", "5"], "ints": [4, 5]}))
+        )
+
+        result_df3 = cut_off(test_df, threshold_column="ints", val=3, mode=">")
+        assert_df_equality(intended_df_3, result_df3, ignore_row_order=True) 
+
+        intended_df_4 = spark.createDataFrame(
+            (pd.DataFrame({"strings": ["1", "2", "3"], "ints": [1, 2, 3]}))
+        )
+
+        result_df4 = cut_off(test_df, threshold_column="ints", val=4, mode="<")
+        assert_df_equality(intended_df_4, result_df4, ignore_row_order=True)
+
+        intended_df_5 = spark.createDataFrame(
+            (pd.DataFrame({"strings": ["1", "2", "3"], "ints": [1, 2, 3]}))
+        )
+
+        result_df5 = cut_off(test_df, threshold_column="ints", val=3, mode="<=")
+        assert_df_equality(intended_df_5, result_df5, ignore_row_order=True)
 
 
 ####################################################################
 
 
 class TestLiteralColumn(object):
     def test_expected(self, spark):
@@ -324,15 +332,15 @@
             ["one", 3, "yes"],
             ["four", 4, "yes"],
             [None, 5, "yes"],
         ]
         intended_df = spark.createDataFrame(intended_data, intended_schema)
 
         result_df = literal_column(test_df, "newStr", "yes")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 ####################################################################
 
 
 class TestDropNulls(object):
     def test_expected(self, spark):
@@ -349,15 +357,15 @@
         )
 
         intended_df = spark.createDataFrame(
             (pd.DataFrame({"lower": ["one", "four"], "after": ["one", "four"]}))
         )
 
         result_df = drop_nulls(test_df, subset="lower", val="five")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 #####################################################################
 
 
 class TestUnionAll(object):
     def test_expected(self, spark):
@@ -444,15 +452,15 @@
                         ],
                     }
                 )
             )
         )
 
         result_df = union_all(test_df1, test_df2, test_df3, fill="xd")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 #########################################################################
 
 
 class TestRenameColumns(object):
     def test_expected(self, spark):
@@ -477,15 +485,15 @@
                 )
             )
         )
 
         result_df = rename_columns(
             test_df, rename_dict={"col1": "first", "col2": "second"}
         )
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 #########################################################################
 
 
 class TestRenameColumns2(object):
     def test_expected(self, spark):
@@ -513,15 +521,15 @@
             )
         )
         result_df = rename_columns(
             test_df,
             rename_dict={"abefore": "aafter", "bbefore": "bafter", "cbefore": "cafter"},
         )
 
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 #########################################################################
 
 
 class TestPrefixColumns(object):
     def test_expected(self, spark):
@@ -545,15 +553,15 @@
                         "mrcol2": [None, None, "one", "four", "five"],
                     }
                 )
             )
         )
 
         result_df = prefix_columns(test_df, prefix="mr", exclude="col1")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 ###########################################################################
 
 
 class TestSuffixColumns(object):
     def test_expected(self, spark):
@@ -576,15 +584,15 @@
                         "col1": [None, None, "one", "four", "five"],
                         "col2mr": [None, None, "one", "four", "five"],
                     }
                 )
             )
         )
         result_df = suffix_columns(test_df, suffix="mr", exclude="col1")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 #######################################################################
 
 
 class TestWindow(object):
     def test_expected(self, spark):
@@ -617,15 +625,15 @@
             ["d", 1, 2],
         ]
         intended_df = spark.createDataFrame(intended_data, intended_schema)
 
         result_df = window(
             test_df, window=["col1", "col2"], target="col2", mode="count", alias="new"
         )
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
         test_df2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "col1": ["a", "b", "c", "c", "d", "e", "d"],
                         "col2": [1, 1, 1, 2, 1, 1, 2],
@@ -651,15 +659,15 @@
             ["e", 1, 1],
         ]
 
         intended_df2 = spark.createDataFrame(intended_data2, intended_schema2)
         result_df2 = window(
             test_df2, window=["col1"], target="col2", mode="min", alias="new"
         ).orderBy("col1", "col2")
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2, ignore_row_order=True)
 
         intended_schema3 = StructType(
             [
                 StructField("col1", StringType(), True),
                 StructField("new", LongType(), True),
                 StructField("col2", LongType(), True),
             ]
@@ -673,15 +681,15 @@
             ["d", 2, 2],
             ["e", 1, 1],
         ]
         intended_df3 = spark.createDataFrame(intended_data3, intended_schema3)
         result_df3 = window(
             test_df2, window=["col1"], target="col2", mode="max", alias="new"
         ).orderBy("col1", "col2")
-        assert_df_equality(intended_df3, result_df3)
+        assert_df_equality(intended_df3, result_df3, ignore_row_order=True)
 
         test_df4 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "col1": [
                             "a",
@@ -726,15 +734,15 @@
             ["e", 1, 1],
         ]
 
         intended_df4 = spark.createDataFrame(intended_data4, intended_schema4)
         result_df4 = window(
             test_df4, window=["col1"], target="col2", mode="max", alias="new"
         ).orderBy("col1", "col2")
-        assert_df_equality(intended_df4, result_df4)
+        assert_df_equality(intended_df4, result_df4, ignore_row_order=True)
 
 
 ###############################################################################
 
 
 class TestSplit(object):
     def test_expected(self, spark):
@@ -754,15 +762,15 @@
                         "after": [["a", "b", "c", "d"], None],
                         "new": [["a", "b", "c", "d"], None],
                     }
                 )
             )
         )
         result_df = split(test_df, "before", col_out="new", split_on="_")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 ###############################################################################
 
 
 class IndexSelectTesting(object):
     def test_expected(self, spark):
@@ -787,15 +795,15 @@
                         "afterneg": ["c", None, "d"],
                         "test": ["a", None, "b"],
                     }
                 )
             )
         )
         result_df = index_select(test_df, "before", "test", 0)
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
 
 ###############################################################################
 
 
 class TestCloneColumn(object):
     def test_expected(self, spark):
@@ -812,15 +820,15 @@
                         "NEW": ["ONE£", 'TW""O', "T^^HREE", "FO+UR", "FI@VE"],
                     }
                 )
             )
         ).select("UPPER", "NEW")
 
         result_df = clone_column(test_df, "UPPER", "NEW")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True)
 
     #######################################################################
 
 
 class TestSubstring(object):
     def test_expected(self, spark):
 
@@ -844,15 +852,15 @@
                         "end": ["ENO", "OWT", "EER", "RUO"],
                         "final": ["ONE", "TWO", "THR", "FOU"],
                     }
                 )
             )
         ).select("NEW", "end", "start", "final")
         result_df = substring(test_df, "final", "NEW", 1, 3)
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df, ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################
 
 
 class TestFilterWindow(object):
     def test_expected(self, spark):
@@ -871,26 +879,102 @@
         intended_df1 = spark.createDataFrame(
             (pd.DataFrame({"col1": ["e", "b", "a"], "col2": [1, 1, 1]}))
         )
 
         result_df1 = filter_window(
             test_df1, "col1", "col2", "count", value=1, condition=True
         )
-        assert_df_equality(intended_df1, result_df1)
+        assert_df_equality(intended_df1, result_df1, ignore_row_order=True)
 
         test_df2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "col1": ["a", "b", "c", "c", "d", "e", "d"],
                         "col2": [1, 1, 2, 3, 1, 1, 2],
                     }
                 )
             )
         )
 
         intended_df2 = spark.createDataFrame(
-            (pd.DataFrame({"col1": ["d", "c"], "col2": ["1", "2"]}))
+            (pd.DataFrame({"col1": ["d", "c"], "col2": [1, 2]}))
         )
         result_df2 = filter_window(test_df2, "col1", "col2", "max", condition=False)
 
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2, ignore_row_order=True)
+
+##############################################################
+
+
+class TestDateDiff(object):
+    def test_expected(self, spark):
+
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "dob": ['1983-05-12', '1983-03-19', '2012-04-01',
+                                '2012-04-01', '2014-05-09','2021-01-12'],
+                        "today": ['2023-05-02','2023-05-02','2023-05-02',
+                                  '2023-05-02','2023-05-02','2023-05-02'],
+                    }
+                )
+            )
+        )
+
+        intended_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "dob": ['1983-05-12', '1983-03-19', '2012-04-01',
+                                '2012-04-01', '2014-05-09','2021-01-12'],
+                        "today": ['2023-05-02','2023-05-02','2023-05-02',
+                                  '2023-05-02','2023-05-02','2023-05-02'],
+                        "Difference": [14600.0, 14653.96, 4048.0, 4048.0, 3280.0, 839.96],
+                    }
+                )
+            )
+        )
+
+        result_df = date_diff(test_df, 'dob','today',in_date_format='yyyy-MM-dd',units='days')
+
+        assert_df_equality(intended_df, result_df, ignore_row_order=True,
+                           ignore_column_order=True)
+
+        intended_df_2 = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "dob": ['1983-05-12', '1983-03-19', '2012-04-01',
+                                '2012-04-01', '2014-05-09','2021-01-12'],
+                        "today": ['2023-05-02','2023-05-02','2023-05-02',
+                                  '2023-05-02','2023-05-02','2023-05-02'],
+                        "Difference": [470.97, 472.71, 130.58, 130.58, 105.81, 27.1],
+                    }
+                )
+            )
+        )
+
+        result_df2 = date_diff(test_df, 'dob','today',in_date_format='yyyy-MM-dd',units='months')
+
+        assert_df_equality(intended_df_2, result_df2, ignore_row_order=True,
+                           ignore_column_order=True)
+
+        intended_df_3 = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "dob": ['1983-05-12', '1983-03-19', '2012-04-01',
+                                '2012-04-01', '2014-05-09','2021-01-12'],
+                        "today": ['2023-05-02','2023-05-02','2023-05-02',
+                                  '2023-05-02','2023-05-02','2023-05-02'],
+                        "Difference": [40.0, 40.15, 11.09, 11.09, 8.99, 2.3],
+                    }
+                )
+            )
+        )
+
+        result_df3 = date_diff(test_df, 'dob','today',in_date_format='yyyy-MM-dd',units='years')
+
+        assert_df_equality(intended_df_3, result_df3, ignore_row_order=True,
+                           ignore_column_order=True)
```

### Comparing `dlh_utils-0.3.1/dlh_utils/tests/test_flags.py` & `dlh_utils-0.4.1/dlh_utils/tests/test_flags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 '''
-Pytesting on Dataframes functions
+Pytesting on Flags functions.
 '''
 import pandas as pd
 import pytest
 from chispa import assert_df_equality
+from pyspark.sql import SparkSession
+from pandas.util.testing import assert_frame_equal
 from dlh_utils.flags import flag, flag_check
 
 pytestmark = pytest.mark.usefixtures("spark")
 
 ###################################################################
+
+
 class TestFlag1:
     """Test for flag function"""
 
     @staticmethod
     def test_expected1(spark):
         """Test the expected functionality"""
 
@@ -75,14 +79,15 @@
             )
         )
 
         assert_df_equality(intended_df, result_df, allow_nan_equality=True)
 
 
 # ===================================================================
+
     @staticmethod
     def test_expected3(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame((pd.DataFrame(
             {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
 
@@ -109,14 +114,15 @@
             )
         )
 
         assert_df_equality(result_df, intended_df, allow_nan_equality=True)
 
 
 # ===================================================================
+
     @staticmethod
     def test_expected4(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame((pd.DataFrame(
             {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
 
@@ -143,14 +149,15 @@
             )
         )
 
         assert_df_equality(result_df, intended_df, allow_nan_equality=True)
 
 
 # ===================================================================
+
     @staticmethod
     def test_expected5(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame((pd.DataFrame(
             {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
 
@@ -181,14 +188,15 @@
             result_df,
             intended_df,
             allow_nan_equality=True,
             ignore_nullable=True)
 
 
 # ===================================================================
+
     @staticmethod
     def test_expected6(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame((pd.DataFrame(
             {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
 
@@ -219,291 +227,96 @@
             result_df,
             intended_df,
             allow_nan_equality=True,
             ignore_nullable=True)
 
 
 ###################################################################
+
 class TestFlagSummary1:
     """Test for flag_summary function"""
 
     @staticmethod
     def test_expected7(spark):
         """Test the expected functionality"""
 
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
-
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition="==",
-            condition_value=25,
-            condition_col=None,
-            alias=None,
-            prefix="FLAG",
-            fill_null=None,
-        )
-
-        intended_df = spark.createDataFrame(
+        df = spark.createDataFrame(
             (pd.DataFrame(
-                {
-                    "ref_col": list(range(40)) + [None] * 10,
-                    "condition_col": 25,
-                    "FLAG_ref_col==25": [False] * 25 + [True] + [False] * 24,
-                })))
-
-        assert_df_equality(
-            result_df,
-            intended_df,
-            allow_nan_equality=True,
-            ignore_nullable=True,
-            ignore_column_order=True,
-        )
-
-
-# ===================================================================
-    @staticmethod
-    def test_expected8(spark):
-        """Test the expected functionality"""
-
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10,
-             "condition_col": 25})))
-
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition="!=",
-            condition_value=25,
-            condition_col=None,
-            alias=None,
-            prefix="FLAG",
-            fill_null=None,
-        )
-
-        intended_df = spark.createDataFrame(
-            (pd.DataFrame(
-                {
-                    "ref_col": list(range(40)) +
-                    [None] *
-                    10,
-                    "condition_col": 25,
-                    "FLAG_ref_col!=25": [True] * 25 + [False] + [True] * 24,
-                })))
-
-        assert_df_equality(
-            result_df,
-            intended_df,
-            allow_nan_equality=True,
-            ignore_nullable=True,
-            ignore_column_order=True,
-        )
-
-
-# ===================================================================
-    @staticmethod
-    def test_expected9(spark):
-        """Test the expected functionality"""
-
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10,
-             "condition_col": 25})))
-
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition=">=",
-            condition_value=25,
-            condition_col=None,
-            alias=None,
-            prefix="FLAG",
-            fill_null=None,
-        )
-
-        intended_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
                     {
-                        "ref_col": list(range(40)) + [None] * 10,
-                        "condition_col": 25,
-                        "FLAG_ref_col>=25": [False] * 25 + [True] * 25,
-                    }
-                )
-            )
-        )
-
-        assert_df_equality(
-            result_df,
-            intended_df,
-            allow_nan_equality=True,
-            ignore_nullable=True,
-            ignore_column_order=True,
-        )
-
-
-# ===================================================================
-    @staticmethod
-    def test_expected10(spark):
-        """Test the expected functionality"""
-
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
-
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition="<=",
-            condition_value=25,
-            condition_col=None,
-            alias=None,
-            prefix="FLAG",
-            fill_null=None,
-        )
+                        "name": ['John', None, 'Arthur', 'Nahida', 
+                                          'Amber', 'Eula', None, 'Wriothesley'],
+                        "FLAG_nameisNotNull": [True, False, True, True, True, True, False, True]
 
-        intended_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
-                    {
-                        "ref_col": list(range(40)) + [None] * 10,
-                        "condition_col": 25,
-                        "FLAG_ref_col<=25": [True] * 26 + [False] * 24,
                     }
                 )
             )
         )
 
-        assert_df_equality(
-            result_df,
-            intended_df,
-            allow_nan_equality=True,
-            ignore_nullable=True,
-            ignore_column_order=True,
-        )
-
 
-# ===================================================================
-    @staticmethod
-    def test_expected11(spark):
-        """Test the expected functionality"""
-
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
-
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition="isNull",
-            condition_value=25,
-            condition_col=None,
-            alias=None,
-            prefix="FLAG",
-            fill_null=None,
-        )
+        result = flag_summary(df, flags='FLAG_nameisNotNull', pandas=False)
 
-        intended_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
-                    {
-                        "ref_col": list(range(40)) + [None] * 10,
-                        "condition_col": 25,
-                        "FLAG_ref_colisNull25": [False] * 40 + [True] * 10,
-                    }
-                )
-            )
-        )
+        expected = spark.createDataFrame(
+            (pd.DataFrame(
+                   {"flag": ['FLAG_nameisNotNull'],
+                    "true": [6],
+                    "false": [2],
+                    "rows": [8],
+                    "percent_true": [75.0],
+                    "percent_false": [25.0],
+                })))
 
         assert_df_equality(
-            result_df,
-            intended_df,
+            result,
+            expected,
             allow_nan_equality=True,
             ignore_nullable=True,
             ignore_column_order=True,
         )
 
 
 # ===================================================================
+
     @staticmethod
-    def test_expected12(spark):
+    def test_expected8(spark):
         """Test the expected functionality"""
 
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
-
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition="isNotNull",
-            condition_value=25,
-            condition_col=None,
-            alias=None,
-            prefix="FLAG",
-            fill_null=None,
-        )
-
-        intended_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
+        df = spark.createDataFrame(
+            (pd.DataFrame(
                     {
-                        "ref_col": list(range(40)) + [None] * 10,
-                        "condition_col": 25,
-                        "FLAG_ref_colisNotNull25": [True] * 40 + [False] * 10,
+                        "name": ['John', None, 'Arthur', 'Nahida', 
+                                          'Amber', 'Eula', None, 'Wriothesley'],
+                        "FLAG_nameisNotNull": [True, False, True, True, True, True, False, True]
+
                     }
                 )
             )
         )
 
-        assert_df_equality(
-            result_df,
-            intended_df,
-            allow_nan_equality=True,
-            ignore_nullable=True,
-            ignore_column_order=True,
-        )
-        
-# ===================================================================
-    @staticmethod
-    def test_expected13(spark):
-        """Test the expected functionality"""
-
-        test_df = spark.createDataFrame((pd.DataFrame(
-            {"ref_col": list(range(40)) + [None] * 10, "condition_col": 25})))
 
-        result_df = flag(
-            test_df,
-            ref_col="ref_col",
-            condition="regex",
-            condition_value="^1",
-            condition_col=None,
-            alias="test",
-            prefix="FLAG",
-            fill_null=None)
+        result = flag_summary(df, flags='FLAG_nameisNotNull', pandas=True)
 
-        intended_df = spark.createDataFrame(
-            (
-                pd.DataFrame(
-                    {
-                        "ref_col": list(range(40)) + [None] * 10,
-                        "condition_col": 25,
-                        "test": [False] + [True] + ([False] * 8)
-                                + ([True] * 10) + ([False] * 30)
-                    }
-                )
-            )
-        )
+        expected = pd.DataFrame(
+                   {"flag": ['FLAG_nameisNotNull'],
+                    "true": [6],
+                    "false": [2],
+                    "rows": [8],
+                    "percent_true": [75.0],
+                    "percent_false": [25.0],
+                })
 
-        assert_df_equality(intended_df, result_df, allow_nan_equality=True)
+        assert_frame_equal(result, expected, check_like=True)
 
 
 ###################################################################
+
 class TestFlagCheck1:
     """Test for flag_check function"""
 
     @staticmethod
-    def test_expected14(spark):
+    def test_expected9(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame(
             (pd.DataFrame({"FLAG_1": ([True] * 50) + ([False] * 50)}))
         )
 
         result_df = flag_check(
@@ -542,24 +355,29 @@
             ignore_nullable=True,
             ignore_column_order=True,
             ignore_schema=True,
         )
 
 
 # ===================================================================
+
     @staticmethod
-    def test_expected15(spark):
+    def test_expected10(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame(
             (pd.DataFrame({"FLAG_1": ([True] * 50) + ([False] * 50)}))
         )
 
         result_df = flag_check(
-            test_df, prefix="FLAG_", flags=None, mode="pass", summary=False
+          test_df,
+          prefix="FLAG_",
+          flags=None,
+          mode="pass",
+          summary=False,
         )
 
         intended_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "FLAG_1": ([False] * 50),
@@ -576,16 +394,17 @@
             ignore_nullable=True,
             ignore_column_order=True,
             ignore_schema=True,
         )
 
 
 # ===================================================================
+
     @staticmethod
-    def test_expected16(spark):
+    def test_expected11(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame(
             (pd.DataFrame({"FLAG_1": ([True] * 50) + ([False] * 50)}))
         )
 
         result_df = flag_check(
@@ -610,16 +429,17 @@
             ignore_nullable=True,
             ignore_column_order=True,
             ignore_schema=True,
         )
 
 
 # ===================================================================
+
     @staticmethod
-    def test_expected17(spark):
+    def test_expected12(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame(
             (pd.DataFrame({"FLAG_1": [True] * 50 + [False] * 50}))
         )
 
         result_df2 = flag_check(
@@ -643,16 +463,17 @@
             ignore_nullable=True,
             ignore_column_order=True,
             ignore_schema=True,
         )
 
 
 # ===================================================================
+
     @staticmethod
-    def test_expected18(spark):
+    def test_expected13(spark):
         """Test the expected functionality"""
 
         test_df = spark.createDataFrame(
             (pd.DataFrame({"FLAG_1": [True] * 50 + [False] * 50}))
         )
 
         result_df1, result_df2 = flag_check(
@@ -709,16 +530,17 @@
             ignore_nullable=True,
             ignore_column_order=True,
             ignore_schema=True,
         )
 
 
 # ===================================================================
+
     @staticmethod
-    def test_expected19(spark):
+    def test_expected14(spark):
         """Test the expected functionality"""
 
         pretest_df_orig = spark.createDataFrame(
             (pd.DataFrame({"FLAG_1": [True] * 50 + [False] * 50}))
         )
 
         pretest_df2 = flag_check(
```

### Comparing `dlh_utils-0.3.1/dlh_utils/tests/test_standardisation.py` & `dlh_utils-0.4.1/dlh_utils/tests/test_standardisation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,26 @@
 '''
-Pytesting on Standardisation functions
+Pytesting on Standardisation functions.
 '''
 
-import pyspark
 from pyspark.sql import SparkSession
-import pyspark.sql.functions as F
 from pyspark.sql.types import StructType,StructField,StringType,IntegerType,DoubleType,LongType
 import pandas as pd
-import chispa
 from chispa import assert_df_equality
 import pytest
 from dlh_utils.standardisation import cast_type,standardise_white_space,remove_punct,\
-trim,standardise_case,standardise_date,max_hyphen,max_white_space,align_forenames,\
-add_leading_zeros,group_single_characters,clean_hyphens,standardise_null,fill_nulls,\
-replace,clean_forename,clean_surname,reg_replace
+    trim,standardise_case,standardise_date,max_hyphen,max_white_space,align_forenames,\
+    add_leading_zeros,group_single_characters,clean_hyphens,standardise_null,fill_nulls,\
+    replace,clean_forename,clean_surname,reg_replace,age_at
 
 
 pytestmark = pytest.mark.usefixtures("spark")
 
 #############################################################################
 
-@pytest.fixture(scope="session")
-def spark(request):
-    """fixture for creating a spark context
-    Args:
-        request: pytest.FixtureRequest object
-    """
-    spark = (
-        SparkSession.builder.appName("dataframe_testing")
-        .config("spark.executor.memory", "5g")
-        .config("spark.yarn.excecutor.memoryOverhead", "2g")
-        .getOrCreate()
-    )
-    request.addfinalizer(lambda: spark.stop())
-    return spark
-
-#############################################################################
 
 class TestCastType(object):
     def test_expected(self, spark):
 
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
@@ -56,28 +37,30 @@
         )
 
         intended_data = [[float("NaN"), None], [2.0, 2], [3.0, 3], [4.0, 4], [5.0, 5]]
         intended_df = spark.createDataFrame(intended_data, intended_schema)
 
         # check if it is string first
         result_df = cast_type(test_df, subset="after", types="string")
-        assert_df_equality(intended_df, result_df, allow_nan_equality=True)
+        assert_df_equality(intended_df, result_df, allow_nan_equality=True,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_schema = StructType(
             [
                 StructField("after", DoubleType(), True),
                 StructField("before", IntegerType(), True),
             ]
         )
 
         intended_data = [[float("NaN"), None], [2.0, 2], [3.0, 3], [4.0, 4], [5.0, 5]]
         intended_df2 = spark.createDataFrame(intended_data, intended_schema)
         # check if columns are the same after various conversions
         result_df2 = cast_type(test_df, subset="before", types="int")
-        assert_df_equality(intended_df2, result_df2, allow_nan_equality=True)
+        assert_df_equality(intended_df2, result_df2, allow_nan_equality=True,
+                           ignore_row_order=True, ignore_column_order=True)
 
 ##############################################################################
 
 
 class TestStandardiseWhiteSpace(object):
     def test_expected(self, spark):
 
@@ -150,15 +133,16 @@
                             "hello_yes",
                         ],
                     }
                 )
             )
         )
         result_df = standardise_white_space(test_df, subset="before", wsl="one")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "before": [
                             None,
@@ -189,15 +173,129 @@
                             "hello_yes",
                         ],
                     }
                 )
             )
         )
         result_df2 = standardise_white_space(test_df, subset="before2", fill="_")
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
+
+    def test_expected_wsl_none(self, spark):
+
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": [
+                            None,
+                            "hello  yes",
+                            "hello yes",
+                            "hello   yes",
+                            "hello yes",
+                        ],
+                        "after": [
+                            None,
+                            "hello yes",
+                            "hello yes",
+                            "hello yes",
+                            "hello yes",
+                        ],
+                        "before2": [
+                            None,
+                            "hello  yes",
+                            "hello yes",
+                            "hello   yes",
+                            "hello yes",
+                        ],
+                        "after2": [
+                            None,
+                            "hello_yes",
+                            "hello_yes",
+                            "hello_yes",
+                            "hello_yes",
+                        ],
+                    }
+                )
+            )
+        )
+
+        intended_df3 = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": [
+                            None,
+                            "hello  yes",
+                            "hello yes",
+                            "hello   yes",
+                            "hello yes",
+                        ],
+                        "after": [
+                            None,
+                            "hello yes",
+                            "hello yes",
+                            "hello yes",
+                            "hello yes",
+                        ],
+                        "before2": [
+                            None,
+                            "helloyes",
+                            "helloyes",
+                            "helloyes",
+                            "helloyes",
+                        ],
+                        "after2": [
+                            None,
+                            "hello_yes",
+                            "hello_yes",
+                            "hello_yes",
+                            "hello_yes",
+                        ],
+                    }
+                )
+            )
+        )
+
+        result_df3 = standardise_white_space(test_df, subset="before2", wsl = 'none')
+        assert_df_equality(intended_df3, result_df3,
+                           ignore_row_order=True, ignore_column_order=True)
+
+##############################################################################
+
+class TestAlignForenames(object):
+    def test_expected(self, spark):
+
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "first_name": ["David Joe", "Dan James", "Neil Oliver", "Rich", "Rachel"],
+                        "middle_name": [" ", 'Jim', "", "Fred", "Amy"],
+                        "id": [101, 102, 103, 104, 105],
+                    }
+                )
+            )
+        )
+
+        intended_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "first_name": ["David", "Dan", "Neil", "Rich", "Rachel"],
+                        "middle_name": ['Joe', "James Jim", "Oliver", "Fred", "Amy"],
+                        "id": [101, 102, 103, 104, 105],
+                    }
+                )
+            )
+        )
+
+        result_df = align_forenames(test_df, 'first_name', 'middle_name', 'id', sep=' ')
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestRemovePunct(object):
     def test_expected(self, spark):
@@ -224,15 +322,16 @@
                     }
                 )
             )
         )
 
         result_df = remove_punct(test_df, keep="^", subset=["after", "before"])
 
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestTrim(object):
     def test_expected(self, spark):
@@ -261,15 +360,16 @@
                     }
                 )
             )
         )
 
         result_df = trim(test_df, subset=["before1", "numeric", "after"])
 
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestStandardiseCase(object):
     def test_expected(self, spark):
@@ -295,30 +395,48 @@
                         "title": ["One", "Two", "Three"],
                     }
                 )
             )
         )
 
         result_df = standardise_case(test_df, subset="lower", val="upper")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "upper": ["one", "two", "three"],
                         "lower": ["one", "two", "three"],
                         "title": ["One", "Two", "Three"],
                     }
                 )
             )
         )
 
         result_df2 = standardise_case(test_df, subset="upper", val="lower")
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
+
+        intended_df3 = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "upper": ["ONE", "TWO", "THREE"],
+                        "lower": ["One", "Two", "Three"],
+                        "title": ["One", "Two", "Three"],
+                    }
+                )
+            )
+        )
+
+        result_df3 = standardise_case(test_df, subset="lower", val="title")
+        assert_df_equality(intended_df3, result_df3,
+                           ignore_row_order=True, ignore_column_order=True)    
 
 
 ##############################################################################
 
 
 class TestStandardiseDate(object):
     def test_expected(self, spark):
@@ -346,15 +464,16 @@
                         "slashedReverse": [None, "1996/05/14", "1996/04/15"],
                     }
                 )
             )
         )
 
         result_df = standardise_date(test_df, col_name="before")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "before": [None, "14/05/1996", "15/04/1996"],
                         "after": [None, "1996-05-14", "1996-04-15"],
@@ -364,15 +483,16 @@
                 )
             )
         )
 
         result_df2 = standardise_date(
             test_df, col_name="before", out_date_format="dd/MM/yyyy"
         )
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df3 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "before": [None, "14-05-1996", "15-04-1996"],
                         "after": [None, "1996-05-14", "1996-04-15"],
@@ -382,20 +502,43 @@
                 )
             )
         )
 
         result_df3 = standardise_date(
             test_df,
             col_name="slashedReverse",
-            in_date_format="yyyy/mm/dd",
-            out_date_format="dd-mm-yyyy",
+            in_date_format="yyyy/MM/dd",
+            out_date_format="dd-MM-yyyy",
         )
 
-        assert_df_equality(intended_df3, result_df3)
+        assert_df_equality(intended_df3, result_df3,
+                           ignore_row_order=True, ignore_column_order=True)
+
+        intended_df4 = spark.createDataFrame(
+          (
+              pd.DataFrame(
+                  {
+                      "before": [None, "14/05/1996", "15/04/1996"],
+                      "after": [None, "1996-05-14", "1996-04-15"],
+                      "slashed": [None, "14/05/1996", "15/04/1996"],
+                      "slashedReverse": [None, "1996/05/14", "1996/04/15"],
+                  }
+              )
+          )
+        )
+
+        result_df4 = standardise_date(
+            test_df,
+            col_name="before",
+            in_date_format="dd-MM-yyyy",
+            out_date_format="dd/MM/yyyy"
+        )
 
+        assert_df_equality(intended_df4, result_df4,
+                         ignore_row_order=True, ignore_column_order=True)
 
 ##############################################################################
 
 
 class TestMaxHyphen(object):
     def test_expected(self, spark):
 
@@ -437,15 +580,16 @@
                         "chicken-wing",
                         "agentjohn",
                     ],
                 }
             )
         )
         result_df = max_hyphen(test_df, limit=2, subset=["before"])
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df2 = spark.createDataFrame(
             pd.DataFrame(
                 {
                     "before": [
                         "james--brad",
                         "tom----ridley",
@@ -459,15 +603,16 @@
                         "chicken-wing",
                         "agentjohn",
                     ],
                 }
             )
         )
         result_df2 = max_hyphen(test_df, limit=4, subset=["before"])
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestMaxWhiteSpace(object):
     def test_expected(self, spark):
@@ -506,15 +651,16 @@
                         "agentjohn",
                     ],
                 }
             )
         )
 
         result_df = max_white_space(test_df, limit=2, subset=["before"])
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df2 = spark.createDataFrame(
             pd.DataFrame(
                 {
                     "before": [
                         "james  brad",
                         "tom    ridley",
@@ -529,15 +675,16 @@
                         "agentjohn",
                     ],
                 }
             )
         )
 
         result_df2 = max_white_space(test_df, limit=4, subset=["before"])
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestAlignForenames(object):
     def test_expected(self, spark):
@@ -568,21 +715,23 @@
                         "middleName": ["green", "hog", "senior", "wick"],
                     }
                 )
             )
         )
 
         result_df = align_forenames(test_df, "firstName", "middleName", "identifier")
-        assert_df_equality(intended_df, result_df, ignore_row_order=True)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestAddLeadingZeros(object):
+
     def test_expected(self, spark):
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "before1": ["1-2-12", "2-2-12", "3-2-12", "4-2-12", None],
                         "after1": ["01-2-12", "02-2-12", "03-2-12", "04-2-12", None],
@@ -599,92 +748,95 @@
                         "after1": ["01-2-12", "02-2-12", "03-2-12", "04-2-12", None],
                     }
                 )
             )
         )
 
         result_df = add_leading_zeros(test_df, subset=["before1"], n=7)
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestGroupSingleCharacters(object):
     def test_expected(self, spark):
 
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
-                        "before1": [None, "", "-t-h r e e", "four", "f i v e", "six ",\
+                        "before1": [None, "", "-t-h r e e", "four", "f i v e", "six ",
                                     " seven", "eigh t", "n ine", "t  e    n", "e leve n"],
-                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",\
+                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",
                                     " seven", "eigh t", "n ine", "t  e    n", "e leve n"],
-                        "after": [None, "", "-t-h ree", "four", "five", "six ",\
+                        "after": [None, "", "-t-h ree", "four", "five", "six ",
                                   " seven", "eigh t", "n ine", "ten", "e leve n"],
                     }
                 )
             )
         )
 
         intended_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
-                        "before1": [None, "", "-t-h ree", "four", "five", "six ",\
+                        "before1": [None, "", "-t-h ree", "four", "five", "six ",
                                     " seven", "eigh t", "n ine", "ten", "e leve n"],
-                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",\
+                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",
                                     " seven", "eigh t", "n ine", "t  e    n", "e leve n"],
-                        "after": [None, "", "-t-h ree", "four", "five", "six ",\
+                        "after": [None, "", "-t-h ree", "four", "five", "six ",
                                   " seven", "eigh t", "n ine", "ten", "e leve n"],
                     }
                 )
             )
         )
         result_df = group_single_characters(test_df, subset="before1")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
     def test_expected_include_terminals(self, spark):
 
         test_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
-                        "before1": [None, "", "-t-h r e e", "four", "f i v e", "six ",\
+                        "before1": [None, "", "-t-h r e e", "four", "f i v e", "six ",
                                     " seven", "eigh t", "n ine", "t  e    n", "e leve n"],
-                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",\
+                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",
                                     " seven", "eigh t", "n ine", "t  e    n", "e leve n"],
-                        "after": [None, "", "-t-h ree", "four", "five", "six ",\
+                        "after": [None, "", "-t-h ree", "four", "five", "six ",
                                   " seven", "eight", "nine", "ten", "eleven"],
                     }
                 )
             )
         )
 
         intended_df = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
-                        "before1": [None, "", "-t-h ree", "four", "five", "six ",\
+                        "before1": [None, "", "-t-h ree", "four", "five", "six ",
                                     " seven", "eight", "nine", "ten", "eleven"],
-                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",\
+                        "before2": [None, "", "-t-h r e e", "four", "f i v e", "six ",
                                     " seven", "eigh t", "n ine", "t  e    n", "e leve n"],
-                        "after": [None, "", "-t-h ree", "four", "five", "six ",\
+                        "after": [None, "", "-t-h ree", "four", "five", "six ",
                                   " seven", "eight", "nine", "ten", "eleven"],
                     }
                 )
             )
         )
         result_df = group_single_characters(
-          test_df,
-          subset="before1",
-          include_terminals=True
+            test_df,
+            subset="before1",
+            include_terminals=True
         )
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestCleanHyphens(object):
     def test_expected(self, spark):
@@ -710,15 +862,16 @@
                         "after": [None, "", "th-ree", "fo-ur", "fi-ve"],
                     }
                 )
             )
         )
 
         result_df = clean_hyphens(test_df, subset="before1")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 #############################################################################
 
 
 class TestStandardiseNull(object):
     def test_expected(self, spark):
@@ -763,15 +916,16 @@
                 )
             )
         )
 
         result_df2 = standardise_null(
             test_df, replace="-999", subset="before1", regex=False
         )
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestFillNulls(object):
     def test_expected(self, spark):
@@ -799,15 +953,60 @@
                         "afternumeric": [1, 2, 0, 3],
                     }
                 )
             )
         )
 
         result_df = fill_nulls(test_df, 0)
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
+
+
+##############################################################################
+
+class TestAgeAt(object):
+    def test_expected(self, spark):
+
+        test_schema = StructType([
+            StructField("ID", LongType(), True),
+            StructField("Forename", StringType(), True),
+            StructField("Surname", StringType(), True),
+            StructField("DOB", StringType(), True)
+        ])
+
+        test_data = [
+          [1, "Homer", "Simpson", "1983-05-12"],
+          [2, "Marge", "Simpson", "1993-03-19"],
+          [3, "Bart", "Simpson", "2012-04-01"],
+          [4, "Lisa", "Simpson", "2014-05-09"]
+        ]
+
+        test_df = spark.createDataFrame(test_data, test_schema)
+
+        expected_schema = StructType([
+            StructField("ID", LongType(), True),
+            StructField("Forename", StringType(), True),
+            StructField("Surname", StringType(), True),
+            StructField("DOB", StringType(), True),
+            StructField("DoB_age_at_2022-11-03", IntegerType(), True),
+        ])
+
+        expected_data = [
+          [1, "Homer", "Simpson", "1983-05-12", 39],
+          [2, "Marge", "Simpson", "1993-03-19", 29],
+          [3, "Bart", "Simpson", "2012-04-01", 10],
+          [4, "Lisa", "Simpson", "2014-05-09", 8]
+        ]
+
+        intended_df = spark.createDataFrame(expected_data, expected_schema)      
+
+        dates = ['2022-11-03']
+        result_df = age_at(test_df,'DoB','yyyy-MM-dd',*dates)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestReplace(object):
     def test_expected(self, spark):
@@ -837,15 +1036,16 @@
                 )
             )
         )
 
         result_df = replace(
             test_df, subset="before", replace_dict={"a": None, "c": "f"}
         )
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
         intended_df2 = spark.createDataFrame(
             (
                 pd.DataFrame(
                     {
                         "before": [None, None, "f", ""],
                         "before1": [None, "b", "f", "d"],
@@ -855,16 +1055,138 @@
                 )
             )
         )
 
         result_df2 = replace(
             test_df, subset=["before", "before1"], replace_dict={"a": None, "c": "f"}
         )
-        assert_df_equality(intended_df2, result_df2)
+        assert_df_equality(intended_df2, result_df2,
+                           ignore_row_order=True, ignore_column_order=True)
+
+    def test_expected_with_join(self, spark):
+
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": ["a", None, "c", ""],
+                        "before1": ["a", "b", "c", "d"],
+                        "after": [None, None, "f", ""],
+                        "after1": [None, "b", "f", "d"],
+                    }
+                )
+            )
+        )
+
+        print("Test")
+        test_df.show()
+        intended_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": ["A", None, "f", ""],
+                        "before1": ["a", "b", "c", "d"],
+                        "after": [None, None, "f", ""],
+                        "after1": [None, "b", "f", "d"],
+                    }
+                )
+            )
+        )
+
+        print("Intended")
+        intended_df.show()
+        result_df = replace(
+            test_df, subset="before", replace_dict={"a": "A", "c": "f"}, use_join=True
+        )
+        print("Result")
+        result_df.show()
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
+
+    def test_expected_with_regex(self, spark):
+
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": ["alan", None, "betty", ""],
+                        "before1": ["a", "b", "c", "d"],
+                        "after": [None, None, "f", ""],
+                        "after1": [None, "b", "f", "d"],
+                    }
+                )
+            )
+        )
+
+        intended_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": ["A", None, "Y", ""],
+                        "before1": ["a", "b", "c", "d"],
+                        "after": [None, None, "f", ""],
+                        "after1": [None, "b", "f", "d"],
+                    }
+                )
+            )
+        )
+
+        result_df = replace(
+            test_df,
+            subset="before",
+            replace_dict={"^a": "A", "y$": "Y"},
+            use_regex=True
+        )
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
+
+    def test_value_error_on_join_and_regex(self, spark):
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": ["alan", None, "betty", ""],
+                        "before1": ["a", "b", "c", "d"],
+                        "after": [None, None, "f", ""],
+                        "after1": [None, "b", "f", "d"],
+                    }
+                )
+            )
+        )
+
+        with pytest.raises(ValueError) as e:
+            result_df = replace(
+                test_df,
+                subset="before",
+                replace_dict={"^a": "A", "y$": "Y"},
+                use_regex=True,
+                use_join=True
+            )
+
+    def test_value_error_on_join_and_none(self, spark):
+        test_df = spark.createDataFrame(
+            (
+                pd.DataFrame(
+                    {
+                        "before": ["alan", None, "betty", ""],
+                        "before1": ["a", "b", "c", "d"],
+                        "after": [None, None, "f", ""],
+                        "after1": [None, "b", "f", "d"],
+                    }
+                )
+            )
+        )
 
+        with pytest.raises(ValueError) as e:
+            result_df = replace(
+                test_df,
+                subset="before",
+                replace_dict={"^a": "A", None: "Y"},
+                use_join=True
+            )
 
 ##############################################################################
 
 
 class TestCleanForename(object):
     def test_expected(self, spark):
 
@@ -887,15 +1209,16 @@
                         "after": [" Maddie", " GEORGE", " Paul", ""],
                     }
                 )
             )
         )
 
         result_df = clean_forename(test_df, "before")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestCleanSurname(object):
     def test_expected(self, spark):
@@ -919,15 +1242,16 @@
                         "after": ["OLeary", "VANDERVAL", "", "MCCREW"],
                     }
                 )
             )
         )
 
         result_df = clean_surname(test_df, "before")
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
 
 
 ##############################################################################
 
 
 class TestRegReplace(object):
     def test_expected(self, spark):
@@ -959,8 +1283,9 @@
             replace_dict={
                 "street": "\\bstr\\b|\\bstrt\\b",
                 "avenue": "road",
                 "bond": "hello",
                 "queen": "king",
             },
         )
-        assert_df_equality(intended_df, result_df)
+        assert_df_equality(intended_df, result_df,
+                           ignore_row_order=True, ignore_column_order=True)
```

### Comparing `dlh_utils-0.3.1/dlh_utils/utilities.py` & `dlh_utils-0.4.1/dlh_utils/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 '''
 Utility functions used to ease difficulty in querying databases and produce descriptive
 metrics about a dataframe
 '''
 import subprocess
 import os
 import re
+import pandas as pd
 from pyspark.sql import SparkSession
 from pyspark.sql.types import TimestampType, LongType, IntegerType, DoubleType,\
     FloatType, StringType, StructType, StructField
 import pyspark.sql.functions as F
-from pyspark.context import SparkContext as sc
 from dlh_utils import dataframes as da
+from dlh_utils import utilities as ut
 
 ###############################################################################
 
 
 def list_files(file_path, walk=False, regex=None, full_path=True):
     """
     Lists files in a given HDFS directory, and/or all of that directory's
@@ -27,50 +28,54 @@
       String path of directory
     walk : boolean {True, False}
       Lists files only in immediate directory specified if walk = False.
       Lists all files in immediate directory and all subfolders if Walk = True
     regex : str
       use regex rexpression to find certain words within the listed files
     full_path : boolean
-      show full file path is full_path = True
+      show full file path if full_path = True
       show just files if full_path = False
 
     Returns
     -------
     list
       List of files
 
 
     """
     list_of_filenames = []
-    list_of_filename = []
 
-    if walk == True:
-        process = subprocess.Popen(["hadoop","fs", "-ls", "-R", file_path]\
-                                   ,stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    if walk is True:
+        process = subprocess.Popen(["hadoop","fs","-ls","-R", file_path],
+                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     else:
-        process = subprocess.Popen(["hadoop","fs", "-ls", "-C", file_path]\
-                                   ,stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        process = subprocess.Popen(["hadoop","fs","-ls","-C", file_path],
+                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     std_out, std_error = process.communicate()
-    std_out = str(std_out).split("\\n")[:-1]
-    std_out[0] = std_out[0].strip("b'")
 
-    if full_path == True:
-        for i in std_out:
-            file_name = str(i).split(' ')[-1]
-            list_of_filenames.append(file_name)
-
-    elif full_path == False:
-        for i in std_out:
-            file_name = str(i).split('/')[-1]
-            list_of_filenames.append(file_name)  
-
-    if regex != None:
-        list_of_filenames = list(filter(re.compile(regex).search, list_of_filenames))
+    try:
+        std_out = str(std_out).split("\\n")[:-1]
+        std_out[0] = std_out[0].strip("b'")
+
+        if full_path is True:
+            for i in std_out:
+                file_name = str(i).split(' ')[-1]
+                list_of_filenames.append(file_name)
+
+        elif full_path is False:
+            for i in std_out:
+                file_name = str(i).split('/')[-1]
+                list_of_filenames.append(file_name)
+
+        if regex is not None:
+            list_of_filenames = list(filter(re.compile(regex).search, list_of_filenames))
+    except:
+        print('no files in this directory')
+        list_of_filenames = []
 
     return list_of_filenames
 
 ###############################################################################
 
 
 def list_checkpoints(checkpoint):
@@ -304,16 +309,16 @@
 
                 # sort by max time since epoch and return corresponding path
                 most_recent_filepath = max(
                     filepath_dict, key=filepath_dict.get)
 
             except Exception as exc:
 
-                raise FileNotFoundError(filetype + " file, matching this regular expression: " +
-                                        regex + " not found in this directory: " + path) from exc
+                raise FileNotFoundError(filetype + " file, matching this regular expression: "
+                                        + regex + " not found in this directory: " + path) from exc
 
         # if filetype != hive
         else:
 
             # return all files in dir recursively, sorted by modification date (ascending),
             # decode from bytes-like to str
             files = subprocess.check_output(
@@ -336,36 +341,36 @@
                         f for f in filtered_files if f.endswith('csv')][-1]
 
                     # return path up until last '/'
                     most_recent_filepath = re.search('.*\/', result).group(0)
 
                 except Exception as exc:
 
-                    raise FileNotFoundError(filetype +
-                                            " file, matching this regular expression: " +
-                                            regex + " not found in this directory: " +
-                                            path) from exc
+                    raise FileNotFoundError(filetype
+                                            + " file, matching this regular expression: "
+                                            + regex + " not found in this directory: "
+                                            + path) from exc
 
             elif filetype == 'parquet':
 
                 try:
 
                     # filter for .csv ext and take last element of list
                     result = [
                         f for f in filtered_files if f.endswith('parquet')][-1]
 
                     # return path up until last '/'
                     most_recent_filepath = re.search('.*\/', result).group(0)
 
                 except Exception as exc:
 
-                    raise FileNotFoundError(filetype +
-                                            " file, matching this regular expression: " +
-                                            regex + " not found in this directory: " +
-                                            path) from exc
+                    raise FileNotFoundError(filetype
+                                            + " file, matching this regular expression: "
+                                            + regex + " not found in this directory: "
+                                            + path) from exc
 
     return most_recent_filepath, filetype
 
 ###############################################################################
 
 
 def write_format(df, write, path,
@@ -407,15 +412,14 @@
     Example
     -------
 
     > write_format(df = df, write = 'parquet', path = 'user/edwara5/simpsons.parquet',
                   mode = 'overwrite')
     """
 
-    spark = SparkSession.builder.getOrCreate()
     if file_name is None:
         if write == 'csv':
             df.write.format('csv').option('header', header).mode(
                 mode).option('sep', sep).save(f'{path}')
         if write == 'parquet':
             df.write.parquet(path=f'{path}', mode=mode)
         if write == 'hive':
@@ -574,14 +578,16 @@
                 if string in line:
                     count_list.append(count)
 
             if len(count_list) != 0:
                 diction[file] = count_list
         except IsADirectoryError:
             continue
+        except UnicodeDecodeError:
+            continue
 
     return diction
 
 ###############################################################################
 
 
 def describe_metrics(df, output_mode='pandas'):
@@ -601,15 +607,15 @@
     df : dataframe
       Dataframe to produce descriptive metrics about.
     output_mode: string, {'spark', 'pandas'}, default = pandas
       the type of dataframe to return
 
     Returns
     -------
-    decribe_df
+    describe_df
       A dataframe with columns detailing descriptive metrics on each variable
 
     Raises
     ------
     None at present.
 
     Example
@@ -625,60 +631,66 @@
     |   Surname|string|    6|       1|16.6666666666664|   0|         0.0|       6|           100.0|
     |       DoB|string|    6|       5| 83.333333333334|   0|         0.0|       6|           100.0|
     |       Sex|string|    6|       2| 33.333333333333|   0|         0.0|       6|           100.0|
     |  Postcode|string|    6|       1|16.6666666666664|   0|         0.0|       6|           100.0|
     +----------+------+-----+--------+----------------+----+------------+--------+----------------+
     """
 
-    spark = SparkSession.builder.getOrCreate()
-
     distinct_df = (df
                    .agg(*(F.countDistinct(F.col(c)).alias(c) for c in df.columns))
                    .withColumn('summary', F.lit('distinct')))
     null_df = (df
                .agg(*(F.count(F.when(F.isnan(F.col(c)) | F.col(c).isNull(), c))
                       .alias(c) for c in df.columns))
                .withColumn('summary', F.lit('null')))
 
-    decribe_df = da.union_all(distinct_df, null_df).persist()
+    describe_df = da.union_all(distinct_df, null_df).persist()
 
     count = df.count()
 
     types = df.dtypes
     types = dict(zip([x[0] for x in types],
                      [x[1] for x in types]))
 
-    decribe_df = decribe_df.toPandas()
-    decribe_df = decribe_df.transpose().reset_index()
-    decribe_df.columns = ['variable']+list(decribe_df[decribe_df['index'] == 'summary']
-                                           .reset_index(drop=True).transpose()[0])[1:]
-    decribe_df = decribe_df[decribe_df['variable'] != 'summary']
-    decribe_df['count'] = count
-    decribe_df['not_null'] = decribe_df['count']-decribe_df['null']
+    describe_df = describe_df.toPandas()
+    describe_df = describe_df.transpose().reset_index()
+    describe_df.columns = ['variable'] + list(describe_df[describe_df['index'] == 'summary']
+                                             .reset_index(drop=True).transpose()[0])[1:]
+    describe_df = describe_df[describe_df['variable'] != 'summary']
+    describe_df['count'] = count
+    describe_df['not_null'] = describe_df['count'] - describe_df['null']
     for variable in ['distinct', 'null', 'not_null']:
-        decribe_df['percent_' +
-                   variable] = (decribe_df[variable]/decribe_df['count'])*100
-    decribe_df['type'] = [types[x] for x in decribe_df['variable']]
+        describe_df['percent_'
+                   + variable] = (describe_df[variable] / describe_df['count']) * 100
+    describe_df['type'] = [types[x] for x in describe_df['variable']]
 
-    decribe_df = decribe_df[[
+    describe_df = describe_df[[
         'variable',
         'type',
         'count',
         'distinct',
         'percent_distinct',
         'null',
         'percent_null',
         'not_null',
         'percent_not_null'
     ]]
 
+    describe_df["count"] = describe_df["count"].astype(int)
+    describe_df["distinct"] = describe_df["distinct"].astype(int)
+    describe_df["null"] = describe_df["null"].astype(int)
+    describe_df["not_null"] = describe_df["not_null"].astype(int)
+    describe_df["percent_null"] = describe_df["percent_null"].astype(float)
+    describe_df["percent_not_null"] = describe_df["percent_not_null"].astype(float)
+    describe_df["percent_distinct"] = describe_df["percent_distinct"].astype(float)
+
     if output_mode == 'spark':
-        decribe_df = pandas_to_spark(decribe_df)
+        describe_df = pandas_to_spark(describe_df)
 
-    return decribe_df
+    return describe_df
 
 ###############################################################################
 
 
 def value_counts(df, limit=20, output_mode='pandas'):
     """
     Counts the most common values in all columns of a dataframe.
@@ -712,39 +724,38 @@
     |  3|       2|    Bart|             2|     Jo-Jo|               2|Simpson|            6|
     |  5|       1|   Homer|             1|      null|               1|       |            0|
     |  1|       1|   Marge|             1|    Juliet|               1|       |            0|
     |  4|       1|  Maggie|             1|     Marie|               1|       |            0|
     |  2|       1|    Lisa|             1|       Jay|               1|       |            0|
     +---+--------+--------+--------------+----------+----------------+-------+-------------+
     """
-    spark = SparkSession.builder.getOrCreate()
 
     def value_count(df, col, limit):
 
         return (df.
                 groupBy(col)
                 .count()
-                .sort('count', ascending=False)
+                .sort(['count', col], ascending=[False, True])
                 .limit(limit)
-                .withColumnRenamed('count', col+'_count')
+                .withColumnRenamed('count', col + '_count')
                 .toPandas())
 
     dfs = [value_count(df, col, limit) for col in df.columns]
 
     def make_limit(df, limit):
 
         count = df.shape[0]
 
         if count < limit:
 
-            dif = limit-count
+            dif = limit - count
 
             dif_df = pd.DataFrame({
-                0: ['']*dif,
-                1: [0]*dif
+                0: [''] * dif,
+                1: [0] * dif
             })[[0, 1]]
 
             dif_df.columns = list(df)
 
             df = (df
                   .append(dif_df)
                   .reset_index(drop=True)
@@ -935,39 +946,39 @@
 
     """
 
     sample_df = (df
                  .limit(limit)
                  ).persist()
 
-    sample_df.count()
+    row_count = sample_df.count()
 
     counts_df = (sample_df
                  .groupBy()
-                 .agg(*
-                      [F.sum(F.when(F.col(col)
-                                     .rlike(regex), 1)
+                 .agg(
+                     *[F.sum(F.when(F.col(col)
+                                    .rlike(regex), 1)
                              ).alias(col)
                        for col in sample_df.columns]
-                      )
+                 )
                  )
 
     counts_df = (counts_df
                  .toPandas()
                  .transpose()
                  .dropna()
                  .reset_index()
                  .rename(columns={
                      'index': 'variable',
                      0: 'count',
                  })
                  )
 
     counts_df['match_rate'] = \
-        counts_df['count']/limit
+        counts_df['count'] / row_count
 
     counts_df = (counts_df
                  [counts_df['match_rate'] >= cut_off]
                  .reset_index(drop=True)
                  )
 
     sample_df.unpersist()
@@ -1035,7 +1046,13 @@
         struct_list.append(define_structure(column, vartype))
 
     p_schema = StructType(struct_list)
 
     return spark.createDataFrame(pandas_df, p_schema)
 
 ###################################################################
+
+
+def chunk_list(_list, _num):
+    '''splits a list into a specified number of chunks'''
+    return [_list[i * _num:(i + 1) * _num]
+            for i in range((len(_list) + _num - 1) // _num)]
```

### Comparing `dlh_utils-0.3.1/pyproject.toml` & `dlh_utils-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "dlh_utils"
-version = "0.3.1"
+version = "0.4.1"
 description = "A PySpark package used to expedite and standardise the data linkage process"
-authors = ["Anthony Edwards <anthonygedwards93@gmail.com>", "Jenna Hart", "David Cobbledick", "Madalina Iova", "Dean Jathoonia"]
+authors = ["ONS Data Linkage Hub <linkage.hub@ons.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "dlh_utils"}]
 homepage = "https://github.com/Data-Linkage/dlh_utils"
 repository = "https://github.com/Data-Linkage/dlh_utils"
 
 [tool.poetry.dependencies]
 python = ">=3.6.8"
 graphframes = "^0.6"
 graphframes-jars = "^0.5"
 jellyfish = "^0.9"
 pandas = ">=0.20.3"
 importlib_metadata =  "^4.8.3"
+numpy = ">=1.15.4"
 
 [tool.poetry.group.dev.dependencies]
 pyspark = "^2.4.0"
 py4j = "^0.10.7"
 pytest = "^7.0"
 chispa = "^0.9.2"
 black = "^22.8.0"
```

### Comparing `dlh_utils-0.3.1/PKG-INFO` & `dlh_utils-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
-Name: dlh-utils
-Version: 0.3.1
+Name: dlh_utils
+Version: 0.4.1
 Summary: A PySpark package used to expedite and standardise the data linkage process
 Home-page: https://github.com/Data-Linkage/dlh_utils
 License: MIT
-Author: Anthony Edwards
-Author-email: anthonygedwards93@gmail.com
+Author: ONS Data Linkage Hub
+Author-email: linkage.hub@ons.gov.uk
 Requires-Python: >=3.6.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: graphframes (>=0.6,<0.7)
 Requires-Dist: graphframes-jars (>=0.5,<0.6)
 Requires-Dist: importlib_metadata (>=4.8.3,<5.0.0)
 Requires-Dist: jellyfish (>=0.9,<0.10)
+Requires-Dist: numpy (>=1.15.4)
 Requires-Dist: pandas (>=0.20.3)
 Project-URL: Repository, https://github.com/Data-Linkage/dlh_utils
 Description-Content-Type: text/markdown
 
 # DLH_utils
 
 [![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
@@ -51,14 +53,21 @@
 ```sh
 pip3 install -U dlh_utils
 ```
 
 ## Demo
 For a worked demonstration notebook of these functions being applied within a data linkage context, head over to our [separate demo repository](https://github.com/anthonye93/dlh_utils_demo)
 
+## Contributing
+
+This repository adheres to pep8 coding standards. These can be automatically checked for when you're making new commits by the repository's pre-commit hooks. To get this working:
+* `pip install` both 'flake8' and 'pre-commit'
+* install the git hook scripts `pre-commit install`
+* When adding new git commits, the pre-commit hooks will now run and make suggestions needed to adhere to pep8 code standards
+
 ## Common issues
 
 ### When using the jaro/jaro_winkler functions the error "no module called Jellyfish found" is thrown
 
 These functions are dependent on the Jellyfish package and this may not be installed on the executors used in your spark session.
 Try submitting Jellyfish to your sparkcontext via addPyFile() or by setting the following environmental variables in your CDSW engine settings (ONS only):
 
@@ -84,9 +93,9 @@
 
 ## Thanks
 
 Thanks to all those in the Data Linkage Hub, Data Engineering and Methodology at ONS that have contributed towards this repository.
 
 ## Any questions?
 
-If you need any additional help, or have any feedback on the package, please contact Jenna Hart (Jenna.Hart@ons.gov.uk) or the Data Linkage Hub at Linkage.Hub@ons.gov.uk . 
+If you need any additional help, or have any feedback on the package, please contact the Data Linkage Hub at Linkage.Hub@ons.gov.uk .
```

