# Comparing `tmp/mrfix-6.0.3.tar.gz` & `tmp/mrfix-6.0.4.tar.gz`

## Comparing `mrfix-6.0.3.tar` & `mrfix-6.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-6.0.3/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-6.0.3/src/mrfix/__init__.py
--rw-r--r--   0        0        0    67259 2020-02-02 00:00:00.000000 mrfix-6.0.3/src/mrfix/mrfix.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 mrfix-6.0.3/src/mrfix/mrfix.zip
--rw-r--r--   0        0        0    21461 2020-02-02 00:00:00.000000 mrfix-6.0.3/README.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 mrfix-6.0.3/pyproject.toml
--rw-r--r--   0        0        0    21993 2020-02-02 00:00:00.000000 mrfix-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-6.0.4/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-6.0.4/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    67260 2020-02-02 00:00:00.000000 mrfix-6.0.4/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 mrfix-6.0.4/src/mrfix/mrfix.zip
+-rw-r--r--   0        0        0    21404 2020-02-02 00:00:00.000000 mrfix-6.0.4/README.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 mrfix-6.0.4/pyproject.toml
+-rw-r--r--   0        0        0    21936 2020-02-02 00:00:00.000000 mrfix-6.0.4/PKG-INFO
```

### Comparing `mrfix-6.0.3/LICENZE` & `mrfix-6.0.4/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-6.0.3/src/mrfix/mrfix.py` & `mrfix-6.0.4/src/mrfix/mrfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1087,15 +1087,15 @@
             return message
             
 
     @staticmethod
     def get_text_list_in_select(driver, select_xpath):
         try:
             #Find the select element by its xpath
-            select_element = driver.find_element_by_xpath(select_xpath)
+            select_element = driver.find_element(By.XPATH, select_xpath)
 
             # Get all option elements inside the select
             options = select_element.find_elements_by_tag_name("option")
 
             # Create an empty list to store the text values
             text_values_list = []
```

### Comparing `mrfix-6.0.3/src/mrfix/mrfix.zip` & `mrfix-6.0.4/src/mrfix/mrfix.zip`

 * *Files identical despite different names*

### Comparing `mrfix-6.0.3/README.md` & `mrfix-6.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,21 @@
     
     • the uniformity of the approach of all methods to the form of organization of input data, which simplifies the memorization and application of methods of module
     
 Link of source code:
 
 https://github.com/MrFix-Autotesting-Framework/MrFix-Autotesting-Framework
 
-ATTENTION! You can check the security of using the MrFix module on this website:  https://app.snyk.io/advisor/python/mrfix
-
 All methods are static (@staticmethod)
 
 If there is a variable "driver" in the method, it is a variable of the Selenium Webdriver type. For example: driver = webdriver.Chrome()
 
+What's new in version 6.0.4 ?
+    - Code optimization, fixed bugs
+
 What's new in version 6.0.3 ?
     - Added the method get_text_list_in_select(driver, select_xpath) in class MrFixUI
         This method This method returns, as a list of text strings, a list of all dropdown list values with xpath = select_xpath if successful, or error text otherwise.
 
 What's new in version 6.0.2 ?
     - The descriptions of the following methods have been changed:
         post_request(requests_url: str, requests_body: dict, requests_headers: dict, pre_script: str = None, auth: list = None)
```

### Comparing `mrfix-6.0.3/pyproject.toml` & `mrfix-6.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "6.0.3"
+version = "6.0.4"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Perfomance Testing."
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mrfix-6.0.3/PKG-INFO` & `mrfix-6.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mrfix
-Version: 6.0.3
+Version: 6.0.4
 Summary: The Mr Fix module is designed to create autotests written in Python for testing UI, API, PostgreSQL, Security and Perfomance Testing.
 Project-URL: Homepage, https://github.com/MrFix-Autotesting-Framework
 Author-email: Valerii Zhuravlev <valerzhurav2011@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -27,20 +27,21 @@
     
     • the uniformity of the approach of all methods to the form of organization of input data, which simplifies the memorization and application of methods of module
     
 Link of source code:
 
 https://github.com/MrFix-Autotesting-Framework/MrFix-Autotesting-Framework
 
-ATTENTION! You can check the security of using the MrFix module on this website:  https://app.snyk.io/advisor/python/mrfix
-
 All methods are static (@staticmethod)
 
 If there is a variable "driver" in the method, it is a variable of the Selenium Webdriver type. For example: driver = webdriver.Chrome()
 
+What's new in version 6.0.4 ?
+    - Code optimization, fixed bugs
+
 What's new in version 6.0.3 ?
     - Added the method get_text_list_in_select(driver, select_xpath) in class MrFixUI
         This method This method returns, as a list of text strings, a list of all dropdown list values with xpath = select_xpath if successful, or error text otherwise.
 
 What's new in version 6.0.2 ?
     - The descriptions of the following methods have been changed:
         post_request(requests_url: str, requests_body: dict, requests_headers: dict, pre_script: str = None, auth: list = None)
```

