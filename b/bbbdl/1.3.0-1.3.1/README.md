# Comparing `tmp/bbbdl-1.3.0.tar.gz` & `tmp/bbbdl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbbdl-1.3.0.tar", last modified: Sun Nov 15 11:47:58 2020, max compression
+gzip compressed data, was "bbbdl-1.3.1.tar", max compression
```

## Comparing `bbbdl-1.3.0.tar` & `bbbdl-1.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2894 2020-11-15 11:46:33.106022 bbbdl-1.3.0/bbbdl/__main__.py
--rw-r--r--   0        0        0     1025 2020-11-15 11:46:33.106022 bbbdl-1.3.0/bbbdl/composer.py
--rw-r--r--   0        0        0       82 2020-11-03 23:03:15.184209 bbbdl-1.3.0/bbbdl/errors.py
--rw-r--r--   0        0        0     2946 2020-11-15 11:46:33.106022 bbbdl-1.3.0/bbbdl/resources.py
--rw-r--r--   0        0        0      658 2020-11-15 11:46:33.106022 bbbdl-1.3.0/bbbdl/tracks.py
--rw-r--r--   0        0        0      344 2020-11-03 23:03:15.184209 bbbdl-1.3.0/bbbdl/urlhandler.py
--rw-r--r--   0        0        0      540 2020-11-15 11:47:53.128954 bbbdl-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      870 2020-11-15 11:47:58.547504 bbbdl-1.3.0/setup.py
--rw-r--r--   0        0        0      657 2020-11-15 11:47:58.547889 bbbdl-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-05-19 23:22:14.618750 bbbdl-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     3052 2024-05-19 23:18:59.227734 bbbdl-1.3.1/bbbdl/__main__.py
+-rw-r--r--   0        0        0     2018 2024-05-19 23:18:59.227734 bbbdl-1.3.1/bbbdl/composer.py
+-rw-r--r--   0        0        0      428 2024-05-19 23:18:59.228734 bbbdl-1.3.1/bbbdl/exc.py
+-rw-r--r--   0        0        0     5351 2024-05-19 23:18:59.228734 bbbdl-1.3.1/bbbdl/resources.py
+-rw-r--r--   0        0        0      942 2024-05-19 23:18:59.228734 bbbdl-1.3.1/bbbdl/tracks.py
+-rw-r--r--   0        0        0      619 2024-05-19 23:18:59.228734 bbbdl-1.3.1/bbbdl/urlhandler.py
+-rw-r--r--   0        0        0      609 2024-05-19 23:22:26.345751 bbbdl-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 bbbdl-1.3.1/PKG-INFO
```

### Comparing `bbbdl-1.3.0/bbbdl/__main__.py` & `bbbdl-1.3.1/bbbdl/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     tracks = compose_lesson(meeting, 1280, 720)
 
     output = ffmpeg.output(tracks.video, tracks.audio, output_file)
 
     if debug:
         click.echo(" ".join(output.compile()))
 
-    output.run(quiet=not verbose_ffmpeg, overwrite_output=True)
+    try:
+        output.run(quiet=not verbose_ffmpeg, overwrite_output=True)
+    except FileNotFoundError:
+        raise click.ClickException("ffmpeg is not installed!\nPlease download it at https://ffmpeg.org/download.")
 
 
 @main.command()
 @click.option("-f", "--file", type=click.File(),
               help="The JSON file containing the files to download.")
 @click.option("-r", "--remote-file", type=str,
               help="The URL where the JSON file containing the files to download can be fetched.")
```

### Comparing `bbbdl-1.3.0/pyproject.toml` & `bbbdl-1.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "bbbdl"
-version = "1.3.0"
+version = "1.3.1"
 description = "A downloader for BigBlueButton meetings"
 authors = [
     "Stefano Pigozzi <ste.pigozzi@gmail.com>",
     "g.minoccari <g.minoccari@gmail.com>",
 ]
-license = "AGPL-3.0-or-later"
+license = "EUPL-1.2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^7.1.2"
 beautifulsoup4 = "^4.9.3"
 requests = "^2.24.0"
 ffmpeg-python = "^0.2.0"
 lxml = "^4.6.1"
 colorama = "^0.4.4"
 
 [tool.poetry.scripts]
 bbbdl = 'bbbdl.__main__:main'
 
+
+[tool.poetry.dev-dependencies]
+sphinx = "^3.3.1"
+sphinx_rtd_theme = "^0.5.0"
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `bbbdl-1.3.0/PKG-INFO` & `bbbdl-1.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: bbbdl
-Version: 1.3.0
+Version: 1.3.1
 Summary: A downloader for BigBlueButton meetings
-License: AGPL-3.0-or-later
+License: EUPL-1.2
 Author: Stefano Pigozzi
 Author-email: ste.pigozzi@gmail.com
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: lxml (>=4.6.1,<5.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
```

