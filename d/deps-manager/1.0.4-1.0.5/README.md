# Comparing `tmp/deps-manager-1.0.4.tar.gz` & `tmp/deps-manager-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps-manager-1.0.4.tar", last modified: Mon May 20 03:10:35 2024, max compression
+gzip compressed data, was "deps-manager-1.0.5.tar", last modified: Mon May 20 04:13:46 2024, max compression
```

## Comparing `deps-manager-1.0.4.tar` & `deps-manager-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 03:10:35.655918 deps-manager-1.0.4/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 03:10:35.655603 deps-manager-1.0.4/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.4/README.md
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 03:10:35.653424 deps-manager-1.0.4/deps_manager/
--rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.4/deps_manager/__init__.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     7887 2024-05-20 00:49:33.000000 deps-manager-1.0.4/deps_manager/dependencies.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     3661 2024-05-20 00:58:55.000000 deps-manager-1.0.4/deps_manager/main.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.4/deps_manager/utils.py
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 03:10:35.654980 deps-manager-1.0.4/deps_manager.egg-info/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/SOURCES.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/dependency_links.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/entry_points.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/requires.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/top_level.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 03:10:35.655987 deps-manager-1.0.4/setup.cfg
--rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 03:10:10.000000 deps-manager-1.0.4/setup.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:13:46.689212 deps-manager-1.0.5/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:13:46.688934 deps-manager-1.0.5/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.5/README.md
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:13:46.686478 deps-manager-1.0.5/deps_manager/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.5/deps_manager/__init__.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     8039 2024-05-20 04:12:08.000000 deps-manager-1.0.5/deps_manager/dependencies.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     3883 2024-05-20 04:12:23.000000 deps-manager-1.0.5/deps_manager/main.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.5/deps_manager/utils.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:13:46.688583 deps-manager-1.0.5/deps_manager.egg-info/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:13:46.000000 deps-manager-1.0.5/deps_manager.egg-info/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 04:13:46.000000 deps-manager-1.0.5/deps_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 04:13:46.000000 deps-manager-1.0.5/deps_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 04:13:46.000000 deps-manager-1.0.5/deps_manager.egg-info/entry_points.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 04:13:46.000000 deps-manager-1.0.5/deps_manager.egg-info/requires.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 04:13:46.000000 deps-manager-1.0.5/deps_manager.egg-info/top_level.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 04:13:46.689268 deps-manager-1.0.5/setup.cfg
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 04:13:35.000000 deps-manager-1.0.5/setup.py
```

### Comparing `deps-manager-1.0.4/README.md` & `deps-manager-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.4/deps_manager/dependencies.py` & `deps-manager-1.0.5/deps_manager/dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,23 +93,23 @@
 @handle_error
 def ensure_pipreqs_installed(pip_executable):
     """
     Ensure pipreqs is installed in the virtual environment.
     """
     # Check if pipreqs is installed
     try:
-        subprocess.run([pip_executable, 'pipreqs', '--version'], 
+        subprocess.run([pip_executable, 'show', 'pipreqs'], 
         check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     except subprocess.CalledProcessError:
         # If not installed, install it
         print("pipreqs is not installed. Installing now...")
         subprocess.run([pip_executable, 'install', 'pipreqs'], check=True)
 
 @handle_error
-def remove_unused_dependencies(venv_path):
+def remove_unused_dependencies(venv_path, source_code_full_path):
     """
     Remove unused dependencies.
     """
     pip_executable = 'pip'
     if venv_path:
         pip_executable = f"{venv_path}/bin/pip"
     
@@ -118,24 +118,26 @@
                                     capture_output=True, text=True)
     current_packages = set([line.split('==')[0] for line in current_reqs.stdout.splitlines()])
 
     # Ensure pipreqs is installed
     ensure_pipreqs_installed(pip_executable)
 
     # Delete existing requirements.txt if it exists
-    if os.path.exists("requirements.txt"):
-        os.remove("requirements.txt")
+    requirements_file_path = f"{source_code_full_path}/requirements.txt"
+
+    if os.path.exists(requirements_file_path):
+        os.remove(requirements_file_path)
 
     # Run pipreqs to generate a new requirements.txt
-    pipreqs_executable = 'pipreqs'
-    subprocess.run([pipreqs_executable, '.'], check=True,
+    pipreqs_executable = f"{venv_path}/bin/pipreqs"
+    subprocess.run([pipreqs_executable, source_code_full_path, '--encoding', 'utf-8'], check=True,
                     stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     # Read the generated requirements.txt to get used packages
-    with open("requirements.txt", "r") as f:
+    with open(requirements_file_path, "r") as f:
         used_packages = set(line.split("==")[0] for line in f.readlines())
 
     # Uninstall unused dependencies
     unused_packages = current_packages - used_packages
     
     for package in unused_packages:
         subprocess.run([pip_executable, 'uninstall', '-y', package], check=True)
@@ -175,15 +177,15 @@
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         return True
     except subprocess.CalledProcessError:
         return False
 
-def containerize_and_run_tests(language, tests_dir):
+def containerize_and_run_tests(tests_dir):
     """
     Containerize the project and run tests in a specified directory.
     """
     # Ensure the virtual environment is activated
     if not is_venv_activated():
         print("This command must be executed from within an active virtual environment.")
         print("Please activate your virtual environment and try again.")
```

### Comparing `deps-manager-1.0.4/deps_manager/main.py` & `deps-manager-1.0.5/deps_manager/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,32 +80,35 @@
     """Generate a lock file for dependencies."""
     lock_dependencies(lock_file, language, venv_path)
 
 @cli.command()
 @click.option('-v', '--venv_path', 
               prompt="Enter the path to the virtual environment",
               help="Path to the virtual environment")
-def remove_unused(venv_path):
+@click.option('-sc', '--source_code_full_path', 
+              prompt="Enter the path to the source code directory in virtual environment",
+              help="Path to the source code directory")
+def remove_unused(venv_path, source_code_full_path):
     """Remove unused dependencies.
     - Currently this feature is supported for python projects only.
     """
-    remove_unused_dependencies(venv_path)
+    remove_unused_dependencies(venv_path, source_code_full_path)
 
 @cli.command()
 @click.option('-td', '--tests_dir', required=True,
               prompt="Enter the tests directory name of the project",
               help="Name of the directory containing the project's tests")
-def containerize_and_test(language, tests_dir):
+def containerize_and_test(tests_dir):
     """
     Containerize and run the tests.
 
     Before running, ensure the following requirements are met:
     - Only applicable to Python projects.
     - Execute within an active virtual environment.
     - 'deps-manager' must be installed in the virtual environment.
     - Docker must be installed and running.
     """
-    containerize_and_run_tests(language, tests_dir)
+    containerize_and_run_tests(tests_dir)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `deps-manager-1.0.4/setup.py` & `deps-manager-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deps-manager',
-    version='1.0.4',
+    version='1.0.5',
     author="Harshada Tupe",
     author_email="harshadatupe8@gmail.com",
     license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3 :: Only",
                  "Operating System :: OS Independent"],
     python_requires='>=3.8',
```

