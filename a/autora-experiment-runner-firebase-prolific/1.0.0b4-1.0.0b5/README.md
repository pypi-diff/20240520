# Comparing `tmp/autora_experiment_runner_firebase_prolific-1.0.0b4.tar.gz` & `tmp/autora_experiment_runner_firebase_prolific-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b4.tar", last modified: Mon May 20 02:09:21 2024, max compression
+gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b5.tar", last modified: Mon May 20 02:11:00 2024, max compression
```

## Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4.tar` & `autora_experiment_runner_firebase_prolific-1.0.0b5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.825561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/firebase_prolific/
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/firebase_prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:09:21.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:21.829561 autora_experiment_runner_firebase_prolific-1.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:09:12.000000 autora_experiment_runner_firebase_prolific-1.0.0b4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/firebase_prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/firebase_prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/tests/__init__.py
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/.github/workflows/python-publish.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/.gitignore` & `autora_experiment_runner_firebase_prolific-1.0.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/.pre-commit-config.yaml` & `autora_experiment_runner_firebase_prolific-1.0.0b5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/LICENSE` & `autora_experiment_runner_firebase_prolific-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/mkdocs/base.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/pyproject.toml` & `autora_experiment_runner_firebase_prolific-1.0.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora/experiment_runner/firebase_prolific/__init__.py` & `autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/firebase_prolific/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     prolific_dict = setup_study(
         kwargs["study_name"],
         kwargs["study_description"],
         kwargs["study_url"],
         kwargs["study_completion_time"],
         kwargs["prolific_token"],
         total_available_places=len(conditions),
-        completion_code=kwargs["completion_code"]
+        completion_code=kwargs["completion_code"],
         exclude_studies=exclude_studies
     )
 
     # get the specification on prolific
     time_out = prolific_dict["maximum_allowed_time"] * 60
     study_id = prolific_dict["id"]
     counter = 1
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b4/tests/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b5/tests/README.md`

 * *Files identical despite different names*

