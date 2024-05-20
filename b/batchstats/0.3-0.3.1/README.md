# Comparing `tmp/batchstats-0.3.tar.gz` & `tmp/batchstats-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchstats-0.3.tar", last modified: Mon May 13 22:08:59 2024, max compression
+gzip compressed data, was "batchstats-0.3.1.tar", last modified: Mon May 20 13:36:16 2024, max compression
```

## Comparing `batchstats-0.3.tar` & `batchstats-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.930142 batchstats-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 22:08:48.000000 batchstats-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-13 22:08:59.930142 batchstats-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-13 22:08:48.000000 batchstats-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.926142 batchstats-0.3/batchstats/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/nanstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-05-13 22:08:48.000000 batchstats-0.3/batchstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.930142 batchstats-0.3/batchstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 22:08:59.000000 batchstats-0.3/batchstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:08:59.930142 batchstats-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-13 22:08:48.000000 batchstats-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:08:59.926142 batchstats-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-13 22:08:48.000000 batchstats-0.3/tests/test_nanstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-13 22:08:48.000000 batchstats-0.3/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:36:16.036875 batchstats-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 13:36:04.000000 batchstats-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-20 13:36:16.036875 batchstats-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-20 13:36:04.000000 batchstats-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:36:16.032875 batchstats-0.3.1/batchstats/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 13:36:04.000000 batchstats-0.3.1/batchstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-20 13:36:04.000000 batchstats-0.3.1/batchstats/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-20 13:36:04.000000 batchstats-0.3.1/batchstats/nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-05-20 13:36:04.000000 batchstats-0.3.1/batchstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:36:16.036875 batchstats-0.3.1/batchstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-20 13:36:15.000000 batchstats-0.3.1/batchstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 13:36:16.000000 batchstats-0.3.1/batchstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:36:15.000000 batchstats-0.3.1/batchstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:36:15.000000 batchstats-0.3.1/batchstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 13:36:15.000000 batchstats-0.3.1/batchstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:36:16.036875 batchstats-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 13:36:04.000000 batchstats-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:36:16.036875 batchstats-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-20 13:36:04.000000 batchstats-0.3.1/tests/test_nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-20 13:36:04.000000 batchstats-0.3.1/tests/test_stats.py
```

### Comparing `batchstats-0.3/LICENSE` & `batchstats-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `batchstats-0.3/PKG-INFO` & `batchstats-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.3
+Version: 0.3.1
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `batchstats-0.3/README.md` & `batchstats-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `batchstats-0.3/batchstats/_misc.py` & `batchstats-0.3.1/batchstats/_misc.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3/batchstats/nanstats.py` & `batchstats-0.3.1/batchstats/nanstats.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3/batchstats/stats.py` & `batchstats-0.3.1/batchstats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import string
 
 import numpy as np
 
-from ._misc import NoValidSamplesError, UnequalSamplesNumber, any_nan, check_params
+from ._misc import (NoValidSamplesError, UnequalSamplesNumber, any_nan,
+                    check_params)
 
 
 class BatchStat:
     """
     Base class for calculating statistics over batches of data.
 
     Attributes:
@@ -235,14 +236,54 @@
         """
         if self.mean is None:
             raise NoValidSamplesError("No valid samples for calculating mean.")
         else:
             return self.mean.copy()
 
 
+class BatchPeakToPeak(BatchStat):
+    """
+    Class for calculating the peak-to-peak (max - min) of batches of data.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.batchmax = BatchMax()
+        self.batchmin = BatchMin()
+
+    def update_batch(self, batch, assume_valid=False):
+        """
+        Update the peak-to-peak with a new batch of data.
+
+        Args:
+            batch (numpy.ndarray): Input batch.
+            assume_valid (bool, optional): If True, assumes all elements in the batch are valid. Default is False.
+
+        Returns:
+            BatchPeakToPeak: Updated BatchPeakToPeak object.
+
+        """
+        self.batchmax.update_batch(batch, assume_valid=assume_valid)
+        self.batchmin.update_batch(batch, assume_valid=assume_valid)
+        return self
+
+    def __call__(self) -> np.ndarray:
+        """
+        Calculate the peak-to-peak.
+
+        Returns:
+            numpy.ndarray: Peak-to-peak of the batches.
+
+        Raises:
+            NoValidSamplesError: If no valid samples are available.
+
+        """
+        return self.batchmax() - self.batchmin()
+
+
 class BatchVar(BatchMean):
     """
     Class for calculating the variance of batches of data.
 
     Args:
         ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
     """
```

### Comparing `batchstats-0.3/batchstats.egg-info/PKG-INFO` & `batchstats-0.3.1/batchstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.3
+Version: 0.3.1
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `batchstats-0.3/setup.py` & `batchstats-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3/tests/test_nanstats.py` & `batchstats-0.3.1/tests/test_nanstats.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3/tests/test_stats.py` & `batchstats-0.3.1/tests/test_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pytest
 
-from batchstats import BatchCov, BatchMax, BatchMean, BatchMin, BatchSum, BatchVar
+from batchstats import (BatchCov, BatchMax, BatchMean, BatchMin,
+                        BatchPeakToPeak, BatchSum, BatchVar)
 
 
 @pytest.fixture
 def data():
     m, n = 1_000_000, 50
     return np.random.randn(m, n)
 
@@ -47,14 +48,24 @@
     batchmean = BatchMean()
     for batch_data in np.array_split(data, n_batches):
         batchmean.update_batch(batch=batch_data)
     batch_stat = batchmean()
     assert np.allclose(true_stat, batch_stat)
 
 
+def test_ptp(data, n_batches):
+    true_stat = np.ptp(data, axis=0)
+
+    batchptp = BatchPeakToPeak()
+    for batch_data in np.array_split(data, n_batches):
+        batchptp.update_batch(batch=batch_data)
+    batch_stat = batchptp()
+    assert np.allclose(true_stat, batch_stat)
+
+
 def test_sum(data, n_batches):
     true_stat = np.sum(data, axis=0)
 
     batchsum = BatchSum()
     for batch_data in np.array_split(data, n_batches):
         batchsum.update_batch(batch=batch_data)
     batch_stat = batchsum()
```

