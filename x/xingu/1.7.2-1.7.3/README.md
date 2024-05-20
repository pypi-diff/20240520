# Comparing `tmp/xingu-1.7.2.tar.gz` & `tmp/xingu-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingu-1.7.2.tar", last modified: Thu May 16 01:22:08 2024, max compression
+gzip compressed data, was "xingu-1.7.3.tar", last modified: Mon May 20 14:40:43 2024, max compression
```

## Comparing `xingu-1.7.2.tar` & `xingu-1.7.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7.2/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-16 01:22:08.088120 xingu-1.7.2/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7.2/README.md
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1277 2024-05-16 01:21:25.000000 xingu-1.7.2/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-16 01:22:08.088120 xingu-1.7.2/setup.cfg
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/xingu/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7.2/xingu/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19715 2024-05-16 01:21:08.000000 xingu-1.7.2/xingu/__main__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50497 2024-05-10 13:13:55.000000 xingu-1.7.2/xingu/coach.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7.2/xingu/config_manager.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22328 2024-05-09 20:54:52.000000 xingu-1.7.2/xingu/dataprovider.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7.2/xingu/dataproviderfactory.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2523 2024-05-09 20:50:35.000000 xingu-1.7.2/xingu/estimator.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/xingu/estimators/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7.2/xingu/estimators/catboost.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101862 2024-05-16 01:14:37.000000 xingu-1.7.2/xingu/model.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-16 01:22:08.088120 xingu-1.7.2/xingu.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/entry_points.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-16 01:22:08.000000 xingu-1.7.2/xingu.egg-info/top_level.txt
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-20 14:40:43.294650 xingu-1.7.3/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7652 2024-01-03 19:20:34.000000 xingu-1.7.3/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-20 14:40:43.294650 xingu-1.7.3/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11571 2024-01-10 19:09:00.000000 xingu-1.7.3/README.md
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1277 2024-05-20 14:39:42.000000 xingu-1.7.3/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-20 14:40:43.294650 xingu-1.7.3/setup.cfg
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-20 14:40:43.290650 xingu-1.7.3/xingu/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      434 2024-01-24 19:13:14.000000 xingu-1.7.3/xingu/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19747 2024-05-16 03:01:28.000000 xingu-1.7.3/xingu/__main__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    50696 2024-05-20 14:39:42.000000 xingu-1.7.3/xingu/coach.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7378 2024-01-03 19:20:34.000000 xingu-1.7.3/xingu/config_manager.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22328 2024-05-09 20:54:52.000000 xingu-1.7.3/xingu/dataprovider.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5498 2024-01-03 19:20:34.000000 xingu-1.7.3/xingu/dataproviderfactory.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2523 2024-05-09 20:50:35.000000 xingu-1.7.3/xingu/estimator.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-20 14:40:43.294650 xingu-1.7.3/xingu/estimators/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12628 2024-01-03 19:20:34.000000 xingu-1.7.3/xingu/estimators/catboost.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)   101910 2024-05-20 14:39:42.000000 xingu-1.7.3/xingu/model.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-20 14:40:43.294650 xingu-1.7.3/xingu.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21761 2024-05-20 14:40:43.000000 xingu-1.7.3/xingu.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      397 2024-05-20 14:40:43.000000 xingu-1.7.3/xingu.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-20 14:40:43.000000 xingu-1.7.3/xingu.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       46 2024-05-20 14:40:43.000000 xingu-1.7.3/xingu.egg-info/entry_points.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2024-05-20 14:40:43.000000 xingu-1.7.3/xingu.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-05-20 14:40:43.000000 xingu-1.7.3/xingu.egg-info/top_level.txt
```

### Comparing `xingu-1.7.2/LICENSE` & `xingu-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/PKG-INFO` & `xingu-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.7.2
+Version: 1.7.3
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `xingu-1.7.2/README.md` & `xingu-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/pyproject.toml` & `xingu-1.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingu"
-version = '1.7.2'
+version = '1.7.3'
 description = "Automated ML model training and packaging"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 authors = [
     { name = "Avi Alkalay", email = "avi@unix.sh" },
 ]
```

### Comparing `xingu-1.7.2/xingu/__main__.py` & `xingu-1.7.3/xingu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     # Suppress well known very annoying modules
     annoying="""
         aiobotocore
         boto3
         botocore
         s3fs
         fsspec
+        matplotlib.font_manager
     """.split()
 
     for stop_annoying in annoying:
         annoying_logger = logging.getLogger(stop_annoying)
         annoying_logger.setLevel(logging.WARNING)
 
     return logger
```

### Comparing `xingu-1.7.2/xingu/coach.py` & `xingu-1.7.3/xingu/coach.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self.databases=dict()
 
         try:
             import pygit2
             self.git_repo=pygit2.Repository(self.get_config('PROJECT_HOME'))
             self.logger.debug("Using git repo on {}".format(self.git_repo))
         except:
+            self.logger.warning("Sorry, your code apparently not under a git repo; can't add git metadata to models")
             self.git_repo=None
 
         self.dp_factory=dp_factory
 
         # Load our map of DataProvider IDs and their current train_ids
         self.load_inventory()
 
@@ -499,22 +500,25 @@
 
             # Update file with what we have
             self.inventory['history'].append(
                 dict(
                     time              = datetime.datetime.now(datetime.timezone.utc),
                     user_name         = self.get_config('USERNAME',os.environ.get('USER', os.environ.get('USERNAME'))),
                     host_name         = self.get_config('HOSTNAME',socket.gethostname()),
-                    git_branch        = self.git_repo.head.name if self.git_repo else None,
-                    git_commit        = self.git_repo.head.target.hex if self.git_repo else None,
-                    github_actor      = self.get_config('GITHUB_ACTOR', None),
-                    github_workflow   = self.get_config('GITHUB_WORKFLOW', None),
-                    github_run_id     = self.get_config('GITHUB_RUN_ID', None),
-                    github_run_number = self.get_config('GITHUB_RUN_NUMBER', None),
+
                     trained_in_session= self.trained_in_session,
-                    train_session_id  = self.train_session_id
+                    train_session_id  = self.train_session_id,
+
+                    # Code repository metadata
+                    git_branch        = self.git_repo.head.name              if self.git_repo else None,
+                    git_commit        = str(self.git_repo.head.target)       if self.git_repo else None,
+                    github_actor      = self.get_config('GITHUB_ACTOR',      None),
+                    github_workflow   = self.get_config('GITHUB_WORKFLOW',   None),
+                    github_run_id     = self.get_config('GITHUB_RUN_ID',     None),
+                    github_run_number = self.get_config('GITHUB_RUN_NUMBER', None),
                 )
             )
 
             # Preserve just last 10 entries in history
             self.inventory['history']=self.inventory['history'][-10:]
 
             for e in self.trained_in_session:
```

### Comparing `xingu-1.7.2/xingu/config_manager.py` & `xingu-1.7.3/xingu/config_manager.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/xingu/dataprovider.py` & `xingu-1.7.3/xingu/dataprovider.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/xingu/dataproviderfactory.py` & `xingu-1.7.3/xingu/dataproviderfactory.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/xingu/estimator.py` & `xingu-1.7.3/xingu/estimator.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/xingu/estimators/catboost.py` & `xingu-1.7.3/xingu/estimators/catboost.py`

 * *Files identical despite different names*

### Comparing `xingu-1.7.2/xingu/model.py` & `xingu-1.7.3/xingu/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,22 +159,24 @@
             self.train_id                 = None
             self.train_session_id         = None
             self.train_queries_signatures = dict()
 
             # Store more contextual and informative metadata from the Coach and environment
             self.user_name         = self.get_config('USERNAME',os.environ.get('USER', os.environ.get('USERNAME')))
             self.host_name         = self.get_config('HOSTNAME',socket.gethostname())
-            self.git_branch        = self.coach.git_repo.head.name if self.coach.git_repo else None
-            self.git_commit        = self.coach.git_repo.head.target.hex if self.coach.git_repo else None
+
+            # Git metadata embedded in models
             self.github_actor      = self.get_config('GITHUB_ACTOR', None)
             self.github_workflow   = self.get_config('GITHUB_WORKFLOW', None)
             self.github_run_id     = self.get_config('GITHUB_RUN_ID', None)
             self.github_run_number = self.get_config('GITHUB_RUN_NUMBER', None)
+            self.git_branch        = self.coach.git_repo.head.name if self.coach.git_repo else None
+            self.git_commit        = str(self.coach.git_repo.head.target) if self.coach.git_repo else None
 
-            self.log(message=str(self.dp.get_estimator_class()))
+            self.logger.info(str(self.dp.get_estimator_class()))
 
         if delayed_prereq_binding is False:
             self.load_pre_req_model()
 
 
 
     ######################################################################################
```

### Comparing `xingu-1.7.2/xingu.egg-info/PKG-INFO` & `xingu-1.7.3/xingu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingu
-Version: 1.7.2
+Version: 1.7.3
 Summary: Automated ML model training and packaging
 Author-email: Avi Alkalay <avi@unix.sh>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

