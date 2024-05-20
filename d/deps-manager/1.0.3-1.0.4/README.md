# Comparing `tmp/deps-manager-1.0.3.tar.gz` & `tmp/deps-manager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps-manager-1.0.3.tar", last modified: Wed May  8 19:10:08 2024, max compression
+gzip compressed data, was "deps-manager-1.0.4.tar", last modified: Mon May 20 03:10:35 2024, max compression
```

## Comparing `deps-manager-1.0.3.tar` & `deps-manager-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-08 19:10:08.167495 deps-manager-1.0.3/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      297 2024-05-08 19:10:08.167222 deps-manager-1.0.3/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.3/README.md
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-08 19:10:08.165547 deps-manager-1.0.3/deps_manager/
--rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.3/deps_manager/__init__.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     8993 2024-05-08 18:53:47.000000 deps-manager-1.0.3/deps_manager/dependencies.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     3000 2024-05-08 19:08:21.000000 deps-manager-1.0.3/deps_manager/main.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.3/deps_manager/utils.py
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-08 19:10:08.166746 deps-manager-1.0.3/deps_manager.egg-info/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      297 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/SOURCES.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/dependency_links.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/entry_points.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       12 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/requires.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-08 19:10:08.000000 deps-manager-1.0.3/deps_manager.egg-info/top_level.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-08 19:10:08.167571 deps-manager-1.0.3/setup.cfg
--rw-r--r--   0 harshadatupe   (501) staff       (20)      551 2024-05-08 19:05:20.000000 deps-manager-1.0.3/setup.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 03:10:35.655918 deps-manager-1.0.4/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 03:10:35.655603 deps-manager-1.0.4/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.4/README.md
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 03:10:35.653424 deps-manager-1.0.4/deps_manager/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.4/deps_manager/__init__.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     7887 2024-05-20 00:49:33.000000 deps-manager-1.0.4/deps_manager/dependencies.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     3661 2024-05-20 00:58:55.000000 deps-manager-1.0.4/deps_manager/main.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.4/deps_manager/utils.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 03:10:35.654980 deps-manager-1.0.4/deps_manager.egg-info/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/entry_points.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/requires.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 03:10:35.000000 deps-manager-1.0.4/deps_manager.egg-info/top_level.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 03:10:35.655987 deps-manager-1.0.4/setup.cfg
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 03:10:10.000000 deps-manager-1.0.4/setup.py
```

### Comparing `deps-manager-1.0.3/README.md` & `deps-manager-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.3/deps_manager/dependencies.py` & `deps-manager-1.0.4/deps_manager/dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,28 +16,29 @@
     """
     # Create the divider
     divider = "#" * 67
 
     # Print with specified spacing
     print("\n" * spacing + divider)
 
-
 @handle_error
 def install_dependencies(requirements_file, language, venv_path):
     """
     Installs dependencies.
     """
     if language == 'python':
         pip_executable = 'pip'
         if venv_path:
             pip_executable = f"{venv_path}/bin/pip"  # For Linux and MacOS
-        subprocess.run([pip_executable, 'install', '-r', requirements_file], check=True)
+        subprocess.run([pip_executable, 'install', '-r',
+                        requirements_file], check=True)
     
     elif language == 'cpp':
-        subprocess.run(['conan', 'install', '-r', requirements_file], check=True)
+        subprocess.run(['conan', 'install', '-r', requirements_file],
+                        check=True)
 
 @handle_error
 def uninstall_dependency(package, language, venv_path):
     """
     Uninstalls dependencies.
     """
     if language == 'python':
@@ -66,30 +67,32 @@
     """
     Updates dependencies.
     """
     if language == 'python':
         pip_executable = 'pip'
         if venv_path:
             pip_executable = f"{venv_path}/bin/pip"  # For Linux and MacOS
-        subprocess.run([pip_executable, 'install', '--upgrade', '-r', requirements_file], check=True)
+        subprocess.run([pip_executable, 'install', '--upgrade', '-r',
+                        requirements_file], check=True)
     elif language == 'cpp':
-        subprocess.run(['conan', 'update', '-r', requirements_file], check=True)
+        subprocess.run(['conan', 'install', '--update', requirements_file], check=True)
 
 @handle_error
 def lock_dependencies(requirements_lock_file, language, venv_path):
     """
     Build a lockfile to lock current dependencies.
     """
     if language == 'python':
+        pip_executable = 'pip'
         if venv_path:
-            python_executable = f"{venv_path}/bin/python"
-            subprocess.run([f"{venv_path}/bin/pip", "freeze"], stdout=open(requirements_lock_file, "w"), check=True)
+            pip_executable = f"{venv_path}/bin/pip" # For Linux and MacOS
+        subprocess.run([pip_executable, 'freeze'],
+                        stdout=open(requirements_lock_file, "w"), check=True)
     elif language == 'cpp':
-        subprocess.run(['conan', 'lock', '-r', requirements_lock_file, '-o', lock_file], check=True)
-
+        subprocess.run(['conan', 'lock', requirements_lock_file], check=True)
 
 @handle_error
 def ensure_pipreqs_installed(pip_executable):
     """
     Ensure pipreqs is installed in the virtual environment.
     """
     # Check if pipreqs is installed
@@ -97,115 +100,89 @@
         subprocess.run([pip_executable, 'pipreqs', '--version'], 
         check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     except subprocess.CalledProcessError:
         # If not installed, install it
         print("pipreqs is not installed. Installing now...")
         subprocess.run([pip_executable, 'install', 'pipreqs'], check=True)
 
-
 @handle_error
-def remove_unused_dependencies(language, venv_path):
+def remove_unused_dependencies(venv_path):
     """
     Remove unused dependencies.
     """
-    if language == 'python':
-        pip_executable = 'pip'
-        if venv_path:
-            pip_executable = f"{venv_path}/bin/pip"
-        
-        # Get current packages
-        current_reqs = subprocess.run([pip_executable, 'freeze'], capture_output=True, text=True)
-        current_packages = set([line.split('==')[0] for line in current_reqs.stdout.splitlines()])
-
-        # Ensure pipreqs is installed
-        ensure_pipreqs_installed(pip_executable)
-
-        # Delete existing requirements.txt if it exists
-        if os.path.exists("requirements.txt"):
-            os.remove("requirements.txt")
-
-        # Run pipreqs to generate a new requirements.txt
-        pipreqs_executable = 'pipreqs'
-        subprocess.run([pipreqs_executable, '.'], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-        # Read the generated requirements.txt to get used packages
-        with open("requirements.txt", "r") as f:
-            used_packages = set(line.split("==")[0] for line in f.readlines())
-
-        # Uninstall unused dependencies
-        unused_packages = current_packages - used_packages
-        
-        for package in unused_packages:
-            subprocess.run([pip_executable, 'uninstall', '-y', package], check=True)
-        
+    pip_executable = 'pip'
+    if venv_path:
+        pip_executable = f"{venv_path}/bin/pip"
+    
+    # Get current packages
+    current_reqs = subprocess.run([pip_executable, 'freeze'],
+                                    capture_output=True, text=True)
+    current_packages = set([line.split('==')[0] for line in current_reqs.stdout.splitlines()])
+
+    # Ensure pipreqs is installed
+    ensure_pipreqs_installed(pip_executable)
+
+    # Delete existing requirements.txt if it exists
+    if os.path.exists("requirements.txt"):
+        os.remove("requirements.txt")
+
+    # Run pipreqs to generate a new requirements.txt
+    pipreqs_executable = 'pipreqs'
+    subprocess.run([pipreqs_executable, '.'], check=True,
+                    stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+
+    # Read the generated requirements.txt to get used packages
+    with open("requirements.txt", "r") as f:
+        used_packages = set(line.split("==")[0] for line in f.readlines())
+
+    # Uninstall unused dependencies
+    unused_packages = current_packages - used_packages
+    
+    for package in unused_packages:
+        subprocess.run([pip_executable, 'uninstall', '-y', package], check=True)
+    
+    print_divider(2)
+    print("Packages that were installed:")
+    for package in current_packages:
+        print(f" - {package}")
+    print_divider()
+    print_divider(2)
+    print("Packages that are needed for the project:")
+    for package in used_packages:
+        print(f" - {package}")
+    print_divider()
+
+    if unused_packages:
         print_divider(2)
-        print("Packages that were installed:")
-        for package in current_packages:
+        print("The following unused packages have been removed:")
+        for package in unused_packages:
             print(f" - {package}")
         print_divider()
+    else:
         print_divider(2)
-        print("Packages that are needed for the project:")
-        for package in used_packages:
-            print(f" - {package}")
+        print("No unused packages to remove.")
         print_divider()
 
-        if unused_packages:
-            print_divider(2)
-            print("The following unused packages have been removed:")
-            for package in unused_packages:
-                print(f" - {package}")
-            print_divider()
-        else:
-            print_divider(2)
-            print("No unused packages to remove.")
-            print_divider()
-    elif language == 'cpp':
-        # Get the Conan dependency tree
-        conan_executable = 'conan'
-        if venv_path:
-            conan_executable = f"{venv_path}/bin/conan"
-        
-        # Fetch the full dependency graph for the project
-        dependency_graph = subprocess.run([conan_executable, 'info', '.'], capture_output=True, text=True)
-        
-        # Parse the dependency tree
-        dependency_json = json.loads(dependency_graph.stdout)
-        
-        # Find unused dependencies
-        unused_dependencies = set()
-        # Custom logic to identify unused dependencies based on your C++ project's structure
-        
-        if unused_dependencies:
-            print("The following unused C++ packages have been removed:")
-            for unused_dep in unused_dependencies:
-                subprocess.run([conan_executable, 'remove', '--force', unused_dep], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-                print(f" - {unused_dep}")
-        else:
-            print("No unused C++ packages to remove.")
-
-
 def is_venv_activated():
     """Helper function to check if virtual environment is activated."""
     return 'VIRTUAL_ENV' in os.environ
 
-
 def is_deps_manager_installed():
     """Helper function to check if deps-manager is installed in venv."""
     try:
         subprocess.run(
             ['deps-manager', '--version'],
             check=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         return True
     except subprocess.CalledProcessError:
         return False
 
-
 def containerize_and_run_tests(language, tests_dir):
     """
     Containerize the project and run tests in a specified directory.
     """
     # Ensure the virtual environment is activated
     if not is_venv_activated():
         print("This command must be executed from within an active virtual environment.")
```

### Comparing `deps-manager-1.0.3/deps_manager/main.py` & `deps-manager-1.0.4/deps_manager/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 """
-The main.py module acts as a cli interface to parse the user inputs in command line
+The main.py module acts as a cli interface to parse
+the user inputs in command line
 and executes related function from dependencies.py module.
 """
 # Third party library imports
 import click
 
 # Local application imports
 from .dependencies import *
 
 
 def common_options(function):
     """
     Decorator to define common click options.
     """
-    function = click.option('-v', '--venv_path', prompt="Enter the path to the virtual environment",
+    function = click.option('-v', '--venv_path', 
+                            prompt="Enter the path to the virtual environment",
                             help="Path to the virtual environment")(function)
-    function = click.option('-l', '--language', prompt="Enter the language", type=click.Choice(['python', 'cpp']),
+    function = click.option('-l', '--language',
+                            prompt="Enter the language",
+                            type=click.Choice(['python', 'cpp']),
                             help="Project language to manage the dependencies")(function)
     return function
 
 def requirements_option(function):
     """
     Decorator for the requirements file option.
     """
-    return click.option('-r', '--requirements_file', prompt="Enter the requirements.txt file name", required=True,
+    return click.option('-r', '--requirements_file',
+                        prompt="Enter the requirements.txt file name",
+                        required=True,
                         help="Path to requirements file")(function)
 
 
 @click.group()
 @click.version_option()
 def cli():
     """Command Line Interface for managing project dependencies."""
@@ -39,15 +45,17 @@
 @requirements_option
 def install(venv_path, requirements_file, language):
     """Install dependencies from a requirements file."""
     install_dependencies(requirements_file, language, venv_path)
 
 @cli.command()
 @common_options
-@click.option('-p', '--package_name', prompt="Enter the package name you need to uninstall", required=True,
+@click.option('-p', '--package_name',
+              prompt="Enter the package name you need to uninstall",
+              required=True,
               help="Package name to uninstall")
 def uninstall(venv_path, language, package_name):
     """Uninstall a package."""
     uninstall_dependency(package_name, language, venv_path)
 
 @cli.command()
 @common_options
@@ -60,30 +68,44 @@
 @requirements_option
 def update(venv_path, requirements_file, language):
     """Update dependencies from a requirements file."""
     update_dependencies(requirements_file, language, venv_path)
 
 @cli.command()
 @common_options
-@click.option('-lf', '--lock_file', prompt="Enter the lock file name with its absolute path", required=True,
+@click.option('-lf', '--lock_file',
+              prompt="Enter the lock file name with its absolute path",
+              required=True,
               help="Name of the lock file to lock and save dependencies")
 def lock(venv_path, language, lock_file):
     """Generate a lock file for dependencies."""
     lock_dependencies(lock_file, language, venv_path)
 
 @cli.command()
-@common_options
-def remove_unused(venv_path, language):
-    """Remove unused dependencies."""
-    remove_unused_dependencies(language, venv_path)
+@click.option('-v', '--venv_path', 
+              prompt="Enter the path to the virtual environment",
+              help="Path to the virtual environment")
+def remove_unused(venv_path):
+    """Remove unused dependencies.
+    - Currently this feature is supported for python projects only.
+    """
+    remove_unused_dependencies(venv_path)
 
 @cli.command()
 @click.option('-td', '--tests_dir', required=True,
               prompt="Enter the tests directory name of the project",
               help="Name of the directory containing the project's tests")
 def containerize_and_test(language, tests_dir):
-    """Containerize and run the tests."""
+    """
+    Containerize and run the tests.
+
+    Before running, ensure the following requirements are met:
+    - Only applicable to Python projects.
+    - Execute within an active virtual environment.
+    - 'deps-manager' must be installed in the virtual environment.
+    - Docker must be installed and running.
+    """
     containerize_and_run_tests(language, tests_dir)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `deps-manager-1.0.3/setup.py` & `deps-manager-1.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deps-manager',
-    version='1.0.3',
+    version='1.0.4',
     author="Harshada Tupe",
     author_email="harshadatupe8@gmail.com",
     license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3 :: Only",
                  "Operating System :: OS Independent"],
     python_requires='>=3.8',
@@ -14,9 +14,10 @@
         'console_scripts': [
             'deps-manager = deps_manager.main:cli',
         ],
     },
     install_requires=[
         'click',
         'conan',
+        'pipreqs',
     ],
 )
```

