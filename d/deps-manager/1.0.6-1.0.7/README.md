# Comparing `tmp/deps-manager-1.0.6.tar.gz` & `tmp/deps-manager-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps-manager-1.0.6.tar", last modified: Mon May 20 04:32:01 2024, max compression
+gzip compressed data, was "deps-manager-1.0.7.tar", last modified: Mon May 20 04:43:00 2024, max compression
```

## Comparing `deps-manager-1.0.6.tar` & `deps-manager-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:32:01.740804 deps-manager-1.0.6/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:32:01.740554 deps-manager-1.0.6/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.6/README.md
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:32:01.738857 deps-manager-1.0.6/deps_manager/
--rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.6/deps_manager/__init__.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     8118 2024-05-20 04:29:16.000000 deps-manager-1.0.6/deps_manager/dependencies.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     4125 2024-05-20 04:29:02.000000 deps-manager-1.0.6/deps_manager/main.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.6/deps_manager/utils.py
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:32:01.740215 deps-manager-1.0.6/deps_manager.egg-info/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:32:01.000000 deps-manager-1.0.6/deps_manager.egg-info/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 04:32:01.000000 deps-manager-1.0.6/deps_manager.egg-info/SOURCES.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 04:32:01.000000 deps-manager-1.0.6/deps_manager.egg-info/dependency_links.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 04:32:01.000000 deps-manager-1.0.6/deps_manager.egg-info/entry_points.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 04:32:01.000000 deps-manager-1.0.6/deps_manager.egg-info/requires.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 04:32:01.000000 deps-manager-1.0.6/deps_manager.egg-info/top_level.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 04:32:01.740863 deps-manager-1.0.6/setup.cfg
--rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 04:31:41.000000 deps-manager-1.0.6/setup.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:43:00.493678 deps-manager-1.0.7/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:43:00.493426 deps-manager-1.0.7/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.7/README.md
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:43:00.491499 deps-manager-1.0.7/deps_manager/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.7/deps_manager/__init__.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     8070 2024-05-20 04:42:41.000000 deps-manager-1.0.7/deps_manager/dependencies.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     4125 2024-05-20 04:29:02.000000 deps-manager-1.0.7/deps_manager/main.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.7/deps_manager/utils.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:43:00.493039 deps-manager-1.0.7/deps_manager.egg-info/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:43:00.000000 deps-manager-1.0.7/deps_manager.egg-info/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 04:43:00.000000 deps-manager-1.0.7/deps_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 04:43:00.000000 deps-manager-1.0.7/deps_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 04:43:00.000000 deps-manager-1.0.7/deps_manager.egg-info/entry_points.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 04:43:00.000000 deps-manager-1.0.7/deps_manager.egg-info/requires.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 04:43:00.000000 deps-manager-1.0.7/deps_manager.egg-info/top_level.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 04:43:00.493731 deps-manager-1.0.7/setup.cfg
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 04:42:56.000000 deps-manager-1.0.7/setup.py
```

### Comparing `deps-manager-1.0.6/README.md` & `deps-manager-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.6/deps_manager/dependencies.py` & `deps-manager-1.0.7/deps_manager/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,18 +217,18 @@
     # Set the working directory in the container
     WORKDIR /app
 
     # Copy the project files into the container
     COPY . /app
 
     # Install the required dependencies
-    RUN {venv_path}/bin/pip install -r {requirements_file} && {venv_path}/bin/pip install pytest
+    RUN pip install -r {requirements_file} && pip install pytest
 
     # Default command to run the specified test directory
-    CMD {venv_path}/bin/pytest {tests_dir}
+    CMD pytest {tests_dir}
     """
 
     # Write Dockerfile to a file
     dockerfile_path = "Dockerfile"
     with open(dockerfile_path, "w") as dockerfile:
         dockerfile.write(dockerfile_content)
```

### Comparing `deps-manager-1.0.6/deps_manager/main.py` & `deps-manager-1.0.7/deps_manager/main.py`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.6/setup.py` & `deps-manager-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deps-manager',
-    version='1.0.6',
+    version='1.0.7',
     author="Harshada Tupe",
     author_email="harshadatupe8@gmail.com",
     license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3 :: Only",
                  "Operating System :: OS Independent"],
     python_requires='>=3.8',
```

