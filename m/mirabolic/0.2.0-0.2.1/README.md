# Comparing `tmp/mirabolic-0.2.0.tar.gz` & `tmp/mirabolic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirabolic-0.2.0.tar", last modified: Mon May 20 03:35:14 2024, max compression
+gzip compressed data, was "mirabolic-0.2.1.tar", last modified: Mon May 20 04:08:31 2024, max compression
```

## Comparing `mirabolic-0.2.0.tar` & `mirabolic-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.622767 mirabolic-0.2.0/
--rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.0/LICENSE
--rw-r--r--   0 wfbradley   (501) staff       (20)     8378 2024-05-20 03:35:14.622487 mirabolic-0.2.0/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)     7224 2024-05-20 03:23:54.000000 mirabolic-0.2.0/README.md
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.615403 mirabolic-0.2.0/mirabolic/
--rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.0/mirabolic/__init__.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.618300 mirabolic-0.2.0/mirabolic/cdf/
--rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.0/mirabolic/cdf/cdf_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.0/mirabolic/cdf/sample_usage.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.618801 mirabolic-0.2.0/mirabolic/cdf/unit_tests/
--rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.0/mirabolic/cdf/unit_tests/test_cdf_tools.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.621084 mirabolic-0.2.0/mirabolic/neural_glm/
--rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.0/mirabolic/neural_glm/__init__.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.0/mirabolic/neural_glm/actuarial_loss_functions.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.0/mirabolic/neural_glm/basic_glm_nn.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.0/mirabolic/neural_glm/generate_synthetic_data.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.0/mirabolic/neural_glm/run_examples.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.621388 mirabolic-0.2.0/mirabolic/rates/
--rw-r--r--   0 wfbradley   (501) staff       (20)     7955 2024-05-20 03:06:23.000000 mirabolic-0.2.0/mirabolic/rates/rate_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-20 03:26:46.000000 mirabolic-0.2.0/mirabolic/version
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 03:35:14.621933 mirabolic-0.2.0/mirabolic.egg-info/
--rw-r--r--   0 wfbradley   (501) staff       (20)     8378 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/SOURCES.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/dependency_links.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/requires.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-20 03:35:14.000000 mirabolic-0.2.0/mirabolic.egg-info/top_level.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-20 03:35:14.623476 mirabolic-0.2.0/setup.cfg
--rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.0/setup.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.263559 mirabolic-0.2.1/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.1/LICENSE
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 04:08:31.263347 mirabolic-0.2.1/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7202 2024-05-20 04:06:56.000000 mirabolic-0.2.1/README.md
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.257520 mirabolic-0.2.1/mirabolic/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.1/mirabolic/__init__.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.259770 mirabolic-0.2.1/mirabolic/cdf/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.1/mirabolic/cdf/cdf_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.1/mirabolic/cdf/sample_usage.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.260100 mirabolic-0.2.1/mirabolic/cdf/unit_tests/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.1/mirabolic/cdf/unit_tests/test_cdf_tools.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.262034 mirabolic-0.2.1/mirabolic/neural_glm/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.1/mirabolic/neural_glm/__init__.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.1/mirabolic/neural_glm/actuarial_loss_functions.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.1/mirabolic/neural_glm/basic_glm_nn.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.1/mirabolic/neural_glm/generate_synthetic_data.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.1/mirabolic/neural_glm/run_examples.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.262358 mirabolic-0.2.1/mirabolic/rates/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7955 2024-05-20 03:06:23.000000 mirabolic-0.2.1/mirabolic/rates/rate_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-20 04:07:44.000000 mirabolic-0.2.1/mirabolic/version
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.262796 mirabolic-0.2.1/mirabolic.egg-info/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/SOURCES.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/dependency_links.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/requires.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/top_level.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-20 04:08:31.264033 mirabolic-0.2.1/setup.cfg
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.1/setup.py
```

### Comparing `mirabolic-0.2.0/LICENSE` & `mirabolic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/PKG-INFO` & `mirabolic-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mirabolic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Statistical and Machine Learning tools from Mirabolic
 Home-page: https://github.com/Mirabolic/mirabolic
-Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.1.tar.gz
 Author: Bill Bradley
 License: MIT
 Keywords: Statistics,Machine Learning,CDF,Quantiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -38,15 +38,15 @@
 Suppose you run a website.  Every day you run a new email campaign to drive traffic to your site.  You're considering a new approach, so you A/B test your campaigns: a portion of your emails use the new style of campaign and the rest use the old style.
 
 Which style won?  The new campaign looks good, but how do you know it's not just a random fluke? You vaguely remember an old stats teacher saying something about designing experiments with sufficient statistical power for a target effect size, but you don't know what the effect size is going to be, and you've already run the experiment!  You really just want some simple way of visualizing the data you already have to see if the new style of campaigns are an improvement, or if it's all just random noise.
 
 We provide such a tool here:
 ```python
 import numpy as np
-from rate_tools import rate_comparison
+import mirabolic
 import matplotlib.pyplot as plt
 
 # Make some synthetic data
 num_campaigns = 8
 num_emails = 2000  # Number of emails in one arm of one campaign
 # In this example, the "B" arm has a slightly higher conversion rate
 num_conversions_A = np.random.binomial(num_emails, 0.03, size=num_campaigns)
```

### Comparing `mirabolic-0.2.0/README.md` & `mirabolic-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Suppose you run a website.  Every day you run a new email campaign to drive traffic to your site.  You're considering a new approach, so you A/B test your campaigns: a portion of your emails use the new style of campaign and the rest use the old style.
 
 Which style won?  The new campaign looks good, but how do you know it's not just a random fluke? You vaguely remember an old stats teacher saying something about designing experiments with sufficient statistical power for a target effect size, but you don't know what the effect size is going to be, and you've already run the experiment!  You really just want some simple way of visualizing the data you already have to see if the new style of campaigns are an improvement, or if it's all just random noise.
 
 We provide such a tool here:
 ```python
 import numpy as np
-from rate_tools import rate_comparison
+import mirabolic
 import matplotlib.pyplot as plt
 
 # Make some synthetic data
 num_campaigns = 8
 num_emails = 2000  # Number of emails in one arm of one campaign
 # In this example, the "B" arm has a slightly higher conversion rate
 num_conversions_A = np.random.binomial(num_emails, 0.03, size=num_campaigns)
```

### Comparing `mirabolic-0.2.0/mirabolic/cdf/cdf_tools.py` & `mirabolic-0.2.1/mirabolic/cdf/cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/cdf/sample_usage.py` & `mirabolic-0.2.1/mirabolic/cdf/sample_usage.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/cdf/unit_tests/test_cdf_tools.py` & `mirabolic-0.2.1/mirabolic/cdf/unit_tests/test_cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/neural_glm/actuarial_loss_functions.py` & `mirabolic-0.2.1/mirabolic/neural_glm/actuarial_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/neural_glm/basic_glm_nn.py` & `mirabolic-0.2.1/mirabolic/neural_glm/basic_glm_nn.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/neural_glm/generate_synthetic_data.py` & `mirabolic-0.2.1/mirabolic/neural_glm/generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/neural_glm/run_examples.py` & `mirabolic-0.2.1/mirabolic/neural_glm/run_examples.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic/rates/rate_tools.py` & `mirabolic-0.2.1/mirabolic/rates/rate_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/mirabolic.egg-info/PKG-INFO` & `mirabolic-0.2.1/mirabolic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mirabolic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Statistical and Machine Learning tools from Mirabolic
 Home-page: https://github.com/Mirabolic/mirabolic
-Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.1.tar.gz
 Author: Bill Bradley
 License: MIT
 Keywords: Statistics,Machine Learning,CDF,Quantiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -38,15 +38,15 @@
 Suppose you run a website.  Every day you run a new email campaign to drive traffic to your site.  You're considering a new approach, so you A/B test your campaigns: a portion of your emails use the new style of campaign and the rest use the old style.
 
 Which style won?  The new campaign looks good, but how do you know it's not just a random fluke? You vaguely remember an old stats teacher saying something about designing experiments with sufficient statistical power for a target effect size, but you don't know what the effect size is going to be, and you've already run the experiment!  You really just want some simple way of visualizing the data you already have to see if the new style of campaigns are an improvement, or if it's all just random noise.
 
 We provide such a tool here:
 ```python
 import numpy as np
-from rate_tools import rate_comparison
+import mirabolic
 import matplotlib.pyplot as plt
 
 # Make some synthetic data
 num_campaigns = 8
 num_emails = 2000  # Number of emails in one arm of one campaign
 # In this example, the "B" arm has a slightly higher conversion rate
 num_conversions_A = np.random.binomial(num_emails, 0.03, size=num_campaigns)
```

### Comparing `mirabolic-0.2.0/mirabolic.egg-info/SOURCES.txt` & `mirabolic-0.2.1/mirabolic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.0/setup.py` & `mirabolic-0.2.1/setup.py`

 * *Files identical despite different names*

