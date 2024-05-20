# Comparing `tmp/divent-4.1.2.tar.gz` & `tmp/divent-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divent-4.1.2.tar", max compression
+gzip compressed data, was "divent-4.1.3.tar", max compression
```

## Comparing `divent-4.1.2.tar` & `divent-4.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1854 2024-03-01 21:24:18.869104 divent-4.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-01 21:24:18.869104 divent-4.1.2/divent/__init__.py
--rw-r--r--   0        0        0       34 2024-03-01 21:24:18.869104 divent-4.1.2/divent/__main__.py
--rw-r--r--   0        0        0    10467 2024-03-01 21:24:18.869104 divent-4.1.2/divent/bot.py
--rw-r--r--   0        0        0        0 2024-03-01 21:24:18.869104 divent-4.1.2/divent/py.typed
--rw-r--r--   0        0        0    31000 2024-03-01 21:24:18.869104 divent-4.1.2/divent/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     2903 2024-03-01 21:24:18.869104 divent-4.1.2/divent/static/css/global.css
--rw-r--r--   0        0        0   134808 2024-03-01 21:24:18.869104 divent-4.1.2/divent/static/fonts/FontAwesome.otf
--rw-r--r--   0        0        0   165742 2024-03-01 21:24:18.873104 divent-4.1.2/divent/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    20704 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/fonts/open-sans-v29-latin-regular.woff
--rw-r--r--   0        0        0    16720 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/fonts/open-sans-v29-latin-regular.woff2
--rw-r--r--   0        0        0   106618 2024-03-01 21:24:18.877104 divent-4.1.2/divent/static/img/deadlink.png
--rw-r--r--   0        0        0      879 2024-03-01 21:24:18.877104 divent-4.1.2/divent/templates/base.html.j2
--rw-r--r--   0        0        0      556 2024-03-01 21:24:18.881104 divent-4.1.2/divent/templates/error.html.j2
--rw-r--r--   0        0        0      979 2024-03-01 21:24:18.881104 divent-4.1.2/divent/templates/footer.html.j2
--rw-r--r--   0        0        0     2176 2024-03-01 21:24:18.881104 divent-4.1.2/divent/templates/guilds.html.j2
--rw-r--r--   0        0        0     1246 2024-03-01 21:24:18.881104 divent-4.1.2/divent/templates/index.html.j2
--rw-r--r--   0        0        0     2035 2024-03-01 21:24:18.881104 divent-4.1.2/divent/templates/subscribe.html.j2
--rw-r--r--   0        0        0     1491 2024-03-01 21:24:18.881104 divent-4.1.2/divent/translations/fr.json
--rw-r--r--   0        0        0      921 2024-03-01 21:24:18.881104 divent-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 divent-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1854 2024-05-20 15:50:09.740279 divent-4.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 15:50:09.740279 divent-4.1.3/divent/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-20 15:50:09.740279 divent-4.1.3/divent/__main__.py
+-rw-r--r--   0        0        0    10467 2024-05-20 15:50:09.740279 divent-4.1.3/divent/bot.py
+-rw-r--r--   0        0        0        0 2024-05-20 15:50:09.740279 divent-4.1.3/divent/py.typed
+-rw-r--r--   0        0        0    31000 2024-05-20 15:50:09.740279 divent-4.1.3/divent/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     2903 2024-05-20 15:50:09.740279 divent-4.1.3/divent/static/css/global.css
+-rw-r--r--   0        0        0   134808 2024-05-20 15:50:09.744279 divent-4.1.3/divent/static/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0   165742 2024-05-20 15:50:09.744279 divent-4.1.3/divent/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2024-05-20 15:50:09.748279 divent-4.1.3/divent/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2024-05-20 15:50:09.748279 divent-4.1.3/divent/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2024-05-20 15:50:09.752279 divent-4.1.3/divent/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2024-05-20 15:50:09.752279 divent-4.1.3/divent/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    20704 2024-05-20 15:50:09.752279 divent-4.1.3/divent/static/fonts/open-sans-v29-latin-regular.woff
+-rw-r--r--   0        0        0    16720 2024-05-20 15:50:09.752279 divent-4.1.3/divent/static/fonts/open-sans-v29-latin-regular.woff2
+-rw-r--r--   0        0        0   106618 2024-05-20 15:50:09.752279 divent-4.1.3/divent/static/img/deadlink.png
+-rw-r--r--   0        0        0      879 2024-05-20 15:50:09.752279 divent-4.1.3/divent/templates/base.html.j2
+-rw-r--r--   0        0        0      556 2024-05-20 15:50:09.752279 divent-4.1.3/divent/templates/error.html.j2
+-rw-r--r--   0        0        0      979 2024-05-20 15:50:09.752279 divent-4.1.3/divent/templates/footer.html.j2
+-rw-r--r--   0        0        0     2176 2024-05-20 15:50:09.752279 divent-4.1.3/divent/templates/guilds.html.j2
+-rw-r--r--   0        0        0     1246 2024-05-20 15:50:09.752279 divent-4.1.3/divent/templates/index.html.j2
+-rw-r--r--   0        0        0     2035 2024-05-20 15:50:09.752279 divent-4.1.3/divent/templates/subscribe.html.j2
+-rw-r--r--   0        0        0     1491 2024-05-20 15:50:09.752279 divent-4.1.3/divent/translations/fr.json
+-rw-r--r--   0        0        0      922 2024-05-20 15:50:09.756279 divent-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 divent-4.1.3/PKG-INFO
```

### Comparing `divent-4.1.2/README.md` & `divent-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/bot.py` & `divent-4.1.3/divent/bot.py`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/css/font-awesome.min.css` & `divent-4.1.3/divent/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/css/global.css` & `divent-4.1.3/divent/static/css/global.css`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/FontAwesome.otf` & `divent-4.1.3/divent/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/fontawesome-webfont.eot` & `divent-4.1.3/divent/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/fontawesome-webfont.svg` & `divent-4.1.3/divent/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/fontawesome-webfont.ttf` & `divent-4.1.3/divent/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/fontawesome-webfont.woff` & `divent-4.1.3/divent/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/fontawesome-webfont.woff2` & `divent-4.1.3/divent/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/open-sans-v29-latin-regular.woff` & `divent-4.1.3/divent/static/fonts/open-sans-v29-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/fonts/open-sans-v29-latin-regular.woff2` & `divent-4.1.3/divent/static/fonts/open-sans-v29-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/static/img/deadlink.png` & `divent-4.1.3/divent/static/img/deadlink.png`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/templates/base.html.j2` & `divent-4.1.3/divent/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/templates/error.html.j2` & `divent-4.1.3/divent/templates/error.html.j2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/templates/footer.html.j2` & `divent-4.1.3/divent/templates/footer.html.j2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/templates/guilds.html.j2` & `divent-4.1.3/divent/templates/guilds.html.j2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/templates/index.html.j2` & `divent-4.1.3/divent/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/templates/subscribe.html.j2` & `divent-4.1.3/divent/templates/subscribe.html.j2`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/divent/translations/fr.json` & `divent-4.1.3/divent/translations/fr.json`

 * *Files identical despite different names*

### Comparing `divent-4.1.2/pyproject.toml` & `divent-4.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "divent"
-version = "4.1.2"
+version = "4.1.3"
 description = "The discord scheduled event calendar generator"
 authors = ["Xéfir Destiny <xefir@crystalyx.net>"]
 license = "WTFPL"
 readme = "README.md"
 homepage = "https://divent.crystalyx.net/"
 repository = "https://git.crystalyx.net/Xefir/Divent"
 
 [tool.poetry.scripts]
 divent = 'divent.bot:run'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
-disnake = "^2.9.1"
+disnake = "^2.9.2"
 ics = "0.8.0.dev0"
 python-dotenv = "^1.0.1"
-quart = "^0.19.4"
-requests-oauthlib = "^1.3.1"
-uvicorn = "^0.27.1"
+quart = "^0.19.6"
+requests-oauthlib = "^2.0.0"
+uvicorn = "^0.29.0"
 
 [tool.poetry.dev-dependencies]
-black = "^24.2.0"
+black = "^24.4.2"
 djlint = "^1.34.1"
 flake8 = "^7.0.0"
 flake8-alphabetize = "^0.0.21"
 flake8-black = "^0.3.6"
 flake8-pyproject = "^1.2.3"
-mypy = "^1.8.0"
+mypy = "^1.10.0"
 types-oauthlib = "^3.2.0"
 
 [tool.flake8]
 max-line-length = 88
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `divent-4.1.2/PKG-INFO` & `divent-4.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: divent
-Version: 4.1.2
+Version: 4.1.3
 Summary: The discord scheduled event calendar generator
 Home-page: https://divent.crystalyx.net/
 License: WTFPL
 Author: Xéfir Destiny
 Author-email: xefir@crystalyx.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: disnake (>=2.9.1,<3.0.0)
+Requires-Dist: disnake (>=2.9.2,<3.0.0)
 Requires-Dist: ics (==0.8.0.dev0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: quart (>=0.19.4,<0.20.0)
-Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
-Requires-Dist: uvicorn (>=0.27.1,<0.28.0)
+Requires-Dist: quart (>=0.19.6,<0.20.0)
+Requires-Dist: requests-oauthlib (>=2.0.0,<3.0.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Project-URL: Repository, https://git.crystalyx.net/Xefir/Divent
 Description-Content-Type: text/markdown
 
 # Divent
 > The discord scheduled event calendar generator
 
 [![Docker Hub](https://img.shields.io/docker/pulls/xefir/divent)](https://hub.docker.com/r/xefir/divent)
```

