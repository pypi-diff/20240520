# Comparing `tmp/onion_clustering-0.2.4.tar.gz` & `tmp/onion_clustering-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.2.4.tar", last modified: Thu May 16 12:45:20 2024, max compression
+gzip compressed data, was "onion_clustering-0.2.5.tar", last modified: Mon May 20 13:18:12 2024, max compression
```

## Comparing `onion_clustering-0.2.4.tar` & `onion_clustering-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.403943 onion_clustering-0.2.4/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-16 12:44:30.000000 onion_clustering-0.2.4/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.4/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-16 12:45:20.403065 onion_clustering-0.2.4/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5465 2024-05-15 12:29:23.000000 onion_clustering-0.2.4/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.390815 onion_clustering-0.2.4/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3647 2024-05-16 08:42:26.000000 onion_clustering-0.2.4/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3637 2024-05-16 08:15:24.000000 onion_clustering-0.2.4/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-16 12:44:50.000000 onion_clustering-0.2.4/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.4/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-16 12:45:20.404119 onion_clustering-0.2.4/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.385793 onion_clustering-0.2.4/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.393908 onion_clustering-0.2.4/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-10 14:39:49.000000 onion_clustering-0.2.4/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    20386 2024-05-15 12:08:37.000000 onion_clustering-0.2.4/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    30001 2024-05-16 12:40:18.000000 onion_clustering-0.2.4/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    26441 2024-05-16 09:15:31.000000 onion_clustering-0.2.4/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    20729 2024-05-15 12:08:37.000000 onion_clustering-0.2.4/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-08 09:25:50.000000 onion_clustering-0.2.4/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.402034 onion_clustering-0.2.4/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-16 12:45:20.000000 onion_clustering-0.2.4/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.397534 onion_clustering-0.2.4/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.4/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.399721 onion_clustering-0.2.4/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      412 2024-05-15 12:16:50.000000 onion_clustering-0.2.4/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-15 12:16:38.000000 onion_clustering-0.2.4/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-15 12:16:38.000000 onion_clustering-0.2.4/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-16 12:45:20.401384 onion_clustering-0.2.4/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1662 2024-05-14 13:55:06.000000 onion_clustering-0.2.4/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-14 13:55:01.000000 onion_clustering-0.2.4/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-14 13:55:01.000000 onion_clustering-0.2.4/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3112 2024-05-15 12:18:40.000000 onion_clustering-0.2.4/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-14 13:56:18.000000 onion_clustering-0.2.4/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.018379 onion_clustering-0.2.5/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-20 12:56:22.000000 onion_clustering-0.2.5/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.5/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-20 13:18:12.017837 onion_clustering-0.2.5/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5465 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.000934 onion_clustering-0.2.5/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3647 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3637 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-20 13:17:00.000000 onion_clustering-0.2.5/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.5/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-20 13:18:12.018501 onion_clustering-0.2.5/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:11.994341 onion_clustering-0.2.5/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.007919 onion_clustering-0.2.5/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    20386 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    30001 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    26453 2024-05-20 12:51:45.000000 onion_clustering-0.2.5/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    20729 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-17 12:50:03.000000 onion_clustering-0.2.5/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.017125 onion_clustering-0.2.5/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.012047 onion_clustering-0.2.5/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.5/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.014143 onion_clustering-0.2.5/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      412 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.016286 onion_clustering-0.2.5/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1662 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3112 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/test_uni.py
```

### Comparing `onion_clustering-0.2.4/.coverage` & `onion_clustering-0.2.5/.coverage`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/LICENSE` & `onion_clustering-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/PKG-INFO` & `onion_clustering-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.4
+Version: 0.2.5
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.4/README.md` & `onion_clustering-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/examples/example_script.py` & `onion_clustering-0.2.5/examples/example_script.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/examples/example_script_2d.py` & `onion_clustering-0.2.5/examples/example_script_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/justfile` & `onion_clustering-0.2.5/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/pyproject.toml` & `onion_clustering-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.2.4"
+version = "0.2.5"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.2.4/src/onion_clustering/classes.py` & `onion_clustering-0.2.5/src/onion_clustering/classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/src/onion_clustering/first_classes.py` & `onion_clustering-0.2.5/src/onion_clustering/first_classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/src/onion_clustering/functions.py` & `onion_clustering-0.2.5/src/onion_clustering/functions.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/src/onion_clustering/main.py` & `onion_clustering-0.2.5/src/onion_clustering/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,22 +301,22 @@
             f"sigma = {state.sigma:.4f} ({perr[1]:.4f}), "
             f"area = {state.area:.4f} ({perr[2]:.4f})",
             file=file,
         )
         print(f"\tFit r2 = {r_2}", file=file)
 
     if full_out:
-        ### Plot the distribution and the fitted gaussians
+        ### 9. Plot the distribution and the fitted gaussians ###
         y_spread = np.max(m_clean) - np.min(m_clean)
         y_lim = [
             np.min(m_clean) - 0.025 * y_spread,
             np.max(m_clean) + 0.025 * y_spread,
         ]
         fig, axes = plt.subplots()
-        plot_histo(axes, counts, bins)
+        plot_histo(axes, counts[:-1], bins)
         axes.set_xlim(y_lim)
         tmp_popt = [state.mean, state.sigma, state.area / flat_m.size]
         axes.plot(
             np.linspace(bins[0], bins[-1], 1000),
             gaussian(np.linspace(bins[0], bins[-1], 1000), *tmp_popt),
         )
```

### Comparing `onion_clustering-0.2.4/src/onion_clustering/main_2d.py` & `onion_clustering-0.2.5/src/onion_clustering/main_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/src/onion_clustering/utilities.py` & `onion_clustering-0.2.5/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.2.5/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.4
+Version: 0.2.5
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.4/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.2.5/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/test/output_uni/final_states.txt` & `onion_clustering-0.2.5/test/output_uni/final_states.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/test/test_multi.py` & `onion_clustering-0.2.5/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.4/test/test_uni.py` & `onion_clustering-0.2.5/test/test_uni.py`

 * *Files identical despite different names*

