# Comparing `tmp/codedepot_git_ai-0.0.25.tar.gz` & `tmp/codedepot_git_ai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_git_ai-0.0.25.tar", last modified: Mon Apr 29 16:08:32 2024, max compression
+gzip compressed data, was "codedepot_git_ai-0.1.0.tar", last modified: Mon May 20 09:56:25 2024, max compression
```

## Comparing `codedepot_git_ai-0.0.25.tar` & `codedepot_git_ai-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.25/LICENSE
--rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.25/README.md
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.645320 codedepot_git_ai-0.0.25/git_ai/__init__.py
--rw-r--r--   0        0        0      220 2023-11-27 16:02:28.645606 codedepot_git_ai-0.0.25/git_ai/cmd/__init__.py
--rw-r--r--   0        0        0       77 2023-11-27 16:02:28.645811 codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/__init__.py
--rw-r--r--   0        0        0    13791 2024-04-17 18:19:20.006058 codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/ai_repo.py
--rw-r--r--   0        0        0     2093 2023-11-27 16:02:28.646238 codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/ai_repo_config.py
--rw-r--r--   0        0        0     5513 2024-04-02 10:13:46.122413 codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/ai_repo_log.py
--rw-r--r--   0        0        0     7956 2024-04-19 09:39:57.073252 codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/credentials.py
--rw-r--r--   0        0        0     1292 2024-04-02 07:32:17.319363 codedepot_git_ai-0.0.25/git_ai/cmd/constants.py
--rw-r--r--   0        0        0     6257 2023-11-27 16:02:28.646779 codedepot_git_ai-0.0.25/git_ai/cmd/diff.py
--rw-r--r--   0        0        0       64 2023-11-27 16:02:28.646875 codedepot_git_ai-0.0.25/git_ai/cmd/error.py
--rw-r--r--   0        0        0      926 2024-04-05 12:00:10.813475 codedepot_git_ai-0.0.25/git_ai/cmd/init.py
--rw-r--r--   0        0        0      370 2024-04-02 10:14:57.943339 codedepot_git_ai-0.0.25/git_ai/cmd/input_repo.py
--rw-r--r--   0        0        0      310 2023-11-27 16:02:28.647348 codedepot_git_ai-0.0.25/git_ai/cmd/log.py
--rw-r--r--   0        0        0      147 2023-11-27 16:02:28.647533 codedepot_git_ai-0.0.25/git_ai/cmd/merge_exp.py
--rw-r--r--   0        0        0       45 2023-11-27 16:02:28.647580 codedepot_git_ai-0.0.25/git_ai/cmd/runner.py
--rw-r--r--   0        0        0       80 2023-11-27 16:02:28.647785 codedepot_git_ai-0.0.25/git_ai/errors/__init__.py
--rw-r--r--   0        0        0     4434 2024-04-17 12:45:58.362534 codedepot_git_ai-0.0.25/git_ai/errors/errors.py
--rw-r--r--   0        0        0        0 2024-04-03 10:15:19.429281 codedepot_git_ai-0.0.25/git_ai/main/__init__.py
--rw-r--r--   0        0        0      878 2024-04-29 16:08:21.830736 codedepot_git_ai-0.0.25/git_ai/main/main.py
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.648024 codedepot_git_ai-0.0.25/git_ai/metrics/__init__.py
--rw-r--r--   0        0        0     5633 2024-04-29 16:08:05.127579 codedepot_git_ai-0.0.25/git_ai/metrics/experiment.py
--rw-r--r--   0        0        0    12294 2024-04-02 08:10:43.723916 codedepot_git_ai-0.0.25/git_ai/metrics/writer.py
--rw-r--r--   0        0        0       73 2023-11-27 16:02:28.648608 codedepot_git_ai-0.0.25/git_ai/pygitutils/__init__.py
--rw-r--r--   0        0        0     1094 2023-11-27 16:02:28.648784 codedepot_git_ai-0.0.25/git_ai/pygitutils/pygitutils.py
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.25/git_ai/test/__init__.py
--rw-r--r--   0        0        0    11834 2024-04-17 17:50:50.114962 codedepot_git_ai-0.0.25/git_ai/test/test_ai_repo.py
--rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.1
--rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.2
--rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.3
--rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.4
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.25/git_ai/test/utils/__init__.py
--rw-r--r--   0        0        0     1544 2024-04-17 13:28:20.714093 codedepot_git_ai-0.0.25/git_ai/test/utils/ai_repo_read.py
--rw-r--r--   0        0        0    14079 2024-04-17 13:29:15.601987 codedepot_git_ai-0.0.25/git_ai/test/utils/data_gen.py
--rw-r--r--   0        0        0     1800 2024-04-17 17:46:06.335729 codedepot_git_ai-0.0.25/git_ai/test/utils/interuptable_test.py
--rw-r--r--   0        0        0     3144 2024-04-17 16:38:11.642332 codedepot_git_ai-0.0.25/git_ai/test/utils/setup_repo.py
--rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.25/git_ai/test/utils/testutils.py
--rw-r--r--   0        0        0       29 2023-11-27 16:02:28.648937 codedepot_git_ai-0.0.25/git_ai/utils/__init__.py
--rw-r--r--   0        0        0      343 2023-11-27 16:02:28.649108 codedepot_git_ai-0.0.25/git_ai/utils/utils.py
--rw-r--r--   0        0        0      819 2024-04-29 16:08:32.780917 codedepot_git_ai-0.0.25/pyproject.toml
--rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.645320 codedepot_git_ai-0.1.0/git_ai/__init__.py
+-rw-r--r--   0        0        0      220 2023-11-27 16:02:28.645606 codedepot_git_ai-0.1.0/git_ai/cmd/__init__.py
+-rw-r--r--   0        0        0       77 2023-11-27 16:02:28.645811 codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/__init__.py
+-rw-r--r--   0        0        0    13791 2024-04-17 18:19:20.006058 codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/ai_repo.py
+-rw-r--r--   0        0        0     2093 2023-11-27 16:02:28.646238 codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/ai_repo_config.py
+-rw-r--r--   0        0        0     5513 2024-04-02 10:13:46.122413 codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/ai_repo_log.py
+-rw-r--r--   0        0        0     7953 2024-05-20 09:53:54.232713 codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/credentials.py
+-rw-r--r--   0        0        0     1292 2024-04-02 07:32:17.319363 codedepot_git_ai-0.1.0/git_ai/cmd/constants.py
+-rw-r--r--   0        0        0     6257 2023-11-27 16:02:28.646779 codedepot_git_ai-0.1.0/git_ai/cmd/diff.py
+-rw-r--r--   0        0        0       64 2023-11-27 16:02:28.646875 codedepot_git_ai-0.1.0/git_ai/cmd/error.py
+-rw-r--r--   0        0        0      926 2024-04-05 12:00:10.813475 codedepot_git_ai-0.1.0/git_ai/cmd/init.py
+-rw-r--r--   0        0        0      370 2024-04-02 10:14:57.943339 codedepot_git_ai-0.1.0/git_ai/cmd/input_repo.py
+-rw-r--r--   0        0        0      310 2023-11-27 16:02:28.647348 codedepot_git_ai-0.1.0/git_ai/cmd/log.py
+-rw-r--r--   0        0        0      147 2023-11-27 16:02:28.647533 codedepot_git_ai-0.1.0/git_ai/cmd/merge_exp.py
+-rw-r--r--   0        0        0       45 2023-11-27 16:02:28.647580 codedepot_git_ai-0.1.0/git_ai/cmd/runner.py
+-rw-r--r--   0        0        0       80 2023-11-27 16:02:28.647785 codedepot_git_ai-0.1.0/git_ai/errors/__init__.py
+-rw-r--r--   0        0        0     4434 2024-04-17 12:45:58.362534 codedepot_git_ai-0.1.0/git_ai/errors/errors.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:15:19.429281 codedepot_git_ai-0.1.0/git_ai/main/__init__.py
+-rw-r--r--   0        0        0      877 2024-05-20 09:54:14.222698 codedepot_git_ai-0.1.0/git_ai/main/main.py
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.648024 codedepot_git_ai-0.1.0/git_ai/metrics/__init__.py
+-rw-r--r--   0        0        0     5633 2024-04-29 16:08:05.127579 codedepot_git_ai-0.1.0/git_ai/metrics/experiment.py
+-rw-r--r--   0        0        0    12294 2024-04-02 08:10:43.723916 codedepot_git_ai-0.1.0/git_ai/metrics/writer.py
+-rw-r--r--   0        0        0       73 2023-11-27 16:02:28.648608 codedepot_git_ai-0.1.0/git_ai/pygitutils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-11-27 16:02:28.648784 codedepot_git_ai-0.1.0/git_ai/pygitutils/pygitutils.py
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.1.0/git_ai/test/__init__.py
+-rw-r--r--   0        0        0    11834 2024-04-17 17:50:50.114962 codedepot_git_ai-0.1.0/git_ai/test/test_ai_repo.py
+-rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.1
+-rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.2
+-rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.3
+-rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.4
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.1.0/git_ai/test/utils/__init__.py
+-rw-r--r--   0        0        0     1544 2024-04-17 13:28:20.714093 codedepot_git_ai-0.1.0/git_ai/test/utils/ai_repo_read.py
+-rw-r--r--   0        0        0    14079 2024-04-17 13:29:15.601987 codedepot_git_ai-0.1.0/git_ai/test/utils/data_gen.py
+-rw-r--r--   0        0        0     1800 2024-04-17 17:46:06.335729 codedepot_git_ai-0.1.0/git_ai/test/utils/interuptable_test.py
+-rw-r--r--   0        0        0     3144 2024-04-17 16:38:11.642332 codedepot_git_ai-0.1.0/git_ai/test/utils/setup_repo.py
+-rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.1.0/git_ai/test/utils/testutils.py
+-rw-r--r--   0        0        0       29 2023-11-27 16:02:28.648937 codedepot_git_ai-0.1.0/git_ai/utils/__init__.py
+-rw-r--r--   0        0        0      343 2023-11-27 16:02:28.649108 codedepot_git_ai-0.1.0/git_ai/utils/utils.py
+-rw-r--r--   0        0        0      818 2024-05-20 09:56:25.268417 codedepot_git_ai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2086 1970-01-01 00:00:00.000000 codedepot_git_ai-0.1.0/PKG-INFO
```

### Comparing `codedepot_git_ai-0.0.25/LICENSE` & `codedepot_git_ai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/README.md` & `codedepot_git_ai-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/ai_repo.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/ai_repo_config.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/ai_repo_config.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/ai_repo_log.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/ai_repo_log.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/ai_repo/credentials.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/ai_repo/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             return result
 
         protocol = self.__get_protocol_from_url(remote)
         if protocol == "ssh":
             # TODO Check ssh config file if key is specified
             username = self.__get_ssh_user(remote)
             if 'DEPOT_SSH_PRIVATE_KEY' in os.environ:
-                print("Using depot's ssh key")
+                print("Using ai's ssh key")
                 public_key = os.environ['DEPOT_SSH_PUBLIC_KEY']
                 private_key = os.environ['DEPOT_SSH_PRIVATE_KEY']
 
                 keypair = pygit2.KeypairFromMemory(
                     username, public_key, private_key, '')
                 succeeded, result = self.try_auth(
                     remote, keypair, operation_fn)
```

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/constants.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/constants.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/diff.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/diff.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/cmd/init.py` & `codedepot_git_ai-0.1.0/git_ai/cmd/init.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/errors/errors.py` & `codedepot_git_ai-0.1.0/git_ai/errors/errors.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/main/main.py` & `codedepot_git_ai-0.1.0/git_ai/main/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         elif sys.argv[1] == 'log':
             log(sys.argv)
         elif sys.argv[1] == 'merge-exp':
             merge_exp(sys.argv)
         elif sys.argv[1] == 'input-repo':
             input_repo(sys.argv)
         else:
-            print('git-ai 0.0.25')
+            print('git-ai 0.1.0')
             print('Usage: git-ai <command> [<args>]')
     except Exception as e:
         print(format_error(e))
         sys.exit(1)
```

### Comparing `codedepot_git_ai-0.0.25/git_ai/metrics/experiment.py` & `codedepot_git_ai-0.1.0/git_ai/metrics/experiment.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/metrics/writer.py` & `codedepot_git_ai-0.1.0/git_ai/metrics/writer.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/pygitutils/pygitutils.py` & `codedepot_git_ai-0.1.0/git_ai/pygitutils/pygitutils.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/test_ai_repo.py` & `codedepot_git_ai-0.1.0/git_ai/test/test_ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.1` & `codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.1`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.2` & `codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.2`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.3` & `codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.3`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/topologies/cnn.4` & `codedepot_git_ai-0.1.0/git_ai/test/topologies/cnn.4`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/utils/ai_repo_read.py` & `codedepot_git_ai-0.1.0/git_ai/test/utils/ai_repo_read.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/utils/data_gen.py` & `codedepot_git_ai-0.1.0/git_ai/test/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/utils/interuptable_test.py` & `codedepot_git_ai-0.1.0/git_ai/test/utils/interuptable_test.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/git_ai/test/utils/setup_repo.py` & `codedepot_git_ai-0.1.0/git_ai/test/utils/setup_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.25/pyproject.toml` & `codedepot_git_ai-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "codedepot-git-ai"
-version = "0.0.25"
+version = "0.1.0"
 description = "Dataset and model support for git"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `codedepot_git_ai-0.0.25/PKG-INFO` & `codedepot_git_ai-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.25
+Version: 0.1.0
 Summary: Dataset and model support for git
 Author-Email: CodeDepot <contact@codedepot.ai>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
```

