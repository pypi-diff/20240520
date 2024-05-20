# Comparing `tmp/mirabolic-0.2.1.tar.gz` & `tmp/mirabolic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirabolic-0.2.1.tar", last modified: Mon May 20 04:08:31 2024, max compression
+gzip compressed data, was "mirabolic-0.2.2.tar", last modified: Mon May 20 04:16:42 2024, max compression
```

## Comparing `mirabolic-0.2.1.tar` & `mirabolic-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.263559 mirabolic-0.2.1/
--rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.1/LICENSE
--rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 04:08:31.263347 mirabolic-0.2.1/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)     7202 2024-05-20 04:06:56.000000 mirabolic-0.2.1/README.md
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.257520 mirabolic-0.2.1/mirabolic/
--rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.1/mirabolic/__init__.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.259770 mirabolic-0.2.1/mirabolic/cdf/
--rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.1/mirabolic/cdf/cdf_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.1/mirabolic/cdf/sample_usage.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.260100 mirabolic-0.2.1/mirabolic/cdf/unit_tests/
--rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.1/mirabolic/cdf/unit_tests/test_cdf_tools.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.262034 mirabolic-0.2.1/mirabolic/neural_glm/
--rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.1/mirabolic/neural_glm/__init__.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.1/mirabolic/neural_glm/actuarial_loss_functions.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.1/mirabolic/neural_glm/basic_glm_nn.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.1/mirabolic/neural_glm/generate_synthetic_data.py
--rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.1/mirabolic/neural_glm/run_examples.py
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.262358 mirabolic-0.2.1/mirabolic/rates/
--rw-r--r--   0 wfbradley   (501) staff       (20)     7955 2024-05-20 03:06:23.000000 mirabolic-0.2.1/mirabolic/rates/rate_tools.py
--rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-20 04:07:44.000000 mirabolic-0.2.1/mirabolic/version
-drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:08:31.262796 mirabolic-0.2.1/mirabolic.egg-info/
--rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/PKG-INFO
--rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/SOURCES.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/dependency_links.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/requires.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-20 04:08:31.000000 mirabolic-0.2.1/mirabolic.egg-info/top_level.txt
--rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-20 04:08:31.264033 mirabolic-0.2.1/setup.cfg
--rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.1/setup.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.265962 mirabolic-0.2.2/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1066 2022-12-13 21:29:13.000000 mirabolic-0.2.2/LICENSE
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 04:16:42.265754 mirabolic-0.2.2/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)     7202 2024-05-20 04:06:56.000000 mirabolic-0.2.2/README.md
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.257548 mirabolic-0.2.2/mirabolic/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      342 2024-05-17 13:21:46.000000 mirabolic-0.2.2/mirabolic/__init__.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.260940 mirabolic-0.2.2/mirabolic/cdf/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     9850 2022-12-31 14:49:14.000000 mirabolic-0.2.2/mirabolic/cdf/cdf_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     1923 2023-01-01 19:46:02.000000 mirabolic-0.2.2/mirabolic/cdf/sample_usage.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.261459 mirabolic-0.2.2/mirabolic/cdf/unit_tests/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     5054 2022-12-30 20:05:39.000000 mirabolic-0.2.2/mirabolic/cdf/unit_tests/test_cdf_tools.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.264499 mirabolic-0.2.2/mirabolic/neural_glm/
+-rw-r--r--   0 wfbradley   (501) staff       (20)      313 2023-01-01 19:46:02.000000 mirabolic-0.2.2/mirabolic/neural_glm/__init__.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8469 2022-12-13 21:29:13.000000 mirabolic-0.2.2/mirabolic/neural_glm/actuarial_loss_functions.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4785 2023-01-01 19:46:02.000000 mirabolic-0.2.2/mirabolic/neural_glm/basic_glm_nn.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     4299 2022-12-13 21:29:13.000000 mirabolic-0.2.2/mirabolic/neural_glm/generate_synthetic_data.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2183 2022-12-13 21:29:13.000000 mirabolic-0.2.2/mirabolic/neural_glm/run_examples.py
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.264806 mirabolic-0.2.2/mirabolic/rates/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8010 2024-05-20 04:14:22.000000 mirabolic-0.2.2/mirabolic/rates/rate_tools.py
+-rw-r--r--   0 wfbradley   (501) staff       (20)        6 2024-05-20 04:16:07.000000 mirabolic-0.2.2/mirabolic/version
+drwxr-xr-x   0 wfbradley   (501) staff       (20)        0 2024-05-20 04:16:42.265236 mirabolic-0.2.2/mirabolic.egg-info/
+-rw-r--r--   0 wfbradley   (501) staff       (20)     8356 2024-05-20 04:16:42.000000 mirabolic-0.2.2/mirabolic.egg-info/PKG-INFO
+-rw-r--r--   0 wfbradley   (501) staff       (20)      574 2024-05-20 04:16:42.000000 mirabolic-0.2.2/mirabolic.egg-info/SOURCES.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)        1 2024-05-20 04:16:42.000000 mirabolic-0.2.2/mirabolic.egg-info/dependency_links.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       93 2024-05-20 04:16:42.000000 mirabolic-0.2.2/mirabolic.egg-info/requires.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)       10 2024-05-20 04:16:42.000000 mirabolic-0.2.2/mirabolic.egg-info/top_level.txt
+-rw-r--r--   0 wfbradley   (501) staff       (20)      103 2024-05-20 04:16:42.266642 mirabolic-0.2.2/setup.cfg
+-rw-r--r--   0 wfbradley   (501) staff       (20)     2190 2022-12-31 16:39:50.000000 mirabolic-0.2.2/setup.py
```

### Comparing `mirabolic-0.2.1/LICENSE` & `mirabolic-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/PKG-INFO` & `mirabolic-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mirabolic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Statistical and Machine Learning tools from Mirabolic
 Home-page: https://github.com/Mirabolic/mirabolic
-Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.2.tar.gz
 Author: Bill Bradley
 License: MIT
 Keywords: Statistics,Machine Learning,CDF,Quantiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `mirabolic-0.2.1/README.md` & `mirabolic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/cdf/cdf_tools.py` & `mirabolic-0.2.2/mirabolic/cdf/cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/cdf/sample_usage.py` & `mirabolic-0.2.2/mirabolic/cdf/sample_usage.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/cdf/unit_tests/test_cdf_tools.py` & `mirabolic-0.2.2/mirabolic/cdf/unit_tests/test_cdf_tools.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/neural_glm/actuarial_loss_functions.py` & `mirabolic-0.2.2/mirabolic/neural_glm/actuarial_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/neural_glm/basic_glm_nn.py` & `mirabolic-0.2.2/mirabolic/neural_glm/basic_glm_nn.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/neural_glm/generate_synthetic_data.py` & `mirabolic-0.2.2/mirabolic/neural_glm/generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/neural_glm/run_examples.py` & `mirabolic-0.2.2/mirabolic/neural_glm/run_examples.py`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/mirabolic/rates/rate_tools.py` & `mirabolic-0.2.2/mirabolic/rates/rate_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     df=None,
     ax=None,
     plot_kwargs=None,
     plot=True,
     patch_type="rectangle",
     patch_alpha=0.3,
     label_font_size=8,
+    xlabel="A arm",
+    ylabel="B arm",
+    title="Response Rate Correlation",
 ):
     """
     We run a series of A/B experiments.  In each experiment, we run a number of trials of
     the A arm and the B arm, recording the number of successes.  We're trying to estimate
     the probability that each arm succeeds.  The probability may differ between different
     experiments.
 
@@ -196,17 +199,17 @@
                         markersize=label_font_size,
                     )
                 )
                 legend_label.append(labels[i])
         if labels is not None:
             plt.legend(legend_proxy, legend_label, prop={"size": label_font_size})
 
-        plt.xlabel("A arm")
-        plt.ylabel("B arm")
-        plt.title("Response Rate Correlation")
+        plt.xlabel(xlabel)
+        plt.ylabel(ylabel)
+        plt.title(title)
         plt.scatter(
             results["A"]["rate"], results["B"]["rate"], marker=".", color="black"
         )
         ax.set_aspect("equal")
 
     return results
```

### Comparing `mirabolic-0.2.1/mirabolic.egg-info/PKG-INFO` & `mirabolic-0.2.2/mirabolic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mirabolic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Statistical and Machine Learning tools from Mirabolic
 Home-page: https://github.com/Mirabolic/mirabolic
-Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.1.tar.gz
+Download-URL: https://github.com/Mirabolic/mirabolic/archive/refs/tags/v0.2.2.tar.gz
 Author: Bill Bradley
 License: MIT
 Keywords: Statistics,Machine Learning,CDF,Quantiles
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `mirabolic-0.2.1/mirabolic.egg-info/SOURCES.txt` & `mirabolic-0.2.2/mirabolic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mirabolic-0.2.1/setup.py` & `mirabolic-0.2.2/setup.py`

 * *Files identical despite different names*

