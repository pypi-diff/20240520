# Comparing `tmp/fastblocks-0.4.0.tar.gz` & `tmp/fastblocks-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.4.0.tar", last modified: Sun May 19 17:35:23 2024, max compression
+gzip compressed data, was "fastblocks-0.4.1.tar", last modified: Sun May 19 20:05:16 2024, max compression
```

## Comparing `fastblocks-0.4.0.tar` & `fastblocks-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.0/LICENSE
--rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.4.0/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.0/fastblocks/Dockerfile
--rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.0/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.0/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.0/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.0/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.0/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.0/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.0/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.0/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.0/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.0/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.0/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.0/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.0/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.0/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.0/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.0/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.0/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.0/fastblocks/adapters/routes/__init__.py
--rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.0/fastblocks/adapters/routes/_base.py
--rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.0/fastblocks/adapters/routes/default.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.0/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.0/fastblocks/adapters/sitemap/_base.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.0/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.0/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.0/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.0/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.0/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.0/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.0/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14822 2024-04-11 21:18:24.305113 fastblocks-0.4.0/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.0/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.0/fastblocks/middleware.py
--rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/display_menu.html
--rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/menu_category.html
--rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/menu_item.html
--rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/layout.html
--rw-r--r--   0        0        0     3052 2024-05-19 17:35:23.713216 fastblocks-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1119 2024-05-19 19:52:53.059423 fastblocks-0.4.1/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.1/fastblocks/Dockerfile
+-rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.1/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.1/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.1/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.1/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.1/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.1/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.1/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.1/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.1/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.1/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.1/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.1/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.1/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.1/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.1/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.1/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.1/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.1/fastblocks/adapters/routes/__init__.py
+-rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.1/fastblocks/adapters/routes/_base.py
+-rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.1/fastblocks/adapters/routes/default.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.1/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.1/fastblocks/adapters/sitemap/_base.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.1/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.1/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.1/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.1/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.1/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.1/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.1/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14822 2024-04-11 21:18:24.305113 fastblocks-0.4.1/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.1/fastblocks/applications.py
+-rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.1/fastblocks/middleware.py
+-rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/display_menu.html
+-rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/menu_category.html
+-rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/menu_item.html
+-rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/layout.html
+-rw-r--r--   0        0        0     3052 2024-05-19 20:05:16.429187 fastblocks-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 fastblocks-0.4.1/PKG-INFO
```

### Comparing `fastblocks-0.4.0/LICENSE` & `fastblocks-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/README.md` & `fastblocks-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -56,9 +56,15 @@
 00000370: 6964 6520 5265 6469 7320 6361 6368 696e  ide Redis cachin
 00000380: 670a 2d20 5079 6461 6e74 6963 2076 3220  g.- Pydantic v2 
 00000390: 2f20 5351 4c4d 6f64 656c 2073 7570 706f  / SQLModel suppo
 000003a0: 7274 0a2d 2044 6570 656e 6465 6e63 7920  rt.- Dependency 
 000003b0: 696e 6a65 6374 696f 6e0a 0a0a 2323 2047  injection...## G
 000003c0: 6574 7469 6e67 2053 7461 7274 6564 0a0a  etting Started..
 000003d0: 0a23 2320 4163 6b6e 6f77 6c65 6467 656d  .## Acknowledgem
-000003e0: 656e 7473 0a0a 0a23 2320 4c69 6365 6e73  ents...## Licens
-000003f0: 650a 0a42 5344 2d33 2d43 6c61 7573 650a  e..BSD-3-Clause.
+000003e0: 656e 7473 0a0a 4143 4220 2262 6c6f 636b  ents..ACB "block
+000003f0: 7322 206c 6f67 6f20 7573 6564 2062 7920  s" logo used by 
+00000400: 7065 726d 6973 7369 6f6e 2066 726f 6d20  permission from 
+00000410: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000420: 2f61 6e64 7963 6f65 6261 6e64 2e63 6f6d  /andycoeband.com
+00000430: 223e 416e 6479 2043 6f65 2042 616e 643c  ">Andy Coe Band<
+00000440: 2f61 3e0a 0a0a 2323 204c 6963 656e 7365  /a>...## License
+00000450: 0a0a 4253 442d 332d 436c 6175 7365 0a    ..BSD-3-Clause.
```

### Comparing `fastblocks-0.4.0/fastblocks/adapters/admin/sqladmin.py` & `fastblocks-0.4.1/fastblocks/adapters/admin/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/app/main.py` & `fastblocks-0.4.1/fastblocks/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/auth/_base.py` & `fastblocks-0.4.1/fastblocks/adapters/auth/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/fonts/google.py` & `fastblocks-0.4.1/fastblocks/adapters/fonts/google.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/routes/default.py` & `fastblocks-0.4.1/fastblocks/adapters/routes/default.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.4.1/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/style/_base.py` & `fastblocks-0.4.1/fastblocks/adapters/style/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.4.1/fastblocks/adapters/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.4.1/fastblocks/adapters/templates/jinja2.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/applications.py` & `fastblocks-0.4.1/fastblocks/applications.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/middleware.py` & `fastblocks-0.4.1/fastblocks/middleware.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/menu_category.html` & `fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/blocks/menu_category.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/layout.html` & `fastblocks-0.4.1/fastblocks/templates/admin/bootstrap/layout.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.0/pyproject.toml` & `fastblocks-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.4.0"
+version = "0.4.1"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -36,51 +36,51 @@
 ]
 readme = "README.md"
 dependencies = [
     "asgi-htmx>=0.1.0",
     "brotli-asgi>=1.4.0",
     "starlette-csrf>=3.0.0",
     "starception>=1.2.1",
-    "pydantic>=2.6.1",
+    "pydantic>=2.7.1",
     "pyfiglet>=1.0.2",
-    "starlette>=0.37.1",
-    "uvicorn>=0.27.1",
+    "starlette>=0.37.2",
+    "uvicorn>=0.29.0",
     "htmlmin>=0.1.12",
     "jsmin>=3.0.1",
     "libsass>=0.23.0",
-    "aiohttp>=3.9.3",
-    "starlette-async-jinja>=1.6.1",
+    "aiohttp>=3.9.5",
+    "starlette-async-jinja>=1.7.5",
     "secure>=0.3.0",
-    "acb[cache,requests,secret,storage]>=0.5.7",
+    "acb[cache,requests,secret,storage]>=0.6.1",
 ]
 
 [project.optional-dependencies]
 sitemap = [
     "asgi-sitemaps>=1.0.0",
 ]
 style = [
     "beautifulsoup4>=4.12.3",
-    "tinycss2>=1.2.1",
+    "tinycss2>=1.3.0",
 ]
 admin = [
-    "sqladmin>=0.16.0",
+    "sqladmin>=0.17.0",
 ]
 
 [project.license]
 text = "BSD-3-Clause"
 
 [tool.pdm.options]
 config = [
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "crackerjack>=0.7.26",
+    "crackerjack>=0.7.34",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
@@ -107,37 +107,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pre-commit",
     "pyfiglet",
-    "libsass",
-    "phonenumbers",
     "pdm-bump",
-    "pdm",
-    "aiohttp",
     "autotyping",
     "pytest",
+    "pre-commit",
+    "aiohttp",
+    "phonenumbers",
+    "pdm",
+    "libsass",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
     "B113",
+    "B603",
     "B404",
     "B403",
-    "B603",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.4.0/PKG-INFO` & `fastblocks-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 626c 6f63 6b73 0a56 6572 7369 6f6e 3a20  blocks.Version: 
-00000030: 302e 342e 300a 5375 6d6d 6172 793a 2053  0.4.0.Summary: S
+00000030: 302e 342e 310a 5375 6d6d 6172 793a 2053  0.4.1.Summary: S
 00000040: 7461 726c 6574 7465 2062 6173 6564 2061  tarlette based a
 00000050: 7070 2066 6f72 2074 6865 2072 6170 6964  pp for the rapid
 00000060: 2064 656c 6976 6572 7920 4854 4d58 2f4a   delivery HTMX/J
 00000070: 696e 6a61 2074 656d 706c 6174 6520 626c  inja template bl
 00000080: 6f63 6b73 0a4b 6579 776f 7264 733a 2073  ocks.Keywords: s
 00000090: 7461 726c 6574 7465 2c68 746d 782c 6a69  tarlette,htmx,ji
 000000a0: 6e6a 612c 6874 7470 782c 6661 7374 6170  nja,httpx,fastap
@@ -59,49 +59,49 @@
 000003a0: 6973 743a 2062 726f 746c 692d 6173 6769  ist: brotli-asgi
 000003b0: 3e3d 312e 342e 300a 5265 7175 6972 6573  >=1.4.0.Requires
 000003c0: 2d44 6973 743a 2073 7461 726c 6574 7465  -Dist: starlette
 000003d0: 2d63 7372 663e 3d33 2e30 2e30 0a52 6571  -csrf>=3.0.0.Req
 000003e0: 7569 7265 732d 4469 7374 3a20 7374 6172  uires-Dist: star
 000003f0: 6365 7074 696f 6e3e 3d31 2e32 2e31 0a52  ception>=1.2.1.R
 00000400: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000410: 6461 6e74 6963 3e3d 322e 362e 310a 5265  dantic>=2.6.1.Re
+00000410: 6461 6e74 6963 3e3d 322e 372e 310a 5265  dantic>=2.7.1.Re
 00000420: 7175 6972 6573 2d44 6973 743a 2070 7966  quires-Dist: pyf
 00000430: 6967 6c65 743e 3d31 2e30 2e32 0a52 6571  iglet>=1.0.2.Req
 00000440: 7569 7265 732d 4469 7374 3a20 7374 6172  uires-Dist: star
-00000450: 6c65 7474 653e 3d30 2e33 372e 310a 5265  lette>=0.37.1.Re
+00000450: 6c65 7474 653e 3d30 2e33 372e 320a 5265  lette>=0.37.2.Re
 00000460: 7175 6972 6573 2d44 6973 743a 2075 7669  quires-Dist: uvi
-00000470: 636f 726e 3e3d 302e 3237 2e31 0a52 6571  corn>=0.27.1.Req
+00000470: 636f 726e 3e3d 302e 3239 2e30 0a52 6571  corn>=0.29.0.Req
 00000480: 7569 7265 732d 4469 7374 3a20 6874 6d6c  uires-Dist: html
 00000490: 6d69 6e3e 3d30 2e31 2e31 320a 5265 7175  min>=0.1.12.Requ
 000004a0: 6972 6573 2d44 6973 743a 206a 736d 696e  ires-Dist: jsmin
 000004b0: 3e3d 332e 302e 310a 5265 7175 6972 6573  >=3.0.1.Requires
 000004c0: 2d44 6973 743a 206c 6962 7361 7373 3e3d  -Dist: libsass>=
 000004d0: 302e 3233 2e30 0a52 6571 7569 7265 732d  0.23.0.Requires-
 000004e0: 4469 7374 3a20 6169 6f68 7474 703e 3d33  Dist: aiohttp>=3
-000004f0: 2e39 2e33 0a52 6571 7569 7265 732d 4469  .9.3.Requires-Di
+000004f0: 2e39 2e35 0a52 6571 7569 7265 732d 4469  .9.5.Requires-Di
 00000500: 7374 3a20 7374 6172 6c65 7474 652d 6173  st: starlette-as
-00000510: 796e 632d 6a69 6e6a 613e 3d31 2e36 2e31  ync-jinja>=1.6.1
+00000510: 796e 632d 6a69 6e6a 613e 3d31 2e37 2e35  ync-jinja>=1.7.5
 00000520: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 00000530: 7365 6375 7265 3e3d 302e 332e 300a 5265  secure>=0.3.0.Re
 00000540: 7175 6972 6573 2d44 6973 743a 2061 6362  quires-Dist: acb
 00000550: 5b63 6163 6865 2c72 6571 7565 7374 732c  [cache,requests,
 00000560: 7365 6372 6574 2c73 746f 7261 6765 5d3e  secret,storage]>
-00000570: 3d30 2e35 2e37 0a52 6571 7569 7265 732d  =0.5.7.Requires-
+00000570: 3d30 2e36 2e31 0a52 6571 7569 7265 732d  =0.6.1.Requires-
 00000580: 4469 7374 3a20 6173 6769 2d73 6974 656d  Dist: asgi-sitem
 00000590: 6170 733e 3d31 2e30 2e30 3b20 6578 7472  aps>=1.0.0; extr
 000005a0: 6120 3d3d 2022 7369 7465 6d61 7022 0a52  a == "sitemap".R
 000005b0: 6571 7569 7265 732d 4469 7374 3a20 6265  equires-Dist: be
 000005c0: 6175 7469 6675 6c73 6f75 7034 3e3d 342e  autifulsoup4>=4.
 000005d0: 3132 2e33 3b20 6578 7472 6120 3d3d 2022  12.3; extra == "
 000005e0: 7374 796c 6522 0a52 6571 7569 7265 732d  style".Requires-
 000005f0: 4469 7374 3a20 7469 6e79 6373 7332 3e3d  Dist: tinycss2>=
-00000600: 312e 322e 313b 2065 7874 7261 203d 3d20  1.2.1; extra == 
+00000600: 312e 332e 303b 2065 7874 7261 203d 3d20  1.3.0; extra == 
 00000610: 2273 7479 6c65 220a 5265 7175 6972 6573  "style".Requires
 00000620: 2d44 6973 743a 2073 716c 6164 6d69 6e3e  -Dist: sqladmin>
-00000630: 3d30 2e31 362e 303b 2065 7874 7261 203d  =0.16.0; extra =
+00000630: 3d30 2e31 372e 303b 2065 7874 7261 203d  =0.17.0; extra =
 00000640: 3d20 2261 646d 696e 220a 5072 6f76 6964  = "admin".Provid
 00000650: 6573 2d45 7874 7261 3a20 7369 7465 6d61  es-Extra: sitema
 00000660: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
 00000670: 3a20 7374 796c 650a 5072 6f76 6964 6573  : style.Provides
 00000680: 2d45 7874 7261 3a20 6164 6d69 6e0a 4465  -Extra: admin.De
 00000690: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
 000006a0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
@@ -163,10 +163,16 @@
 00000a20: 6c69 656e 742d 7369 6465 2052 6564 6973  lient-side Redis
 00000a30: 2063 6163 6869 6e67 0a2d 2050 7964 616e   caching.- Pydan
 00000a40: 7469 6320 7632 202f 2053 514c 4d6f 6465  tic v2 / SQLMode
 00000a50: 6c20 7375 7070 6f72 740a 2d20 4465 7065  l support.- Depe
 00000a60: 6e64 656e 6379 2069 6e6a 6563 7469 6f6e  ndency injection
 00000a70: 0a0a 0a23 2320 4765 7474 696e 6720 5374  ...## Getting St
 00000a80: 6172 7465 640a 0a0a 2323 2041 636b 6e6f  arted...## Ackno
-00000a90: 776c 6564 6765 6d65 6e74 730a 0a0a 2323  wledgements...##
-00000aa0: 204c 6963 656e 7365 0a0a 4253 442d 332d   License..BSD-3-
-00000ab0: 436c 6175 7365 0a                        Clause.
+00000a90: 776c 6564 6765 6d65 6e74 730a 0a41 4342  wledgements..ACB
+00000aa0: 2022 626c 6f63 6b73 2220 6c6f 676f 2075   "blocks" logo u
+00000ab0: 7365 6420 6279 2070 6572 6d69 7373 696f  sed by permissio
+00000ac0: 6e20 6672 6f6d 203c 6120 6872 6566 3d22  n from <a href="
+00000ad0: 6874 7470 733a 2f2f 616e 6479 636f 6562  https://andycoeb
+00000ae0: 616e 642e 636f 6d22 3e41 6e64 7920 436f  and.com">Andy Co
+00000af0: 6520 4261 6e64 3c2f 613e 0a0a 0a23 2320  e Band</a>...## 
+00000b00: 4c69 6365 6e73 650a 0a42 5344 2d33 2d43  License..BSD-3-C
+00000b10: 6c61 7573 650a                           lause.
```

