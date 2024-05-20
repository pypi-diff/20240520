# Comparing `tmp/google-auth-st-1.2.tar.gz` & `tmp/google-auth-st-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-auth-st-1.2.tar", last modified: Mon May 13 14:18:35 2024, max compression
+gzip compressed data, was "google-auth-st-1.3.tar", last modified: Mon May 20 11:38:39 2024, max compression
```

## Comparing `google-auth-st-1.2.tar` & `google-auth-st-1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:18:35.078102 google-auth-st-1.2/
--rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-1.2/LICENSE
--rw-rw-rw-   0        0        0     1831 2024-05-13 14:18:35.076102 google-auth-st-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2024-05-10 14:20:05.000000 google-auth-st-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:18:35.059103 google-auth-st-1.2/google_auth_st/
--rw-rw-rw-   0        0        0       36 2024-05-13 14:10:25.000000 google-auth-st-1.2/google_auth_st/__init__.py
--rw-rw-rw-   0        0        0      568 2024-05-13 14:18:00.000000 google-auth-st-1.2/google_auth_st/aggregate_auth.py
--rw-rw-rw-   0        0        0     3186 2024-05-12 21:15:40.000000 google-auth-st-1.2/google_auth_st/google_auth.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:18:35.074102 google-auth-st-1.2/google_auth_st.egg-info/
--rw-rw-rw-   0        0        0     1831 2024-05-13 14:18:34.000000 google-auth-st-1.2/google_auth_st.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-13 14:18:34.000000 google-auth-st-1.2/google_auth_st.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:18:34.000000 google-auth-st-1.2/google_auth_st.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-13 14:18:34.000000 google-auth-st-1.2/google_auth_st.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 14:18:34.000000 google-auth-st-1.2/google_auth_st.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:18:35.078102 google-auth-st-1.2/setup.cfg
--rw-rw-rw-   0        0        0      588 2024-05-13 14:18:03.000000 google-auth-st-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:38:39.838189 google-auth-st-1.3/
+-rw-rw-rw-   0        0        0     1065 2024-05-10 14:11:09.000000 google-auth-st-1.3/LICENSE
+-rw-rw-rw-   0        0        0     1925 2024-05-20 11:38:39.837188 google-auth-st-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1574 2024-05-20 11:36:55.000000 google-auth-st-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 11:38:39.798310 google-auth-st-1.3/google_auth_st/
+-rw-rw-rw-   0        0        0       36 2024-05-13 14:10:25.000000 google-auth-st-1.3/google_auth_st/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-05-13 14:18:00.000000 google-auth-st-1.3/google_auth_st/aggregate_auth.py
+-rw-rw-rw-   0        0        0     3192 2024-05-20 11:28:04.000000 google-auth-st-1.3/google_auth_st/google_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-20 11:38:39.835221 google-auth-st-1.3/google_auth_st.egg-info/
+-rw-rw-rw-   0        0        0     1925 2024-05-20 11:38:39.000000 google-auth-st-1.3/google_auth_st.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-20 11:38:39.000000 google-auth-st-1.3/google_auth_st.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 11:38:39.000000 google-auth-st-1.3/google_auth_st.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-20 11:38:39.000000 google-auth-st-1.3/google_auth_st.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-20 11:38:39.000000 google-auth-st-1.3/google_auth_st.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 11:38:39.838189 google-auth-st-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      588 2024-05-20 11:38:15.000000 google-auth-st-1.3/setup.py
```

### Comparing `google-auth-st-1.2/LICENSE` & `google-auth-st-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-auth-st-1.2/PKG-INFO` & `google-auth-st-1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 1.2
+Version: 1.3
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
-
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
-
 Author: [@valantoni](https://instagram.com/tonidevpy)
 
+☕ Apoya al desarrollador [aquí](https://buymeacoffee.com/toni_dev) / Support me [here](https://buymeacoffee.com/toni_dev)
+
 
 ## Installation
 
 ```sh
 pip install google-auth-st
 ```
 
-
 <p>&nbsp;</p>
 
 # 🔐 google-auth-st
 
 <strong>A python package for adding google auth to your streamlit apps! </strong>
 
 ## Documentation
@@ -53,7 +50,12 @@
 redirect_url = "https://your_app_url..."
 ```
 
 
 ### Feedback:
 
 If you have feedback about this package, please reach out to me on [instagram](https://instagram.com/tonidevpy).
+
+### Shotout
+
+Shotout to [@tylerjrichards](https://github.com/tylerjrichards) for creating the st-paywall package and inspiring me to create this new version without the
+payment method.
```

### Comparing `google-auth-st-1.2/README.md` & `google-auth-st-1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-[![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
-
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
-
 Author: [@valantoni](https://instagram.com/tonidevpy)
 
+☕ Apoya al desarrollador [aquí](https://buymeacoffee.com/toni_dev) / Support me [here](https://buymeacoffee.com/toni_dev)
+
 
 ## Installation
 
 ```sh
 pip install google-auth-st
 ```
 
-
 <p>&nbsp;</p>
 
 # 🔐 google-auth-st
 
 <strong>A python package for adding google auth to your streamlit apps! </strong>
 
 ## Documentation
@@ -42,8 +39,13 @@
 redirect_url_test = 'http://localhost:8501/'
 redirect_url = "https://your_app_url..."
 ```
 
 
 ### Feedback:
 
-If you have feedback about this package, please reach out to me on [instagram](https://instagram.com/tonidevpy).
+If you have feedback about this package, please reach out to me on [instagram](https://instagram.com/tonidevpy).
+
+### Shotout
+
+Shotout to [@tylerjrichards](https://github.com/tylerjrichards) for creating the st-paywall package and inspiring me to create this new version without the
+payment method.
```

### Comparing `google-auth-st-1.2/google_auth_st/aggregate_auth.py` & `google-auth-st-1.3/google_auth_st/aggregate_auth.py`

 * *Files identical despite different names*

### Comparing `google-auth-st-1.2/google_auth_st/google_auth.py` & `google-auth-st-1.3/google_auth_st/google_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     )
     return authorization_url
 
 
 def markdown_button(
     url: str, text: Optional[str] = None, color="#FD504D", sidebar: bool = True
 ):
+    
     markdown = st.sidebar.markdown if sidebar else st.markdown
     
     markdown(
         f"""
     <a href="{url}" target="_blank">
         <div style="
             display: inline-flex;
```

### Comparing `google-auth-st-1.2/google_auth_st.egg-info/PKG-INFO` & `google-auth-st-1.3/google_auth_st.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: google-auth-st
-Version: 1.2
+Version: 1.3
 Summary: Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.
 Home-page: https://github.com/valantoni/google-auth-st.git
 Author: Toni Dev
 Author-email: classtonidev@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Releases](https://img.shields.io/pypi/v/st-paywall)](https://pypi.org/project/st-paywall/)
-
-[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
-
 Author: [@valantoni](https://instagram.com/tonidevpy)
 
+☕ Apoya al desarrollador [aquí](https://buymeacoffee.com/toni_dev) / Support me [here](https://buymeacoffee.com/toni_dev)
+
 
 ## Installation
 
 ```sh
 pip install google-auth-st
 ```
 
-
 <p>&nbsp;</p>
 
 # 🔐 google-auth-st
 
 <strong>A python package for adding google auth to your streamlit apps! </strong>
 
 ## Documentation
@@ -53,7 +50,12 @@
 redirect_url = "https://your_app_url..."
 ```
 
 
 ### Feedback:
 
 If you have feedback about this package, please reach out to me on [instagram](https://instagram.com/tonidevpy).
+
+### Shotout
+
+Shotout to [@tylerjrichards](https://github.com/tylerjrichards) for creating the st-paywall package and inspiring me to create this new version without the
+payment method.
```

### Comparing `google-auth-st-1.2/setup.py` & `google-auth-st-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='google-auth-st',
-    version='1.2',
+    version='1.3',
     packages= ['google_auth_st'],
     description='Librería para añadir autenticación con Google en aplicaciones web con el framework de Streamlit.',
     long_description=open('README.md',encoding='utf-8').read(),
     long_description_content_type='text/markdown',  
     author='Toni Dev',
     author_email='classtonidev@gmail.com',
     url='https://github.com/valantoni/google-auth-st.git',
```

