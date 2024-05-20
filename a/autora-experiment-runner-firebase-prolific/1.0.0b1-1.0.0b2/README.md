# Comparing `tmp/autora-experiment-runner-firebase-prolific-1.0.0b1.tar.gz` & `tmp/autora_experiment_runner_firebase_prolific-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-firebase-prolific-1.0.0b1.tar", last modified: Sun Mar 31 12:19:38 2024, max compression
+gzip compressed data, was "autora_experiment_runner_firebase_prolific-1.0.0b2.tar", last modified: Mon May 20 01:44:55 2024, max compression
```

## Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1.tar` & `autora_experiment_runner_firebase_prolific-1.0.0b2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.843100 autora-experiment-runner-firebase-prolific-1.0.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-03-31 12:19:38.843100 autora-experiment-runner-firebase-prolific-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 12:19:38.843100 autora-experiment-runner-firebase-prolific-1.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.839100 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora/experiment_runner/firebase_prolific/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora/experiment_runner/firebase_prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.843100 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-03-31 12:19:38.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-31 12:19:38.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 12:19:38.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 12:19:38.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 12:19:38.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:38.843100 autora-experiment-runner-firebase-prolific-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:19:29.000000 autora-experiment-runner-firebase-prolific-1.0.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.663446 autora_experiment_runner_firebase_prolific-1.0.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 01:44:55.663446 autora_experiment_runner_firebase_prolific-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:44:55.663446 autora_experiment_runner_firebase_prolific-1.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.659446 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora/experiment_runner/firebase_prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora/experiment_runner/firebase_prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.663446 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 01:44:55.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 01:44:55.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:44:55.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 01:44:55.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 01:44:55.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:55.663446 autora_experiment_runner_firebase_prolific-1.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:44:51.000000 autora_experiment_runner_firebase_prolific-1.0.0b2/tests/__init__.py
```

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/.github/workflows/python-publish.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/.gitignore` & `autora_experiment_runner_firebase_prolific-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/.pre-commit-config.yaml` & `autora_experiment_runner_firebase_prolific-1.0.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/LICENSE` & `autora_experiment_runner_firebase_prolific-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/mkdocs/base.yml` & `autora_experiment_runner_firebase_prolific-1.0.0b2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/pyproject.toml` & `autora_experiment_runner_firebase_prolific-1.0.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora/experiment_runner/firebase_prolific/__init__.py` & `autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora/experiment_runner/firebase_prolific/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,18 +91,23 @@
                 )
 
             check_prolific = check_prolific_status(study_id, kwargs["prolific_token"])
             if (
                     check_prolific["number_of_submissions"]
                     >= check_prolific["total_available_places"] and check_firebase == "finished"
             ):
-                observation = get_observations("autora", kwargs["firebase_credentials"])
-                observation_list = [observation[key] for key in sorted(observation.keys())]
-                return observation_list
-
+                if check_firebase == "finished":
+                    observation = get_observations("autora", kwargs["firebase_credentials"])
+                    observation_list = [observation[key] for key in sorted(observation.keys())]
+                    return observation_list
+                else:
+                    print("Warning: Number of collected participants was lower than submission number")
+                    observation = get_observations("autora", kwargs["firebase_credentials"])
+                    observation_list = [observation[key] for key in sorted(observation.keys())]
+                    return observation_list
         # firebase places available
         if check_firebase == "finished":
             pass
             # return get_observations("autora", kwargs["firebase_credentials"])
         if check_firebase == "available":
             if check_prolific["status"] == "UNPUBLISHED":
                 publish_study(
```

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-firebase-prolific
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: AutoRA Firebase Prolific Experiment Runner provides experiment runners to run experiments with prolific and firebase
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_firebase_prolific-1.0.0b2/src/autora_experiment_runner_firebase_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-firebase-prolific-1.0.0b1/tests/README.md` & `autora_experiment_runner_firebase_prolific-1.0.0b2/tests/README.md`

 * *Files identical despite different names*

