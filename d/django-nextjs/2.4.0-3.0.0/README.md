# Comparing `tmp/django-nextjs-2.4.0.tar.gz` & `tmp/django_nextjs-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nextjs-2.4.0.tar", last modified: Sat Sep  2 07:29:08 2023, max compression
+gzip compressed data, was "django_nextjs-3.0.0.tar", last modified: Mon May 20 09:05:48 2024, max compression
```

## Comparing `django-nextjs-2.4.0.tar` & `django_nextjs-3.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/
--rw-r--r--   0 danial    (1000) danial    (1000)     1076 2022-12-17 14:25:24.000000 django-nextjs-2.4.0/LICENSE
--rw-r--r--   0 danial    (1000) danial    (1000)       62 2022-12-17 14:25:24.000000 django-nextjs-2.4.0/MANIFEST.in
--rw-r--r--   0 danial    (1000) danial    (1000)     9967 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/PKG-INFO
--rw-r--r--   0 danial    (1000) danial    (1000)     8919 2023-08-12 14:44:08.000000 django-nextjs-2.4.0/README.md
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/django_nextjs/
--rw-r--r--   0 danial    (1000) danial    (1000)       22 2023-09-02 07:28:16.000000 django-nextjs-2.4.0/django_nextjs/__init__.py
--rw-r--r--   0 danial    (1000) danial    (1000)      191 2023-08-20 12:12:34.000000 django-nextjs-2.4.0/django_nextjs/app_settings.py
--rw-r--r--   0 danial    (1000) danial    (1000)      135 2022-12-17 14:25:24.000000 django-nextjs-2.4.0/django_nextjs/apps.py
--rw-r--r--   0 danial    (1000) danial    (1000)       54 2022-12-17 14:25:24.000000 django-nextjs-2.4.0/django_nextjs/exceptions.py
--rw-r--r--   0 danial    (1000) danial    (1000)     3893 2023-08-12 07:00:21.000000 django-nextjs-2.4.0/django_nextjs/proxy.py
--rw-r--r--   0 danial    (1000) danial    (1000)     6881 2023-09-02 07:27:43.000000 django-nextjs-2.4.0/django_nextjs/render.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/django_nextjs/templates/
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/django_nextjs/templates/django_nextjs/
--rw-r--r--   0 danial    (1000) danial    (1000)      246 2023-08-09 15:28:12.000000 django-nextjs-2.4.0/django_nextjs/templates/django_nextjs/document_base.html
--rw-r--r--   0 danial    (1000) danial    (1000)      287 2022-12-17 14:25:24.000000 django-nextjs-2.4.0/django_nextjs/urls.py
--rw-r--r--   0 danial    (1000) danial    (1000)      364 2023-09-02 07:23:53.000000 django-nextjs-2.4.0/django_nextjs/utils.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/django_nextjs.egg-info/
--rw-r--r--   0 danial    (1000) danial    (1000)     9967 2023-09-02 07:29:08.000000 django-nextjs-2.4.0/django_nextjs.egg-info/PKG-INFO
--rw-r--r--   0 danial    (1000) danial    (1000)      513 2023-09-02 07:29:08.000000 django-nextjs-2.4.0/django_nextjs.egg-info/SOURCES.txt
--rw-r--r--   0 danial    (1000) danial    (1000)        1 2023-09-02 07:29:08.000000 django-nextjs-2.4.0/django_nextjs.egg-info/dependency_links.txt
--rw-r--r--   0 danial    (1000) danial    (1000)      120 2023-09-02 07:29:08.000000 django-nextjs-2.4.0/django_nextjs.egg-info/requires.txt
--rw-r--r--   0 danial    (1000) danial    (1000)       14 2023-09-02 07:29:08.000000 django-nextjs-2.4.0/django_nextjs.egg-info/top_level.txt
--rw-r--r--   0 danial    (1000) danial    (1000)      281 2023-09-02 07:27:43.000000 django-nextjs-2.4.0/pyproject.toml
--rw-r--r--   0 danial    (1000) danial    (1000)       38 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/setup.cfg
--rw-r--r--   0 danial    (1000) danial    (1000)     1814 2023-09-02 07:27:43.000000 django-nextjs-2.4.0/setup.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-09-02 07:29:08.575749 django-nextjs-2.4.0/tests/
--rw-r--r--   0 danial    (1000) danial    (1000)     3454 2023-08-12 14:42:37.000000 django-nextjs-2.4.0/tests/test_render.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2024-05-20 09:05:48.961934 django_nextjs-3.0.0/
+-rw-r--r--   0 danial    (1000) danial    (1000)     1076 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/LICENSE
+-rw-r--r--   0 danial    (1000) danial    (1000)       62 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/MANIFEST.in
+-rw-r--r--   0 danial    (1000) danial    (1000)    10431 2024-05-20 09:05:48.961934 django_nextjs-3.0.0/PKG-INFO
+-rw-r--r--   0 danial    (1000) danial    (1000)     9020 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/README.md
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2024-05-20 09:05:48.958600 django_nextjs-3.0.0/django_nextjs/
+-rw-r--r--   0 danial    (1000) danial    (1000)       22 2024-05-20 08:48:34.000000 django_nextjs-3.0.0/django_nextjs/__init__.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      191 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/django_nextjs/app_settings.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      135 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/django_nextjs/apps.py
+-rw-r--r--   0 danial    (1000) danial    (1000)       54 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/django_nextjs/exceptions.py
+-rw-r--r--   0 danial    (1000) danial    (1000)     3893 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/django_nextjs/proxy.py
+-rw-r--r--   0 danial    (1000) danial    (1000)     5370 2024-05-20 08:44:38.000000 django_nextjs-3.0.0/django_nextjs/render.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2024-05-20 09:05:48.958600 django_nextjs-3.0.0/django_nextjs/templates/
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2024-05-20 09:05:48.958600 django_nextjs-3.0.0/django_nextjs/templates/django_nextjs/
+-rw-r--r--   0 danial    (1000) danial    (1000)      246 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/django_nextjs/templates/django_nextjs/document_base.html
+-rw-r--r--   0 danial    (1000) danial    (1000)      287 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/django_nextjs/urls.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      364 2024-05-12 10:26:52.000000 django_nextjs-3.0.0/django_nextjs/utils.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      590 2024-05-20 08:45:16.000000 django_nextjs-3.0.0/django_nextjs/views.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2024-05-20 09:05:48.958600 django_nextjs-3.0.0/django_nextjs.egg-info/
+-rw-r--r--   0 danial    (1000) danial    (1000)    10431 2024-05-20 09:05:48.000000 django_nextjs-3.0.0/django_nextjs.egg-info/PKG-INFO
+-rw-r--r--   0 danial    (1000) danial    (1000)      536 2024-05-20 09:05:48.000000 django_nextjs-3.0.0/django_nextjs.egg-info/SOURCES.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)        1 2024-05-20 09:05:48.000000 django_nextjs-3.0.0/django_nextjs.egg-info/dependency_links.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)      120 2024-05-20 09:05:48.000000 django_nextjs-3.0.0/django_nextjs.egg-info/requires.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)       14 2024-05-20 09:05:48.000000 django_nextjs-3.0.0/django_nextjs.egg-info/top_level.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)      281 2023-12-10 11:50:43.000000 django_nextjs-3.0.0/pyproject.toml
+-rw-r--r--   0 danial    (1000) danial    (1000)       38 2024-05-20 09:05:48.961934 django_nextjs-3.0.0/setup.cfg
+-rw-r--r--   0 danial    (1000) danial    (1000)     1788 2024-05-12 10:57:50.000000 django_nextjs-3.0.0/setup.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2024-05-20 09:05:48.958600 django_nextjs-3.0.0/tests/
+-rw-r--r--   0 danial    (1000) danial    (1000)     4328 2024-05-13 12:34:09.000000 django_nextjs-3.0.0/tests/test_render.py
```

### Comparing `django-nextjs-2.4.0/LICENSE` & `django_nextjs-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-nextjs-2.4.0/PKG-INFO` & `django_nextjs-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: django-nextjs
-Version: 2.4.0
+Version: 3.0.0
 Summary: Next.js + Django integration
 Home-page: https://github.com/QueraTeam/django-nextjs
 Download-URL: https://github.com/QueraTeam/django-nextjs
 Author: Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>
 Keywords: django,next,nextjs,django-nextjs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Django>=4.2
+Requires-Dist: aiohttp
+Requires-Dist: channels
+Requires-Dist: websockets
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest>=7; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-django; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 # Django Next.js
 
 [![](https://img.shields.io/pypi/v/django-nextjs.svg)](https://pypi.python.org/pypi/django-nextjs/)
 [![](https://github.com/QueraTeam/django-nextjs/workflows/tests/badge.svg)](https://github.com/QueraTeam/django-nextjs/actions)
 [![](https://img.shields.io/github/license/QueraTeam/django-nextjs.svg)](https://github.com/QueraTeam/django-nextjs/blob/master/LICENSE)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -128,25 +138,28 @@
 
 | URL                 | Action                                     |
 | ------------------- | ------------------------------------------ |
 | `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
 | `/_next/...`        | Proxy to `http://localhost:3000`           |
 | `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
 
-Pass `x-real-ip` header when proxying `/_next/`. Example config for Nginx:
+Example config for Nginx:
 
 ```conf
 location /_next/static/ {
     alias NEXTJS_PATH/.next/static/;
     expires max;
     add_header Cache-Control "public";
 }
 location /_next/ {
-    proxy_set_header  x-real-ip $remote_addr;
     proxy_pass  http://127.0.0.1:3000;
+    proxy_set_header Host $http_host;
+    proxy_set_header X-Real-IP $remote_addr;
+    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
+    proxy_set_header X-Forwarded-Proto $scheme;
 }
 location /next/ {
     alias NEXTJS_PATH/public/next/;
     expires max;
     add_header Cache-Control "public";
 }
 ```
```

### Comparing `django-nextjs-2.4.0/README.md` & `django_nextjs-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,25 +102,28 @@
 
 | URL                 | Action                                     |
 | ------------------- | ------------------------------------------ |
 | `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
 | `/_next/...`        | Proxy to `http://localhost:3000`           |
 | `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
 
-Pass `x-real-ip` header when proxying `/_next/`. Example config for Nginx:
+Example config for Nginx:
 
 ```conf
 location /_next/static/ {
     alias NEXTJS_PATH/.next/static/;
     expires max;
     add_header Cache-Control "public";
 }
 location /_next/ {
-    proxy_set_header  x-real-ip $remote_addr;
     proxy_pass  http://127.0.0.1:3000;
+    proxy_set_header Host $http_host;
+    proxy_set_header X-Real-IP $remote_addr;
+    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
+    proxy_set_header X-Forwarded-Proto $scheme;
 }
 location /next/ {
     alias NEXTJS_PATH/public/next/;
     expires max;
     add_header Cache-Control "public";
 }
 ```
```

### Comparing `django-nextjs-2.4.0/django_nextjs/proxy.py` & `django_nextjs-3.0.0/django_nextjs/proxy.py`

 * *Files identical despite different names*

### Comparing `django-nextjs-2.4.0/django_nextjs.egg-info/PKG-INFO` & `django_nextjs-3.0.0/django_nextjs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: django-nextjs
-Version: 2.4.0
+Version: 3.0.0
 Summary: Next.js + Django integration
 Home-page: https://github.com/QueraTeam/django-nextjs
 Download-URL: https://github.com/QueraTeam/django-nextjs
 Author: Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>
 Keywords: django,next,nextjs,django-nextjs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Django>=4.2
+Requires-Dist: aiohttp
+Requires-Dist: channels
+Requires-Dist: websockets
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest>=7; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-django; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
 
 # Django Next.js
 
 [![](https://img.shields.io/pypi/v/django-nextjs.svg)](https://pypi.python.org/pypi/django-nextjs/)
 [![](https://github.com/QueraTeam/django-nextjs/workflows/tests/badge.svg)](https://github.com/QueraTeam/django-nextjs/actions)
 [![](https://img.shields.io/github/license/QueraTeam/django-nextjs.svg)](https://github.com/QueraTeam/django-nextjs/blob/master/LICENSE)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -128,25 +138,28 @@
 
 | URL                 | Action                                     |
 | ------------------- | ------------------------------------------ |
 | `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
 | `/_next/...`        | Proxy to `http://localhost:3000`           |
 | `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
 
-Pass `x-real-ip` header when proxying `/_next/`. Example config for Nginx:
+Example config for Nginx:
 
 ```conf
 location /_next/static/ {
     alias NEXTJS_PATH/.next/static/;
     expires max;
     add_header Cache-Control "public";
 }
 location /_next/ {
-    proxy_set_header  x-real-ip $remote_addr;
     proxy_pass  http://127.0.0.1:3000;
+    proxy_set_header Host $http_host;
+    proxy_set_header X-Real-IP $remote_addr;
+    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
+    proxy_set_header X-Forwarded-Proto $scheme;
 }
 location /next/ {
     alias NEXTJS_PATH/public/next/;
     expires max;
     add_header Cache-Control "public";
 }
 ```
```

### Comparing `django-nextjs-2.4.0/django_nextjs.egg-info/SOURCES.txt` & `django_nextjs-3.0.0/django_nextjs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 django_nextjs/app_settings.py
 django_nextjs/apps.py
 django_nextjs/exceptions.py
 django_nextjs/proxy.py
 django_nextjs/render.py
 django_nextjs/urls.py
 django_nextjs/utils.py
+django_nextjs/views.py
 django_nextjs.egg-info/PKG-INFO
 django_nextjs.egg-info/SOURCES.txt
 django_nextjs.egg-info/dependency_links.txt
 django_nextjs.egg-info/requires.txt
 django_nextjs.egg-info/top_level.txt
 django_nextjs/templates/django_nextjs/document_base.html
 tests/test_render.py
```

### Comparing `django-nextjs-2.4.0/setup.py` & `django_nextjs-3.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,26 +28,25 @@
     long_description_content_type="text/markdown",
     keywords=["django", "next", "nextjs", "django-nextjs"],
     author="Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>",
     url="https://github.com/QueraTeam/django-nextjs",
     download_url="https://github.com/QueraTeam/django-nextjs",
     packages=find_packages(".", include=("django_nextjs", "django_nextjs.*")),
     include_package_data=True,
-    install_requires=["Django >= 3.2", "aiohttp", "channels", "websockets"],
+    install_requires=["Django >= 4.2", "aiohttp", "channels", "websockets"],
     extras_require={"dev": dev_requirements},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `django-nextjs-2.4.0/tests/test_render.py` & `django_nextjs-3.0.0/tests/test_render.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from unittest.mock import AsyncMock, MagicMock, patch
 
 import pytest
 from django.test import RequestFactory
 from django.utils.datastructures import MultiValueDict
 
 from django_nextjs.app_settings import NEXTJS_SERVER_URL
-from django_nextjs.render import _get_render_context, render_nextjs_page
+from django_nextjs.render import _get_render_context, render_nextjs_page_to_string
+from django_nextjs.views import nextjs_page
 
 
 def test_get_render_context_empty_html():
     assert _get_render_context("") is None
 
 
 def test_get_render_context_html_without_children():
@@ -44,28 +45,28 @@
     assert _get_render_context(html) == expected_context
 
     context = {"extra_context": "content"}
     assert _get_render_context(html, context) == {**expected_context, **context}
 
 
 @pytest.mark.asyncio
-async def test_render_nextjs_page(rf: RequestFactory):
+async def test_nextjs_page(rf: RequestFactory):
     path = "random/path"
     params = MultiValueDict({"name": ["Adrian", "Simon"], "position": ["Developer"]})
     request = rf.get(f"/{path}", data=params)
     nextjs_response = "<html><head></head><body></body></html>"
 
     with patch("aiohttp.ClientSession") as mock_session:
         with patch("aiohttp.ClientSession.get") as mock_get:
             mock_get.return_value.__aenter__.return_value.text = AsyncMock(return_value=nextjs_response)
             mock_get.return_value.__aenter__.return_value.status = 200
             mock_get.return_value.__aenter__.return_value.headers = {"Location": "target_value", "unimportant": ""}
             mock_session.return_value.__aenter__ = AsyncMock(return_value=MagicMock(get=mock_get))
 
-            http_response = await render_nextjs_page(request, allow_redirects=True, headers={"extra": "headers"})
+            http_response = await nextjs_page(allow_redirects=True, headers={"extra": "headers"})(request)
 
             assert http_response.content == nextjs_response.encode()
             assert http_response.status_code == 200
             assert http_response.has_header("Location")
             assert http_response.has_header("unimportant") is False
 
             # Arguments passed to aiohttp.ClientSession.get
@@ -76,7 +77,22 @@
             assert kwargs["allow_redirects"] is True
 
         args, kwargs = mock_session.call_args
         assert "csrftoken" in kwargs["cookies"]
         assert kwargs["headers"]["user-agent"] == ""
         assert kwargs["headers"]["x-real-ip"] == "127.0.0.1"
         assert kwargs["headers"]["extra"] == "headers"
+
+
+@pytest.mark.asyncio
+async def test_render_nextjs_page_to_string(rf: RequestFactory):
+    request = rf.get(f"/random/path")
+    nextjs_response = """<html><head><link/></head><body id="__django_nextjs_body"><div id="__django_nextjs_body_begin"/><div id="__django_nextjs_body_end"/></body></html>"""
+
+    with patch("aiohttp.ClientSession") as mock_session:
+        with patch("aiohttp.ClientSession.get") as mock_get:
+            mock_get.return_value.__aenter__.return_value.text = AsyncMock(return_value=nextjs_response)
+            mock_session.return_value.__aenter__ = AsyncMock(return_value=MagicMock(get=mock_get))
+
+            response_text = await render_nextjs_page_to_string(request, template_name="custom_document.html")
+            assert "before_head" in response_text
+            assert "after_head" in response_text
```

