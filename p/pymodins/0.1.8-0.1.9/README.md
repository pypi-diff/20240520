# Comparing `tmp/pymodins-0.1.8.tar.gz` & `tmp/pymodins-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-mc15hk6w\pymodins-0.1.8.tar", last modified: Mon May 20 09:39:16 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-jvp3jpni\pymodins-0.1.9.tar", last modified: Mon May 20 10:03:22 2024, max compression
```

## Comparing `pymodins-0.1.8.tar` & `pymodins-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:39:16.279389 pymodins-0.1.8/
--rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3815 2024-05-20 09:39:16.278390 pymodins-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3184 2024-05-19 22:59:39.000000 pymodins-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 09:39:16.272554 pymodins-0.1.8/pymodins/
--rw-rw-rw-   0        0        0      335 2024-05-20 09:38:36.000000 pymodins-0.1.8/pymodins/__init__.py
--rw-rw-rw-   0        0        0    50270 2024-05-20 09:38:11.000000 pymodins-0.1.8/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:39:16.278390 pymodins-0.1.8/pymodins.egg-info/
--rw-rw-rw-   0        0        0     3815 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 09:39:16.279389 pymodins-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-05-20 09:38:47.000000 pymodins-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:03:22.285297 pymodins-0.1.9/
+-rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-05-20 10:03:22.284299 pymodins-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3232 2024-05-20 10:01:59.000000 pymodins-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 10:03:22.277313 pymodins-0.1.9/pymodins/
+-rw-rw-rw-   0        0        0      335 2024-05-20 10:03:07.000000 pymodins-0.1.9/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    54643 2024-05-20 09:57:56.000000 pymodins-0.1.9/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:03:22.283301 pymodins-0.1.9/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-05-20 10:03:22.000000 pymodins-0.1.9/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-20 10:03:22.000000 pymodins-0.1.9/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:03:22.000000 pymodins-0.1.9/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-20 10:03:22.000000 pymodins-0.1.9/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 10:03:22.000000 pymodins-0.1.9/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 10:03:22.000000 pymodins-0.1.9/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 10:03:22.285297 pymodins-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-05-20 10:03:01.000000 pymodins-0.1.9/setup.py
```

### Comparing `pymodins-0.1.8/LICENSE` & `pymodins-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-0.1.8/PKG-INFO` & `pymodins-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 0.1.8
+Version: 0.1.9
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -74,17 +74,17 @@
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 ```
-MIT License
+                            MIT License
 
-Copyright (c) 2024 Nandhan
+                    Copyright (c) 2024 Nandhan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymodins-0.1.8/README.md` & `pymodins-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 ```
-MIT License
+                            MIT License
 
-Copyright (c) 2024 Nandhan
+                    Copyright (c) 2024 Nandhan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymodins-0.1.8/pymodins/installer.py` & `pymodins-0.1.9/pymodins/installer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import os
 import getpass
 import sys
-import ctypes
+import urllib.request
+from datetime import datetime
 import subprocess
+import ctypes
 import webbrowser
 import pymsgbox
-import urllib.request
-from datetime import datetime
 from rich.console import Console
 
 user = getpass.getuser()
-version="0.1.8"
+
 def internet(ping="https://google.com"):
     try:
         urllib.request.urlopen(ping)
         return True
     except:
         return False
 
-
 def os_platform():
     platform = {
         'win32': 'Windows'
     }
     if sys.platform not in platform:
         return sys.platform
     return platform[sys.platform]
 
-
 def banner():
     console = Console()
 
     ascii_art = """
               \ |   \    \ | _ \ |  |   \    \ |    |  / 
              .  |  _ \  .  | |  |__ |  _ \  .  |    . <  
             _|\_|_/  _\_|\_|___/_| _|_/  _\_|\_|   _|\_\ 
@@ -40,21 +38,18 @@
     console.print("Creator: Nandhan K", style="bold cyan")
     console.print("Github: @github.com/Nandhan-KA", style="bold yellow")
 
 
 def sys_info():
     print("System Platform:", sys.platform)
     print("Python verion:", sys.version)
-    print("pymodins Version:",version )
-
 
 def clear():
     return os.system('cls')
 
-
 def log_mod(module_type, module_name, python_folder):
     timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     log_entry = f"{timestamp} - Installed {module_name} from {module_type} in {python_folder}"
     with open("module_installation_log.txt", "a") as log_file:
         log_file.write(log_entry + "\n")
 
 def install_vscode_build_tools():
@@ -135,24 +130,23 @@
         print("Failed to install Rust. Opening the Rust installation webpage.")
         webbrowser.open('https://www.rust-lang.org/tools/install')
         return False
 
     print("Installation of Rust completed successfully.")
     return True
 
-
 # Module Lists
+
 basic_modules = [
     'numpy', 'pandas', 'matplotlib', 'scipy', 'requests', 'beautifulsoup4', 'seaborn', 'tqdm', 'docutils', 'pyyaml', 'python-dotenv', 'pillow',
+      'datetime',  'statistics', 'glob',  'configparser'
 ]
 
 advanced_modules = [
-    'argparse', 'asyncio', 'collections', 'contextlib', 'dataclasses', 'pytz', 'pathlib', 'typing_extensions',
-        'numpy', 'pandas', 'matplotlib', 'scipy', 'requests', 'beautifulsoup4', 'seaborn', 'tqdm', 'docutils', 'pyyaml', 'python-dotenv', 'pillow',
-
+    'argparse', 'asyncio', 'dataclasses', 'pytz', 'pathlib', 'typing_extensions', 'jsonschema', 'pydantic'
 ]
 
 science_modules = [
     'numpy', 'scipy', 'matplotlib', 'pandas', 'scikit-image', 'statsmodels', 'sympy', 'networkx', 'biopython',
     'h5py', 'numba', 'Cython', 'pandas-profiling', 'pytest', 'openpyxl', 'xlrd', 'scrapy', 'tabula-py', 'geopandas', 'pyproj'
 ]
 
@@ -179,67 +173,45 @@
 network_modules = [
     'socket', 'http.client', 'urllib', 'requests', 'socketIO-client', 'websockets', 'http.server', 'flask', 'django',
     'ftplib', 'smtplib', 'imaplib', 'poplib', 'telnetlib', 'paramiko', 'dnspython', 'pyftpdlib', 'twisted', 'pyngrok', 'snmp', 'netmiko', 'nmap', 'scapy'
 ]
 
 build_modules = [
     'pep517', 'setuptools', 'build', 'wheel', 'pytoml', 'cmake',
-    'pyproject.toml', 'ninja', 'meson', 'scons', 'bazel', 'autoconf', 'automake', 'libtool','rust'
+    'pyproject.toml', 'ninja', 'meson', 'scons', 'bazel', 'autoconf', 'automake', 'libtool', 'rust'
 ]
 
 jupyter_modules = [
     'jupyter',
     'notebook', 'jupyterlab', 'nbconvert', 'nbformat', 'ipywidgets', 'ipykernel', 'voila', 'jupyter_contrib_nbextensions', 'jupyter_dash', 'jupyter_bokeh', 'jupytext', 'jupyterhub', 'jupyter_client', 'qtconsole'
 ]
 
-
 def installer():
     if internet():
         clear()
-        try:
-            if os_platform() == "Windows":
-                pass
-            else:
-                print("This software is only for Windows. Exiting.")
-                sys.exit()
-            banner()
+        banner()
+        sys_info()
 
-            print("""
-            1. Basic Modules
-            2. Advanced Modules
-            3. Science Modules
-            4. Computer Vision Modules
-            5. Machine Learning Modules
-            6. Deep Learning Modules
-            7. Full Stack Development Modules
-            8. Network Modules
-            9. Build Modules
-            10.Jupyter Modules
-            """)
-
-            selected_option = int(
-                input("Enter the number corresponding to the module type: "))
-            clear()
-            module_types = [
-                None,
-                'Basic Modules',
-                'Advanced Modules',
-                'Science Modules',
-                'Computer Vision Modules',
-                'Machine Learning Modules',
-                'Deep Learning Modules',
-                'Full Stack Development Modules',
-                'Network Modules',
-                'Build Modules',
-                'Jupyter Modules'
-            ]
+        module_types = [
+            'Basic Modules', 'Advanced Modules', 'Science Modules', 'Computer Vision Modules',
+            'Machine Learning Modules', 'Deep Learning Modules', 'Full Stack Development Modules',
+            'Network Modules', 'Build Modules', 'Jupyter Modules'
+        ]
+
+        print("\nPlease select the type of modules you want to install:\n")
+        for i, module_type in enumerate(module_types, 1):
+            print(f"{i}. {module_type}")
 
-            selected_module_type = module_types[selected_option]
+        try:
+            selected_module_type = int(
+                input("\nEnter the number corresponding to your choice: "))
 
-            if selected_module_type:
+            if 1 <= selected_module_type <= len(module_types):
+                clear()
+                selected_module_type = module_types[selected_module_type - 1]
                 print(f"\nSelected Module Type: {selected_module_type}")
                 print("Modules:")
                 modules = globals()[
                     selected_module_type.lower().replace(" ", "_")]
                 for i, module in enumerate(modules, 1):
                     print(f"{i}. {module}")
 
@@ -278,28 +250,35 @@
                             x = input("Do you want to install Rust? (y/n): ").lower()
                             if x == "y":
                                 if install_rust():
                                     print("Rust installed successfully.")
                                 else:
                                     print("Failed to install Rust. Opening the Rust installation webpage.")
                                     webbrowser.open('https://www.rust-lang.org/tools/install')
-                                    break
+                                    break  
+
                         clear()
                         command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
                         os.system(command)
                         log_mod(selected_module_type, module, python_folder)
 
                     print("\nAll modules installed successfully.")
                     more = input("Do you want to install more? (Yes/No): ")
                     if more.lower() in ["no", "n"]:
                         print(f"{user} Thank you for using.")
                         sys.exit()
                     elif more.lower() in ["yes", "y"]:
                         installer()
                 else:
+                    print("Modules:")
+                    modules = globals()[
+                        selected_module_type.lower().replace(" ", "_")]
+                    for i, module in enumerate(modules, 1):
+                        print(f"{i}. {module}")
+
                     module_index = int(input(
                         "Enter the number corresponding to the module to install (type '0' to exit): "))
 
                     if module_index == 0:
                         print(
                             "\nReload this program to install new modules of Python.")
                         sys.exit()
@@ -313,14 +292,36 @@
                         print(f"\nYou have two folders in your Python installation:")
                         print("(1)", versions[0])
                         print("(2)", versions[1])
                         python_folder = versions[int(
                             input("Select your Python folder (1 or 2): ")) - 1]
                     else:
                         python_folder = str(*versions)
+                    
+                    if selected_module == 'dlib':
+                        print("Module dlib has to be installed after you have installed visual studio build tools")
+                        x = input("Do you want to install VS Build Tools? (y/n): ").lower()
+                        if x == "y":
+                            if install_vscode_build_tools():
+                                print("Build tools installed successfully.")
+                            else:
+                                print("Failed to install build tools.")
+                                sys.exit()  
+                    
+                    if selected_module == 'rust':
+                        print("Module rust needs to be installed separately.")
+                        x = input("Do you want to install Rust? (y/n): ").lower()
+                        if x == "y":
+                            if install_rust():
+                                print("Rust installed successfully.")
+                            else:
+                                print("Failed to install Rust. Opening the Rust installation webpage.")
+                                webbrowser.open('https://www.rust-lang.org/tools/install')
+                                sys.exit()  
+
                     command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
                     os.system(command)
 
                     more = input("Do you want to install more? (Yes/No): ")
                     if more.lower() in ["no", "n"]:
                         print(f"{user} Thank you for using.")
                         sys.exit()
@@ -333,18 +334,17 @@
         except Exception as e:
             print("Error:", e, "\nPlease try again.")
             installer()
     else:
         print("No Internet Connection")
 
 
-
 def run():
     installer()
-    
+
 def install_basic_modules():
     selected_option = 1
     clear()
     module_types = [
         None,
         'Basic Modules',
         'Advanced Modules',
@@ -395,14 +395,20 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -485,14 +491,20 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
+                
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -575,14 +587,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -665,14 +682,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -755,14 +777,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -845,14 +872,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -945,14 +977,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -966,14 +1003,26 @@
                 print(f"\nYou have two folders in your Python installation:")
                 print("(1)", versions[0])
                 print("(2)", versions[1])
                 python_folder = versions[int(
                     input("Select your Python folder (1 or 2): ")) - 1]
             else:
                 python_folder = str(*versions)
+                
+            if selected_module == 'dlib':
+                pymsgbox.alert("This Modules Required VSBuild Tools")
+                print("Module dlib has to be installed after you have installed visual studio build tools")
+                x = input("Do you want to install VS Build Tools? (y/n): ").lower()
+                if x == "y":
+                    if install_vscode_build_tools():
+                        print("Build tools installed successfully.")
+                    else:
+                        print("Failed to install build tools.")
+                            
+                
             command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
             os.system(command)
 
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
@@ -1034,14 +1083,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -1137,14 +1191,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -1158,14 +1217,26 @@
                 print(f"\nYou have two folders in your Python installation:")
                 print("(1)", versions[0])
                 print("(2)", versions[1])
                 python_folder = versions[int(
                     input("Select your Python folder (1 or 2): ")) - 1]
             else:
                 python_folder = str(*versions)
+                
+            if selected_module == 'rust':
+                pymsgbox.alert("This Modules Required VSBuild Tools")
+                print("Module rust needs to be installed separately.")
+                x = input("Do you want to install Rust? (y/n): ").lower()
+                if x == "y":
+                    if install_rust():
+                        print("Rust installed successfully.")
+                    else:
+                        print("Failed to install Rust. Opening the Rust installation webpage.")
+                        webbrowser.open('https://www.rust-lang.org/tools/install')
+                        
             command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {selected_module}"
             os.system(command)
 
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
@@ -1227,14 +1298,19 @@
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
                 installer()
         else:
+            print("Modules:")
+            modules = globals()[
+            selected_module_type.lower().replace(" ", "_")]
+            for i, module in enumerate(modules, 1):
+                print(f"{i}. {module}")
             module_index = int(input(
                 "Enter the number corresponding to the module to install (type '0' to exit): "))
 
             if module_index == 0:
                 print(
                     "\nReload this program to install new modules of Python.")
                 sys.exit()
@@ -1256,8 +1332,8 @@
             os.system(command)
 
             more = input("Do you want to install more? (Yes/No): ")
             if more.lower() in ["no", "n"]:
                 print(f"{user} Thank you for using.")
                 sys.exit()
             elif more.lower() in ["yes", "y"]:
-                installer()
+                installer()
```

### Comparing `pymodins-0.1.8/pymodins.egg-info/PKG-INFO` & `pymodins-0.1.9/pymodins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 0.1.8
+Version: 0.1.9
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -74,17 +74,17 @@
 
 Please make sure to update tests as appropriate.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 ```
-MIT License
+                            MIT License
 
-Copyright (c) 2024 Nandhan
+                    Copyright (c) 2024 Nandhan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pymodins-0.1.8/setup.py` & `pymodins-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymodins",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         "rich",
         "pymsgbox"
     ],
     entry_points={
         "console_scripts": [
```

