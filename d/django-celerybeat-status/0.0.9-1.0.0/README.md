# Comparing `tmp/django-celerybeat-status-0.0.9.tar.gz` & `tmp/django_celerybeat_status-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-celerybeat-status-0.0.9.tar", last modified: Tue Dec 12 20:11:18 2017, max compression
+gzip compressed data, was "django_celerybeat_status-1.0.0.tar", last modified: Mon May 20 15:03:14 2024, max compression
```

## Comparing `django-celerybeat-status-0.0.9.tar` & `django_celerybeat_status-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/django_celerybeat_status.egg-info/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        1 2017-12-12 20:01:31.000000 django-celerybeat-status-0.0.9/django_celerybeat_status.egg-info/not-zip-safe
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        1 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/django_celerybeat_status.egg-info/dependency_links.txt
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       42 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/django_celerybeat_status.egg-info/top_level.txt
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      546 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/django_celerybeat_status.egg-info/PKG-INFO
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      813 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/django_celerybeat_status.egg-info/SOURCES.txt
--rwxrwxr-x   0 hugo      (1000) hugo      (1000)     2797 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/setup.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)       85 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/setup.cfg
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      546 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/PKG-INFO
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/celerybeat_status/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      108 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/apps.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      102 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/admin.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      234 2017-12-12 20:00:58.000000 django-celerybeat-status-0.0.9/celerybeat_status/__init__.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      127 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/custom_index.html
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/sidebar_widgets/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      213 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/sidebar_widgets/statuscheck.html
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1085 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/sidebar_widgets/actions.html
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      144 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/sidebar.html
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/celerybeat_status/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1250 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/templates/celerybeat_status/periodic_tasks_status_list.html
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1031 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/views.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      961 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/helpers.py
-drwxrwxr-x   0 hugo      (1000) hugo      (1000)        0 2017-12-12 20:11:18.000000 django-celerybeat-status-0.0.9/celerybeat_status/tests/
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      353 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/tests/test_views.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)        0 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/tests/__init__.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)      226 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/celerybeat_status/urls.py
--rw-rw-r--   0 hugo      (1000) hugo      (1000)     1069 2017-12-12 19:58:42.000000 django-celerybeat-status-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/celerybeat_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.972495 django_celerybeat_status-1.0.0/celerybeat_status/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/sidebar_widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/sidebar_widgets/actions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/sidebar_widgets/statuscheck.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/periodic_tasks_status_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/celerybeat_status/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/celerybeat_status/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/django_celerybeat_status.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-20 15:03:14.000000 django_celerybeat_status-1.0.0/django_celerybeat_status.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-20 15:03:14.000000 django_celerybeat_status-1.0.0/django_celerybeat_status.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:03:14.000000 django_celerybeat_status-1.0.0/django_celerybeat_status.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:03:14.000000 django_celerybeat_status-1.0.0/django_celerybeat_status.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 15:03:14.000000 django_celerybeat_status-1.0.0/django_celerybeat_status.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 15:03:14.976495 django_celerybeat_status-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2916 2024-05-20 15:03:03.000000 django_celerybeat_status-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-celerybeat-status-0.0.9/setup.py` & `django_celerybeat_status-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,90 +4,95 @@
 import re
 import shutil
 import sys
 from io import open
 
 from setuptools import setup
 
-long_description = ''
+long_description = ""
 try:
-    from pypandoc import convert
-    long_description = convert('README.md', 'rst')
-except ImportError:
-    print("warning: pypandoc module not found, could not convert Markdown to RST")
+    with open("README.md") as f:
+        long_description = f.read()
+except FileNotFoundError:
+    print("warning: README.md not found, could not set long_description")
 
 
 def get_version(package):
     """
     Return package version as listed in `__version__` in `init.py`.
     """
-    init_py = open(os.path.join(package, '__init__.py')).read()
+    init_py = open(os.path.join(package, "__init__.py")).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
 
 def get_packages(package):
     """
     Return root package and all sub-packages.
     """
-    return [dirpath
-            for dirpath, dirnames, filenames in os.walk(package)
-            if os.path.exists(os.path.join(dirpath, '__init__.py'))]
+    return [
+        dirpath
+        for dirpath, dirnames, filenames in os.walk(package)
+        if os.path.exists(os.path.join(dirpath, "__init__.py"))
+    ]
 
 
 def get_package_data(package):
     """
     Return all files under the root package, that are not in a
     package themselves.
     """
-    walk = [(dirpath.replace(package + os.sep, '', 1), filenames)
-            for dirpath, dirnames, filenames in os.walk(package)
-            if not os.path.exists(os.path.join(dirpath, '__init__.py'))]
+    walk = [
+        (dirpath.replace(package + os.sep, "", 1), filenames)
+        for dirpath, dirnames, filenames in os.walk(package)
+        if not os.path.exists(os.path.join(dirpath, "__init__.py"))
+    ]
 
     filepaths = []
     for base, filenames in walk:
-        filepaths.extend([os.path.join(base, filename)
-                          for filename in filenames])
+        filepaths.extend([os.path.join(base, filename) for filename in filenames])
     return {package: filepaths}
 
 
-version = get_version('celerybeat_status')
+version = get_version("celerybeat_status")
 
 
-if sys.argv[-1] == 'publish':
-    try:
-        import pypandoc
-    except ImportError:
-        print("pypandoc not installed.\nUse `pip install pypandoc`.\nExiting.")
+if sys.argv[-1] == "publish":
     if os.system("pip freeze | grep twine"):
         print("twine not installed.\nUse `pip install twine`.\nExiting.")
         sys.exit()
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
-    shutil.rmtree('dist')
-    shutil.rmtree('build')
-    shutil.rmtree('django_celerybeat_status.egg-info')
+    shutil.rmtree("dist")
+    shutil.rmtree("build")
+    shutil.rmtree("django_celerybeat_status.egg-info")
     sys.exit()
 
 
 setup(
-    name='django-celerybeat-status',
+    name="django-celerybeat-status",
     version=version,
-    license='MIT',
-    description='A simple django admin extension that shows when your periodic are going to run next',
+    license="MIT",
+    description="A simple django admin extension that shows when your periodic are going to run next",
     long_description=long_description,
-    author='Vinta Software',
-    author_email='contact@vinta.com.br',
-    packages=get_packages('celerybeat_status'),
-    package_data=get_package_data('celerybeat_status'),
+    long_description_content_type="text/markdown",
+    author="Vinta Software",
+    author_email="contact@vinta.com.br",
+    packages=get_packages("celerybeat_status"),
+    package_data=get_package_data("celerybeat_status"),
     install_requires=[],
     zip_safe=False,
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Framework :: Django',
-        'Framework :: Django :: 1.11',
-        'Programming Language :: Python :: 3.5',
-    ]
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Framework :: Django",
+        "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+    ],
 )
```

### Comparing `django-celerybeat-status-0.0.9/celerybeat_status/templates/admin/sidebar_widgets/actions.html` & `django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/custom_admin/sidebar_widgets/actions.html`

 * *Files identical despite different names*

### Comparing `django-celerybeat-status-0.0.9/celerybeat_status/templates/celerybeat_status/periodic_tasks_status_list.html` & `django_celerybeat_status-1.0.0/celerybeat_status/templates/celerybeat_status/periodic_tasks_status_list.html`

 * *Files identical despite different names*

### Comparing `django-celerybeat-status-0.0.9/celerybeat_status/helpers.py` & `django_celerybeat_status-1.0.0/celerybeat_status/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-from celery.beat import Service
-from django.utils import timezone
 import datetime
 import json
 
+from celery.beat import Service
+from django.utils import timezone
+
 
 def get_periodic_tasks_info():
-    from celery.schedules import current_app
+    from celery import current_app
+
     schedule = Service(current_app).get_scheduler().get_schedule()
     tasks = []
     for key, entry in schedule.items():
         # entry.is_due() returns (is_due, time_in_seconds_for_next_execution)
         is_due_tpl = entry.is_due()
 
         next_execution = timezone.now() + datetime.timedelta(seconds=is_due_tpl[1])
 
         # remove delay between the timezone.now and the schedule entry due date
         next_execution = next_execution.replace(microsecond=0)
 
-        tasks.append({
-            'name': key,
-            'task': entry.task,
-            'args': '(' + ', '.join([json.dumps(arg) for arg in entry.args]) + ')',
-            'kwargs': json.dumps(entry.kwargs),
-            'is_due': is_due_tpl[0],
-            'next_execution': next_execution
-        })
+        tasks.append(
+            {
+                "name": key,
+                "task": entry.task,
+                "args": "(" + ", ".join([json.dumps(arg) for arg in entry.args]) + ")",
+                "kwargs": json.dumps(entry.kwargs),
+                "is_due": is_due_tpl[0],
+                "next_execution": next_execution,
+            }
+        )
 
     return tasks
```

