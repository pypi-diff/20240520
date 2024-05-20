# Comparing `tmp/mrfix-6.0.2.tar.gz` & `tmp/mrfix-6.0.3.tar.gz`

## Comparing `mrfix-6.0.2.tar` & `mrfix-6.0.3.tar`

### file list

```diff
@@ -1,10 +1,7 @@
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mrfix-6.0.2/LICENZE
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mrfix-6.0.2/token.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-6.0.2/src/mrfix/__init__.py
--rw-r--r--   0        0        0    65333 2020-02-02 00:00:00.000000 mrfix-6.0.2/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 mrfix-6.0.2/src/mrfix/Метод проверки АПИ-запроса на атаки.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 mrfix-6.0.2/src/mrfix/Нагрузочное тестирование - методы.txt
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-6.0.2/.gitignore
--rw-r--r--   0        0        0    21050 2020-02-02 00:00:00.000000 mrfix-6.0.2/README.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mrfix-6.0.2/pyproject.toml
--rw-r--r--   0        0        0    21539 2020-02-02 00:00:00.000000 mrfix-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-6.0.3/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-6.0.3/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    67259 2020-02-02 00:00:00.000000 mrfix-6.0.3/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 mrfix-6.0.3/src/mrfix/mrfix.zip
+-rw-r--r--   0        0        0    21461 2020-02-02 00:00:00.000000 mrfix-6.0.3/README.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 mrfix-6.0.3/pyproject.toml
+-rw-r--r--   0        0        0    21993 2020-02-02 00:00:00.000000 mrfix-6.0.3/PKG-INFO
```

### Comparing `mrfix-6.0.2/LICENZE` & `mrfix-6.0.3/LICENZE`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 MIT License  
-Copyright (c) 2023 Valerii Zhuravlev
+Copyright (c) 2022 Valerii Zhuravlev  
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:  
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.  
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mrfix-6.0.2/src/mrfix/mrfix.py` & `mrfix-6.0.3/src/mrfix/mrfix.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pyperclip
 import json
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from datetime import datetime
 from bs4 import BeautifulSoup
 import subprocess
-import psycopg2
+import psycopg2    # pip install psycopg2-binary
 import sh
 import csv
 import socket
 from cryptography.fernet import Fernet
 import os
 import requests
 import concurrent.futures
@@ -1081,19 +1081,72 @@
             driver.execute_script("arguments[0].removeAttribute('disabled');", element)
             print(f"Element with XPath '{element_xpath}' enabled now.")
             return  True
         except Exception as e:
             message = f"An error occurred: {e}"
             print(message)
             return message
+            
+
+    @staticmethod
+    def get_text_list_in_select(driver, select_xpath):
+        try:
+            #Find the select element by its xpath
+            select_element = driver.find_element_by_xpath(select_xpath)
+
+            # Get all option elements inside the select
+            options = select_element.find_elements_by_tag_name("option")
+
+            # Create an empty list to store the text values
+            text_values_list = []
+
+            # Extract text from each option element and add it to the list
+            for option in options:
+                text_values_list.append(option.text)
+
+            # Return this list
+            return text_values_list
+
+        except NoSuchElementException:
+            # If the element is not found, return an error code
+            return f"Element with xpath {select_xpath} not found"
+        except Exception as e:
+            # If other errors occur, return an error message
+            return f"An error occurred: {e}"
+
 
 
 class MrFixSQL:
 
     @staticmethod
+    def run_openvpn_commands(ovpn_file):
+        try:
+            # Stop the OpenVPN service
+            stop_command = "sudo systemctl stop openvpn@server"
+            subprocess.run(stop_command, shell=True, check=True)
+
+            # Enable the OpenVPN service
+            enable_command = "sudo systemctl enable openvpn@server.service"
+            subprocess.run(enable_command, shell=True, check=True)
+
+            # Start OpenVPN client with the specified configuration file
+            config_file = ovpn_file
+            openvpn_command = f"sudo openvpn --client --config {config_file}"
+            subprocess.run(openvpn_command, shell=True, check=True)
+
+            # If all commands succeed, return True
+            return True
+
+        except subprocess.CalledProcessError as e:
+            # If any command fails, return the error message
+            return f"Error: {e}"
+
+
+
+    @staticmethod
     # Launches OpenVPN with a command with administrator privileges on the Linux command line using the ".ovpn" settings file
     # Returns a success message or error text
     def run_openvpn_for_linux(config_path: str, pas: str):
         try:
             with sh.contrib.sudo(pas, _with=True):
                 rezult = subprocess.run(['sudo', '-S', 'openvpn', '--client', '--config', config_path])
```

### Comparing `mrfix-6.0.2/README.md` & `mrfix-6.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Module MrFix
 
 General information 
 
-The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Loading.
+The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Perfomance Testing.
 Mr Fix is a module with a set of decorators methods for writing autotests for frontend and backend. It contains all the basic methods needed to write UI-, API- and SQL-autotests. 
 It is an open source product. It is distributed on the terms of free software (i.e. it allows you to legally use it, including on commercial projects). Supports the principle of "all in one and in one place". 
 Allows a beginner (and not just a beginner) specialist in quality control automation not to search for a solution through various manuals and websites, but to immediately find it and use proven methods of work in the MrFix module.
 
 The advantages of the module are also:
 
     • reducing the amount of code when using methods of  module;
@@ -21,14 +21,18 @@
 
 ATTENTION! You can check the security of using the MrFix module on this website:  https://app.snyk.io/advisor/python/mrfix
 
 All methods are static (@staticmethod)
 
 If there is a variable "driver" in the method, it is a variable of the Selenium Webdriver type. For example: driver = webdriver.Chrome()
 
+What's new in version 6.0.3 ?
+    - Added the method get_text_list_in_select(driver, select_xpath) in class MrFixUI
+        This method This method returns, as a list of text strings, a list of all dropdown list values with xpath = select_xpath if successful, or error text otherwise.
+
 What's new in version 6.0.2 ?
     - The descriptions of the following methods have been changed:
         post_request(requests_url: str, requests_body: dict, requests_headers: dict, pre_script: str = None, auth: list = None)
         get_request(requests_url: str, requests_headers: dict, auth: list = None)
         put_request(requests_url: str, requests_body: dict, requests_headers: dict, pre_script: str = None, auth: list = None)
         delete_request(requests_url: str, requests_headers: dict, auth: list = None)
 
@@ -399,9 +403,11 @@
 
     def get_separator():
     # get system's separator in files path (It is for example for Windows "\", for Linux "/")
 
     def change_element_text(driver, span_xpath, new_text):
     # - modify the innerHTML of an element identified by XPath.
 
+    def get_text_list_in_select(driver, select_xpath):
+    # - get the list of text of element with type "select'
```

### Comparing `mrfix-6.0.2/pyproject.toml` & `mrfix-6.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "6.0.2"
+version = "6.0.3"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
-description = "A package with a set of decorator-methods for automatic testing for UI, API and PostgreSQL"
+description = "The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Perfomance Testing."
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [     
   "Programming Language :: Python :: 3",     
   "License :: OSI Approved :: MIT License",     
   "Operating System :: OS Independent", 
 ]
```

### Comparing `mrfix-6.0.2/PKG-INFO` & `mrfix-6.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mrfix
-Version: 6.0.2
-Summary: A package with a set of decorator-methods for automatic testing for UI, API and PostgreSQL
+Version: 6.0.3
+Summary: The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Perfomance Testing.
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 Module MrFix
 
 General information 
 
-The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Loading.
+The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Perfomance Testing.
 Mr Fix is a module with a set of decorators methods for writing autotests for frontend and backend. It contains all the basic methods needed to write UI-, API- and SQL-autotests. 
 It is an open source product. It is distributed on the terms of free software (i.e. it allows you to legally use it, including on commercial projects). Supports the principle of "all in one and in one place". 
 Allows a beginner (and not just a beginner) specialist in quality control automation not to search for a solution through various manuals and websites, but to immediately find it and use proven methods of work in the MrFix module.
 
 The advantages of the module are also:
 
     • reducing the amount of code when using methods of  module;
@@ -33,14 +33,18 @@
 
 ATTENTION! You can check the security of using the MrFix module on this website:  https://app.snyk.io/advisor/python/mrfix
 
 All methods are static (@staticmethod)
 
 If there is a variable "driver" in the method, it is a variable of the Selenium Webdriver type. For example: driver = webdriver.Chrome()
 
+What's new in version 6.0.3 ?
+    - Added the method get_text_list_in_select(driver, select_xpath) in class MrFixUI
+        This method This method returns, as a list of text strings, a list of all dropdown list values with xpath = select_xpath if successful, or error text otherwise.
+
 What's new in version 6.0.2 ?
     - The descriptions of the following methods have been changed:
         post_request(requests_url: str, requests_body: dict, requests_headers: dict, pre_script: str = None, auth: list = None)
         get_request(requests_url: str, requests_headers: dict, auth: list = None)
         put_request(requests_url: str, requests_body: dict, requests_headers: dict, pre_script: str = None, auth: list = None)
         delete_request(requests_url: str, requests_headers: dict, auth: list = None)
 
@@ -411,9 +415,11 @@
 
     def get_separator():
     # get system's separator in files path (It is for example for Windows "\", for Linux "/")
 
     def change_element_text(driver, span_xpath, new_text):
     # - modify the innerHTML of an element identified by XPath.
 
+    def get_text_list_in_select(driver, select_xpath):
+    # - get the list of text of element with type "select'
```

