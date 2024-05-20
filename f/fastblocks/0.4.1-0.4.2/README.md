# Comparing `tmp/fastblocks-0.4.1.tar.gz` & `tmp/fastblocks-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.4.1.tar", last modified: Sun May 19 20:05:16 2024, max compression
+gzip compressed data, was "fastblocks-0.4.2.tar", last modified: Mon May 20 08:54:22 2024, max compression
```

## Comparing `fastblocks-0.4.1.tar` & `fastblocks-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.1/LICENSE
--rw-r--r--   0        0        0     1119 2024-05-19 19:52:53.059423 fastblocks-0.4.1/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.1/fastblocks/Dockerfile
--rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.1/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.1/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.1/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.1/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.1/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.1/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.1/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.1/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.1/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.1/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.1/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.1/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.1/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.1/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.1/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.1/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.1/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.1/fastblocks/adapters/routes/__init__.py
--rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.1/fastblocks/adapters/routes/_base.py
--rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.1/fastblocks/adapters/routes/default.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.1/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.1/fastblocks/adapters/sitemap/_base.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.1/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.1/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.1/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.1/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.1/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.1/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.1/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14822 2024-04-11 21:18:24.305113 fastblocks-0.4.1/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.1/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.1/fastblocks/middleware.py
--rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/display_menu.html
--rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/menu_category.html
--rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/menu_item.html
--rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/layout.html
--rw-r--r--   0        0        0     3052 2024-05-19 20:05:16.429187 fastblocks-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 fastblocks-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1181 2024-05-20 05:59:48.364048 fastblocks-0.4.2/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.2/fastblocks/Dockerfile
+-rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.2/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.2/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.2/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.2/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.2/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.2/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.2/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.2/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.2/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.2/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.2/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.2/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.2/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.2/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.2/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.2/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.2/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.2/fastblocks/adapters/routes/__init__.py
+-rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.2/fastblocks/adapters/routes/_base.py
+-rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.2/fastblocks/adapters/routes/default.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.2/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.2/fastblocks/adapters/sitemap/_base.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.2/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.2/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.2/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.2/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.2/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.2/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.2/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14844 2024-05-20 08:52:09.572948 fastblocks-0.4.2/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.2/fastblocks/applications.py
+-rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.2/fastblocks/middleware.py
+-rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.2/fastblocks/templates/admin/bootstrap/blocks/display_menu.html
+-rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.2/fastblocks/templates/admin/bootstrap/blocks/menu_category.html
+-rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.2/fastblocks/templates/admin/bootstrap/blocks/menu_item.html
+-rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 fastblocks-0.4.2/fastblocks/templates/admin/bootstrap/layout.html
+-rw-r--r--   0        0        0     3052 2024-05-20 08:54:22.136723 fastblocks-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 fastblocks-0.4.2/PKG-INFO
```

### Comparing `fastblocks-0.4.1/LICENSE` & `fastblocks-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/README.md` & `fastblocks-0.4.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   [template rendering](https://github.com/lesleslie/starlette-async-jinja)
 - Integrated asynchronous [Jinja Partials](https://github.com/mikeckennedy/jinja_partials)
   and [Jinja Fragments](https://github.com/sponsfreixes/jinja2-fragments)
 - HTMX support
 - Client-side Redis caching
 - Pydantic v2 / SQLModel support
 - Dependency injection
+- [SQLAlchemy Admin](https://aminalaee.dev/sqladmin/) support
 
 
 ## Getting Started
 
 
 ## Acknowledgements
```

#### html2text {}

```diff
@@ -6,9 +6,10 @@
 template blocks. ## Features - [Asynchronous Component Base](https://
 github.com/lesleslie/acb) - Asynchronous [Jinja template loaders, environment]
 (https://github.com/lesleslie/jinja2-async-environment) & [template rendering]
 (https://github.com/lesleslie/starlette-async-jinja) - Integrated asynchronous
 [Jinja Partials](https://github.com/mikeckennedy/jinja_partials) and [Jinja
 Fragments](https://github.com/sponsfreixes/jinja2-fragments) - HTMX support -
 Client-side Redis caching - Pydantic v2 / SQLModel support - Dependency
-injection ## Getting Started ## Acknowledgements ACB "blocks" logo used by
-permission from _A_n_d_y_ _C_o_e_ _B_a_n_d ## License BSD-3-Clause
+injection - [SQLAlchemy Admin](https://aminalaee.dev/sqladmin/) support ##
+Getting Started ## Acknowledgements ACB "blocks" logo used by permission from
+_A_n_d_y_ _C_o_e_ _B_a_n_d ## License BSD-3-Clause
```

### Comparing `fastblocks-0.4.1/fastblocks/adapters/admin/sqladmin.py` & `fastblocks-0.4.2/fastblocks/adapters/admin/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/app/main.py` & `fastblocks-0.4.2/fastblocks/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/auth/_base.py` & `fastblocks-0.4.2/fastblocks/adapters/auth/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/fonts/google.py` & `fastblocks-0.4.2/fastblocks/adapters/fonts/google.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/routes/default.py` & `fastblocks-0.4.2/fastblocks/adapters/routes/default.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.4.2/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/style/_base.py` & `fastblocks-0.4.2/fastblocks/adapters/style/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.4.2/fastblocks/adapters/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.4.2/fastblocks/adapters/templates/jinja2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from acb.depends import depends
 from aiopath import AsyncPath
 from jinja2 import TemplateNotFound
 from jinja2.ext import debug as jinja_debug
 from jinja2.ext import Extension
 from jinja2.ext import i18n
 from jinja2.ext import loopcontrols
-from jinja2_async_environment.loaders import AsyncBaseLoader
 from jinja2_async_environment.bccache import AsyncRedisBytecodeCache
+from jinja2_async_environment.loaders import AsyncBaseLoader
 from pydantic import BaseModel
 from starlette_async_jinja import AsyncJinja2Templates
 from ._base import TemplatesBase
 from ._base import TemplatesBaseSettings
 
 Logger = import_adapter()
 Cache = import_adapter()
@@ -314,15 +314,15 @@
             searchpaths.extend([path, path / "blocks"])
         loaders: list[AsyncBaseLoader] = [
             RedisLoader(searchpaths),
             CloudLoader(searchpaths),
         ]
         file_loaders: list[AsyncBaseLoader] = [FileSystemLoader(searchpaths)]
         if admin:
-            file_loaders.append(PackageLoader("sqladmin"))
+            file_loaders.append(PackageLoader("sqladmin", "templates/sqladmin"))
         jinja_loaders = loaders + file_loaders  # type: ignore[override]
         if not self.config.deployed and not self.config.debug.production:
             jinja_loaders = file_loaders + loaders  # type: ignore[override]
         return ChoiceLoader(jinja_loaders, template_paths.style)
 
     async def init_envs(
         self, template_paths: EnvTemplatePaths, admin: bool = False
```

### Comparing `fastblocks-0.4.1/fastblocks/applications.py` & `fastblocks-0.4.2/fastblocks/applications.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/middleware.py` & `fastblocks-0.4.2/fastblocks/middleware.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/menu_category.html` & `fastblocks-0.4.2/fastblocks/templates/admin/bootstrap/blocks/menu_category.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/layout.html` & `fastblocks-0.4.2/fastblocks/templates/admin/bootstrap/layout.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.1/pyproject.toml` & `fastblocks-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.4.1"
+version = "0.4.2"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -107,37 +107,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pyfiglet",
-    "pdm-bump",
-    "autotyping",
     "pytest",
-    "pre-commit",
     "aiohttp",
+    "autotyping",
     "phonenumbers",
     "pdm",
     "libsass",
+    "pre-commit",
+    "pdm-bump",
+    "pyfiglet",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
+    "B403",
     "B113",
-    "B603",
     "B404",
-    "B403",
+    "B603",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.4.1/PKG-INFO` & `fastblocks-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastblocks
-Version: 0.4.1
+Version: 0.4.2
 Summary: Starlette based app for the rapid delivery HTMX/Jinja template blocks
 Keywords: starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
@@ -63,14 +63,15 @@
   [template rendering](https://github.com/lesleslie/starlette-async-jinja)
 - Integrated asynchronous [Jinja Partials](https://github.com/mikeckennedy/jinja_partials)
   and [Jinja Fragments](https://github.com/sponsfreixes/jinja2-fragments)
 - HTMX support
 - Client-side Redis caching
 - Pydantic v2 / SQLModel support
 - Dependency injection
+- [SQLAlchemy Admin](https://aminalaee.dev/sqladmin/) support
 
 
 ## Getting Started
 
 
 ## Acknowledgements
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastblocks Version: 0.4.1 Summary: Starlette based
+Metadata-Version: 2.1 Name: fastblocks Version: 0.4.2 Summary: Starlette based
 app for the rapid delivery HTMX/Jinja template blocks Keywords:
 starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie
 wedgwoodwebworks.com> Maintainer-Email: lesleslie
 wedgwoodwebworks.com> License: BSD-3-Clause Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
@@ -30,9 +30,10 @@
 template blocks. ## Features - [Asynchronous Component Base](https://
 github.com/lesleslie/acb) - Asynchronous [Jinja template loaders, environment]
 (https://github.com/lesleslie/jinja2-async-environment) & [template rendering]
 (https://github.com/lesleslie/starlette-async-jinja) - Integrated asynchronous
 [Jinja Partials](https://github.com/mikeckennedy/jinja_partials) and [Jinja
 Fragments](https://github.com/sponsfreixes/jinja2-fragments) - HTMX support -
 Client-side Redis caching - Pydantic v2 / SQLModel support - Dependency
-injection ## Getting Started ## Acknowledgements ACB "blocks" logo used by
-permission from _A_n_d_y_ _C_o_e_ _B_a_n_d ## License BSD-3-Clause
+injection - [SQLAlchemy Admin](https://aminalaee.dev/sqladmin/) support ##
+Getting Started ## Acknowledgements ACB "blocks" logo used by permission from
+_A_n_d_y_ _C_o_e_ _B_a_n_d ## License BSD-3-Clause
```

