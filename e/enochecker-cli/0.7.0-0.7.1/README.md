# Comparing `tmp/enochecker_cli-0.7.0.tar.gz` & `tmp/enochecker_cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enochecker_cli-0.7.0.tar", last modified: Sun May 23 10:02:19 2021, max compression
+gzip compressed data, was "enochecker_cli-0.7.1.tar", last modified: Mon May 20 17:59:42 2024, max compression
```

## Comparing `enochecker_cli-0.7.0.tar` & `enochecker_cli-0.7.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 10:02:19.337369 enochecker_cli-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-05-23 10:02:19.337369 enochecker_cli-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 10:02:19.333369 enochecker_cli-0.7.0/enochecker_cli/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/enochecker_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/enochecker_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/enochecker_cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-23 10:02:19.337369 enochecker_cli-0.7.0/enochecker_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-05-23 10:02:19.000000 enochecker_cli-0.7.0/enochecker_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-05-23 10:02:19.000000 enochecker_cli-0.7.0/enochecker_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-23 10:02:19.000000 enochecker_cli-0.7.0/enochecker_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-05-23 10:02:19.000000 enochecker_cli-0.7.0/enochecker_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-05-23 10:02:19.000000 enochecker_cli-0.7.0/enochecker_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-05-23 10:02:19.000000 enochecker_cli-0.7.0/enochecker_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-23 10:02:19.337369 enochecker_cli-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      952 2021-05-23 10:02:11.000000 enochecker_cli-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:59:42.758311 enochecker_cli-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-20 17:59:42.758311 enochecker_cli-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:59:42.758311 enochecker_cli-0.7.1/enochecker_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/enochecker_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/enochecker_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/enochecker_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/enochecker_cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:59:42.758311 enochecker_cli-0.7.1/enochecker_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-20 17:59:42.000000 enochecker_cli-0.7.1/enochecker_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-20 17:59:42.000000 enochecker_cli-0.7.1/enochecker_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:59:42.000000 enochecker_cli-0.7.1/enochecker_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 17:59:42.000000 enochecker_cli-0.7.1/enochecker_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 17:59:42.000000 enochecker_cli-0.7.1/enochecker_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 17:59:42.000000 enochecker_cli-0.7.1/enochecker_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:59:42.758311 enochecker_cli-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:59:42.758311 enochecker_cli-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-20 17:59:39.000000 enochecker_cli-0.7.1/tests/test_base.py
```

### Comparing `enochecker_cli-0.7.0/LICENSE` & `enochecker_cli-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enochecker_cli-0.7.0/enochecker_cli/base.py` & `enochecker_cli-0.7.1/enochecker_cli/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,18 @@
 
 def main() -> None:
     parser = argparse.ArgumentParser(description="Your friendly checker script")
     _add_arguments(parser)
     ns = parser.parse_args(sys.argv[1:])
     msg = json_task_message_from_namespace(ns)
 
-    result = requests.post(ns.checker_address, data=msg, headers={"content-type": "application/json"},)
+    result = requests.post(
+        ns.checker_address,
+        data=msg,
+        headers={"content-type": "application/json"},
+    )
     if result.ok:
         result_msg = jsons.loads(result.content, CheckerResultMessage)
         print(result_msg.result)
     else:
         print(result.status_code)
         print(result.text)
```

### Comparing `enochecker_cli-0.7.0/setup.py` & `enochecker_cli-0.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name='enochecker_cli',
-    version='0.7.0',
+    version='0.7.1',
     entry_points = {
         "console_scripts": ['enochecker_cli = enochecker_cli.base:main']
     },
     author="Benedikt Radtke",
     author_email="benediktradtke@gmail.com",
     description="Enochecker CLI",
     long_description=long_description,
@@ -21,10 +21,10 @@
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
-     python_requires=">=3.7",
+     python_requires=">=3.8",
      package_data={"enochecker_cli":["py.typed"]},
  )
```

