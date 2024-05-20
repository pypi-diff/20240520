# Comparing `tmp/django_bootstrap5_dark_mode_switch-0.2.1.tar.gz` & `tmp/django_bootstrap5_dark_mode_switch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bootstrap5_dark_mode_switch-0.2.1.tar", last modified: Mon May 20 13:53:40 2024, max compression
+gzip compressed data, was "django_bootstrap5_dark_mode_switch-0.2.2.tar", last modified: Mon May 20 14:14:14 2024, max compression
```

## Comparing `django_bootstrap5_dark_mode_switch-0.2.1.tar` & `django_bootstrap5_dark_mode_switch-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.399682 django_bootstrap5_dark_mode_switch-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-20 13:53:40.399682 django_bootstrap5_dark_mode_switch-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.395682 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.395682 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.399682 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/static/dark_mode_switch/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/static/dark_mode_switch/dark-mode-switch.css
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/static/dark_mode_switch/dark-mode-switch.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.395682 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.399682 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/templates/dark_mode_switch/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/templates/dark_mode_switch/dark_mode_switch.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:40.399682 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-20 13:53:40.000000 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-20 13:53:40.000000 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:53:40.000000 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:53:40.000000 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 13:53:40.000000 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 13:53:40.000000 django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:53:40.399682 django_bootstrap5_dark_mode_switch-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-20 13:53:36.000000 django_bootstrap5_dark_mode_switch-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.240064 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/static/dark_mode_switch/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/static/dark_mode_switch/dark-mode-switch.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/static/dark_mode_switch/dark-mode-switch.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.240064 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/templates/dark_mode_switch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/templates/dark_mode_switch/dark_mode_switch.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 14:14:14.000000 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-20 14:14:14.000000 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:14:14.000000 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:14:14.000000 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 14:14:14.000000 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 14:14:14.000000 django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:14:14.244064 django_bootstrap5_dark_mode_switch-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-20 14:14:10.000000 django_bootstrap5_dark_mode_switch-0.2.2/setup.py
```

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/LICENSE` & `django_bootstrap5_dark_mode_switch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/PKG-INFO` & `django_bootstrap5_dark_mode_switch-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5-dark-mode-switch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Dark mode switch for Django with Bootstrap 5
 Home-page: https://github.com/christianwgd/django-bootstrap5-dark-mode-switch
 Author: Christian Wiegand
 License: MIT
 Keywords: django,bootstrap,dark mode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,18 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.2
 Requires-Dist: django-bootstrap5>=24.2
 
 # Django Bootstrap 5 Dark Mode Switch
 
-Use of bootstrap 5 dark mode made easy.
+[![image](https://img.shields.io/pypi/v/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
 
-**Please be aware that this library is in early development.**
-**This library is not yet available on pypi!**
+Use of bootstrap 5 dark mode made easy.
 
 ## What is this for?
 
 django-bootstrap5-dark-mode-switch enables you to use the 
 [Bootstrap 5 dark mode](https://getbootstrap.com/docs/5.3/customize/color-modes/) 
 in your Django projects. With this library installed you get a menu from which 
 you can select light mode, dark mode and an auto mode that automatically adapts 
@@ -36,17 +36,14 @@
 
 ## Installing
 
 `django-bootstrap5-dark-mode-switch` can be found on pypi. Run 
 `pip install django-bootstrap5-dark-mode-switch` to install the 
 package on your machine or in your virtual environment.
 
-**!! As long as this package isn't available from pypi you can install 
-it using `pip install git+https://github.com/christianwgd/django-bootstrap5-dark-mode-switch.git` !**!
-
 ## Getting Started
 
 You need to have [django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/) >= 24.2 installed.
 
 Add the app to your settings.py:
 
 ```
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: django-bootstrap5-dark-mode-switch Version: 0.2.1
+Metadata-Version: 2.1 Name: django-bootstrap5-dark-mode-switch Version: 0.2.2
 Summary: Dark mode switch for Django with Bootstrap 5 Home-page: https://
 github.com/christianwgd/django-bootstrap5-dark-mode-switch Author: Christian
 Wiegand License: MIT Keywords: django,bootstrap,dark mode Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 django>=4.2 Requires-Dist: django-bootstrap5>=24.2 # Django Bootstrap 5 Dark
-Mode Switch Use of bootstrap 5 dark mode made easy. **Please be aware that this
-library is in early development.** **This library is not yet available on
-pypi!** ## What is this for? django-bootstrap5-dark-mode-switch enables you to
-use the [Bootstrap 5 dark mode](https://getbootstrap.com/docs/5.3/customize/
-color-modes/) in your Django projects. With this library installed you get a
-menu from which you can select light mode, dark mode and an auto mode that
-automatically adapts your theme to the theme selected with your browser or
-operating system. The dark mode switch is fully compatible with the django
-admin dark mode. So if you select dark mode in your django admin it will also
-be enabled with your frontend templates and vice versa. ## Installing `django-
-bootstrap5-dark-mode-switch` can be found on pypi. Run `pip install django-
-bootstrap5-dark-mode-switch` to install the package on your machine or in your
-virtual environment. **!! As long as this package isn't available from pypi you
-can install it using `pip install git+https://github.com/christianwgd/django-
-bootstrap5-dark-mode-switch.git` !**! ## Getting Started You need to have
-[django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/) >=
-24.2 installed. Add the app to your settings.py: ``` INSTALLED_APPS = [ ...,
-'dark_mode_switch', ..., ] ``` Include the css file in your base template: ```
-{% block bootstrap5_extra_head %} {{ block.super }}
+Mode Switch [![image](https://img.shields.io/pypi/v/django-bootstrap5-dark-
+mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-bootstrap5-dark-
+mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+Use of bootstrap 5 dark mode made easy. ## What is this for? django-bootstrap5-
+dark-mode-switch enables you to use the [Bootstrap 5 dark mode](https://
+getbootstrap.com/docs/5.3/customize/color-modes/) in your Django projects. With
+this library installed you get a menu from which you can select light mode,
+dark mode and an auto mode that automatically adapts your theme to the theme
+selected with your browser or operating system. The dark mode switch is fully
+compatible with the django admin dark mode. So if you select dark mode in your
+django admin it will also be enabled with your frontend templates and vice
+versa. ## Installing `django-bootstrap5-dark-mode-switch` can be found on pypi.
+Run `pip install django-bootstrap5-dark-mode-switch` to install the package on
+your machine or in your virtual environment. ## Getting Started You need to
+have [django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/
+) >= 24.2 installed. Add the app to your settings.py: ``` INSTALLED_APPS =
+[ ..., 'dark_mode_switch', ..., ] ``` Include the css file in your base
+template: ``` {% block bootstrap5_extra_head %} {{ block.super }}
 {% endblock %} ``` Include the javascript file in your base template: ``` {%
 block bootstrap5_extra_script %} {{ block.super }}
 {% endblock %} ``` Finally include the html for the switch into your navbar:
 ```
 _Y_o_u_r_ _a_p_p_ _n_a_m_e
     * {% include 'dark_mode_switch/dark_mode_switch.html' %}
 ``` If you like to have the switch outside the navbar you can create your own
```

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/README.md` & `django_bootstrap5_dark_mode_switch-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Django Bootstrap 5 Dark Mode Switch
 
-Use of bootstrap 5 dark mode made easy.
+[![image](https://img.shields.io/pypi/v/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
 
-**Please be aware that this library is in early development.**
-**This library is not yet available on pypi!**
+Use of bootstrap 5 dark mode made easy.
 
 ## What is this for?
 
 django-bootstrap5-dark-mode-switch enables you to use the 
 [Bootstrap 5 dark mode](https://getbootstrap.com/docs/5.3/customize/color-modes/) 
 in your Django projects. With this library installed you get a menu from which 
 you can select light mode, dark mode and an auto mode that automatically adapts 
@@ -19,17 +19,14 @@
 
 ## Installing
 
 `django-bootstrap5-dark-mode-switch` can be found on pypi. Run 
 `pip install django-bootstrap5-dark-mode-switch` to install the 
 package on your machine or in your virtual environment.
 
-**!! As long as this package isn't available from pypi you can install 
-it using `pip install git+https://github.com/christianwgd/django-bootstrap5-dark-mode-switch.git` !**!
-
 ## Getting Started
 
 You need to have [django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/) >= 24.2 installed.
 
 Add the app to your settings.py:
 
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-# Django Bootstrap 5 Dark Mode Switch Use of bootstrap 5 dark mode made easy.
-**Please be aware that this library is in early development.** **This library
-is not yet available on pypi!** ## What is this for? django-bootstrap5-dark-
-mode-switch enables you to use the [Bootstrap 5 dark mode](https://
-getbootstrap.com/docs/5.3/customize/color-modes/) in your Django projects. With
-this library installed you get a menu from which you can select light mode,
-dark mode and an auto mode that automatically adapts your theme to the theme
-selected with your browser or operating system. The dark mode switch is fully
-compatible with the django admin dark mode. So if you select dark mode in your
-django admin it will also be enabled with your frontend templates and vice
-versa. ## Installing `django-bootstrap5-dark-mode-switch` can be found on pypi.
-Run `pip install django-bootstrap5-dark-mode-switch` to install the package on
-your machine or in your virtual environment. **!! As long as this package isn't
-available from pypi you can install it using `pip install git+https://
-github.com/christianwgd/django-bootstrap5-dark-mode-switch.git` !**! ## Getting
-Started You need to have [django-bootstrap5](https://django-
+# Django Bootstrap 5 Dark Mode Switch [![image](https://img.shields.io/pypi/v/
+django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-
+bootstrap5-dark-mode-switch) [![PyPI - Downloads](https://img.shields.io/pypi/
+dm/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-
+bootstrap5-dark-mode-switch) Use of bootstrap 5 dark mode made easy. ## What is
+this for? django-bootstrap5-dark-mode-switch enables you to use the [Bootstrap
+5 dark mode](https://getbootstrap.com/docs/5.3/customize/color-modes/) in your
+Django projects. With this library installed you get a menu from which you can
+select light mode, dark mode and an auto mode that automatically adapts your
+theme to the theme selected with your browser or operating system. The dark
+mode switch is fully compatible with the django admin dark mode. So if you
+select dark mode in your django admin it will also be enabled with your
+frontend templates and vice versa. ## Installing `django-bootstrap5-dark-mode-
+switch` can be found on pypi. Run `pip install django-bootstrap5-dark-mode-
+switch` to install the package on your machine or in your virtual environment.
+## Getting Started You need to have [django-bootstrap5](https://django-
 bootstrap5.readthedocs.io/en/latest/) >= 24.2 installed. Add the app to your
 settings.py: ``` INSTALLED_APPS = [ ..., 'dark_mode_switch', ..., ] ``` Include
 the css file in your base template: ``` {% block bootstrap5_extra_head %} {
 { block.super }}
 {% endblock %} ``` Include the javascript file in your base template: ``` {%
 block bootstrap5_extra_script %} {{ block.super }}
 {% endblock %} ``` Finally include the html for the switch into your navbar:
```

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/static/dark_mode_switch/dark-mode-switch.js` & `django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/static/dark_mode_switch/dark-mode-switch.js`

 * *Files identical despite different names*

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/dark_mode_switch/templates/dark_mode_switch/dark_mode_switch.html` & `django_bootstrap5_dark_mode_switch-0.2.2/dark_mode_switch/templates/dark_mode_switch/dark_mode_switch.html`

 * *Files identical despite different names*

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/PKG-INFO` & `django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5-dark-mode-switch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Dark mode switch for Django with Bootstrap 5
 Home-page: https://github.com/christianwgd/django-bootstrap5-dark-mode-switch
 Author: Christian Wiegand
 License: MIT
 Keywords: django,bootstrap,dark mode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,18 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.2
 Requires-Dist: django-bootstrap5>=24.2
 
 # Django Bootstrap 5 Dark Mode Switch
 
-Use of bootstrap 5 dark mode made easy.
+[![image](https://img.shields.io/pypi/v/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-bootstrap5-dark-mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
 
-**Please be aware that this library is in early development.**
-**This library is not yet available on pypi!**
+Use of bootstrap 5 dark mode made easy.
 
 ## What is this for?
 
 django-bootstrap5-dark-mode-switch enables you to use the 
 [Bootstrap 5 dark mode](https://getbootstrap.com/docs/5.3/customize/color-modes/) 
 in your Django projects. With this library installed you get a menu from which 
 you can select light mode, dark mode and an auto mode that automatically adapts 
@@ -36,17 +36,14 @@
 
 ## Installing
 
 `django-bootstrap5-dark-mode-switch` can be found on pypi. Run 
 `pip install django-bootstrap5-dark-mode-switch` to install the 
 package on your machine or in your virtual environment.
 
-**!! As long as this package isn't available from pypi you can install 
-it using `pip install git+https://github.com/christianwgd/django-bootstrap5-dark-mode-switch.git` !**!
-
 ## Getting Started
 
 You need to have [django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/) >= 24.2 installed.
 
 Add the app to your settings.py:
 
 ```
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: django-bootstrap5-dark-mode-switch Version: 0.2.1
+Metadata-Version: 2.1 Name: django-bootstrap5-dark-mode-switch Version: 0.2.2
 Summary: Dark mode switch for Django with Bootstrap 5 Home-page: https://
 github.com/christianwgd/django-bootstrap5-dark-mode-switch Author: Christian
 Wiegand License: MIT Keywords: django,bootstrap,dark mode Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 django>=4.2 Requires-Dist: django-bootstrap5>=24.2 # Django Bootstrap 5 Dark
-Mode Switch Use of bootstrap 5 dark mode made easy. **Please be aware that this
-library is in early development.** **This library is not yet available on
-pypi!** ## What is this for? django-bootstrap5-dark-mode-switch enables you to
-use the [Bootstrap 5 dark mode](https://getbootstrap.com/docs/5.3/customize/
-color-modes/) in your Django projects. With this library installed you get a
-menu from which you can select light mode, dark mode and an auto mode that
-automatically adapts your theme to the theme selected with your browser or
-operating system. The dark mode switch is fully compatible with the django
-admin dark mode. So if you select dark mode in your django admin it will also
-be enabled with your frontend templates and vice versa. ## Installing `django-
-bootstrap5-dark-mode-switch` can be found on pypi. Run `pip install django-
-bootstrap5-dark-mode-switch` to install the package on your machine or in your
-virtual environment. **!! As long as this package isn't available from pypi you
-can install it using `pip install git+https://github.com/christianwgd/django-
-bootstrap5-dark-mode-switch.git` !**! ## Getting Started You need to have
-[django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/) >=
-24.2 installed. Add the app to your settings.py: ``` INSTALLED_APPS = [ ...,
-'dark_mode_switch', ..., ] ``` Include the css file in your base template: ```
-{% block bootstrap5_extra_head %} {{ block.super }}
+Mode Switch [![image](https://img.shields.io/pypi/v/django-bootstrap5-dark-
+mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/django-bootstrap5-dark-
+mode-switch)](https://pypi.python.org/pypi/django-bootstrap5-dark-mode-switch)
+Use of bootstrap 5 dark mode made easy. ## What is this for? django-bootstrap5-
+dark-mode-switch enables you to use the [Bootstrap 5 dark mode](https://
+getbootstrap.com/docs/5.3/customize/color-modes/) in your Django projects. With
+this library installed you get a menu from which you can select light mode,
+dark mode and an auto mode that automatically adapts your theme to the theme
+selected with your browser or operating system. The dark mode switch is fully
+compatible with the django admin dark mode. So if you select dark mode in your
+django admin it will also be enabled with your frontend templates and vice
+versa. ## Installing `django-bootstrap5-dark-mode-switch` can be found on pypi.
+Run `pip install django-bootstrap5-dark-mode-switch` to install the package on
+your machine or in your virtual environment. ## Getting Started You need to
+have [django-bootstrap5](https://django-bootstrap5.readthedocs.io/en/latest/
+) >= 24.2 installed. Add the app to your settings.py: ``` INSTALLED_APPS =
+[ ..., 'dark_mode_switch', ..., ] ``` Include the css file in your base
+template: ``` {% block bootstrap5_extra_head %} {{ block.super }}
 {% endblock %} ``` Include the javascript file in your base template: ``` {%
 block bootstrap5_extra_script %} {{ block.super }}
 {% endblock %} ``` Finally include the html for the switch into your navbar:
 ```
 _Y_o_u_r_ _a_p_p_ _n_a_m_e
     * {% include 'dark_mode_switch/dark_mode_switch.html' %}
 ``` If you like to have the switch outside the navbar you can create your own
```

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/django_bootstrap5_dark_mode_switch.egg-info/SOURCES.txt` & `django_bootstrap5_dark_mode_switch-0.2.2/django_bootstrap5_dark_mode_switch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_bootstrap5_dark_mode_switch-0.2.1/setup.py` & `django_bootstrap5_dark_mode_switch-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='django-bootstrap5-dark-mode-switch',
-    version='0.2.1',
+    version='0.2.2',
     packages=[
         'dark_mode_switch',
         'dark_mode_switch.templates.dark_mode_switch',
         'dark_mode_switch.static.dark_mode_switch',
     ],
     include_package_data=True,
     description='Dark mode switch for Django with Bootstrap 5',
```

