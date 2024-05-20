# Comparing `tmp/packaged-0.4.0.tar.gz` & `tmp/packaged-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaged-0.4.0.tar", last modified: Fri May 17 13:51:48 2024, max compression
+gzip compressed data, was "packaged-0.5.0.tar", last modified: Sun May 19 21:41:47 2024, max compression
```

## Comparing `packaged-0.4.0.tar` & `packaged-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.150334 packaged-0.4.0/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.4.0/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4540 2024-05-17 13:51:48.150263 packaged-0.4.0/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3289 2024-05-17 13:49:45.000000 packaged-0.4.0/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1342 2024-05-17 13:51:48.150624 packaged-0.4.0/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.4.0/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.145815 packaged-0.4.0/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.148715 packaged-0.4.0/src/packaged/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4221 2024-05-17 13:49:45.000000 packaged-0.4.0/src/packaged/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.4.0/src/packaged/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2555 2024-05-17 13:49:45.000000 packaged-0.4.0/src/packaged/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1536 2024-05-17 13:49:45.000000 packaged-0.4.0/src/packaged/config.py
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.4.0/src/packaged/makeself-header.sh
--rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.4.0/src/packaged/makeself.sh
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.4.0/src/packaged/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-17 13:51:48.149761 packaged-0.4.0/src/packaged.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4540 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      105 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-17 13:51:48.000000 packaged-0.4.0/src/packaged.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-19 21:41:47.788223 packaged-0.5.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    18089 2024-05-14 12:10:36.000000 packaged-0.5.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4894 2024-05-19 21:41:47.788157 packaged-0.5.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3643 2024-05-19 21:41:10.000000 packaged-0.5.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1342 2024-05-19 21:41:47.788723 packaged-0.5.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2024-05-09 19:00:34.000000 packaged-0.5.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-19 21:41:47.783837 packaged-0.5.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-19 21:41:47.786706 packaged-0.5.0/src/packaged/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     6367 2024-05-19 21:41:10.000000 packaged-0.5.0/src/packaged/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      184 2024-05-04 21:39:47.000000 packaged-0.5.0/src/packaged/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2555 2024-05-17 13:49:45.000000 packaged-0.5.0/src/packaged/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1536 2024-05-17 13:49:45.000000 packaged-0.5.0/src/packaged/config.py
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    19207 2024-05-14 12:16:01.000000 packaged-0.5.0/src/packaged/makeself-header.sh
+-rwxr-xr-x   0 tusharsadhwani   (501) staff       (20)    21228 2024-05-13 10:09:30.000000 packaged-0.5.0/src/packaged/makeself.sh
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2024-05-04 21:39:47.000000 packaged-0.5.0/src/packaged/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2024-05-19 21:41:47.787598 packaged-0.5.0/src/packaged.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     4894 2024-05-19 21:41:47.000000 packaged-0.5.0/src/packaged.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      426 2024-05-19 21:41:47.000000 packaged-0.5.0/src/packaged.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2024-05-19 21:41:47.000000 packaged-0.5.0/src/packaged.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       46 2024-05-19 21:41:47.000000 packaged-0.5.0/src/packaged.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      105 2024-05-19 21:41:47.000000 packaged-0.5.0/src/packaged.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2024-05-19 21:41:47.000000 packaged-0.5.0/src/packaged.egg-info/top_level.txt
```

### Comparing `packaged-0.4.0/LICENSE` & `packaged-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packaged-0.4.0/PKG-INFO` & `packaged-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.4.0
+Version: 0.5.0
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
-![Demo](https://github.com/tusharsadhwani/packaged/blob/main/demo.jpg)
+![Demo](https://raw.githubusercontent.com/tusharsadhwani/packaged/main/demo.jpg)
 
 `packaged` can take any Python project, and package it into a self contained
 executable, that can run on other machines without needing Python installed.
 
 ## Installation
 
 ```bash
@@ -59,29 +59,29 @@
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
-### Graphs / matplotlib
+### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
-packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
+packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
 
-This produces a `./curve.bin` binary with:
+This produces a `./mandelbrot.bin` binary with:
 
 - Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
-That outputs an interactive graph GUI.
+That outputs an interactive mandelbrot set GUI.
 
 ### Minesweeper (using `packaged.toml` for configuration)
 
 You can use a `packaged.toml` file and simply do `packaged path/to/project` to
 create your package. For example, try the `minesweeper` project:
 
 ```bash
@@ -92,36 +92,47 @@
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
 packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
-### Textual Demo
+### Textual (TUI) Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged ./textualdemo.bin 'pip install textual' 'python -m textual'
+packaged ./textual.bin 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
 packaged ./aliens 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
 Another one that you can try out is `pygame.examples.chimp`.
 
+### IPython (console scripts)
+
+Packages that expose shell scripts (like `ipython`) should also just work when
+creating a package, and these scripts can be used as the startup command:
+
+```bash
+packaged ./ipython 'pip install ipython' 'ipython'
+```
+
+Now running `./ipython` runs a portable version of IPython!
+
 ## Local Development / Testing
 
 To test and modify the package locally:
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

### Comparing `packaged-0.4.0/README.md` & `packaged-0.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # packaged
 
 The easiest way to ship python applications.
 
-![Demo](https://github.com/tusharsadhwani/packaged/blob/main/demo.jpg)
+![Demo](https://raw.githubusercontent.com/tusharsadhwani/packaged/main/demo.jpg)
 
 `packaged` can take any Python project, and package it into a self contained
 executable, that can run on other machines without needing Python installed.
 
 ## Installation
 
 ```bash
@@ -27,29 +27,29 @@
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
-### Graphs / matplotlib
+### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
-packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
+packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
 
-This produces a `./curve.bin` binary with:
+This produces a `./mandelbrot.bin` binary with:
 
 - Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
-That outputs an interactive graph GUI.
+That outputs an interactive mandelbrot set GUI.
 
 ### Minesweeper (using `packaged.toml` for configuration)
 
 You can use a `packaged.toml` file and simply do `packaged path/to/project` to
 create your package. For example, try the `minesweeper` project:
 
 ```bash
@@ -60,36 +60,47 @@
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
 packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
-### Textual Demo
+### Textual (TUI) Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged ./textualdemo.bin 'pip install textual' 'python -m textual'
+packaged ./textual.bin 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
 packaged ./aliens 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
 Another one that you can try out is `pygame.examples.chimp`.
 
+### IPython (console scripts)
+
+Packages that expose shell scripts (like `ipython`) should also just work when
+creating a package, and these scripts can be used as the startup command:
+
+```bash
+packaged ./ipython 'pip install ipython' 'ipython'
+```
+
+Now running `./ipython` runs a portable version of IPython!
+
 ## Local Development / Testing
 
 To test and modify the package locally:
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

### Comparing `packaged-0.4.0/setup.cfg` & `packaged-0.5.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packaged
-version = 0.4.0
+version = 0.5.0
 description = The easiest way to ship python applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/packaged
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = GPL-2.0-or-later
```

### Comparing `packaged-0.4.0/src/packaged/cli.py` & `packaged-0.5.0/src/packaged/cli.py`

 * *Files identical despite different names*

### Comparing `packaged-0.4.0/src/packaged/config.py` & `packaged-0.5.0/src/packaged/config.py`

 * *Files identical despite different names*

### Comparing `packaged-0.4.0/src/packaged/makeself-header.sh` & `packaged-0.5.0/src/packaged/makeself-header.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.4.0/src/packaged/makeself.sh` & `packaged-0.5.0/src/packaged/makeself.sh`

 * *Files identical despite different names*

### Comparing `packaged-0.4.0/src/packaged.egg-info/PKG-INFO` & `packaged-0.5.0/src/packaged.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaged
-Version: 0.4.0
+Version: 0.5.0
 Summary: The easiest way to ship python applications.
 Home-page: https://github.com/tusharsadhwani/packaged
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: GPL-2.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # packaged
 
 The easiest way to ship python applications.
 
-![Demo](https://github.com/tusharsadhwani/packaged/blob/main/demo.jpg)
+![Demo](https://raw.githubusercontent.com/tusharsadhwani/packaged/main/demo.jpg)
 
 `packaged` can take any Python project, and package it into a self contained
 executable, that can run on other machines without needing Python installed.
 
 ## Installation
 
 ```bash
@@ -59,29 +59,29 @@
 
 ## Examples
 
 All examples below create a self contained executable. You can send the produced
 binary file to another machine with the same OS and architecture, and it will
 run the same.
 
-### Graphs / matplotlib
+### Mandelbrot (`numpy`, `matplotlib`, GUI)
 
 ```bash
-packaged ./curve.bin 'pip install -r requirements.txt' 'python bubble_sort_curve.py' ./example/matplotlib
+packaged ./mandelbrot.bin 'pip install -r requirements.txt' 'python mandelbrot.py' ./example/mandelbrot
 ```
 
-This produces a `./curve.bin` binary with:
+This produces a `./mandelbrot.bin` binary with:
 
 - Python 3.12
 - `matplotlib`
 - `numba`
 - `llvmlite`
 - `pillow`
 
-That outputs an interactive graph GUI.
+That outputs an interactive mandelbrot set GUI.
 
 ### Minesweeper (using `packaged.toml` for configuration)
 
 You can use a `packaged.toml` file and simply do `packaged path/to/project` to
 create your package. For example, try the `minesweeper` project:
 
 ```bash
@@ -92,36 +92,47 @@
 is used for building the package. The equivalent command to build the project
 without `pyproject.toml` would be:
 
 ```bash
 packaged minesweeper.bin 'pip install .' 'python -m minesweeper' ./example/minesweeper
 ```
 
-### Textual Demo
+### Textual (TUI) Demo
 
 Since the dependencies themselves contain all the source code needed, you can
 skip the last argument. With this, no other files will be packaged other than
 what is produced in the build step.
 
 ```bash
-packaged ./textualdemo.bin 'pip install textual' 'python -m textual'
+packaged ./textual.bin 'pip install textual' 'python -m textual'
 ```
 
 This will simply package the `textual` library's own demo into a single file.
 
 ### Aliens (pygame)
 
 Pygame ships with various games as well, `pygame.examples.aliens` is one of them:
 
 ```bash
 packaged ./aliens 'pip install pygame' 'python -m pygame.examples.aliens'
 ```
 
 Another one that you can try out is `pygame.examples.chimp`.
 
+### IPython (console scripts)
+
+Packages that expose shell scripts (like `ipython`) should also just work when
+creating a package, and these scripts can be used as the startup command:
+
+```bash
+packaged ./ipython 'pip install ipython' 'ipython'
+```
+
+Now running `./ipython` runs a portable version of IPython!
+
 ## Local Development / Testing
 
 To test and modify the package locally:
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

