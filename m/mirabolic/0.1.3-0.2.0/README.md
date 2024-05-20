# Comparing `tmp/mirabolic-0.1.3.tar.gz` & `tmp/mirabolic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirabolic-0.1.3.tar", last modified: Sun Jan  1 19:48:04 2023, max compression
+gzip compressed data, was "mirabolic-0.2.0.tar", last modified: Mon May 20 03:35:14 2024, max compression
```

## Comparing `mirabolic-0.1.3.tar` & `mirabolic-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2023-01-01 19:48:04.657259 mirabolic-0.1.3/
--rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.1.3/LICENSE
--rw-r--r--   0 wfbradley   (501) staff       (20)     6035 2023-01-01 19:48:04.657373 mirabolic-0.1.3/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)     5044 2023-01-01 19:46:02.000000 mirabolic-0.1.3/README.md
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2023-01-01 19:48:04.653170 mirabolic-0.1.3/mirabolic/
--rw-r--r--   0 wfbradley   (501) staff       (20)      287 2023-01-01 19:46:02.000000 mirabolic-0.1.3/mirabolic/__init__.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2023-01-01 19:48:04.655112 mirabolic-0.1.3/mirabolic/cdf/
--rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.1.3/mirabolic/cdf/cdf_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.1.3/mirabolic/cdf/sample_usage.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2023-01-01 19:48:04.655411 mirabolic-0.1.3/mirabolic/cdf/unit_tests/
--rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.1.3/mirabolic/cdf/unit_tests/test_cdf_tools.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2023-01-01 19:48:04.657000 mirabolic-0.1.3/mirabolic/neural_glm/
--rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.1.3/mirabolic/neural_glm/__init__.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.1.3/mirabolic/neural_glm/actuarial_loss_functions.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.1.3/mirabolic/neural_glm/basic_glm_nn.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.1.3/mirabolic/neural_glm/generate_synthetic_data.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.1.3/mirabolic/neural_glm/run_examples.py
--rw-r--r--   0 wfbradley   (501) staff       (20)        6 2023-01-01 19:47:19.000000 mirabolic-0.1.3/mirabolic/version
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2023-01-01 19:48:04.654533 mirabolic-0.1.3/mirabolic.egg-info/
--rw-r--r--   0 wfbradley   (501) staff       (20)     6035 2023-01-01 19:48:04.000000 mirabolic-0.1.3/mirabolic.egg-info/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)      544 2023-01-01 19:48:04.000000 mirabolic-0.1.3/mirabolic.egg-info/SOURCES.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)        1 2023-01-01 19:48:04.000000 mirabolic-0.1.3/mirabolic.egg-info/dependency_links.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       93 2023-01-01 19:48:04.000000 mirabolic-0.1.3/mirabolic.egg-info/requires.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       15 2023-01-01 19:48:04.000000 mirabolic-0.1.3/mirabolic.egg-info/top_level.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)      103 2023-01-01 19:48:04.657786 mirabolic-0.1.3/setup.cfg
--rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.1.3/setup.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.622767 mirabolic-0.2.0/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.0/LICENSE
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8378 2024-05-20 03:35:14.622487 mirabolic-0.2.0/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7224 2024-05-20 03:23:54.000000 mirabolic-0.2.0/README.md
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.615403 mirabolic-0.2.0/mirabolic/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.0/mirabolic/__init__.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.618300 mirabolic-0.2.0/mirabolic/cdf/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.0/mirabolic/cdf/cdf_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.0/mirabolic/cdf/sample_usage.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.618801 mirabolic-0.2.0/mirabolic/cdf/unit_tests/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.0/mirabolic/cdf/unit_tests/test_cdf_tools.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.621084 mirabolic-0.2.0/mirabolic/neural_glm/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.0/mirabolic/neural_glm/__init__.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.0/mirabolic/neural_glm/actuarial_loss_functions.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.0/mirabolic/neural_glm/basic_glm_nn.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.0/mirabolic/neural_glm/generate_synthetic_data.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.0/mirabolic/neural_glm/run_examples.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.621388 mirabolic-0.2.0/mirabolic/rates/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7955 2024-05-20 03:06:23.000000 mirabolic-0.2.0/mirabolic/rates/rate_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-20 03:26:46.000000 mirabolic-0.2.0/mirabolic/version
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.621933 mirabolic-0.2.0/mirabolic.egg-info/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8378 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/SOURCES.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/dependency_links.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/requires.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/top_level.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-20 03:35:14.623476 mirabolic-0.2.0/setup.cfg
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.0/setup.py
```

### Comparing `mirabolic-0.1.3/LICENSE` & `mirabolic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/cdf/cdf_tools.py` & `mirabolic-0.2.0/mirabolic/cdf/cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/cdf/sample_usage.py` & `mirabolic-0.2.0/mirabolic/cdf/sample_usage.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/cdf/unit_tests/test_cdf_tools.py` & `mirabolic-0.2.0/mirabolic/cdf/unit_tests/test_cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/neural_glm/actuarial_loss_functions.py` & `mirabolic-0.2.0/mirabolic/neural_glm/actuarial_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/neural_glm/basic_glm_nn.py` & `mirabolic-0.2.0/mirabolic/neural_glm/basic_glm_nn.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/neural_glm/generate_synthetic_data.py` & `mirabolic-0.2.0/mirabolic/neural_glm/generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic/neural_glm/run_examples.py` & `mirabolic-0.2.0/mirabolic/neural_glm/run_examples.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.1.3/mirabolic.egg-info/SOURCES.txt` & `mirabolic-0.2.0/mirabolic.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 mirabolic/cdf/cdf_tools.py
 mirabolic/cdf/sample_usage.py
 mirabolic/cdf/unit_tests/test_cdf_tools.py
 mirabolic/neural_glm/__init__.py
 mirabolic/neural_glm/actuarial_loss_functions.py
 mirabolic/neural_glm/basic_glm_nn.py
 mirabolic/neural_glm/generate_synthetic_data.py
-mirabolic/neural_glm/run_examples.py
+mirabolic/neural_glm/run_examples.py
+mirabolic/rates/rate_tools.py
```

### Comparing `mirabolic-0.1.3/setup.py` & `mirabolic-0.2.0/setup.py`

 * *Files identical despite different names*

