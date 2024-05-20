# Comparing `tmp/autora_experiment_runner_firebase_prolific-1.0.0b3.tar.gz` & `tmp/autora_experiment_runner_firebase_prolific-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b3.tar", last modified: Mon May 20 02:03:10 2024, max compression
+gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b4.tar", last modified: Mon May 20 02:09:21 2024, max compression
```

## Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3.tar` & `autora_experiment_runner_firebase_prolific-1.0.0b4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.240894 autora_experiment_runner_firebase_prolific-1.0.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.232895 autora_experiment_runner_firebase_prolific-1.0.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:03:10.240894 autora_experiment_runner_firebase_prolific-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:03:10.240894 autora_experiment_runner_firebase_prolific-1.0.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.232895 autora_experiment_runner_firebase_prolific-1.0.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.232895 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.232895 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora/experiment_runner/firebase_prolific/
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora/experiment_runner/firebase_prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:03:10.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 02:03:10.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:03:10.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:03:10.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:03:10.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:10.236894 autora_experiment_runner_firebase_prolific-1.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:05.000000 autora_experiment_runner_firebase_prolific-1.0.0b3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/firebase_prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/firebase_prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/tests/__init__.py
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/.github/workflows/python-publish.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/.gitignore` & `autora_experiment_runner_firebase_prolific-1.0.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/.pre-commit-config.yaml` & `autora_experiment_runner_firebase_prolific-1.0.0b4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/LICENSE` & `autora_experiment_runner_firebase_prolific-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/mkdocs/base.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/pyproject.toml` & `autora_experiment_runner_firebase_prolific-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora/experiment_runner/firebase_prolific/__init__.py` & `autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/firebase_prolific/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from autora.experiment_runner.recruitment_manager.prolific import (
     check_prolific_status,
     pause_study,
     setup_study,
     start_study,
     publish_study,
     get_submissions_incompleted,
-    request_return_all
+    request_return_all,
     approve_all_no_code
 )
 
 
 def _firebase_run(conditions, **kwargs):
     """
     Running an experiment with firebase to host the experiment and store the data.
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b3/tests/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b4/tests/README.md`

 * *Files identical despite different names*

