# Comparing `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b8.tar.gz` & `tmp/autora_experiment_runner_recruitment_manager_prolific-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b8.tar", last modified: Thu Apr 18 21:59:08 2024, max compression
+gzip compressed data, was "autora_experiment_runner_recruitment_manager_prolific-1.0.0b9.tar", last modified: Mon May 20 02:03:33 2024, max compression
```

## Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8.tar` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.162250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:59:08.162250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:59:08.162250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.158250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.162250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 21:59:08.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-18 21:59:08.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:59:08.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 21:59:08.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 21:59:08.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:08.162250 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 21:59:03.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.834042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.834042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.834042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.834042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.834042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.834042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (127)    18927 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-20 02:03:33.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 02:03:33.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:03:33.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 02:03:33.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 02:03:33.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:33.838042 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 02:03:29.000000 autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.github/workflows/python-publish.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.gitignore` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/.pre-commit-config.yaml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/LICENSE` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/docs/Basic Usage.ipynb` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/mkdocs/base.yml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/pyproject.toml` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,20 +167,32 @@
     data = {"request_return_reasons": ["No completion code.", "Did not finish study."]}
     __save_post(
         f"https://api.prolific.com/api/v1/submissions/{id}/request-return/",
         headers={"Authorization": f"Token {prolific_token}"},
         _json=data,
     )
 
+def _approve(id: str, prolific_token: str):
+    __save_post(
+                    f'https://api.prolific.com/api/v1/submissions/{sub["id"]}/transition/',
+                    headers={"Authorization": f"Token {prolific_token}"},
+                    _json={"action": "APPROVE"}
+                )
+
 
 def request_return_all(study_id: str, prolific_token: str):
     submissions = _get_submissions_no_code_not_returned(study_id, prolific_token)
     for id in submissions:
         _request_return(id, prolific_token)
 
+def approve_all_no_code(study_id: str, prolific_token: str):
+    subissions = _get_submissions_no_code_not_returned(study_id, prolific_token)
+    for id in submissions:
+        _approve(id, prolif)
+
 
 def _update_study(study_id: str, prolific_token: str, **kwargs) -> bool:
     """
     Updates the parameters of a given study.
     If a study is already published, only internal_name
     and total_available_places can be updated.
     """
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experiment_runner_recruitment_manager_prolific-1.0.0b8/tests/README.md` & `autora_experiment_runner_recruitment_manager_prolific-1.0.0b9/tests/README.md`

 * *Files identical despite different names*

