# Comparing `tmp/easier-1.3.9.tar.gz` & `tmp/easier-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easier-1.3.9.tar", last modified: Sun Aug 27 15:19:12 2023, max compression
+gzip compressed data, was "easier-1.4.0.tar", last modified: Mon May 20 00:50:18 2024, max compression
```

## Comparing `easier-1.3.9.tar` & `easier-1.4.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-08-27 15:19:12.263555 easier-1.3.9/
--rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.3.9/CONTRIBUTORS.txt
--rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.3.9/LICENSE
--rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.3.9/MANIFEST.in
--rw-rw-r--   0 rob        (501) staff       (20)      448 2023-08-27 15:19:12.263613 easier-1.3.9/PKG-INFO
--rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.3.9/README.md
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-08-27 15:19:12.261305 easier-1.3.9/easier/
--rw-rw-r--   0 rob        (501) staff       (20)      687 2023-08-27 15:08:50.000000 easier-1.3.9/easier/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     6003 2023-08-13 21:28:46.000000 easier-1.3.9/easier/api.py
--rw-rw-r--   0 rob        (501) staff       (20)    11673 2023-07-29 15:18:13.000000 easier-1.3.9/easier/bernstein.py
--rw-rw-r--   0 rob        (501) staff       (20)    15579 2023-08-27 15:08:50.000000 easier-1.3.9/easier/bigquery.py
--rw-rw-r--   0 rob        (501) staff       (20)     1460 2023-08-27 15:08:50.000000 easier-1.3.9/easier/cli.py
--rw-rw-r--   0 rob        (501) staff       (20)     4382 2023-08-27 15:08:50.000000 easier-1.3.9/easier/clock.py
--rw-rw-r--   0 rob        (501) staff       (20)     2152 2023-08-27 15:08:50.000000 easier-1.3.9/easier/crypt.py
--rw-rw-r--   0 rob        (501) staff       (20)    12830 2023-08-27 15:08:50.000000 easier-1.3.9/easier/dataframe_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     4933 2023-08-27 15:08:50.000000 easier-1.3.9/easier/distributions.py
--rw-rw-r--   0 rob        (501) staff       (20)     3737 2023-08-27 15:08:50.000000 easier-1.3.9/easier/duck.py
--rw-rw-r--   0 rob        (501) staff       (20)     7130 2023-08-27 15:08:50.000000 easier-1.3.9/easier/duck_model.py
--rw-rw-r--   0 rob        (501) staff       (20)     1355 2023-08-27 15:08:50.000000 easier-1.3.9/easier/ecdf_lib.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-08-27 15:19:12.263422 easier-1.3.9/easier/filtering/
--rw-rw-r--   0 rob        (501) staff       (20)       89 2023-08-27 15:08:50.000000 easier-1.3.9/easier/filtering/__init__.py
--rw-rw-r--   0 rob        (501) staff       (20)     5853 2023-08-27 15:08:50.000000 easier-1.3.9/easier/filtering/elliptic_filter.py
--rw-rw-r--   0 rob        (501) staff       (20)     2108 2023-08-27 15:08:50.000000 easier-1.3.9/easier/filtering/tvd.py
--rw-rw-r--   0 rob        (501) staff       (20)    14279 2023-08-27 15:08:50.000000 easier-1.3.9/easier/fit_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     8572 2023-08-27 15:08:50.000000 easier-1.3.9/easier/gsheet.py
--rw-rw-r--   0 rob        (501) staff       (20)     7827 2023-08-27 15:08:50.000000 easier-1.3.9/easier/hvtools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-08-27 15:08:50.000000 easier-1.3.9/easier/ibis_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     1780 2023-08-27 15:08:50.000000 easier-1.3.9/easier/item.py
--rw-rw-r--   0 rob        (501) staff       (20)     2136 2023-08-27 15:08:50.000000 easier-1.3.9/easier/iterify.py
--rw-rw-r--   0 rob        (501) staff       (20)      207 2023-08-27 15:08:50.000000 easier-1.3.9/easier/memory.py
--rw-rw-r--   0 rob        (501) staff       (20)    11644 2023-08-27 15:08:50.000000 easier-1.3.9/easier/minimodel.py
--rw-rw-r--   0 rob        (501) staff       (20)     8242 2023-08-27 15:08:50.000000 easier-1.3.9/easier/minimodel_orig.py
--rw-rw-r--   0 rob        (501) staff       (20)     5230 2023-08-27 15:08:50.000000 easier-1.3.9/easier/nice_dates.py
--rw-rw-r--   0 rob        (501) staff       (20)     2076 2023-08-27 15:08:50.000000 easier-1.3.9/easier/outlier_tools.py
--rw-rw-r--   0 rob        (501) staff       (20)     3268 2023-08-27 15:08:50.000000 easier-1.3.9/easier/parallel.py
--rw-rw-r--   0 rob        (501) staff       (20)     7850 2023-08-27 15:08:50.000000 easier-1.3.9/easier/param_state.py
--rw-rw-r--   0 rob        (501) staff       (20)     1219 2023-08-27 15:08:50.000000 easier-1.3.9/easier/plotting.py
--rw-rw-r--   0 rob        (501) staff       (20)     8456 2023-08-27 15:08:50.000000 easier-1.3.9/easier/postgres.py
--rw-rw-r--   0 rob        (501) staff       (20)      663 2023-08-27 15:08:50.000000 easier-1.3.9/easier/print_catcher.py
--rw-rw-r--   0 rob        (501) staff       (20)     6292 2023-08-27 15:08:50.000000 easier-1.3.9/easier/proportion_lib.py
--rw-rw-r--   0 rob        (501) staff       (20)     3218 2023-08-27 15:08:50.000000 easier-1.3.9/easier/salesforce.py
--rw-rw-r--   0 rob        (501) staff       (20)     3215 2023-08-27 15:08:50.000000 easier-1.3.9/easier/shaper.py
--rw-rw-r--   0 rob        (501) staff       (20)     2903 2023-08-27 15:08:50.000000 easier-1.3.9/easier/timer.py
--rw-rw-r--   0 rob        (501) staff       (20)    19316 2023-08-27 15:08:50.000000 easier-1.3.9/easier/utils.py
--rw-rw-r--   0 rob        (501) staff       (20)       22 2023-08-27 15:13:07.000000 easier-1.3.9/easier/version.py
-drwxrwxr-x   0 rob        (501) staff       (20)        0 2023-08-27 15:19:12.262997 easier-1.3.9/easier.egg-info/
--rw-r--r--   0 rob        (501) staff       (20)      448 2023-08-27 15:19:12.000000 easier-1.3.9/easier.egg-info/PKG-INFO
--rw-r--r--   0 rob        (501) staff       (20)     1018 2023-08-27 15:19:12.000000 easier-1.3.9/easier.egg-info/SOURCES.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-08-27 15:19:12.000000 easier-1.3.9/easier.egg-info/dependency_links.txt
--rw-r--r--   0 rob        (501) staff       (20)      117 2023-08-27 15:19:12.000000 easier-1.3.9/easier.egg-info/entry_points.txt
--rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.3.9/easier.egg-info/not-zip-safe
--rw-r--r--   0 rob        (501) staff       (20)       36 2023-08-27 15:19:12.000000 easier-1.3.9/easier.egg-info/requires.txt
--rw-r--r--   0 rob        (501) staff       (20)        7 2023-08-27 15:19:12.000000 easier-1.3.9/easier.egg-info/top_level.txt
--rw-rw-r--   0 rob        (501) staff       (20)      504 2023-08-27 15:19:12.263908 easier-1.3.9/setup.cfg
--rw-rw-r--   0 rob        (501) staff       (20)     1641 2023-08-27 15:08:50.000000 easier-1.3.9/setup.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2024-05-20 00:50:18.217162 easier-1.4.0/
+-rw-rw-r--   0 rob        (501) staff       (20)       39 2017-12-14 15:28:52.000000 easier-1.4.0/CONTRIBUTORS.txt
+-rw-rw-r--   0 rob        (501) staff       (20)     1081 2017-12-14 15:28:52.000000 easier-1.4.0/LICENSE
+-rw-rw-r--   0 rob        (501) staff       (20)       73 2017-12-14 15:28:52.000000 easier-1.4.0/MANIFEST.in
+-rw-r--r--   0 rob        (501) staff       (20)      585 2024-05-20 00:50:18.217090 easier-1.4.0/PKG-INFO
+-rw-rw-r--   0 rob        (501) staff       (20)    12815 2019-12-20 21:04:42.000000 easier-1.4.0/README.md
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2024-05-20 00:50:18.215049 easier-1.4.0/easier/
+-rw-rw-r--   0 rob        (501) staff       (20)      687 2023-08-13 22:02:16.000000 easier-1.4.0/easier/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6242 2024-05-20 00:43:42.000000 easier-1.4.0/easier/api.py
+-rw-rw-r--   0 rob        (501) staff       (20)    12887 2024-05-17 19:23:31.000000 easier-1.4.0/easier/bernstein.py
+-rw-rw-r--   0 rob        (501) staff       (20)    15579 2023-08-13 22:02:16.000000 easier-1.4.0/easier/bigquery.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1460 2023-08-13 22:02:16.000000 easier-1.4.0/easier/cli.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4382 2023-08-13 22:02:16.000000 easier-1.4.0/easier/clock.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2152 2023-08-13 22:02:16.000000 easier-1.4.0/easier/crypt.py
+-rw-rw-r--   0 rob        (501) staff       (20)    13038 2023-12-22 17:30:18.000000 easier-1.4.0/easier/dataframe_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8456 2023-08-13 21:41:01.000000 easier-1.4.0/easier/deleteme_postgres.py
+-rw-rw-r--   0 rob        (501) staff       (20)     4933 2023-08-13 22:02:16.000000 easier-1.4.0/easier/distributions.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3737 2023-08-13 22:02:16.000000 easier-1.4.0/easier/duck.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7130 2023-08-13 22:02:16.000000 easier-1.4.0/easier/duck_model.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1355 2023-08-13 22:02:16.000000 easier-1.4.0/easier/ecdf_lib.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2024-05-20 00:50:18.216519 easier-1.4.0/easier/filtering/
+-rw-rw-r--   0 rob        (501) staff       (20)       89 2023-08-13 22:02:16.000000 easier-1.4.0/easier/filtering/__init__.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5853 2023-08-13 22:02:16.000000 easier-1.4.0/easier/filtering/elliptic_filter.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2108 2023-08-13 22:02:16.000000 easier-1.4.0/easier/filtering/tvd.py
+-rw-rw-r--   0 rob        (501) staff       (20)    19082 2024-03-04 15:48:06.000000 easier-1.4.0/easier/fit_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8572 2023-08-13 22:02:16.000000 easier-1.4.0/easier/gsheet.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7827 2023-08-13 22:02:16.000000 easier-1.4.0/easier/hvtools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3749 2023-08-13 22:02:16.000000 easier-1.4.0/easier/ibis_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1780 2023-08-13 22:02:16.000000 easier-1.4.0/easier/item.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2136 2023-08-13 22:02:16.000000 easier-1.4.0/easier/iterify.py
+-rw-rw-r--   0 rob        (501) staff       (20)      207 2023-08-13 22:02:16.000000 easier-1.4.0/easier/memory.py
+-rw-rw-r--   0 rob        (501) staff       (20)    11644 2023-08-13 22:02:16.000000 easier-1.4.0/easier/minimodel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8242 2023-08-13 22:02:16.000000 easier-1.4.0/easier/minimodel_orig.py
+-rw-rw-r--   0 rob        (501) staff       (20)     5230 2023-08-13 22:02:16.000000 easier-1.4.0/easier/nice_dates.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2076 2023-08-13 22:02:16.000000 easier-1.4.0/easier/outlier_tools.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3268 2023-08-13 22:02:16.000000 easier-1.4.0/easier/parallel.py
+-rw-rw-r--   0 rob        (501) staff       (20)     7850 2023-08-13 22:02:16.000000 easier-1.4.0/easier/param_state.py
+-rw-rw-r--   0 rob        (501) staff       (20)     1219 2023-08-13 22:02:16.000000 easier-1.4.0/easier/plotting.py
+-rw-rw-r--   0 rob        (501) staff       (20)     8457 2024-05-08 15:43:49.000000 easier-1.4.0/easier/postgres.py
+-rw-rw-r--   0 rob        (501) staff       (20)      663 2023-08-13 22:02:16.000000 easier-1.4.0/easier/print_catcher.py
+-rw-rw-r--   0 rob        (501) staff       (20)     6292 2023-08-13 22:02:16.000000 easier-1.4.0/easier/proportion_lib.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3218 2023-08-13 22:02:16.000000 easier-1.4.0/easier/salesforce.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3215 2023-08-13 22:02:16.000000 easier-1.4.0/easier/shaper.py
+-rw-rw-r--   0 rob        (501) staff       (20)     2903 2023-08-13 22:02:16.000000 easier-1.4.0/easier/timer.py
+-rw-rw-r--   0 rob        (501) staff       (20)    19316 2023-08-13 22:02:16.000000 easier-1.4.0/easier/utils.py
+-rw-rw-r--   0 rob        (501) staff       (20)       22 2024-05-20 00:49:46.000000 easier-1.4.0/easier/version.py
+-rw-rw-r--   0 rob        (501) staff       (20)     3505 2024-05-20 00:48:23.000000 easier-1.4.0/easier/vonmises.py
+drwxrwxr-x   0 rob        (501) staff       (20)        0 2024-05-20 00:50:18.216704 easier-1.4.0/easier.egg-info/
+-rw-r--r--   0 rob        (501) staff       (20)      585 2024-05-20 00:50:18.000000 easier-1.4.0/easier.egg-info/PKG-INFO
+-rw-r--r--   0 rob        (501) staff       (20)     1065 2024-05-20 00:50:18.000000 easier-1.4.0/easier.egg-info/SOURCES.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2024-05-20 00:50:18.000000 easier-1.4.0/easier.egg-info/dependency_links.txt
+-rw-r--r--   0 rob        (501) staff       (20)      117 2024-05-20 00:50:18.000000 easier-1.4.0/easier.egg-info/entry_points.txt
+-rw-r--r--   0 rob        (501) staff       (20)        1 2023-01-04 21:15:28.000000 easier-1.4.0/easier.egg-info/not-zip-safe
+-rw-r--r--   0 rob        (501) staff       (20)       36 2024-05-20 00:50:18.000000 easier-1.4.0/easier.egg-info/requires.txt
+-rw-r--r--   0 rob        (501) staff       (20)        7 2024-05-20 00:50:18.000000 easier-1.4.0/easier.egg-info/top_level.txt
+-rw-rw-r--   0 rob        (501) staff       (20)      504 2024-05-20 00:50:18.217508 easier-1.4.0/setup.cfg
+-rw-rw-r--   0 rob        (501) staff       (20)     1641 2023-08-13 22:02:16.000000 easier-1.4.0/setup.py
```

### Comparing `easier-1.3.9/LICENSE` & `easier-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/README.md` & `easier-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/__init__.py` & `easier-1.4.0/easier/__init__.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/api.py` & `easier-1.4.0/easier/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,25 +69,29 @@
     Soql = Importable("easier.salesforce", "Soql")
     Timer = Importable("easier.timer", "Timer")
     beta_plots = Importable("easier.hvtools", "beta_plots")
     cached_container = Importable("easier.utils", "cached_container")
     cached_dataframe = Importable("easier.utils", "cached_dataframe")
     cached_property = Importable("easier.utils", "cached_property")
     cc = Importable("easier.plotting", "ColorCyle", instantiate=True)
+    classifier_evaluation_plots = Importable(
+        "easier.fit_lib", "classifier_evaluation_plots"
+    )
     column_level_flattener = Importable(
         "easier.dataframe_tools", "column_level_flattener"
     )
     date_formatter = Importable("easier.nice_dates", "nice_dates")
     django_reconnect = Importable("easier.utils", "django_reconnect")
     ecdf = Importable("easier.ecdf_lib", "ecdf")
     events_from_starting_ending = Importable(
         "easier.dataframe_tools", "events_from_starting_ending"
     )
     figure = Importable("easier.plotting", "figure")
     get_logger = Importable("easier.utils", "get_logger")
+    heatmap = Importable("easier.dataframe_tools", "heatmap")
     hist = Importable("easier.hvtools", "hist")
     ibis_conn_to_sqlalchemy_conn = Importable(
         "easier.ibis_tools", "ibis_conn_to_sqlalchemy_conn"
     )
     ibis_duck_connection = Importable("easier.ibis_tools", "ibis_duck_connection")
     ibis_get_sql = Importable("easier.ibis_tools", "get_sql")
     ibis_postgres_connection = Importable(
@@ -120,9 +124,10 @@
     pickle_cached_container = Importable("easier.utils", "pickle_cached_container")
     print_error = Importable("easier.utils", "print_error")
     python_type = Importable("easier.utils", "python_type")
     screen_width_full = Importable("easier.utils", "screen_width_full")
     slugify = Importable("easier.dataframe_tools", "slugify")
     tqdm_flex = Importable("easier.utils", "tqdm_flex")
     tvd = Importable("easier.filtering.tvd", "tvd")
+    VonMisesFitter = Importable("easier.vonmises", "VonMisesFitter")
     warnings_mute = Importable("easier.utils", "mute_warnings")
     weekday_string = Importable("easier.dataframe_tools", "weekday_string")
```

### Comparing `easier-1.3.9/easier/bernstein.py` & `easier-1.4.0/easier/bernstein.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     w = BlobAttr(None)
     scaler_blob = BlobAttr(None)
 
     def __init__(
         self,
         non_negative=False,
         monotonic=False,
-        increasing=False,
+        increasing=True,
         match_left=False,
         match_right=False,
         match_endpoint_values=False,
         match_endpoint_derivatives=False,
     ):
         super().__init__()
         self._non_negative = non_negative
@@ -263,15 +263,44 @@
 
         for k in range(0, degree + 1):
             term1 = self._bern_term(n - 1, k - 1, x)
             term2 = self._bern_term(n - 1, k, x)
             B[:, k] = n * (term1 - term2)
         return B
 
-    def fit(self, x, y, degree, verbose=False):
+    def _get_integral_matrix(self, x, degree):
+        import numpy as np
+
+        n = degree
+
+        A = self._get_design_matrix(x, degree + 1)
+        B = np.zeros_like(A)
+        coeff = 1 / (n + 1)
+        for k in range(0, degree + 1):
+            X = A[:, (k + 1) :]
+            B[:, k] = coeff * np.sum(X, axis=1)
+        return B
+
+    def get_design_matrix(self, x, degree):
+        import numpy as np
+
+        x = np.array(x)
+
+        scaler = Scaler()
+        x = scaler.fit_transform(x)
+        self.scaler_blob = scaler.to_blob()
+
+        A = self._get_design_matrix(x, degree)
+        return A
+
+    def fit_predict(self, x, y, degree, regulizer=0.0, verbose=False):
+        self.fit(x, y, degree, regulizer=regulizer, verbose=verbose)
+        return self.predict(x)
+
+    def fit(self, x, y, degree, regulizer=0.0, verbose=False):
         import cvxpy as cp
         import numpy as np
 
         x = np.array(x)
         y = np.array(y)
 
         scaler = Scaler()
@@ -282,15 +311,15 @@
         A = self._get_design_matrix(x, degree)
         B = self._get_derivative_matrix(x, degree)
 
         # Define a weight variable to be optimized
         w = cp.Variable(name="w", shape=(degree + 1, 1))
 
         # The objective is the mininum squared error
-        objective = cp.Minimize(cp.sum_squares(A @ w - yv))
+        objective = cp.Minimize(cp.sum_squares(A @ w - yv) + regulizer * cp.norm(w, 2))
 
         # Default to unconstrained
         constraints = []
 
         if self._non_negative:
             constraints.append(w >= np.zeros(w.shape))
 
@@ -352,14 +381,25 @@
             )
 
         scaler = Scaler()
         scaler.from_blob(self.scaler_blob)
         diffs = self._get_prediction(x, "derivative")
         return diffs / (scaler.limits[1] - scaler.limits[0])
 
+    def predict_integral(self, x):
+        if self.w is None:
+            raise ValueError(
+                "You must run fit() or load a blob before running predict()"
+            )
+
+        scaler = Scaler()
+        scaler.from_blob(self.scaler_blob)
+        result = self._get_prediction(x, "integral")
+        return result * (scaler.limits[1] - scaler.limits[0])
+
     def _get_prediction(self, x, what):
         import numpy as np
 
         if self.w is None:
             raise ValueError(
                 "You must run fit() or load a blob before running predict()"
             )
@@ -378,31 +418,31 @@
         wv = np.reshape(self.w, (-1, 1))
         if what == "value":
             A = self._get_design_matrix(x, degree)
             yv = A @ wv
         elif what == "derivative":
             B = self._get_derivative_matrix(x, degree)
             yv = B @ wv
+        elif what == "integral":
+            B = self._get_integral_matrix(x, degree)
+            yv = B @ wv
         else:
-            raise ValueError('Nope!  Bad "what" argument')
+            raise ValueError(f'Nope!  {what!r} is a bad "what" argument')
 
         yv = yv.flatten()
         if is_scalar:
             return yv[0]
         else:
             return yv
 
-    def fit_predict(self, x, y, degree):
-        self.fit(x, y, degree)
-        return self.predict(x)
-
     def to_blob(self):
         blob = super().to_blob()
         blob["w"] = list(blob["w"])
         return blob
 
     def from_blob(self, blob):
         import numpy as np
 
         super().from_blob(blob)
         self.w = np.array(self.w)
+
         return self
```

### Comparing `easier-1.3.9/easier/bigquery.py` & `easier-1.4.0/easier/bigquery.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/cli.py` & `easier-1.4.0/easier/cli.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/clock.py` & `easier-1.4.0/easier/clock.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/crypt.py` & `easier-1.4.0/easier/crypt.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/dataframe_tools.py` & `easier-1.4.0/easier/dataframe_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from typing import Union, Iterable
 import re
 
 
+def heatmap(df, axis=None, cmap="magma", format="{:.1f}"):
+    # This will crash if not run in a jupyter notebook.  That's ok.
+    display(df.style.background_gradient(axis=axis, cmap=cmap).format(format))
+
+
 def column_level_flattener(df, level=1):
     """
     Takes a multi-level column dataframe and returns a flattened version.
     Default is to use level=1, but you can use other levels as well.
     Args:
         level: The level of the index you want to use (defaults to 1)
         level: "smash" will join column levels with an underscore
```

### Comparing `easier-1.3.9/easier/distributions.py` & `easier-1.4.0/easier/distributions.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/duck.py` & `easier-1.4.0/easier/duck.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/duck_model.py` & `easier-1.4.0/easier/duck_model.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/ecdf_lib.py` & `easier-1.4.0/easier/ecdf_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/filtering/elliptic_filter.py` & `easier-1.4.0/easier/filtering/elliptic_filter.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/filtering/tvd.py` & `easier-1.4.0/easier/filtering/tvd.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/fit_lib.py` & `easier-1.4.0/easier/fit_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -433,7 +433,149 @@
             color=line_color
         )
         traces = [scatter, line]
         if as_components:
             return traces
         else:
             return hv.Overlay(traces)
+
+
+# I'm not sure where this should actually live, but I'm putting it here for now.
+def classifier_evaluation_plots(
+    trained_model,
+    X_test,
+    y_test,
+    threshold=0.5,
+    plots="confusion_matrix, variable_importance, roc_curve, precision_recall, lift",
+):
+    """
+    Creates classifier evalutaion plots.
+    Args:
+        trained_model: A trained sklearn or xbg model
+        X_test: A test dataframe of X variables
+        y_test A test dataframe of y variables (0 or 1)
+        threshold: The operating point of the classifier
+    """
+    import matplotlib.pyplot as plt
+    import numpy as np
+    import pandas as pd
+    from IPython.display import display
+    from sklearn.metrics import (
+        auc,
+        average_precision_score,
+        confusion_matrix,
+        precision_recall_curve,
+        roc_curve,
+    )
+
+    if "variable_importance" in plots:
+        # Plot variable importance
+        imp = pd.Series(
+            trained_model.feature_importances_, index=trained_model.feature_names_in_
+        ).sort_values()
+        plt.figure()
+        ax = imp.plot.barh(xlabel="Variable Importance")
+        ax.figure.subplots_adjust(left=0.3)
+        plt.show()
+
+    # Step 2: Prediction and Threshold Selection
+    y_pred_prob = trained_model.predict_proba(X_test)[
+        :, 1
+    ]  # probabilities of positive class
+    y_pred = (y_pred_prob >= threshold).astype(int)
+
+    if "confusion_matrix" in plots:
+        # Step 3: Generating and Displaying Confusion Matrix
+        conf_matrix = confusion_matrix(y_test, y_pred)
+        conf_matrix_df = pd.DataFrame(
+            conf_matrix,
+            index=["True Negative", "True Positive"],
+            columns=["Predicted Negative", "Predicted Positive"],
+        )
+        display(conf_matrix_df)
+
+    if "roc_curve" in plots:
+        # Step 4: Plotting ROC Curve and Calculating AUC
+        fpr, tpr, thresholds_roc = roc_curve(y_test, y_pred_prob)
+        roc_auc = auc(fpr, tpr)
+        # Find the closest threshold to the selected one on the ROC curve
+        closest_threshold_index = np.argmin(np.abs(thresholds_roc - threshold))
+        operating_point_roc = (
+            fpr[closest_threshold_index],
+            tpr[closest_threshold_index],
+        )
+
+        plt.figure()
+        plt.plot(
+            fpr,
+            tpr,
+            color="darkorange",
+            lw=2,
+            label=f"ROC curve (area = {roc_auc:.2f})",
+        )
+        plt.plot([0, 1], [0, 1], color="navy", lw=2, linestyle="-")
+        max_ind = min([len(fpr), len(thresholds_roc)])
+        plt.plot(
+            fpr[:max_ind],
+            thresholds_roc[:max_ind],
+            label="threshold (y ax)",
+            color="grey",
+            linestyle="--",
+        )
+
+        plt.scatter(*operating_point_roc, color="red", label="Operating Point")
+        plt.xlabel("False Positive Rate")
+        plt.ylabel("True Positive Rate")
+        plt.title("Receiver Operating Characteristic (ROC)")
+        plt.legend(loc="best")
+        plt.show()
+
+    if "precision_recall" in plots:
+        # Step 5: Plotting Precision-Recall Curve
+        precision, recall, thresholds_pr = precision_recall_curve(y_test, y_pred_prob)
+        average_precision = average_precision_score(y_test, y_pred_prob)
+        # Find the closest threshold to the selected one on the precision-recall curve
+        closest_threshold_index = np.argmin(np.abs(thresholds_pr - threshold))
+        operating_point_pr = (
+            recall[closest_threshold_index],
+            precision[closest_threshold_index],
+        )
+
+        plt.figure()
+        plt.step(
+            recall, precision, color="b", alpha=0.2, where="post", label="precision"
+        )
+        plt.fill_between(recall, precision, alpha=0.2, color="b", step="post")
+        plt.scatter(*operating_point_pr, color="red", label="Operating Point")
+        max_ind = min([len(recall), len(thresholds_pr)])
+        plt.plot(
+            recall[:max_ind],
+            thresholds_pr[:max_ind],
+            label="threshold (y ax)",
+            color="grey",
+            linestyle="--",
+        )
+        plt.xlabel("Recall")
+        plt.ylabel("Precision")
+        plt.ylim([0.0, 1.05])
+        plt.xlim([0.0, 1.0])
+        plt.title(f"Precision-Recall curve: AP={average_precision:.2f}")
+        plt.legend(loc="best")
+        plt.show()
+
+    if "lift" in plots:
+        lift = precision / precision[0]
+        operating_point_lift = (
+            recall[closest_threshold_index],
+            lift[closest_threshold_index],
+        )
+        plt.figure()
+        plt.plot(
+            recall,
+            lift,
+            color="k",
+        )
+        plt.scatter(*operating_point_lift, color="red", label="Operating Point")
+
+        plt.xlabel("Recall")
+        plt.ylabel("Lift")
+        plt.show()
```

### Comparing `easier-1.3.9/easier/gsheet.py` & `easier-1.4.0/easier/gsheet.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/hvtools.py` & `easier-1.4.0/easier/hvtools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/ibis_tools.py` & `easier-1.4.0/easier/ibis_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/item.py` & `easier-1.4.0/easier/item.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/iterify.py` & `easier-1.4.0/easier/iterify.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/minimodel.py` & `easier-1.4.0/easier/minimodel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/minimodel_orig.py` & `easier-1.4.0/easier/minimodel_orig.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/nice_dates.py` & `easier-1.4.0/easier/nice_dates.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/outlier_tools.py` & `easier-1.4.0/easier/outlier_tools.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/parallel.py` & `easier-1.4.0/easier/parallel.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/param_state.py` & `easier-1.4.0/easier/param_state.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/plotting.py` & `easier-1.4.0/easier/plotting.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/postgres.py` & `easier-1.4.0/easier/deleteme_postgres.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/print_catcher.py` & `easier-1.4.0/easier/print_catcher.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/proportion_lib.py` & `easier-1.4.0/easier/proportion_lib.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/salesforce.py` & `easier-1.4.0/easier/salesforce.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/shaper.py` & `easier-1.4.0/easier/shaper.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/timer.py` & `easier-1.4.0/easier/timer.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier/utils.py` & `easier-1.4.0/easier/utils.py`

 * *Files identical despite different names*

### Comparing `easier-1.3.9/easier.egg-info/SOURCES.txt` & `easier-1.4.0/easier.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 easier/api.py
 easier/bernstein.py
 easier/bigquery.py
 easier/cli.py
 easier/clock.py
 easier/crypt.py
 easier/dataframe_tools.py
+easier/deleteme_postgres.py
 easier/distributions.py
 easier/duck.py
 easier/duck_model.py
 easier/ecdf_lib.py
 easier/fit_lib.py
 easier/gsheet.py
 easier/hvtools.py
@@ -34,14 +35,15 @@
 easier/print_catcher.py
 easier/proportion_lib.py
 easier/salesforce.py
 easier/shaper.py
 easier/timer.py
 easier/utils.py
 easier/version.py
+easier/vonmises.py
 easier.egg-info/PKG-INFO
 easier.egg-info/SOURCES.txt
 easier.egg-info/dependency_links.txt
 easier.egg-info/entry_points.txt
 easier.egg-info/not-zip-safe
 easier.egg-info/requires.txt
 easier.egg-info/top_level.txt
```

### Comparing `easier-1.3.9/setup.py` & `easier-1.4.0/setup.py`

 * *Files identical despite different names*

