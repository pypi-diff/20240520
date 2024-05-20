# Comparing `tmp/liteium-1.0.3.tar.gz` & `tmp/liteium-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteium-1.0.3.tar", last modified: Mon May 13 02:12:19 2024, max compression
+gzip compressed data, was "liteium-1.0.4.tar", last modified: Mon May 20 20:34:53 2024, max compression
```

## Comparing `liteium-1.0.3.tar` & `liteium-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:12:19.878422 liteium-1.0.3/
--rw-rw-rw-   0        0        0      853 2024-05-13 02:12:19.877424 liteium-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-05-11 04:46:56.000000 liteium-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 02:12:19.843451 liteium-1.0.3/liteium/
--rw-rw-rw-   0        0        0       19 2024-05-11 18:49:55.000000 liteium-1.0.3/liteium/__init__.py
--rw-rw-rw-   0        0        0    10102 2024-05-13 02:09:51.000000 liteium-1.0.3/liteium/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:12:19.875426 liteium-1.0.3/liteium.egg-info/
--rw-rw-rw-   0        0        0      853 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 02:12:19.000000 liteium-1.0.3/liteium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 02:12:19.878422 liteium-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-05-13 02:11:49.000000 liteium-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:34:53.560053 liteium-1.0.4/
+-rw-rw-rw-   0        0        0      853 2024-05-20 20:34:53.557055 liteium-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-05-11 04:46:56.000000 liteium-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 20:34:53.511369 liteium-1.0.4/liteium/
+-rw-rw-rw-   0        0        0       19 2024-05-20 20:20:46.000000 liteium-1.0.4/liteium/__init__.py
+-rw-rw-rw-   0        0        0    10078 2024-05-20 20:31:18.000000 liteium-1.0.4/liteium/main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:34:53.552057 liteium-1.0.4/liteium.egg-info/
+-rw-rw-rw-   0        0        0      853 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-20 20:34:53.000000 liteium-1.0.4/liteium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 20:34:53.560053 liteium-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      630 2024-05-20 20:31:26.000000 liteium-1.0.4/setup.py
```

### Comparing `liteium-1.0.3/PKG-INFO` & `liteium-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteium
-Version: 1.0.3
+Version: 1.0.4
 Summary: Description of your package
 Home-page: https://github.com/XredaX/liteium
 Author: El Bettioui Reda
 Author-email: redaelbettioui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liteium-1.0.3/liteium/main.py` & `liteium-1.0.4/liteium/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from io import open as io_open
 from urllib.parse import urlparse
 from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import TimeoutException, NoSuchElementException
 
+global driver1
+driver1 = ''
+
 class ElementWrapper:
     def __init__(self, element):
         self.element = element
 
 class ElementsWrapper:
     def __init__(self, elements):
         self.elements = elements
 
-global driver1 
-driver1 = ''
-
 def driver(driver_path):
     try:
         global driver1
         driver1 = webdriver.Chrome(service=Service(driver_path))
         return driver1
     except Exception as e:
         print("An error occurred while initializing driver:", e)
@@ -52,15 +52,15 @@
     except NoSuchElementException:
         print("Element not found.")
 
 def find_elements(by, value, time=0):
     try:
         locator = (by, value)
         wait = WebDriverWait(driver1, time)
-        return ElementWrapper(wait.until(EC.presence_of_all_elements_located(locator)))
+        return ElementsWrapper(wait.until(EC.presence_of_all_elements_located(locator)))
         # return ElementsWrapper(driver1.find_elements(*locator))
     except Exception as e:
         print("An error occurred while finding elements:", e)
 
 def id(value,  time=0):
     try:
         return find_element(By.ID, value, time).element
@@ -92,15 +92,15 @@
         print("An error occurred while finding element by partial link text:", e)
 
 def tag_name(value,  time=0):
     try:
         return find_element(By.TAG_NAME, value, time).element
     except Exception as e:
         print("An error occurred while finding element by tag name:", e)
-        
+
 def class_name(value, time=0):
     try:
         return find_element(By.CLASS_NAME, value, time).element
     except Exception as e:
         print("An error occurred while finding element by class name:", e)
 
 def css_selector(value,  time=0):
@@ -160,15 +160,15 @@
 def browser_version():
     global driver1
     try:
         return driver1.capabilities['browserVersion']
     except Exception as e:
         print("Exception:", e)
         return ""
-    
+
 def window_position(x, y):
     global driver1
     try:
         driver1.set_window_position(x, y)
     except Exception as e:
         print("Exception:", e)
 
@@ -187,15 +187,15 @@
         elif not os.path.isabs(filename):
             filename = os.path.join(os.getcwd(), filename)
         
         driver1.save_screenshot(filename)
         print("Screenshot saved at:", filename)
     except Exception as e:
         print("Exception:", e)
-    
+
 def save_cookies(filename=None):
     try:
         if filename is None:
             current_url = driver1.current_url
             parsed_url = urlparse(current_url)
             hostname = parsed_url.hostname
             if hostname:
@@ -296,24 +296,20 @@
 
 def back():
     try:
         driver1.back()
     except Exception as e:
         print("Exception:", e)
 
-
-
 # def perform_actions(*actions):
 #     global driver1
 #     try:
 #         action_chains = webdriver.ActionChains(driver1)
 #         for action in actions:
 #             action_chains = action_chains.perform(action)
 #     except Exception as e:
 #         print("Exception:", e)
 
-
-
 __all__ = ['driver', 'open', 'close', 'id', 'name', 'xpath', 'link_text', 'partial_link_text', 'tag_name', 'class_name', 'css_selector', 
            'ids', 'names', 'xpaths', 'link_texts', 'partial_link_texts', 'tag_names', 'class_names', 'css_selectors', 'browser_version',
            'window_position', 'window_size', 'screenshot', 'save_cookies', 'delete_cookies', 'set_cookies', 'switch_to_alert', 'switch_to_default',
            'switch_to_frame', 'switch_to_window', 'new_window', 'js', 'refresh', 'back', 'forward']
```

### Comparing `liteium-1.0.3/liteium.egg-info/PKG-INFO` & `liteium-1.0.4/liteium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteium
-Version: 1.0.3
+Version: 1.0.4
 Summary: Description of your package
 Home-page: https://github.com/XredaX/liteium
 Author: El Bettioui Reda
 Author-email: redaelbettioui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liteium-1.0.3/setup.py` & `liteium-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from setuptools import setup, find_packages
 
-
 setup(
     name='liteium',
-    version='1.0.3',
+    version='1.0.4',
     description='Description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='El Bettioui Reda',
     author_email='redaelbettioui@gmail.com',
     url='https://github.com/XredaX/liteium',
     packages=find_packages(),
```

