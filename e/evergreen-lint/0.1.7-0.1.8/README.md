# Comparing `tmp/evergreen_lint-0.1.7.tar.gz` & `tmp/evergreen_lint-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evergreen_lint-0.1.7.tar", max compression
+gzip compressed data, was "evergreen_lint-0.1.8.tar", max compression
```

## Comparing `evergreen_lint-0.1.7.tar` & `evergreen_lint-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       93 2024-05-14 15:19:23.354097 evergreen_lint-0.1.7/evergreen_lint/__init__.py
--rw-r--r--   0        0        0     2814 2024-02-02 11:05:21.130327 evergreen_lint-0.1.7/evergreen_lint/__main__.py
--rw-r--r--   0        0        0     5025 2024-04-08 16:46:32.760490 evergreen_lint-0.1.7/evergreen_lint/config.py
--rw-r--r--   0        0        0      630 2024-02-02 11:05:21.130758 evergreen_lint-0.1.7/evergreen_lint/config_with_bad_yaml.yml
--rw-r--r--   0        0        0    11356 2024-05-14 10:36:02.423492 evergreen_lint-0.1.7/evergreen_lint/helpers.py
--rw-r--r--   0        0        0      584 2024-02-02 11:05:21.131176 evergreen_lint-0.1.7/evergreen_lint/model.py
--rw-r--r--   0        0        0     2890 2024-04-08 16:46:32.761218 evergreen_lint-0.1.7/evergreen_lint/rules/__init__.py
--rw-r--r--   0        0        0     5809 2024-02-02 11:05:21.131646 evergreen_lint-0.1.7/evergreen_lint/rules/commonsense.py
--rw-r--r--   0        0        0     1694 2024-02-02 11:05:21.131861 evergreen_lint-0.1.7/evergreen_lint/rules/dependency_for_func.py
--rw-r--r--   0        0        0     4696 2024-04-08 16:46:32.761955 evergreen_lint-0.1.7/evergreen_lint/rules/enforce_tags_for_tasks.py
--rw-r--r--   0        0        0     4188 2024-04-08 16:46:32.762393 evergreen_lint-0.1.7/evergreen_lint/rules/enforce_tags_for_variants.py
--rw-r--r--   0        0        0     1388 2024-02-02 14:46:52.358352 evergreen_lint-0.1.7/evergreen_lint/rules/invalid_build_parameter.py
--rw-r--r--   0        0        0    12357 2024-05-14 15:19:23.355195 evergreen_lint-0.1.7/evergreen_lint/rules/required_expansions_write.py
--rw-r--r--   0        0        0     3210 2024-02-02 11:05:21.132563 evergreen_lint-0.1.7/evergreen_lint/rules/tasks_for_variants.py
--rw-r--r--   0        0        0      925 2024-02-06 15:46:18.003257 evergreen_lint-0.1.7/evergreen_lint/yamlhandler.py
--rw-r--r--   0        0        0     1266 2024-05-14 15:19:23.356121 evergreen_lint-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 evergreen_lint-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       93 2024-05-20 07:21:08.892622 evergreen_lint-0.1.8/evergreen_lint/__init__.py
+-rw-r--r--   0        0        0     2814 2024-02-02 11:05:21.130327 evergreen_lint-0.1.8/evergreen_lint/__main__.py
+-rw-r--r--   0        0        0     5156 2024-05-20 07:21:08.893619 evergreen_lint-0.1.8/evergreen_lint/config.py
+-rw-r--r--   0        0        0      630 2024-02-02 11:05:21.130758 evergreen_lint-0.1.8/evergreen_lint/config_with_bad_yaml.yml
+-rw-r--r--   0        0        0    11356 2024-05-14 10:36:02.423492 evergreen_lint-0.1.8/evergreen_lint/helpers.py
+-rw-r--r--   0        0        0      584 2024-02-02 11:05:21.131176 evergreen_lint-0.1.8/evergreen_lint/model.py
+-rw-r--r--   0        0        0     3005 2024-05-20 07:21:08.894462 evergreen_lint-0.1.8/evergreen_lint/rules/__init__.py
+-rw-r--r--   0        0        0     5809 2024-02-02 11:05:21.131646 evergreen_lint-0.1.8/evergreen_lint/rules/commonsense.py
+-rw-r--r--   0        0        0     1694 2024-02-02 11:05:21.131861 evergreen_lint-0.1.8/evergreen_lint/rules/dependency_for_func.py
+-rw-r--r--   0        0        0     4696 2024-04-08 16:46:32.761955 evergreen_lint-0.1.8/evergreen_lint/rules/enforce_tags_for_tasks.py
+-rw-r--r--   0        0        0     4188 2024-04-08 16:46:32.762393 evergreen_lint-0.1.8/evergreen_lint/rules/enforce_tags_for_variants.py
+-rw-r--r--   0        0        0     1388 2024-02-02 14:46:52.358352 evergreen_lint-0.1.8/evergreen_lint/rules/invalid_build_parameter.py
+-rw-r--r--   0        0        0    12357 2024-05-14 15:19:23.355195 evergreen_lint-0.1.8/evergreen_lint/rules/required_expansions_write.py
+-rw-r--r--   0        0        0     3210 2024-02-02 11:05:21.132563 evergreen_lint-0.1.8/evergreen_lint/rules/tasks_for_variants.py
+-rw-r--r--   0        0        0     9714 2024-05-20 07:21:08.895223 evergreen_lint-0.1.8/evergreen_lint/rules/variant_expansions.py
+-rw-r--r--   0        0        0      925 2024-02-06 15:46:18.003257 evergreen_lint-0.1.8/evergreen_lint/yamlhandler.py
+-rw-r--r--   0        0        0     1266 2024-05-20 07:21:08.895911 evergreen_lint-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 evergreen_lint-0.1.8/PKG-INFO
```

### Comparing `evergreen_lint-0.1.7/evergreen_lint/__main__.py` & `evergreen_lint-0.1.8/evergreen_lint/__main__.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/config.py` & `evergreen_lint-0.1.8/evergreen_lint/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,10 +131,15 @@
     # Enforce tasks must have tags
     - rule: "enforce-tags-for-tasks"
       tag_groups: {[]}
 
     # Enforce variants must have tags
     - rule: "enforce-tags-for-variants"
       tags: {[]}
+
+    # Validate variant expansions
+    - rule: "variant-expansions"
+      require_expansions: {[]}
+      prohibit_expansions: {[]}
 """[
     1:-1
 ]  # <--- this strips the leading and trailing newlines from this HEREDOC
```

### Comparing `evergreen_lint-0.1.7/evergreen_lint/config_with_bad_yaml.yml` & `evergreen_lint-0.1.8/evergreen_lint/config_with_bad_yaml.yml`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/helpers.py` & `evergreen_lint-0.1.8/evergreen_lint/helpers.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/model.py` & `evergreen_lint-0.1.8/evergreen_lint/model.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/__init__.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 )
 from evergreen_lint.rules.dependency_for_func import DependencyForFunc
 from evergreen_lint.rules.enforce_tags_for_tasks import EnforceTagsForTasks
 from evergreen_lint.rules.enforce_tags_for_variants import EnforceTagsForVariants
 from evergreen_lint.rules.invalid_build_parameter import InvalidBuildParameter
 from evergreen_lint.rules.required_expansions_write import RequiredExpansionsWrite
 from evergreen_lint.rules.tasks_for_variants import TasksForVariants
+from evergreen_lint.rules.variant_expansions import VariantExpansions
 
 RULES: Dict[str, Type[Rule]] = {
     "limit-keyval-inc": LimitKeyvalInc,
     "shell-exec-explicit-shell": ShellExecExplicitShell,
     "no-working-dir-on-shell": NoWorkingDirOnShell,
     "invalid-function-name": InvalidFunctionName,
     "no-shell-exec": NoShellExec,
     "no-multiline-expansions-update": NoMultilineExpansionsUpdate,
     "invalid-build-parameter": InvalidBuildParameter,
     "required-expansions-write": RequiredExpansionsWrite,
     "dependency-for-func": DependencyForFunc,
     "tasks-for-variants": TasksForVariants,
     "enforce-tags-for-tasks": EnforceTagsForTasks,
     "enforce-tags-for-variants": EnforceTagsForVariants,
+    "variant-expansions": VariantExpansions,
 }
 # Thoughts on Writing Rules
 # - see .helpers for reliable iteration helpers
 # - Do not assume a key exists, unless it's been mentioned here
 # - Do not allow exceptions to percolate outside of the rule function
 # - YAML anchors are not available. Unless you want to write your own yaml
 #   parser, or fork adrienverge/yamllint, abandon all hope on that idea you have.
```

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/commonsense.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/commonsense.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/dependency_for_func.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/dependency_for_func.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/enforce_tags_for_tasks.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/enforce_tags_for_tasks.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/enforce_tags_for_variants.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/enforce_tags_for_variants.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/invalid_build_parameter.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/invalid_build_parameter.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/required_expansions_write.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/required_expansions_write.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/rules/tasks_for_variants.py` & `evergreen_lint-0.1.8/evergreen_lint/rules/tasks_for_variants.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/evergreen_lint/yamlhandler.py` & `evergreen_lint-0.1.8/evergreen_lint/yamlhandler.py`

 * *Files identical despite different names*

### Comparing `evergreen_lint-0.1.7/pyproject.toml` & `evergreen_lint-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evergreen-lint"
-version = "0.1.7"  # Duplicated in the top-level __init__.py.
+version = "0.1.8"  # Duplicated in the top-level __init__.py.
 description = ""
 authors = [
     "DevProd Build Team <devprod-build-team@mongodb.com>",
     "DevProd Correctness Team <devprod-correctness-team@mongodb.com>",
 ]
 
 [tool.poetry.scripts]
```

