# Comparing `tmp/autora_experiment_runner_firebase_prolific-1.0.0b5.tar.gz` & `tmp/autora_experiment_runner_firebase_prolific-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b5.tar", last modified: Mon May 20 02:11:00 2024, max compression
+gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b6.tar", last modified: Mon May 20 02:23:20 2024, max compression
```

## Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5.tar` & `autora_experiment_runner_firebase_prolific-1.0.0b6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.554778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/firebase_prolific/
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/firebase_prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:11:00.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:11:00.558778 autora_experiment_runner_firebase_prolific-1.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:10:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.581918 autora_experiment_runner_firebase_prolific-1.0.0b6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.573918 autora_experiment_runner_firebase_prolific-1.0.0b6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:23:20.581918 autora_experiment_runner_firebase_prolific-1.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:23:20.581918 autora_experiment_runner_firebase_prolific-1.0.0b6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.573918 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora/experiment_runner/firebase_prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora/experiment_runner/firebase_prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 02:23:20.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 02:23:20.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:23:20.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 02:23:20.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:23:20.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:20.577918 autora_experiment_runner_firebase_prolific-1.0.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:15.000000 autora_experiment_runner_firebase_prolific-1.0.0b6/tests/__init__.py
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/.github/workflows/python-publish.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/.gitignore` & `autora_experiment_runner_firebase_prolific-1.0.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/.pre-commit-config.yaml` & `autora_experiment_runner_firebase_prolific-1.0.0b6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/LICENSE` & `autora_experiment_runner_firebase_prolific-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/mkdocs/base.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b6/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/pyproject.toml` & `autora_experiment_runner_firebase_prolific-1.0.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora/experiment_runner/firebase_prolific/__init__.py` & `autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora/experiment_runner/firebase_prolific/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     check_prolific_status,
     pause_study,
     setup_study,
     start_study,
     publish_study,
     get_submissions_incompleted,
     request_return_all,
-    approve_all_no_code
+    approve_all_no_code,
+    approve_all
 )
 
 
 def _firebase_run(conditions, **kwargs):
     """
     Running an experiment with firebase to host the experiment and store the data.
     Args:
@@ -92,28 +93,29 @@
         # check firebase
         check_firebase = check_firebase_status(
             "autora", kwargs["firebase_credentials"], time_out
         )
         # check prolific
         if prolific_dict:
             if not counter % 5:
+                approve_all(study_id, kwargs["prolific_token"])
                 if approve_no_code:
                     approve_all_no_code(study_id, kwargs["prolific_token"])
                 else:
                     request_return_all(study_id, kwargs["prolific_token"])
                 incomplete_submissions = get_submissions_incompleted(study_id,
                                                                      kwargs["prolific_token"])
                 check_firebase = check_firebase_status(
                     "autora", kwargs["firebase_credentials"], time_out, incomplete_submissions
                 )
 
             check_prolific = check_prolific_status(study_id, kwargs["prolific_token"])
             if (
                     check_prolific["number_of_submissions"]
-                    >= check_prolific["total_available_places"] and check_firebase == "finished"
+                    >= check_prolific["total_available_places"]
             ):
                 if check_firebase == "finished":
                     observation = get_observations("autora", kwargs["firebase_credentials"])
                     observation_list = [observation[key] for key in sorted(observation.keys())]
                     return observation_list
                 else:
                     print("Warning: Number of collected participants was lower than submission number")
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_firebase_prolific-1.0.0b6/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_firebase_prolific-1.0.0b5/tests/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b6/tests/README.md`

 * *Files identical despite different names*

