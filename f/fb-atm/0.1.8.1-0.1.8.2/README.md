# Comparing `tmp/fb_atm-0.1.8.1.tar.gz` & `tmp/fb_atm-0.1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_atm-0.1.8.1.tar", last modified: Fri May 10 21:01:23 2024, max compression
+gzip compressed data, was "fb_atm-0.1.8.2.tar", last modified: Mon May 20 07:44:34 2024, max compression
```

## Comparing `fb_atm-0.1.8.1.tar` & `fb_atm-0.1.8.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-10 21:01:19.000000 fb_atm-0.1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/fb_atm/
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-10 21:01:19.000000 fb_atm-0.1.8.1/fb_atm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/fb_atm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 21:01:23.000000 fb_atm-0.1.8.1/fb_atm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 21:01:23.659420 fb_atm-0.1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-10 21:01:19.000000 fb_atm-0.1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:44:34.398489 fb_atm-0.1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-20 07:44:34.398489 fb_atm-0.1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-20 07:44:27.000000 fb_atm-0.1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:44:34.394489 fb_atm-0.1.8.2/fb_atm/
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-20 07:44:27.000000 fb_atm-0.1.8.2/fb_atm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:44:34.398489 fb_atm-0.1.8.2/fb_atm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 07:44:34.000000 fb_atm-0.1.8.2/fb_atm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:44:34.398489 fb_atm-0.1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-20 07:44:27.000000 fb_atm-0.1.8.2/setup.py
```

### Comparing `fb_atm-0.1.8.1/PKG-INFO` & `fb_atm-0.1.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_atm
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: An application that informs you of the different modules and very easy to use.
 Home-page: https://www.facebook.com/bk4human
 Author: Mahdi Hasan Shuvo
 Author-email: shvo.mex@gmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/Shuvo-BBHH/
 Project-URL: Bug Reports, https://www.facebook.com/bk4human
```

### Comparing `fb_atm-0.1.8.1/README.md` & `fb_atm-0.1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `fb_atm-0.1.8.1/fb_atm/__init__.py` & `fb_atm-0.1.8.2/fb_atm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                     cookies (str or set): The input cookies to format.
 
                 Returns:
                     dict: A dictionary containing the formatted cookies.
                 """
             try:  
                 if isinstance(cookes, set):
-                        cookies =cookes
+                        return cookies
                 elif isinstance(cookes, str):
                     cookies = dict(urllib.parse.parse_qsl(cookes, keep_blank_values=True))
                     return cookies
             except Exception as e:
                   print('parsing error',e)
     def get_page_ID(self,cookes):
             try:
@@ -112,27 +112,19 @@
                     jazoest=re.search('type="hidden" name="jazoest" value="(.*?)"',str(data_responce)).group(1)
                 except:
                     try:
                         jazoest=re.search('"jazoest", "(.*?)"',str(data_responce)).group(1)
                     except:jazoest=''
                 lsd=re.search('"LSD",\[\],{"token":"(.*?)"}',str(data_responce)).group(1)
             elif  'www.facebook' in url:
-                uidx = re.search('"actorID":"(.*?)"', str(data_responce)).group(1)
+                uidx = re.search('__user=(.*?)&', str(data_responce)).group(1)
+                fb_dtsg = re.search('"DTSGInitialData",\[\],{"token":"(.*?)"', str(data_responce)).group(1)
+                jazoest = re.search('&jazoest=(.*?)",', str(data_responce)).group(1)
+                lsd = re.search('"LSD",\[\],{"token":"(.*?)"', str(data_responce)).group(1)
                 
-                try:
-                    fb_dtsg=re.search('"name":"fb_dtsg","value":"(.*?)"',str(data_responce)).group(1)
-                except:
-                    fb_dtsg=re.search('{"dtsg":{"token":"(.*?)"',str(data_responce)).group(1)
-                try:
-                    jazoest=re.search('"name":"jazoest","value":"(.*?)"',str(data_responce)).group(1)
-                except:
-                    try:
-                        jazoest=re.search('"jazoest", "(.*?)"',str(data_responce)).group(1)
-                    except:jazoest=''
-                lsd=re.search('"LSD",\[\],{"token":"(.*?)"}',str(data_responce)).group(1)
             return {
                 "fb_dtsg":fb_dtsg,
                 "jazoest":jazoest,
                 "lsd":lsd,
                 "Profile_ID":uidx
             }
         except Exception as e:print(e)
```

### Comparing `fb_atm-0.1.8.1/fb_atm.egg-info/PKG-INFO` & `fb_atm-0.1.8.2/fb_atm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_atm
-Version: 0.1.8.1
+Version: 0.1.8.2
 Summary: An application that informs you of the different modules and very easy to use.
 Home-page: https://www.facebook.com/bk4human
 Author: Mahdi Hasan Shuvo
 Author-email: shvo.mex@gmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/Shuvo-BBHH/
 Project-URL: Bug Reports, https://www.facebook.com/bk4human
```

### Comparing `fb_atm-0.1.8.1/setup.py` & `fb_atm-0.1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 long_description='Mahdi Hasan Shuvo'
 setup(
     name="fb_atm",
-    version='0.1.8.1',
+    version='0.1.8.2',
     author="Mahdi Hasan Shuvo",
     author_email="shvo.mex@gmail.com",
     url="https://www.facebook.com/bk4human",
     description="An application that informs you of the different modules and very easy to use.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

