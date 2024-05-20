# Comparing `tmp/spade_anomaly_detection-0.2.1.tar.gz` & `tmp/spade_anomaly_detection-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade_anomaly_detection-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spade_anomaly_detection-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spade_anomaly_detection-0.2.1.tar` & `spade_anomaly_detection-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    30078 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/LICENSE
--rw-r--r--   0        0        0    14507 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/README.md
--rw-r--r--   0        0        0     2723 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1808 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/Dockerfile
--rw-r--r--   0        0        0     1384 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/__init__.py
--rw-r--r--   0        0        0    27516 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_loader.py
--rw-r--r--   0        0        0     1198 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/__init__.py
--rw-r--r--   0        0        0    30172 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset.py
--rw-r--r--   0        0        0     2055 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py
--rw-r--r--   0        0        0     4475 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_utils.py
--rw-r--r--   0        0        0    36573 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/feature_metadata.py
--rw-r--r--   0        0        0     1570 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/README.md
--rw-r--r--   0        0        0  3671818 2024-05-19 00:11:15.211628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_10000.csv
--rw-r--r--   0        0        0 36719403 2024-05-19 00:11:15.335627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_100000.csv
--rw-r--r--   0        0        0  3689614 2024-05-19 00:11:15.347627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pu_labeled.csv
--rw-r--r--   0        0        0   582290 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv
--rw-r--r--   0        0        0    42111 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/thyroid_labeled.csv
--rw-r--r--   0        0        0    11656 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/occ_ensemble.py
--rw-r--r--   0        0        0     9364 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/parameters.py
--rw-r--r--   0        0        0      746 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/requirements.txt
--rw-r--r--   0        0        0    23357 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/runner.py
--rwxr-xr-x   0        0        0     1146 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/build_and_push_image.sh
--rw-r--r--   0        0        0     3578 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh
--rw-r--r--   0        0        0     6333 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/supervised_model.py
--rw-r--r--   0        0        0    11178 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/task.py
--rw-r--r--   0        0        0    16300 1970-01-01 00:00:00.000000 spade_anomaly_detection-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    30078 2024-05-20 01:53:12.127968 spade_anomaly_detection-0.2.2/LICENSE
+-rw-r--r--   0        0        0    14507 2024-05-20 01:53:12.127968 spade_anomaly_detection-0.2.2/README.md
+-rw-r--r--   0        0        0     2723 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1808 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/Dockerfile
+-rw-r--r--   0        0        0     1384 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/__init__.py
+-rw-r--r--   0        0        0    27516 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_loader.py
+-rw-r--r--   0        0        0     1198 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/__init__.py
+-rw-r--r--   0        0        0    30172 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/bq_dataset.py
+-rw-r--r--   0        0        0     2055 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py
+-rw-r--r--   0        0        0     4475 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/bq_utils.py
+-rw-r--r--   0        0        0    36573 2024-05-20 01:53:12.131968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/feature_metadata.py
+-rw-r--r--   0        0        0     1570 2024-05-20 01:53:12.135968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/README.md
+-rw-r--r--   0        0        0  3671818 2024-05-20 01:53:12.147968 spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/covertype_pnu_10000.csv
+-rw-r--r--   0        0        0 36719403 2024-05-20 01:53:12.259969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/covertype_pnu_100000.csv
+-rw-r--r--   0        0        0  3689614 2024-05-20 01:53:12.275969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/covertype_pu_labeled.csv
+-rw-r--r--   0        0        0   582290 2024-05-20 01:53:12.275969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv
+-rw-r--r--   0        0        0    42111 2024-05-20 01:53:12.275969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/thyroid_labeled.csv
+-rw-r--r--   0        0        0    11656 2024-05-20 01:53:12.275969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/occ_ensemble.py
+-rw-r--r--   0        0        0     9364 2024-05-20 01:53:12.275969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/parameters.py
+-rw-r--r--   0        0        0      746 2024-05-20 01:53:12.279969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/requirements.txt
+-rw-r--r--   0        0        0    24260 2024-05-20 01:53:12.279969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/runner.py
+-rwxr-xr-x   0        0        0     1146 2024-05-20 01:53:12.279969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/scripts/build_and_push_image.sh
+-rw-r--r--   0        0        0     3578 2024-05-20 01:53:12.279969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh
+-rw-r--r--   0        0        0     6333 2024-05-20 01:53:12.279969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/supervised_model.py
+-rw-r--r--   0        0        0    11178 2024-05-20 01:53:12.279969 spade_anomaly_detection-0.2.2/spade_anomaly_detection/task.py
+-rw-r--r--   0        0        0    16300 1970-01-01 00:00:00.000000 spade_anomaly_detection-0.2.2/PKG-INFO
```

### Comparing `spade_anomaly_detection-0.2.1/LICENSE` & `spade_anomaly_detection-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/README.md` & `spade_anomaly_detection-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/pyproject.toml` & `spade_anomaly_detection-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/Dockerfile` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/Dockerfile`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/__init__.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """spade_anomaly_detection API."""
 
 # A new PyPI release will be pushed every time `__version__` is increased.
 # When changing this, also update the CHANGELOG.md.
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_loader.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_loader.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/__init__.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/bq_dataset.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_utils.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/bq_utils.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/feature_metadata.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/data_utils/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/README.md` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/README.md`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_10000.csv` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/covertype_pnu_10000.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_100000.csv` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/covertype_pnu_100000.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pu_labeled.csv` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/covertype_pu_labeled.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/thyroid_labeled.csv` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/example_data/thyroid_labeled.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/occ_ensemble.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/occ_ensemble.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/parameters.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/parameters.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/requirements.txt` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/requirements.txt`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/runner.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,39 @@
       )
       self.runner_parameters.negative_threshold = (
           input_table_statistics['negative_threshold']
           if self.runner_parameters.negative_threshold is None
           else self.runner_parameters.negative_threshold
       )
 
+  def _get_record_count_based_on_labels(self, label_value: int) -> int:
+    """Gets the number of records in the table.
+
+    Args:
+      label_value: The value of the label to use as the filter for records.
+
+    Returns:
+      The count of records.
+    """
+    label_record_count_filter = (
+        f'{self.runner_parameters.label_col_name} = {label_value}'
+    )
+    if self.runner_parameters.where_statements:
+      label_record_count_where_statements = [
+          self.runner_parameters.where_statements
+      ] + [label_record_count_filter]
+    else:
+      label_record_count_where_statements = [label_record_count_filter]
+
+    label_record_count = self.data_loader.get_query_record_result_length(
+        input_path=self.runner_parameters.input_bigquery_table_path,
+        where_statements=label_record_count_where_statements,
+    )
+    return label_record_count
+
   def check_data_tables(
       self,
       total_record_count: int,
       unlabeled_record_count: int,
   ) -> None:
     """Runs sanity checks on the table that is passed to this algorithm.
 
@@ -162,44 +187,50 @@
             'labeling_and_model_training_batch_size can not be greater than '
             f'the total number of examples. There are {total_record_count} '
             'examples and batch size is set to '
             f'{self.runner_parameters.labeling_and_model_training_batch_size}.'
         )
 
   def instantiate_and_fit_ensemble(
-      self, unlabeled_record_count: int
+      self, unlabeled_record_count: int, negative_record_count: int
   ) -> occ_ensemble.GmmEnsemble:
     """Creates and fits an OCC ensemble on the specified input data.
 
     Args:
       unlabeled_record_count: Number of unlabeled records in the table.
+      negative_record_count: Number of negative records in the table.
 
     Returns:
       A trained one class classifier ensemble.
     """
 
     ensemble_object = occ_ensemble.GmmEnsemble(
         ensemble_count=self.runner_parameters.ensemble_count,
         positive_threshold=self.runner_parameters.positive_threshold,
         negative_threshold=self.runner_parameters.negative_threshold,
     )
 
-    records_per_occ = unlabeled_record_count // ensemble_object.ensemble_count
+    training_record_count = unlabeled_record_count + negative_record_count
+    records_per_occ = training_record_count // ensemble_object.ensemble_count
     batch_size = records_per_occ // self.runner_parameters.batches_per_model
     batch_size = np.min([batch_size, self.runner_parameters.max_occ_batch_size])
 
     logging.info('Batch size for OCC ensemble: %s', batch_size)
 
     unlabeled_data = self.data_loader.load_tf_dataset_from_bigquery(
         input_path=self.runner_parameters.input_bigquery_table_path,
         label_col_name=self.runner_parameters.label_col_name,
         where_statements=self.runner_parameters.where_statements,
         ignore_columns=self.runner_parameters.ignore_columns,
         batch_size=batch_size,
-        label_column_filter_value=self.runner_parameters.unlabeled_data_value,
+        # Train using negative labeled data and unlabeled data.
+        label_column_filter_value=[
+            self.runner_parameters.unlabeled_data_value,
+            self.runner_parameters.negative_data_value,
+        ],
     )
 
     logging.info('Fitting ensemble.')
     ensemble_object.fit(
         train_x=unlabeled_data,
         batches_per_occ=self.runner_parameters.batches_per_model,
     )
@@ -523,37 +554,29 @@
     self._check_runner_parameters()
 
     total_record_count = self.data_loader.get_query_record_result_length(
         input_path=self.runner_parameters.input_bigquery_table_path,
         where_statements=self.runner_parameters.where_statements,
     )
 
-    unlabeled_record_count_filter = (
-        f'{self.runner_parameters.label_col_name} = '
-        f'{self.runner_parameters.unlabeled_data_value}'
+    unlabeled_record_count = self._get_record_count_based_on_labels(
+        self.runner_parameters.unlabeled_data_value
     )
-    if self.runner_parameters.where_statements:
-      unlabeled_record_count_where_statements = [
-          self.runner_parameters.where_statements
-      ] + [unlabeled_record_count_filter]
-    else:
-      unlabeled_record_count_where_statements = [unlabeled_record_count_filter]
-
-    unlabeled_record_count = self.data_loader.get_query_record_result_length(
-        input_path=self.runner_parameters.input_bigquery_table_path,
-        where_statements=unlabeled_record_count_where_statements,
+    negative_record_count = self._get_record_count_based_on_labels(
+        self.runner_parameters.negative_data_value
     )
 
     self.check_data_tables(
         total_record_count=total_record_count,
         unlabeled_record_count=unlabeled_record_count,
     )
 
     ensemble_object = self.instantiate_and_fit_ensemble(
-        unlabeled_record_count=unlabeled_record_count
+        unlabeled_record_count=unlabeled_record_count,
+        negative_record_count=negative_record_count,
     )
 
     batch_size = (
         self.runner_parameters.labeling_and_model_training_batch_size
         or total_record_count
     )
     tf_dataset = self.data_loader.load_tf_dataset_from_bigquery(
@@ -611,14 +634,15 @@
         self.train_supervised_model(
             features=updated_features,
             labels=updated_labels,
             weights=weights,
         )
 
     if not self.runner_parameters.upload_only:
+      if self.supervised_model_object is None:
+        raise ValueError('Supervised model was not created and trained.')
       self.evaluate_model()
-      if self.supervised_model_object is not None:
-        self.supervised_model_object.save(
-            save_location=self.runner_parameters.output_gcs_uri
-        )
+      self.supervised_model_object.save(
+          save_location=self.runner_parameters.output_gcs_uri
+      )
 
     logging.info('SPADE training completed.')
```

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/build_and_push_image.sh` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/scripts/build_and_push_image.sh`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/supervised_model.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/supervised_model.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/spade_anomaly_detection/task.py` & `spade_anomaly_detection-0.2.2/spade_anomaly_detection/task.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.1/PKG-INFO` & `spade_anomaly_detection-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spade_anomaly_detection
-Version: 0.2.1
+Version: 0.2.2
 Summary: Semi-supervised Pseudo Labeler Anomaly Detection with Ensembling (SPADE) is a semi-supervised anomaly detection method that uses an ensemble of one class classifiers as the pseudo-labelers and supervised classifiers to achieve state of the art results especially on datasets with distribution mismatch between labeled and unlabeled samples.
 Keywords: anomaly detection,ensemble model,one class classifiers
 Author-email: spade_anomaly_detection authors <spade_anomaly_detection@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
```

