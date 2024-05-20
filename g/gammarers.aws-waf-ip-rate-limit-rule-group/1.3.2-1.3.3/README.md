# Comparing `tmp/gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2.tar.gz` & `tmp/gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2.tar", last modified: Mon May 13 19:19:37 2024, max compression
+gzip compressed data, was "gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3.tar", last modified: Mon May 20 19:19:45 2024, max compression
```

## Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2.tar` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:19:37.474073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-13 19:19:37.474073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:19:37.474073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:19:37.470073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:19:37.470073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:19:37.474073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:19:37.474073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23730 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.3.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:19:25.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:19:37.474073 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-13 19:19:37.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 19:19:37.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:19:37.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 19:19:37.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 19:19:37.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:19:45.455867 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-20 19:19:45.455867 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:19:45.455867 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:19:45.451866 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:19:45.451866 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:19:45.455867 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:19:45.455867 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23729 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.3.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:19:34.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:19:45.455867 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-20 19:19:45.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 19:19:45.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:19:45.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 19:19:45.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 19:19:45.000000 gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/top_level.txt
```

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/LICENSE` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/PKG-INFO` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-ip-rate-limit-rule-group
-Version: 1.3.2
+Version: 1.3.3
 Summary: This is an AWS CDK Construct for Rate Limit Rule on WAF V2.
 Home-page: https://github.com/gammarers/aws-waf-ip-rate-limit-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-ip-rate-limit-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/README.md` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/setup.py` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-waf-ip-rate-limit-rule-group",
-    "version": "1.3.2",
+    "version": "1.3.3",
     "description": "This is an AWS CDK Construct for Rate Limit Rule on WAF V2.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-waf-ip-rate-limit-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_waf_ip_rate_limit_rule_group",
         "gammarers.aws_waf_ip_rate_limit_rule_group._jsii"
     ],
     "package_data": {
         "gammarers.aws_waf_ip_rate_limit_rule_group._jsii": [
-            "aws-waf-ip-rate-limit-rule-group@1.3.2.jsii.tgz"
+            "aws-waf-ip-rate-limit-rule-group@1.3.3.jsii.tgz"
         ],
         "gammarers.aws_waf_ip_rate_limit_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/__init__.py` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-waf-ip-rate-limit-rule-group",
-    "1.3.2",
+    "1.3.3",
     __name__[0:-6],
-    "aws-waf-ip-rate-limit-rule-group@1.3.2.jsii.tgz",
+    "aws-waf-ip-rate-limit-rule-group@1.3.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-ip-rate-limit-rule-group
-Version: 1.3.2
+Version: 1.3.3
 Summary: This is an AWS CDK Construct for Rate Limit Rule on WAF V2.
 Home-page: https://github.com/gammarers/aws-waf-ip-rate-limit-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-ip-rate-limit-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.2/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt` & `gammarers.aws-waf-ip-rate-limit-rule-group-1.3.3/src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/SOURCES.txt
 src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/dependency_links.txt
 src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/requires.txt
 src/gammarers.aws_waf_ip_rate_limit_rule_group.egg-info/top_level.txt
 src/gammarers/aws_waf_ip_rate_limit_rule_group/__init__.py
 src/gammarers/aws_waf_ip_rate_limit_rule_group/py.typed
 src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/__init__.py
-src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.3.2.jsii.tgz
+src/gammarers/aws_waf_ip_rate_limit_rule_group/_jsii/aws-waf-ip-rate-limit-rule-group@1.3.3.jsii.tgz
```

