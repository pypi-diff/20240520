# Comparing `tmp/pymodins-0.1.7.tar.gz` & `tmp/pymodins-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-yeku4cnn\pymodins-0.1.7.tar", last modified: Sun May 19 22:53:35 2024, max compression
+gzip compressed data, was "C:\Users\Vimal\Desktop\pymodins\dist\.tmp-mc15hk6w\pymodins-0.1.8.tar", last modified: Mon May 20 09:39:16 2024, max compression
```

## Comparing `pymodins-0.1.7.tar` & `pymodins-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 22:53:35.428681 pymodins-0.1.7/
--rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     3746 2024-05-19 22:53:35.426700 pymodins-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3149 2024-05-19 19:56:43.000000 pymodins-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 22:53:35.410729 pymodins-0.1.7/pymodins/
--rw-rw-rw-   0        0        0      335 2024-05-19 19:57:21.000000 pymodins-0.1.7/pymodins/__init__.py
--rw-rw-rw-   0        0        0    44054 2024-05-19 22:53:08.000000 pymodins-0.1.7/pymodins/installer.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:53:35.424692 pymodins-0.1.7/pymodins.egg-info/
--rw-rw-rw-   0        0        0     3746 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-19 22:53:35.000000 pymodins-0.1.7/pymodins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 22:53:35.428681 pymodins-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      913 2024-05-19 19:59:41.000000 pymodins-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:39:16.279389 pymodins-0.1.8/
+-rw-rw-rw-   0        0        0     1085 2024-05-17 08:05:08.000000 pymodins-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3815 2024-05-20 09:39:16.278390 pymodins-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3184 2024-05-19 22:59:39.000000 pymodins-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 09:39:16.272554 pymodins-0.1.8/pymodins/
+-rw-rw-rw-   0        0        0      335 2024-05-20 09:38:36.000000 pymodins-0.1.8/pymodins/__init__.py
+-rw-rw-rw-   0        0        0    50270 2024-05-20 09:38:11.000000 pymodins-0.1.8/pymodins/installer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:39:16.278390 pymodins-0.1.8/pymodins.egg-info/
+-rw-rw-rw-   0        0        0     3815 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 09:39:16.000000 pymodins-0.1.8/pymodins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 09:39:16.279389 pymodins-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-05-20 09:38:47.000000 pymodins-0.1.8/setup.py
```

### Comparing `pymodins-0.1.7/LICENSE` & `pymodins-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodins-0.1.7/PKG-INFO` & `pymodins-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 0.1.7
+Version: 0.1.8
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
+Requires-Dist: pymsgbox
 
 # PYMODINS
 
-pymodins is a Python Modules Installer for Developers and Peoples who are new to python.
+[pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
 
 ```bash
 pip install pymodins
@@ -121,10 +122,9 @@
             8. Network Modules
             9. Build Modules
             10.Jupyter Modules
 
 Enter the number corresponding to the module type:
 ```
 
-# CONCLUSION
-### Thank you for using this Program
-### Feel free to ask your queries
+# ðŸŽ‰ Thank you for using this project!
+# Feel free to ask your queries ðŸ˜Š
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodins-0.1.7/README.md` & `pymodins-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PYMODINS
 
-pymodins is a Python Modules Installer for Developers and Peoples who are new to python.
+[pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
 
 ```bash
 pip install pymodins
@@ -105,10 +105,9 @@
             8. Network Modules
             9. Build Modules
             10.Jupyter Modules
 
 Enter the number corresponding to the module type:
 ```
 
-# CONCLUSION
-### Thank you for using this Program
-### Feel free to ask your queries
+# 🎉 Thank you for using this project!
+# Feel free to ask your queries 😊
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodins-0.1.7/pymodins/installer.py` & `pymodins-0.1.8/pymodins/installer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import os
 import getpass
 import sys
+import ctypes
+import subprocess
+import webbrowser
+import pymsgbox
 import urllib.request
 from datetime import datetime
 from rich.console import Console
 
 user = getpass.getuser()
-
+version="0.1.8"
 def internet(ping="https://google.com"):
     try:
         urllib.request.urlopen(ping)
         return True
     except:
         return False
 
@@ -36,34 +40,119 @@
     console.print("Creator: Nandhan K", style="bold cyan")
     console.print("Github: @github.com/Nandhan-KA", style="bold yellow")
 
 
 def sys_info():
     print("System Platform:", sys.platform)
     print("Python verion:", sys.version)
+    print("pymodins Version:",version )
 
 
 def clear():
     return os.system('cls')
 
 
 def log_mod(module_type, module_name, python_folder):
     timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     log_entry = f"{timestamp} - Installed {module_name} from {module_type} in {python_folder}"
     with open("module_installation_log.txt", "a") as log_file:
         log_file.write(log_entry + "\n")
 
+def install_vscode_build_tools():
+    def run_command(command):
+        result = subprocess.run(command, shell=True)
+        return result.returncode
+
+    def install_chocolatey():
+        choco_install_cmd = (
+            '@"%"SystemRoot%"\\System32\\WindowsPowerShell\\v1.0\\powershell.exe" '
+            '-NoProfile -InputFormat None -ExecutionPolicy Bypass -Command '
+            '"iex ((New-Object System.Net.WebClient).DownloadString(\'https://chocolatey.org/install.ps1\'))" '
+            '&& SET "PATH=%PATH%;%ALLUSERSPROFILE%\\chocolatey\\bin"'
+        )
+        return run_command(choco_install_cmd)
+
+    def install_vs_build_tools():
+        vs_build_tools_cmd = 'choco install -y visualstudio2019buildtools'
+        return run_command(vs_build_tools_cmd)
+
+    try:
+        is_admin = os.getuid() == 0
+    except AttributeError:
+        is_admin = ctypes.windll.shell32.IsUserAnAdmin() != 0
+
+    if not is_admin:
+        print("This script requires administrator privileges. Please run as an administrator.")
+        return False
+
+    choco_installed = subprocess.run("choco -v", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    if choco_installed.returncode != 0:
+        if install_chocolatey() != 0:
+            print("Failed to install Chocolatey.")
+            return False
+
+    if install_vs_build_tools() != 0:
+        print("Failed to install Visual Studio Build Tools.")
+        return False
+
+    print("Installation of Visual Studio Build Tools completed successfully.")
+    return True
+
+def install_rust():
+    def run_command(command):
+        result = subprocess.run(command, shell=True)
+        return result.returncode
+
+    def download_rust_installer():
+        url = "https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe"
+        installer_path = os.path.join(os.getenv('TEMP'), 'rustup-init.exe')
+        try:
+            urllib.request.urlretrieve(url, installer_path)
+            return installer_path
+        except Exception as e:
+            print(f"Failed to download Rust installer: {e}")
+            return None
+
+    def install_rustup(installer_path):
+        rustup_install_cmd = f'"{installer_path}" -y'
+        return run_command(rustup_install_cmd)
+
+    try:
+        is_admin = os.getuid() == 0
+    except AttributeError:
+        is_admin = ctypes.windll.shell32.IsUserAnAdmin() != 0
+
+    if not is_admin:
+        print("This script requires administrator privileges. Please run as an administrator.")
+        return False
+
+    installer_path = download_rust_installer()
+    if not installer_path:
+        print("Failed to download Rust installer. Opening the Rust installation webpage.")
+        webbrowser.open('https://www.rust-lang.org/tools/install')
+        return False
+
+    if install_rustup(installer_path) != 0:
+        print("Failed to install Rust. Opening the Rust installation webpage.")
+        webbrowser.open('https://www.rust-lang.org/tools/install')
+        return False
+
+    print("Installation of Rust completed successfully.")
+    return True
+
 
 # Module Lists
 basic_modules = [
     'numpy', 'pandas', 'matplotlib', 'scipy', 'requests', 'beautifulsoup4', 'seaborn', 'tqdm', 'docutils', 'pyyaml', 'python-dotenv', 'pillow',
 ]
 
 advanced_modules = [
-    'functools', 'logging', 'argparse', 'asyncio', 'collections', 'contextlib', 'dataclasses', 'pytz', 'pathlib', 'typing_extensions',
+    'argparse', 'asyncio', 'collections', 'contextlib', 'dataclasses', 'pytz', 'pathlib', 'typing_extensions',
+        'numpy', 'pandas', 'matplotlib', 'scipy', 'requests', 'beautifulsoup4', 'seaborn', 'tqdm', 'docutils', 'pyyaml', 'python-dotenv', 'pillow',
+
 ]
 
 science_modules = [
     'numpy', 'scipy', 'matplotlib', 'pandas', 'scikit-image', 'statsmodels', 'sympy', 'networkx', 'biopython',
     'h5py', 'numba', 'Cython', 'pandas-profiling', 'pytest', 'openpyxl', 'xlrd', 'scrapy', 'tabula-py', 'geopandas', 'pyproj'
 ]
 
@@ -90,15 +179,15 @@
 network_modules = [
     'socket', 'http.client', 'urllib', 'requests', 'socketIO-client', 'websockets', 'http.server', 'flask', 'django',
     'ftplib', 'smtplib', 'imaplib', 'poplib', 'telnetlib', 'paramiko', 'dnspython', 'pyftpdlib', 'twisted', 'pyngrok', 'snmp', 'netmiko', 'nmap', 'scapy'
 ]
 
 build_modules = [
     'pep517', 'setuptools', 'build', 'wheel', 'pytoml', 'cmake',
-    'pyproject.toml', 'ninja', 'meson', 'scons', 'bazel', 'autoconf', 'automake', 'libtool'
+    'pyproject.toml', 'ninja', 'meson', 'scons', 'bazel', 'autoconf', 'automake', 'libtool','rust'
 ]
 
 jupyter_modules = [
     'jupyter',
     'notebook', 'jupyterlab', 'nbconvert', 'nbformat', 'ipywidgets', 'ipykernel', 'voila', 'jupyter_contrib_nbextensions', 'jupyter_dash', 'jupyter_bokeh', 'jupytext', 'jupyterhub', 'jupyter_client', 'qtconsole'
 ]
 
@@ -168,14 +257,36 @@
                         print("(2)", versions[1])
                         python_folder = versions[int(
                             input("Select your Python folder (1 or 2): ")) - 1]
                     else:
                         python_folder = str(*versions)
 
                     for module in modules:
+                        if module == 'dlib':
+                            pymsgbox.alert("This Modules Required VSBuild Tools")
+                            print("Module dlib has to be installed after you have installed visual studio build tools")
+                            x = input("Do you want to install VS Build Tools? (y/n): ").lower()
+                            if x == "y":
+                                if install_vscode_build_tools():
+                                    print("Build tools installed successfully.")
+                                else:
+                                    print("Failed to install build tools.")
+                                    continue  
+                        
+                        if module == 'rust':
+                            pymsgbox.alert("This Modules Required VSBuild Tools")
+                            print("Module rust needs to be installed separately.")
+                            x = input("Do you want to install Rust? (y/n): ").lower()
+                            if x == "y":
+                                if install_rust():
+                                    print("Rust installed successfully.")
+                                else:
+                                    print("Failed to install Rust. Opening the Rust installation webpage.")
+                                    webbrowser.open('https://www.rust-lang.org/tools/install')
+                                    break
                         clear()
                         command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
                         os.system(command)
                         log_mod(selected_module_type, module, python_folder)
 
                     print("\nAll modules installed successfully.")
                     more = input("Do you want to install more? (Yes/No): ")
@@ -810,14 +921,25 @@
                 print("(2)", versions[1])
                 python_folder = versions[int(
                     input("Select your Python folder (1 or 2): ")) - 1]
             else:
                 python_folder = str(*versions)
 
             for module in modules:
+                if module == 'dlib':
+                    pymsgbox.alert("This Modules Required VSBuild Tools")
+                    print("Module dlib has to be installed after you have installed visual studio build tools")
+                    x = input("Do you want to install VS Build Tools? (y/n): ").lower()
+                    if x == "y":
+                        if install_vscode_build_tools():
+                            print("Build tools installed successfully.")
+                        else:
+                            print("Failed to install build tools.")
+                            continue  
+                        
                 clear()
                 command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
                 os.system(command)
                 log_mod(selected_module_type, module, python_folder)
 
             print("\nAll modules installed successfully.")
             more = input("Do you want to install more? (Yes/No): ")
@@ -989,14 +1111,27 @@
                 print("(2)", versions[1])
                 python_folder = versions[int(
                     input("Select your Python folder (1 or 2): ")) - 1]
             else:
                 python_folder = str(*versions)
 
             for module in modules:
+                if module == 'rust':
+                    pymsgbox.alert("This Modules Required VSBuild Tools")
+                    print("Module rust needs to be installed separately.")
+                    x = input("Do you want to install Rust? (y/n): ").lower()
+                    if x == "y":
+                        if install_rust():
+                            print("Rust installed successfully.")
+                        else:
+                            print("Failed to install Rust. Opening the Rust installation webpage.")
+                            webbrowser.open('https://www.rust-lang.org/tools/install')
+                            break  
+
+                    
                 clear()
                 command = f"cd C:\\Users\\{user}\\AppData\\Local\\Programs\\Python\\{python_folder}\\Scripts && pip.exe install {module}"
                 os.system(command)
                 log_mod(selected_module_type, module, python_folder)
 
             print("\nAll modules installed successfully.")
             more = input("Do you want to install more? (Yes/No): ")
```

### Comparing `pymodins-0.1.7/pymodins.egg-info/PKG-INFO` & `pymodins-0.1.8/pymodins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pymodins
-Version: 0.1.7
+Version: 0.1.8
 Summary: A module to install various Python packages.
 Home-page: https://github.com/Nandhan-KA/pymodins
 Author: Nandhan K
 Author-email: nandhan2003alamelu@gmail.com 
 Keywords: Python Module Installer,Python Package Installer,python modules installer,python package installer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
+Requires-Dist: pymsgbox
 
 # PYMODINS
 
-pymodins is a Python Modules Installer for Developers and Peoples who are new to python.
+[pymodins](https://github.com/Nandhan-KA/pymodins) is a Python Modules Installer for Developers and Peoples who are new to python.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pymodins.
 
 ```bash
 pip install pymodins
@@ -121,10 +122,9 @@
             8. Network Modules
             9. Build Modules
             10.Jupyter Modules
 
 Enter the number corresponding to the module type:
 ```
 
-# CONCLUSION
-### Thank you for using this Program
-### Feel free to ask your queries
+# ðŸŽ‰ Thank you for using this project!
+# Feel free to ask your queries ðŸ˜Š
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymodins-0.1.7/setup.py` & `pymodins-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pymodins",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
-        "rich"
+        "rich",
+        "pymsgbox"
     ],
     entry_points={
         "console_scripts": [
             "pymodins=pymodins.installer:run",
         ],
     },
     author="Nandhan K",
```

