# Comparing `tmp/dodonacli-2024.5.16.tar.gz` & `tmp/dodonacli-2024.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodonacli-2024.5.16.tar", last modified: Thu May 16 12:25:51 2024, max compression
+gzip compressed data, was "dodonacli-2024.5.20.tar", last modified: Mon May 20 14:27:35 2024, max compression
```

## Comparing `dodonacli-2024.5.16.tar` & `dodonacli-2024.5.20.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.597000 dodonacli-2024.5.16/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.589000 dodonacli-2024.5.16/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.589000 dodonacli-2024.5.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/DodonaCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 12:25:51.000000 dodonacli-2024.5.16/DodonaCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-16 12:25:51.597000 dodonacli-2024.5.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.589000 dodonacli-2024.5.16/dodonacli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/dodonacli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/cli_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/commands/up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/dodonacli/source/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/interactive_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/pretty_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/set_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/submission_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli/source/syntax_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1628 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/dodonacli_completion_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:25:51.593000 dodonacli-2024.5.16/man-page/
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/man-page/dodonacli.1
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/man-page/dodonacli.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 12:25:47.000000 dodonacli-2024.5.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:25:51.597000 dodonacli-2024.5.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.644019 dodonacli-2024.5.20/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.644019 dodonacli-2024.5.20/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/DodonaCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.644019 dodonacli-2024.5.20/dodonacli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/dodonacli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/cli_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/dodonacli/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/interactive_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/pretty_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/submission_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/syntax_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1637 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli_completion_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/man-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/man-page/dodonacli.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/man-page/dodonacli.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/setup.cfg
```

### Comparing `dodonacli-2024.5.16/.github/workflows/publish.yml` & `dodonacli-2024.5.20/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: Publish to PyPI from release
 
 on:
   release:
-    type: created
+    types: [published]
 
 jobs:
   build-and-publish:
     runs-on: ubuntu-latest
     environment: Publish release
     permissions:
       id-token: write
```

### Comparing `dodonacli-2024.5.16/.github/workflows/publish_test.yml` & `dodonacli-2024.5.20/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.16/DodonaCLI.egg-info/PKG-INFO` & `dodonacli-2024.5.20/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,40 @@
-Metadata-Version: 2.1
-Name: DodonaCLI
-Version: 2024.5.16
-Summary: A CLI tool for Dodona
-Author-email: Bram Windey <windey.bram@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Bram Windey
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/BWindey/DodonaCLI
-Keywords: dodona,cli
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: bs4
-Requires-Dist: click
-Requires-Dist: click-default-group
-Requires-Dist: markdownify
-Requires-Dist: packaging
-Requires-Dist: pkg-info
-Requires-Dist: rich
-
 # Command Line Interface for [Dodona](https://dodona.be)
 
 PyPI page: https://pypi.org/project/DodonaCLI/#description
 
 **Contents**:
 1) [Disclaimers](#disclaimers)
-2) [How to install](#how-to-install)
+2) [Installation and updating](#installation-and-updating)
 3) [How to use](#how-to-use)
 4) [Flags that could be important](#flags-that-could-be-important)
-5) [How to update](#how-to-update)
-6) [Help, DodonaCLI freezes](#help-dodonacli-freezes)
-7) [Roadmap](#roadmap)
+5) [Settings](#settings)
+6) [Tab-completion and man-pages](#tab-completion-and-man-pages)
+7) [Help, DodonaCLI freezes](#help-dodonacli-freezes)
+8) [Roadmap](#roadmap)
+
 
 ## Disclaimers
 
 - DodonaCLI is an independent tool created by me, a student, and is not officially affiliated with the Dodona service or its team. Dodona, provided by the dedicated team at UGent University, offers an exceptional service, and this tool has been created as a complementary project. Only issues related to the Dodona website itself should be directed to the official Dodona support channels. Issues with the CLI tool should be posted on this [project’s Issues](https://github.com/BWindey/DodonaCLI/issues).
 
 - Although the exercise-description formatting is mostly useable, do NOT rely on this for tests and exams! The printed description may be incomplete, or even incorrect. Please be aware of this!
 
-
 - I did my best to format the output of DodonaCLI in a nice manner. If this is not the case for your terminal, please reach out via the [Issues](https://github.com/BWindey/DodonaCLI/issues) to see if we can fix that. I use the Alacritty and Gnome terminal, so if you’re using those, you can be mostly sure that what you see is intended.
 
 
-## How to install
-`pip install DodonaCLI`
+## Installation and updating
+Both installation and updating happen through pip:
+```pip install DodonaCLI```
+and
+```pip install --upgrade DodonaCLI```
 
 Alternatively, you can `git clone https://github.com/BWindey/DodonaCLI` and when inside the DodonaCLI folder,
-do `pip install -e .`.
-This is mostly useful for those wanting to change/add to the code.
-
-Tab-completion is supported for bash. You can 
-download ["dodonacli_completion_script.sh" from GitHub](https://github.com/BWindey/DodonaCLI/blob/master/dodonacli_completion_script.sh),
-and source it in your ~/.bashrc. 
-If you use Zsh or Fish, you can run this:
-```
-_DODONA_COMPLETE=zsh_source dodona > ~/.dodona-complete.zsh
-_DODONA_COMPLETE=fish_source dodona > ~/.config/fish/completions/foo-bar.fish
-```
-On Zsh, you'll have to then source this file in `.zshrc`.
-Testing this on bash (yes, that's possible too), tab-completion was really slow. 
-That's why I'd recommend the first method for bash, 
-and I'm looking to get a full completion script for at least Zsh as well.
-
-
-There is also a manual page. You can download ["dodonacli.1.gz"](https://github.com/BWindey/DodonaCLI/blob/master/man-page/dodonacli.1.gz) and save this in a folder included in `$(manpath)`. 
+do `pip install -e .`. The `-e` flag ensures that when you change files (or did a `git pull`), the cli will use the new code.
+This is mostly useful for those wanting to change/add to the code, or test new features on the develop-branch (not recommended for normal users).
 
 
 ## How to use
 There are three main things you can do with Dodona: displaying info (`dodona display`),
 selecting (`dodona select`) and posting exercises (`dodona post`).
 The behaviour of displaying and selecting will depend on your current selection,
 which can be viewed with `dodona status`.
@@ -135,15 +80,15 @@
 For some exercise-descriptions, this can, however, be a nice addition,
 and in the future the formatting-"engine" can improve.
 
 
 ### Hidden 
 This flag is used in combination with the `select` command, when selecting an exercise-series that is hidden. 
 Series can be hidden when they are used in tests or exams, and to get to them, you’ll receive a link to it from your 
-teachers. This link will be of the form ".../series/<SERIES-ID>/?token=<TOKEN>". 
+teachers. This link will be of the form `.../series/<SERIES-ID>/?token=<TOKEN>`. 
 The only correct syntax to then select that hidden series with DodonaCLI is:
     ```dodona select --hidden <TOKEN> <SERIES-ID>```
 
 
 ### Other 
 This flag is used in combination with the `select` command, when selecting a course you’re not registered for.
 This allows you, for example, to select courses from previous years to try out those old tests or exams.
@@ -155,34 +100,63 @@
 when posting a solution-file to a link provided at the first line of the solution-file.
 The link has to include "/courses/<COURSE-ID>" and "/activities/<ACTIVITIES-ID"
 to know which exercise to submit your solution to.
 It also has to start with "https:<!-- comment to prevent link from appearing as real link-->//dodona.be/".
 This link is not included in the solution submitted to the Dodona servers; it is stripped out.
 
 
-## How to update
-Updating is simple: 
-`pip install DodonaCLI --update`
+## Settings
+DodonaCLI has some settings (starting from version 2024.5.20). 
+Currently they are only editable by editing the settings.json file directly.
+In the future, there will be a sub-command to edit these in a more convenient way.
+For info on what is all changeable with these settings, take a look at the changelog
+```dodona info changelog```
+
 
-Alternatively, if you installed it with cloning from GitHub, you can `git pull`.
+## Tab-completion and man-pages
+Tab-completion is supported for bash, fish and zsh. The easiest way to install it, is by following the short instructions at 
+https://click.palletsprojects.com/en/8.1.x/shell-completion/#enabling-completion,
+where you replace all occurences of 'foo-bar' with 'dodona'.
+
+You can also use my custom-written script for bash (if you're using bash), by downloading the autocomplete-script from  
+https://github.com/BWindey/DodonaCLI/blob/master/dodonacli_completion_script.sh 
+and source it in your ~/.bashrc. 
+I personally use this custom one, as it allows me more control over the completion.
+The disadvantage over using this, however, is that you'll need to redownload it if it ever changes.
+I'll promise here and now that if I don't forget, I will always mention in the changelog 
+(`dodona info changelog`), that you need to download the new completion-script.
+
+A while ago, I strongly recommended the custom script, because the other way took about 200ms to complete, which felt slow, but due to some code-restructuring, the completion happens in around 50ms.
+
+There is also a manual page available (very prefessional). 
+You can download ["dodonacli.1.gz"](https://github.com/BWindey/DodonaCLI/blob/master/man-page/dodonacli.1.gz) and save this in a folder included in `$(manpath)`. 
+This will have to be downloaded again if it is updated. I'll let you know in the changelogs.
 
 
 ## Help, DodonaCLI freezes
 Since I just got this situation, I wanted to tell you how I fixed it.
 My computer didn’t succeed in making any network requests over IPv6, and thus waited and waited and waited ...
 To fix this, I had to disable IPv6 entirely on my own pc. 
 This is not something I’ll show you how to do, you’ll have to do some research on the internet.
 Before trying that, confirm first if this is indeed the issue by running `wget` with --inet6-only and --inet4-only 
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
-- user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
+- user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, ...)
+  - language
+  - whether to save feedback to a file
+  - auto download links from sandbox.dodona when selecting exercise
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
+
+Code cleanup:
+- general refactoring of too large files (>150 lines can often be split)
+- 'display_after_select' should maybe not need to make a 2nd API call? 
+- special print that prints with right amount of new-lines to group that together
```

### Comparing `dodonacli-2024.5.16/DodonaCLI.egg-info/SOURCES.txt` & `dodonacli-2024.5.20/DodonaCLI.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 dodonacli/main.py
 dodonacli/commands/__init__.py
 dodonacli/commands/cli_next.py
 dodonacli/commands/display.py
 dodonacli/commands/info.py
 dodonacli/commands/post.py
 dodonacli/commands/select.py
+dodonacli/commands/settings.py
 dodonacli/commands/status.py
 dodonacli/commands/submission.py
 dodonacli/commands/tutorial.py
 dodonacli/commands/up.py
 dodonacli/source/__init__.py
 dodonacli/source/get_data.py
 dodonacli/source/interactive_tutorial.py
```

### Comparing `dodonacli-2024.5.16/LICENSE` & `dodonacli-2024.5.20/LICENSE`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.16/PKG-INFO` & `dodonacli-2024.5.20/DodonaCLI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.16
+Version: 2024.5.20
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,53 +43,41 @@
 
 # Command Line Interface for [Dodona](https://dodona.be)
 
 PyPI page: https://pypi.org/project/DodonaCLI/#description
 
 **Contents**:
 1) [Disclaimers](#disclaimers)
-2) [How to install](#how-to-install)
+2) [Installation and updating](#installation-and-updating)
 3) [How to use](#how-to-use)
 4) [Flags that could be important](#flags-that-could-be-important)
-5) [How to update](#how-to-update)
-6) [Help, DodonaCLI freezes](#help-dodonacli-freezes)
-7) [Roadmap](#roadmap)
+5) [Settings](#settings)
+6) [Tab-completion and man-pages](#tab-completion-and-man-pages)
+7) [Help, DodonaCLI freezes](#help-dodonacli-freezes)
+8) [Roadmap](#roadmap)
+
 
 ## Disclaimers
 
 - DodonaCLI is an independent tool created by me, a student, and is not officially affiliated with the Dodona service or its team. Dodona, provided by the dedicated team at UGent University, offers an exceptional service, and this tool has been created as a complementary project. Only issues related to the Dodona website itself should be directed to the official Dodona support channels. Issues with the CLI tool should be posted on this [project’s Issues](https://github.com/BWindey/DodonaCLI/issues).
 
 - Although the exercise-description formatting is mostly useable, do NOT rely on this for tests and exams! The printed description may be incomplete, or even incorrect. Please be aware of this!
 
-
 - I did my best to format the output of DodonaCLI in a nice manner. If this is not the case for your terminal, please reach out via the [Issues](https://github.com/BWindey/DodonaCLI/issues) to see if we can fix that. I use the Alacritty and Gnome terminal, so if you’re using those, you can be mostly sure that what you see is intended.
 
 
-## How to install
-`pip install DodonaCLI`
+## Installation and updating
+Both installation and updating happen through pip:
+```pip install DodonaCLI```
+and
+```pip install --upgrade DodonaCLI```
 
 Alternatively, you can `git clone https://github.com/BWindey/DodonaCLI` and when inside the DodonaCLI folder,
-do `pip install -e .`.
-This is mostly useful for those wanting to change/add to the code.
-
-Tab-completion is supported for bash. You can 
-download ["dodonacli_completion_script.sh" from GitHub](https://github.com/BWindey/DodonaCLI/blob/master/dodonacli_completion_script.sh),
-and source it in your ~/.bashrc. 
-If you use Zsh or Fish, you can run this:
-```
-_DODONA_COMPLETE=zsh_source dodona > ~/.dodona-complete.zsh
-_DODONA_COMPLETE=fish_source dodona > ~/.config/fish/completions/foo-bar.fish
-```
-On Zsh, you'll have to then source this file in `.zshrc`.
-Testing this on bash (yes, that's possible too), tab-completion was really slow. 
-That's why I'd recommend the first method for bash, 
-and I'm looking to get a full completion script for at least Zsh as well.
-
-
-There is also a manual page. You can download ["dodonacli.1.gz"](https://github.com/BWindey/DodonaCLI/blob/master/man-page/dodonacli.1.gz) and save this in a folder included in `$(manpath)`. 
+do `pip install -e .`. The `-e` flag ensures that when you change files (or did a `git pull`), the cli will use the new code.
+This is mostly useful for those wanting to change/add to the code, or test new features on the develop-branch (not recommended for normal users).
 
 
 ## How to use
 There are three main things you can do with Dodona: displaying info (`dodona display`),
 selecting (`dodona select`) and posting exercises (`dodona post`).
 The behaviour of displaying and selecting will depend on your current selection,
 which can be viewed with `dodona status`.
@@ -135,15 +123,15 @@
 For some exercise-descriptions, this can, however, be a nice addition,
 and in the future the formatting-"engine" can improve.
 
 
 ### Hidden 
 This flag is used in combination with the `select` command, when selecting an exercise-series that is hidden. 
 Series can be hidden when they are used in tests or exams, and to get to them, you’ll receive a link to it from your 
-teachers. This link will be of the form ".../series/<SERIES-ID>/?token=<TOKEN>". 
+teachers. This link will be of the form `.../series/<SERIES-ID>/?token=<TOKEN>`. 
 The only correct syntax to then select that hidden series with DodonaCLI is:
     ```dodona select --hidden <TOKEN> <SERIES-ID>```
 
 
 ### Other 
 This flag is used in combination with the `select` command, when selecting a course you’re not registered for.
 This allows you, for example, to select courses from previous years to try out those old tests or exams.
@@ -155,34 +143,63 @@
 when posting a solution-file to a link provided at the first line of the solution-file.
 The link has to include "/courses/<COURSE-ID>" and "/activities/<ACTIVITIES-ID"
 to know which exercise to submit your solution to.
 It also has to start with "https:<!-- comment to prevent link from appearing as real link-->//dodona.be/".
 This link is not included in the solution submitted to the Dodona servers; it is stripped out.
 
 
-## How to update
-Updating is simple: 
-`pip install DodonaCLI --update`
+## Settings
+DodonaCLI has some settings (starting from version 2024.5.20). 
+Currently they are only editable by editing the settings.json file directly.
+In the future, there will be a sub-command to edit these in a more convenient way.
+For info on what is all changeable with these settings, take a look at the changelog
+```dodona info changelog```
+
 
-Alternatively, if you installed it with cloning from GitHub, you can `git pull`.
+## Tab-completion and man-pages
+Tab-completion is supported for bash, fish and zsh. The easiest way to install it, is by following the short instructions at 
+https://click.palletsprojects.com/en/8.1.x/shell-completion/#enabling-completion,
+where you replace all occurences of 'foo-bar' with 'dodona'.
+
+You can also use my custom-written script for bash (if you're using bash), by downloading the autocomplete-script from  
+https://github.com/BWindey/DodonaCLI/blob/master/dodonacli_completion_script.sh 
+and source it in your ~/.bashrc. 
+I personally use this custom one, as it allows me more control over the completion.
+The disadvantage over using this, however, is that you'll need to redownload it if it ever changes.
+I'll promise here and now that if I don't forget, I will always mention in the changelog 
+(`dodona info changelog`), that you need to download the new completion-script.
+
+A while ago, I strongly recommended the custom script, because the other way took about 200ms to complete, which felt slow, but due to some code-restructuring, the completion happens in around 50ms.
+
+There is also a manual page available (very prefessional). 
+You can download ["dodonacli.1.gz"](https://github.com/BWindey/DodonaCLI/blob/master/man-page/dodonacli.1.gz) and save this in a folder included in `$(manpath)`. 
+This will have to be downloaded again if it is updated. I'll let you know in the changelogs.
 
 
 ## Help, DodonaCLI freezes
 Since I just got this situation, I wanted to tell you how I fixed it.
 My computer didn’t succeed in making any network requests over IPv6, and thus waited and waited and waited ...
 To fix this, I had to disable IPv6 entirely on my own pc. 
 This is not something I’ll show you how to do, you’ll have to do some research on the internet.
 Before trying that, confirm first if this is indeed the issue by running `wget` with --inet6-only and --inet4-only 
 to see if this is indeed the issue.
 
 
 ## Roadmap
 This section has a bunch of ideas for me to work on, but also for you, the potential contributor!
 Remember to look at the recent branches/commits to see if I’m not working on one of these:
-- user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, config location, ...)
+- user-settings (f.e. auto-download of files, language, formatting, number of submissions shown, ...)
+  - language
+  - whether to save feedback to a file
+  - auto download links from sandbox.dodona when selecting exercise
 - easy (automatic?) downloading of files mentioned in exercise description
 - improve the rendering of all html/markdown frankensteins, in descriptions of exercises and exercise-descriptions 
 - add connection time-out to prevent long waiting when IPv6 doesn’t want to work along
 - add support for more languages syntax checkers
 - caching some info for faster navigation and/or autocompletion
 - add indicator to series to mark if all their exercises are completely solved (maybe fetch from html-version)
 - get exercise-names via html-parsing for a submission list to only need 1 API call (instead of 30)
+
+Code cleanup:
+- general refactoring of too large files (>150 lines can often be split)
+- 'display_after_select' should maybe not need to make a 2nd API call? 
+- special print that prints with right amount of new-lines to group that together
```

### Comparing `dodonacli-2024.5.16/dodonacli/commands/cli_next.py` & `dodonacli-2024.5.20/dodonacli/commands/cli_next.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,40 +19,45 @@
               is_flag=True, default=False)
 def cli_next(reverse, unsolved):
     import http.client
     from dodonacli.source import get_data, set_data
 
     # Read configs in
     config = get_data.get_configs()
+    settings = get_data.get_settings()
 
     # Start up the connection to Dodona
     connection = http.client.HTTPSConnection("dodona.be")
     headers = {
         "Content-type": "application/json",
         "Accept": "application/json",
         "Authorization": config['TOKEN']
     }
 
     if config.get('exercise_id') is not None:
-        config = get_next_exercise(config, connection, headers, reverse, unsolved)
+        config = get_next_exercise(config, settings, connection, headers, reverse, unsolved)
 
     elif config.get('serie_id') is not None:
-        config = get_next_series(config, connection, headers, reverse, unsolved)
+        config = get_next_series(config, settings, connection, headers, reverse, unsolved)
 
     elif config.get('course_id') is not None:
-        config = get_next_course(config, connection, headers, reverse, unsolved)
+        config = get_next_course(config, settings, connection, headers, reverse, unsolved)
 
     else:
-        print("\nCan't select a next course when non are selected.\n")
+        print(
+            '\n' * settings['new_lines_above']
+            + "Can't select a next course when non are selected."
+            + '\n' * settings['new_lines_below']
+        )
         return
 
     set_data.dump_config(config)
 
 
-def get_next_exercise(config, connection, headers, reverse, unsolved):
+def get_next_exercise(config, settings, connection, headers, reverse, unsolved):
     from dodonacli.source import get_data, pretty_print
 
     # Get all exercises of selected series
     exercise_data_json = get_data.exercises_data(
         connection, headers, config['serie_id'], f"/?token={config['serie_token']}" if config['serie_token'] else ""
     )
 
@@ -77,45 +82,55 @@
     else:
         i = 1
         while next_id == -1 and i < len(id_list):
             if not exercises_dict[id_list[(previous_id_index + i * (-1) ** reverse) % len(id_list)]]['accepted']:
                 next_id = id_list[(previous_id_index + i * (-1) ** reverse) % len(id_list)]
             i += 1
         if next_id == -1:
-            print("\nYou already solved everything, there is no unsolved exercise to go to!\n")
+            print(
+                '\n' * settings['new_lines_above']
+                + "You already solved everything, there is no unsolved exercise to go to!"
+                + '\n' * settings['new_lines_below']
+            )
             return config
 
     # Store new exercise
     config['exercise_id'] = str(next_id)
     config['exercise_name'] = exercises_dict[next_id]['name']
     if exercises_dict[next_id]['programming_language']:
         config['programming_language'] = exercises_dict[next_id]['programming_language']['name']
 
     prefixes = make_visual_representation(previous_id, previous_id_index, next_id, id_list)
 
-    pretty_print.print_exercise_data(exercise_data_json, prefixes)
+    pretty_print.print_exercise_data(exercise_data_json, settings, prefixes)
 
     # Handle potential boilerplate.
     # I decided to not print the boilerplate (as a 'select' would do), it felt too clunky here.
     boilerplate = exercises_dict[next_id]['boilerplate']
     if boilerplate is not None and boilerplate.strip() != "":
         file_extension = exercises_dict[next_id]['programming_language']['extension']
-        print(f"\nBoilerplate code is put in 'boilerplate.{file_extension}'-file\n")
+        print(f"Boilerplate code is put in 'boilerplate.{file_extension}'-file" + '\n' * settings['new_lines_below'])
         with open(f"boilerplate.{file_extension}", "w") as boilerplate_file:
             boilerplate_file.write(boilerplate)
 
     return config
 
 
-def get_next_series(config, connection, headers, reverse, unsolved):
+def get_next_series(config, settings, connection, headers, reverse, unsolved):
     if config['serie_token']:
-        print("\nSorry, you can't use 'next' when inside a hidden series.\n")
+        print(
+            '\n' * settings['new_lines_below']
+            + "Sorry, you can't use 'next' when inside a hidden series."
+            + '\n' * settings['new_lines_below']
+        )
         return config
 
+    # Only import when we need it, speeds things up
     from dodonacli.source import get_data, pretty_print
+
     # Get all series of selected course
     series_data_json = get_data.series_data(
         connection, headers, config['course_id']
     )
 
     # Take only necessary info from the large json
     # Series have an order, so sort them so the order is guarenteed
@@ -130,57 +145,64 @@
     previous_id = config['serie_id']
     previous_id_index = id_list.index(int(previous_id))
 
     # Find the next series (loop back to front if it was the last)
     # If series ever get a solved/unsolved status support in API, this can get
     # the same logic found in get_next_exercise()
     if unsolved:
-        print("\nUnsolved flag not supported yet for series and courses.\n")
+        print(
+            '\n' * settings['new_lines_above']
+            + "Unsolved flag not supported yet for series and courses."
+            + '\n' * settings['new_lines_below']
+        )
     next_id = id_list[(previous_id_index + 1 - (2 * reverse)) % len(id_list)]
 
     # Store new series
     config['serie_id'] = str(next_id)
     config['serie_name'] = [
         series['name'] for series in series_list if series['id'] == next_id
     ][0]
 
     prefixes = make_visual_representation(previous_id, previous_id_index, next_id, id_list)
-
-    pretty_print.print_series_data(series_data_json, prefixes=prefixes)
+    pretty_print.print_series_data(series_data_json, settings, prefixes=prefixes)
 
     return config
 
 
-def get_next_course(config, connection, headers, reverse, unsolved):
+def get_next_course(config, settings, connection, headers, reverse, unsolved):
     from dodonacli.source import get_data, pretty_print
+
     # Get all registred courses
     course_data_json = get_data.courses_data(connection, headers)
 
-    # Simplified data
-    # courses_dict = {course['id']: course['name'] for course in course_data_json}
-
     id_list = [course['id'] for course in course_data_json]
     previous_id = config['course_id']
     previous_id_index = id_list.index(int(previous_id))
 
     # Find the next course (loop back to front if it was the last)
     # If courses get more data that indicates if it's completely solved,
     # then this will get the same logic found in get_next_exercise()
     if unsolved:
-        print("\nUnsolved flag not supported yet for series and courses.\n")
+        pretty_print.custom_print(
+            "Unsolved flag not supported yet for series and courses.",
+            {'new_lines_above': settings['new_lines_above']}
+        )
+
     next_id = id_list[(previous_id_index + 1 - (2 * reverse)) % len(id_list)]
 
     # Store new course
     config['course_id'] = str(next_id)
     config['course_name'] = [
         course['name'] for course in course_data_json if course['id'] == next_id
     ][0]
 
     prefixes = make_visual_representation(previous_id, previous_id_index, next_id, id_list)
-    pretty_print.print_courses_data(course_data_json, prefixes=prefixes)
+    pretty_print.print_courses_data(
+        course_data_json, {'new_lines_below': settings['new_lines_below']}, prefixes=prefixes
+    )
 
     return config
 
 
 def make_visual_representation(previous_id, previous_id_index, next_id, id_list) -> dict:
     next_id_index = id_list.index(int(next_id))
```

### Comparing `dodonacli-2024.5.16/dodonacli/commands/display.py` & `dodonacli-2024.5.20/dodonacli/commands/display.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,41 +8,43 @@
               is_flag=True, default=False)
 def display(force):
     import http.client
     from dodonacli.source import get_data, pretty_print
 
     # Read configs in
     config = get_data.get_configs()
+    settings = get_data.get_settings()
 
     # Start up the connection to Dodona
     connection = http.client.HTTPSConnection("dodona.be")
     headers = {
         "Content-type": "application/json",
         "Accept": "application/json",
         "Authorization": config['TOKEN']
     }
 
     # Display flag changes behaviour depending on the values in the config-dictionary.
     if config['course_id'] is None:
         # Print available courses
         json_data = get_data.courses_data(connection, headers)
-        pretty_print.print_courses_data(json_data)
+        pretty_print.print_courses_data(json_data, settings)
 
     elif config['serie_id'] is None:
         # Print available series
         json_data = get_data.series_data(connection, headers, config['course_id'])
-        pretty_print.print_series_data(json_data, force)
+        pretty_print.print_series_data(json_data, settings, force)
 
     elif config['exercise_id'] is None:
         # Print available exercises
         if config['serie_token'] is None:
             serie_token = ""
         else:
             serie_token = "?token=" + config['serie_token']
 
         json_data = get_data.exercises_data(connection, headers, config['serie_id'], serie_token)
-        pretty_print.print_exercise_data(json_data)
+        pretty_print.print_exercise_data(json_data, settings)
 
     else:
         # Print exercise-description
+        settings = get_data.get_settings()
         json_data = get_data.exercise_data(connection, headers, config['course_id'], config['exercise_id'])
-        pretty_print.print_exercise(json_data, config['TOKEN'], force)
+        pretty_print.print_exercise(json_data, config['TOKEN'], settings, force)
```

### Comparing `dodonacli-2024.5.16/dodonacli/commands/post.py` & `dodonacli-2024.5.20/dodonacli/commands/post.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,60 +19,82 @@
 @click.argument('file', type=click.Path(exists=True, file_okay=True, dir_okay=False, resolve_path=True))
 def post(file, use_link, check):
     import http.client
     from dodonacli.source import set_data, get_data, syntax_checker
 
     # Read configs in
     config = get_data.get_configs()
+    settings = get_data.get_settings()
+
+    # Quick check if combination of selected exercise and -l flag are valid
+    if not use_link and not config['exercise_id']:
+        print(
+            '\n' * settings['new_lines_above']
+            + "No exercise selected! If you want to use a link at the top of your file, use the -l flag."
+            + '\n' * settings['new_lines_below']
+        )
 
     # Start up the connection to Dodona
     connection = http.client.HTTPSConnection("dodona.be")
     headers = {
         "Content-type": "application/json",
         "Accept": "application/json",
         "Authorization": config['TOKEN']
     }
 
     # Check for the link at the top of the file
     if use_link:
         with open(file, 'r') as solutionfile:
             link = solutionfile.readline()
-            if link[:2] == '#!':
+
+            # If file starts with hashbang, look at 2nd line
+            if link[:2].strip() == '#!':
+                hashbang = link
                 link = solutionfile.readline()
+
+            # Check if valid link to try to post to
             link_index = link.find("https://dodona.be/")
             if link_index < 0:
-                print("\nNo valid link found on the first line of your file. Please confirm again.\n"
-                      "A valid link starts with 'https://dodona.be/'\n")
+                print(
+                    '\n' * settings['new_lines_above']
+                    + "No valid link found on the first line of your file. Please confirm again.\n"
+                      "A valid link starts with 'https://dodona.be/'"
+                    + '\n' * settings['new_lines_below']
+                )
                 return
             link = link[link_index:]
 
+            # Take out the id's we need
             if link.find("/courses/") != -1:
                 course_id_index_start = link.find("/courses/") + len("/courses/")
                 course_id_index_stop = link.find("/", course_id_index_start)
                 course_id = link[course_id_index_start:course_id_index_stop]
             else:
                 course_id = None
+
             exercise_id_index_start = link.find("/activities/") + len("/activities/")
             exercise_id_index_stop = link.find("/", exercise_id_index_start)
             exercise_id = link[exercise_id_index_start:exercise_id_index_stop]
 
             # We can read the content of the file now as the file-pointer is already at the 2nd line
-            content = solutionfile.read()
+            if hashbang:
+                content = hashbang + solutionfile.read()
+            else:
+                content = solutionfile.read()
+
     else:
-        # Syntax check not available with link at top of file
+        # Syntax check only available without link at top of file
         if check:
             if not syntax_checker.check_syntax(file, config['programming_language']):
                 return
 
         with open(file, 'r') as solutionfile:
             content = solutionfile.read()
+
         course_id = config['course_id']
         exercise_id = config['exercise_id']
 
-    # Make sure the amount of newlines is exactly 1
+    # Make sure the amount of newlines is exactly 1 to make Dodona's linters happy
     content = content.rstrip() + "\n"
 
-    # Post exercise to Dodona, does not work if there is no exercise selected or -l flag not used
-    if not use_link and not config['exercise_id']:
-        print("\nNo exercise selected! If you want to use a link at the top of your file, use the -l flag.\n")
-    else:
-        set_data.post_solution(content, connection, headers, course_id, exercise_id)
+    # Post exercise to Dodona
+    set_data.post_solution(content, connection, headers, course_id, exercise_id, settings)
```

### Comparing `dodonacli-2024.5.16/dodonacli/commands/submission.py` & `dodonacli-2024.5.20/dodonacli/commands/submission.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,39 +34,41 @@
         json_all_submissions = get_data.all_submissions(connection, headers)
         extension = ""
 
     submission = json_all_submissions[-int(number)]
 
     submission_info = get_data.submission_info(submission['id'], connection, headers, config)
     set_data.save_to_file(
-        submission_info['exercise_name'], submission_info['id'], submission_info['code'], extension
+        submission_info['exercise_name'], submission_info['id'], submission_info['code'],
+        get_data.get_settings(), extension
     )
 
     return
 
 
 @click.command(help="View subimmision data")
 def view():
     import http.client
     from dodonacli.source import get_data, pretty_print
 
     # Read configs in
     config = get_data.get_configs()
+    settings = get_data.get_settings()
 
     # Start up the connection to Dodona
     connection = http.client.HTTPSConnection("dodona.be")
     headers = {
         "Content-type": "application/json",
         "Accept": "application/json",
         "Authorization": config['TOKEN']
     }
 
     if config['exercise_id']:
         json_data = get_data.exercise_submissions(config, connection, headers)
-        pretty_print.print_exercise_submissions(json_data)
+        pretty_print.print_exercise_submissions(json_data, settings)
     else:
         json_data = get_data.all_submissions(connection, headers)
-        pretty_print.print_all_submissions(connection, headers, json_data)
+        pretty_print.print_all_submissions(connection, headers, json_data, settings)
 
 
 sub.add_command(load)
 sub.add_command(view)
```

### Comparing `dodonacli-2024.5.16/dodonacli/commands/up.py` & `dodonacli-2024.5.20/dodonacli/commands/up.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,38 @@
                     "Can be used with an argument to deselect everything with "
                     "'all' or 'top', or deselect 1, 2 or 3 levels.")
 @click.argument('amount', default='1',
                 type=click.Choice(['all', 'top', '1', '2', '3'], 
                                   case_sensitive=False))
 def up(amount):
     from dodonacli.source import set_data, get_data
+
     # Read configs in
     config = get_data.get_configs()
+    settings = get_data.get_settings()
 
     if str(amount).lower().strip() in ('all', 'top'):
         for e in ('exercise_id', 'exercise_name', 'serie_id', 'serie_name', 'serie_token', 'course_id', 'course_name'):
             config[e] = None
-        print("\nDeselected everything.\n")
+        print(
+            '\n' * settings['new_lines_above']
+            + "Deselected everything."
+            + "\n" * settings['new_lines_below']
+        )
 
     elif not isinstance(amount, int) and not amount.isnumeric():
-        print("You didn't provide a number or 'all', nothing deselected.")
+        print(
+            '\n' * settings['new_lines_above']
+            + "You didn't provide a number or 'all', nothing deselected."
+            + "\n" * settings['new_lines_below']
+        )
 
     else:
         levels = int(amount)
-        print()
+        print('\n' * settings['new_lines_above'], end='')
         for _ in range(levels):
             if config.get('exercise_id') is not None:
                 config['exercise_id'] = None
                 config['exercise_name'] = None
                 config['programming_language'] = None
                 print("Deselected exercise.")
             elif config.get('serie_id') is not None:
@@ -37,10 +47,10 @@
             elif config.get('course_id') is not None:
                 config['course_id'] = None
                 config['course_name'] = None
                 print("Deselected course")
             else:
                 print("Nothing selected.")
                 break
-        print()
+        print('\n' * settings['new_lines_below'], end='')
 
     set_data.dump_config(config)
```

### Comparing `dodonacli-2024.5.16/dodonacli/main.py` & `dodonacli-2024.5.20/dodonacli/main.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.16/dodonacli/source/get_data.py` & `dodonacli-2024.5.20/dodonacli/source/get_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     """
     Get config data from config.json
     :return: json object with config data
     """
     # Get the path of the config-file.
     config_file_path = os.path.join(get_config_home(), "config.json")
 
-    # fallback to the old path
+    # Fallback to the old path
     needs_migration = False
     if not os.path.exists(config_file_path):
         config_file_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "../../config.json")
         needs_migration = True
 
     # First try to open, if unable to open, create a new config-file and ask user for a token
     try:
@@ -263,24 +263,22 @@
                       "exercise_name"]
         }
 
         print("\nThis may be your first time using DodonaCLI, do you wish to follow a short tutorial?")
         answer = input("(yes/no): ")
 
         if answer.lower().startswith("yes"):
-            config = interactive_tutorial.start_tutorial(config)
+            settings = get_settings()
+            config = interactive_tutorial.start_tutorial(config, settings)
         else:
-            TOKEN = input('API-Token not found! Enter your code here: ')
-            config["TOKEN"] = TOKEN
+            config["TOKEN"] = input('API-Token not found! Enter your code here: ')
 
         # Save configs
         set_data.dump_config(config)
 
-        exit(0)
-
     return config
 
 
 def validate_config(config: dict):
     """
     Checks whether the config file contains all the necessary keys.
     This is needed when an update introduces new keys.
@@ -290,15 +288,15 @@
     keys_to_check = (
         "course_id", "course_name",
         "serie_id", "serie_name",
         "exercise_id", "exercise_name",
         "serie_token", "programming_language"
     )
     for key in keys_to_check:
-        if key not in config:
+        if key not in config or (not isinstance(config[key], str) and config[key] is not None):
             config[key] = None
 
     if "TOKEN" not in config:
         print("API token not found.")
         config = get_api_token(config)
 
     # Not needed any more with the "info update" command
@@ -314,7 +312,73 @@
     :param config: Dictionary with the content of config.json
     :return: Updated config dictionary
     """
     config['TOKEN'] = input("Paste your API-token here: ")
     set_data.dump_config(config)
 
     return config
+
+
+def get_settings():
+    """
+    Get the contents of settings.json and return it.
+    If the file didn't exist yet, the default settings will be made
+    :return: Settings dictionary
+    """
+    # Get the path of the config-file.
+    settings_file_path = os.path.join(get_config_home(), "settings.json")
+
+    # First try to open, if unable to open, create a new settings-file
+    try:
+        with open(settings_file_path, "r") as file:
+            settings = json.load(file)
+            settings = validate_settings(settings)
+
+    except FileNotFoundError:
+        settings = {}
+        settings = validate_settings(settings)
+        set_data.dump_settings(settings)
+
+    return settings
+
+
+def validate_settings(settings: dict):
+    """
+    Make sure that all the needed settings are present,
+    if they're absent, they will be set to the default value
+    :param settings: Dictionary with settings to validate
+    :return: Updated settings dictionary
+    """
+    # Settings to check, with their default value
+    settings_to_check = {
+        'amount_feedback_context': 3,
+        'amount_feedback_tab': -1,
+        'amount_feedback_testcase': 3,
+        'amount_feedback_test': 3,
+        'amount_sub_exercise': 10,
+        'amount_sub_global': -1,
+        'new_lines_above': 1,
+        'new_lines_below': 1,
+        'paste_force_warning': True,
+        'display_series_after_select': False,
+        'display_exercises_after_select': False,
+        'display_exercise_after_select': False
+    }
+
+    anything_changed = False
+
+    # Remove redundant settings
+    for setting in list(settings.keys()):
+        if setting not in settings_to_check:
+            settings.pop(setting)
+            anything_changed = True
+
+    # Add missing settings with their default value
+    for setting in settings_to_check:
+        if setting not in settings or not isinstance(settings[setting], type(settings_to_check[setting])):
+            settings[setting] = settings_to_check[setting]
+            anything_changed = True
+
+    if anything_changed:
+        set_data.dump_settings(settings)
+
+    return settings
```

### Comparing `dodonacli-2024.5.16/dodonacli/source/interactive_tutorial.py` & `dodonacli-2024.5.20/dodonacli/source/interactive_tutorial.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 import json
 import os
 
 import dodonacli.source.get_data
 from . import pretty_print, pretty_console, set_data
 
 
-def start_tutorial(config: dict):
+def start_tutorial(config: dict, settings: dict):
     """
     Runs the tutorial and asks for API token if it wasn't present yet.
-    :param config: dict
+    :param config: dict with configs
+    :param settings: dict with settings
     :return: config: dict
     """
     # Clear screen for tutorial
     os.system('cls' if os.name == 'nt' else 'clear')
     print(
         "Welcome to the Dodona CLI,\n"
         "this tutorial will show you everything you need to interact\n"
@@ -41,20 +42,20 @@
     connection = http.client.HTTPSConnection("dodona.be")
     headers = {
         "Content-type": "application/json",
         "Accept": "application/json",
         "Authorization": config['TOKEN']
     }
 
-    config = tutorial_select_course(config, connection, headers)
-    config = tutorial_select_series(config, connection, headers)
-    config = tutorial_select_exercise(config, connection, headers)
+    config = tutorial_select_course(config, connection, headers, settings)
+    config = tutorial_select_series(config, connection, headers, settings)
+    config = tutorial_select_exercise(config, connection, headers, settings)
 
-    tutorial_view_exercise(config, connection, headers)
-    tutorial_post_exercise(config, connection, headers)
+    tutorial_view_exercise(config, connection, headers, settings)
+    tutorial_post_exercise(config, connection, headers, settings)
 
     config = tutorial_conclude(config)
 
     return config
 
 
 def tutorial_handle_connection(config: dict, connection: http.client.HTTPSConnection):
@@ -81,30 +82,30 @@
     data = res.read()
     connection.close()
 
     return json.loads(data)
 
 
 def tutorial_select_course(config: dict, connection: http.client.HTTPSConnection,
-                           headers: dict):
+                           headers: dict, settings: dict):
     os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
         "Use the command `dodona display` to show the available courses."
     )
 
     command = input("$ ")
 
     while command.rstrip() != "dodona display":
         print("That was not the right command, please try again")
         command = input("$ ")
 
     connection.request("GET", "/courses?tab=featured", headers=headers)
     json_data = tutorial_handle_connection(config, connection)
 
-    pretty_print.print_courses_data(json_data, "Featured courses")
+    pretty_print.print_courses_data(json_data, settings, "Featured courses")
 
     pretty_console.console.print(
         "\nSelect now \"The Coder's Apprenctice\" with `dodona select` + the courses id,"
         "\nor (distinct part of) the courses name"
     )
     command = input("$ ")
 
@@ -130,15 +131,15 @@
     )
     input(" <Enter to continue>")
 
     return config
 
 
 def tutorial_select_series(config: dict, connection: http.client.HTTPSConnection,
-                           headers: dict):
+                           headers: dict, settings: dict):
     os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
         "Use the command `dodona display` to show the available exercise-series."
     )
     command = input("$ ")
 
     while command.strip() != "dodona display":
@@ -148,15 +149,15 @@
     connection.request(
         "GET", "/courses/" + str(config['course_id']) + '/series',
         headers=headers)
     json_data = tutorial_handle_connection(config, connection)
 
     # To prevent the screen being blasted with a lot of text,
     # only print out the first 6 exercise series
-    pretty_print.print_series_data(json_data[:6])
+    pretty_print.print_series_data(json_data[:6], settings)
 
     pretty_console.console.print(
         "Select now \"2. Using Python\" with `dodona select` + the series' id,"
         "\nor (distinct part of) the series' name."
     )
     command = input("$ ")
 
@@ -190,15 +191,15 @@
     print("Fantastic, let's move on to selecting an exercise.\n")
     input(" <Enter to continue>")
 
     return config
 
 
 def tutorial_select_exercise(config: dict, connection: http.client.HTTPSConnection,
-                             headers: dict):
+                             headers: dict, settings: dict):
     os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
         "Use the command `dodona display` to show the available exercises."
     )
     command = input("$ ")
 
     while command.strip() != "dodona display":
@@ -208,15 +209,15 @@
     connection.request(
         "GET",
         "/series/" + str(config['serie_id']) + '/activities',
         headers=headers
     )
     json_data = tutorial_handle_connection(config, connection)
 
-    pretty_print.print_exercise_data(json_data)
+    pretty_print.print_exercise_data(json_data, settings)
 
     pretty_console.console.print(
         "Select now \"Hello, World!\" with `dodona select` + the series' id,\n"
         "or (distinct part of) the series' name."
     )
     command = input("$ ")
 
@@ -253,15 +254,15 @@
     )
     input(" <Enter to continue>")
 
     return config
 
 
 def tutorial_view_exercise(config: dict, connection: http.client.HTTPSConnection,
-                           headers: dict):
+                           headers: dict, settings: dict):
     os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
         "Use the command `dodona display` to show the description of the exercise."
     )
     command = input("$ ")
 
     while command.strip() != "dodona display":
@@ -272,21 +273,21 @@
         "GET",
         f"/courses/{str(config['course_id'])}"
         + f"/series/{str(config['serie_id'])}"
         + f"/activities/{str(config['exercise_id'])}",
         headers=headers)
 
     json_data = tutorial_handle_connection(config, connection)
-    pretty_print.print_exercise(json_data, config['TOKEN'])
+    pretty_print.print_exercise(json_data, config['TOKEN'], settings)
 
     input(" <Enter to continue>")
 
 
 def tutorial_post_exercise(config: dict, connection: http.client.HTTPSConnection,
-                           headers: dict):
+                           headers: dict, settings: dict):
     os.system('cls' if os.name == 'nt' else 'clear')
     pretty_console.console.print(
         "Now you can post the solution. You don't need to write any code for this exercise, \n"
         "as it is already writtin in the 'boilerplate.py'-file.\n"
         "You can post it with the command `dodona post <SOLUTION_FILE_NAME>`.\n"
         "Replace <SOLUTION_FILE_NAME> with the correct file-name, in this case 'boilerplate.py'."
     )
@@ -294,15 +295,16 @@
 
     while command.strip() != "dodona post boilerplate.py":
         print("That was not the right command, please try again")
         command = input("$ ")
 
     set_data.post_solution(
         "print( \"Hello, world!\" )",
-        connection, headers, config['course_id'], config['exercise_id']
+        connection, headers, config['course_id'], config['exercise_id'],
+        settings
     )
 
     pretty_console.console.print(
         "Nice, programmed that like a pro.\n"
         "You're nearly done with this tutorial, I want to show you one last thing. \n"
     )
     input(" <Enter to continue>")
```

### Comparing `dodonacli-2024.5.16/dodonacli/source/pretty_print.py` & `dodonacli-2024.5.20/dodonacli/source/pretty_print.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 import http.client
 import json
 import markdownify
 import re
-import shutil
-import textwrap
 
 from bs4 import BeautifulSoup
 from rich.markdown import Markdown
 from rich.padding import Padding
 
 from . import get_data, pretty_console, submission_data_handler
 
 
-def print_courses_data(json_data: dict, title: str = "Your courses:", prefixes: dict = None):
+def custom_print(text: str, settings: dict, pretty: bool = False):
+    """
+    Prints out the text with the amount of newlines specified in settings
+    :param text: text to print
+    :param settings: dict with settings
+    :param pretty: whether to use the pretty_console print, or the standard Python print
+    """
+    if pretty:
+        printer = pretty_console.console.print
+    else:
+        printer = print
+
+    printer(
+        '\n' * settings.get('new_lines_above', 0)
+        + text
+        + '\n' * settings.get('new_lines_below', 0)
+    )
+
+
+def print_courses_data(json_data: dict, settings: dict, title: str = "Your courses:", prefixes: dict = None):
     """
     Print out the courses in json_data in a neat way
     :param json_data: json object with data about Dodona courses
+    :param settings: dict with settings
     :param title: title to display above the courses-list
     :param prefixes: dictionary with a prefix for each id in json_data
     """
     if prefixes is None:
         prefixes = {}
 
     # List of tuples where each tuple represents a course by id, name and teacher
-    display_data = []
+    display_data: list[tuple] = []
 
     for field in json_data:
         display_data.append((str(field['id']), field['name'], field['teacher']))
 
     # Find the maximum length of all but the last element in all tuples to align them in the terminal
     max_course_id_length = max(len(e[0]) for e in display_data)
     max_course_name_length = max(len(e[1]) for e in display_data)
 
     # Print out all courses in display_data
-    pretty_console.console.print(f'\n[u bright_blue]{title}[/]')
+    result = f'[u bright_blue]{title}[/]\n'
     for course in display_data:
-        pretty_console.console.print(
-            (prefixes.get(course[0]) or "\t") +
-            f"{course[0].ljust(max_course_id_length)}: "
-            f"[bold]{course[1].ljust(max_course_name_length)}[/]\tby {course[2]}"
-        )
-    # Newline for clarity
-    print()
+        result += (prefixes.get(course[0]) or "\t")
+        result += (f"{course[0].ljust(max_course_id_length)}: [bold]"
+                   f"{course[1].ljust(max_course_name_length)}[/]\tby {course[2]}\n")
 
+    custom_print(result.strip(), settings, pretty=True)
 
-def print_series_data(json_data: dict, force: bool = False, prefixes: dict = None):
+
+def print_series_data(json_data: dict, settings: dict, force: bool = False, prefixes: dict = None):
     """
-    Print out the exercise-series in json_data in a neat way.
+    Print out the exercise-series in json_data in a neat (unless force) way.
     :param json_data: Json object with data about Dodona exercise-series
+    :param settings: dict with settings
     :param force: Boolean to decide if the series description has to be printed, or only a link to it
     :param prefixes: Dictionary with a prefix for each id in json_data
     """
     if prefixes is None:
         prefixes = {}
 
     # List of tuples where each tuple represents an exercise-series by id, name and description
@@ -66,73 +83,49 @@
             )
         )
 
     # Find the maximum length of all but the last element in all tuples to align them in the terminal
     max_series_id_length = max(len(e[0]) for e in display_data)
     max_series_name_length = max(len(e[1]) for e in display_data)
 
-    # Newline for clarity
-    print()
     # Print out all the series in display_data while also handling the Markdown inside the series-description
-    pretty_console.console.print("[u bright_blue]All series:[/]")
-    for series in display_data:
-        if force:
-            description = series[2].split('\n')
-            new_description = ''
-
-            for line in description:
-                line = line.rstrip()
-
-                # Remove target pattern from links as they try to open the link in a new tab, not useful for terminal
-                line = re.sub(r'{: target="_blank"}', '', line)
-
-                # Replace Markdown bold to Rich Console bold
-                line = re.sub(r'\*\*(.*?)\*\*', r'[bold]\1[/bold]', line)
-
-                # Replace Markdown italics to Rich Console italics if it is not in a (link)
-                pattern = re.compile(r'([ ,][^ (]*)_(.*?)_([^ ]*[ ,.])')
-                line = pattern.sub(r'\1[i]\2[/i]\3', line)
-
-                # Replace Markdown titles to something that appears as a title in terminal
-                line = re.sub(r'##+ (.*)', r'[bold white]\1[/bold white]', line)
-
-                # Split lines in multiple when they are too long for the terminal while keeping all lines indented.
-                if len(line.replace("[bold]", "").replace("[/bold]", "")) > shutil.get_terminal_size().columns - 8:
-                    line = line.split(" ")
-                    new_line = ''
-                    line_size = 0
-                    for word in line:
-                        if line_size + len(word) > shutil.get_terminal_size().columns - 8:
-                            new_line += '\n'
-                            line_size = 0
-                        new_line += word + ' '
-                        line_size += len(word + ' ')
-                    line = new_line
+    result = "[u bright_blue]All series:[/]\n"
+    if force:
+        pretty_console.console.print('\n' * settings['new_lines_above'] + result, end='')
+
+        for i, series in enumerate(display_data):
+            description = series[2].strip('\n')
+            description = re.sub(r'{: *target="_blank"}', '', description).strip()
+            md_description = Markdown(markdownify.markdownify(description))
 
-                new_description += line + '\n'
-
-            new_description = textwrap.indent(new_description, '\t')
             pretty_console.console.print(
                 f"\t{series[0].ljust(max_series_id_length)}: "
                 f"[bold]{series[1].ljust(max_series_name_length)}[/]"
-                f"\n{new_description}")
-        else:
+            )
             pretty_console.console.print(
-                (prefixes.get(series[0]) or "\t")
-                + f"{series[0].ljust(max_series_id_length)}: "
-                + f"[bold]{series[1].ljust(max_series_name_length)}[/]"
+                Padding(
+                    md_description,
+                    pad=(0, 0, 1 if description and i + 1 < len(display_data) else 0, 12)
+                ), end=''
             )
-    # Newline for clarity
-    print()
+        print('\n' * settings['new_lines_below'], end='')
+
+    else:
+        for i, series in enumerate(display_data):
+            result += prefixes.get(series[0]) or "\t"
+            result += f"{series[0].ljust(max_series_id_length)}: [bold]{series[1].ljust(max_series_name_length)}[/]\n"
+
+        custom_print(result.strip(), settings, pretty=True)
 
 
-def print_exercise_data(json_data: dict, prefixes: dict = None):
+def print_exercise_data(json_data: dict, settings: dict, prefixes: dict = None):
     """
     Print out the exercises in json_data in a neat way
     :param json_data: json object with data about Dodona exercises in a series
+    :param settings: dict with settings
     :param prefixes: dictionary with a prefix for each id in json_data
     """
     if prefixes is None:
         prefixes = {}
 
     # List of tuples where each tuple represents an exercise by id, name, solved and has_attempt
     display_data = []
@@ -157,121 +150,118 @@
             })
 
     # Find the maximum length of all but the last element in all tuples to align them in the terminal
     max_exercise_id_length = max(len(e['id']) for e in display_data)
     max_exercise_name_length = max(len(e['name']) for e in display_data)
 
     # Print out all exercises in display_data with indicator about solution-status: solved, wrong or not yet solved
-    pretty_console.console.print('\n[u bright_blue]Exercises:[/]')
+    result = '[u bright_blue]Exercises:[/]\n'
     for exercise in display_data:
         if exercise['type'] == "Exercise":
             if exercise['accepted']:
                 solve_status = "[bold bright_green]SOLVED[/]"
             elif exercise['has_solution']:
                 solve_status = "[bold bright_red]WRONG[/]"
             else:
                 solve_status = "[bold]NOT YET SOLVED[/]"
 
-            """
-            if not exercise['has_solution']:
-                solve_status = "[bold]NOT YET SOLVED[/]"
-            elif exercise['last_solution_is_best'] and exercise['has_correct_solution']:
-                solve_status = "[bold bright_green]SOLVED[/]"
-            else:
-                solve_status = "[bold bright_red]WRONG[/]"
-            """
-
         elif exercise['type'] == "ContentPage":
             if exercise['has_read']:
                 solve_status = "[bold bright_green]READ[/]"
             else:
                 solve_status = "[bold]NOT YET READ[/]"
 
         else:
             solve_status = "[bold]SOLVE STATUS UNKNOWN"
 
-        pretty_console.console.print(
-            (prefixes.get(exercise['id']) or "\t")
-            + f"{exercise['id'].ljust(max_exercise_id_length)}: "
-            + f"[bold]{exercise['name'].ljust(max_exercise_name_length)}[/]\t"
-            + solve_status
-        )
-    # Newline for clarity
-    print()
+        result += (prefixes.get(exercise['id']) or "\t")
+        result += f"{exercise['id'].ljust(max_exercise_id_length)}: "
+        result += f"[bold]{exercise['name'].ljust(max_exercise_name_length)}[/]\t" + solve_status + '\n'
 
+    custom_print(result.strip(), settings, pretty=True)
 
-def print_exercise(json_data: dict, token: str, force: bool = False):
+
+def print_exercise(json_data: dict, token: str, settings: dict, force: bool = False):
     """
     Print out the exercise-description.
     Needs to call the Dodona sandbox and convert HTML to text.
     Print out a warning for potential incompleteness, which may be dangerous for tests and exams.
     :param token: API-token as authorization
     :param json_data: json object with info about a Dodona exercise
     :param force: boolean to decide if the exercise description has to be printed, or only a link to it
+    :param settings: dict with settings
     """
     if json_data['type'] == 'ContentPage':
-        pretty_console.console.print(
-            "\nNo need to program anything this time, but you'll have to go read this and mark it as read:\n"
-            + json_data['url'].replace(".json", "") + '\n'
+        custom_print(
+            "No need to program anything this time, but you'll have to go read this and mark it as read:\n"
+            + json_data['url'].replace(".json", ""),
+            settings, pretty=True
         )
 
     elif not force:
-        pretty_console.console.print(
-            f"\nYou can find the exercise description at \n{json_data['description_url']}\n"
+        custom_print(
+            f"You can find the exercise description at \n{json_data['description_url']}",
+            settings,
+            pretty=True
         )
 
     else:
-        # Print the HTML with warnings
-        warning = (
-                "\n[u bold bright_red]WARNING:[/] the description may be incorrect, "
-                "DO NOT rely on this for exams and tests!\n"
-                "View in browser: " + json_data['description_url'] + '\n'
-        )
-        pretty_console.console.print(warning)
-
-        pretty_console.console.print(
-            '\n'
-            "Expected programming language: " + json_data['programming_language']['name'] +
-            '\n'
+        custom_print(
+            "Expected programming language: " + json_data['programming_language']['name'] + '\n',
+            {'new_lines_above': settings['new_lines_above']},
+            pretty=True
         )
 
         # Make sandbox.dodona connection for exercise description:
         sandbox = http.client.HTTPSConnection("sandbox.dodona.be")
         headers = {"Authorization": token}
 
         stripped_link = json_data['description_url'].replace("https://sandbox.dodona.be", "", 1)
         sandbox.request("GET", stripped_link, headers=headers)
 
         data = get_data.handle_connection_response(sandbox).decode()
 
         soup = BeautifulSoup(data, features="html.parser")
         html_description = str(soup.find("div", {"class": "card-supporting-text"}))
 
-        md_description = markdownify.markdownify(html_description)
+        md_description = markdownify.markdownify(html_description).strip()
 
         md = Markdown(md_description)
 
-        pretty_console.console.print(Padding(md, pad=(0, 0, 0, 3)))
+        if settings['paste_force_warning']:
+            # Print the HTML with warnings
+            warning = (
+                    "\n[u bold bright_red]WARNING:[/] the description may be incorrect, "
+                    "DO NOT rely on this for exams and tests!\n"
+                    "View in browser: " + json_data['description_url'] + '\n'
+            )
+            pretty_console.console.print(warning)
+            pretty_console.console.print(Padding(md, pad=(0, 0, 0, 3)))
+            pretty_console.console.print(warning)
+        else:
+            pretty_console.console.print(Padding(md, pad=(0, 0, 0, 3)))
 
-        # Print the HTML with warnings
-        pretty_console.console.print(warning)
+        print('\n' * settings['new_lines_below'], end='')
 
 
-def print_result(json_results: dict):
+def print_result(json_results: dict, url: str, settings: dict):
     """
     Print out the results of a submission in a neat way
     :param json_results: json object with data about a submission
+    :param url: link to the submission
+    :param settings: dict with settings
     """
     if json_results['accepted']:
         # Everything passed, well done!
-        pretty_console.console.print(
-            "[bold bright_green]All tests passed![/] You can continue to next exercise."
-        )
+        result = "[bold bright_green]All tests passed![/] You can continue to next exercise.\n"
     else:
-        pretty_console.console.print(submission_data_handler.submission_data_handler(json_results))
+        result = submission_data_handler.submission_data_handler(json_results, settings).strip() + '\n'
+
+    result += url
+    custom_print(result, settings, pretty=True)
 
 
 def print_status(config: dict):
     """
     Print out the current selection of course, exercise-series and exercise.
     :param config: Dictionary with the configs
     """
@@ -283,23 +273,29 @@
         f"\n[u bright_blue]Status:[/]\n"
         f"\t{'Course: '.ljust(10)}{course_string}\n"
         f"\t{'Series: '.ljust(10)}{config['serie_name']}\n"
         f"\t{'Exercise: '.ljust(10)}{config['exercise_name']}\n"
     )
 
 
-def print_exercise_submissions(json_data: dict):
+def print_exercise_submissions(json_data: dict, settings: dict):
     """
     Print out a list of the (up to) 10 most recent submissions as found in json_data
     :param json_data: Dictionary with submission data
+    :param settings: Dictionary with settings
     """
     pretty_console.console.print(
         "\n[u bright_blue]Most recent submissions:[/]"
     )
-    for i, submission in enumerate(json_data[:10]):
+
+    amount_shown = min(settings['amount_sub_exercise'], len(json_data))
+    if amount_shown == -1:
+        amount_shown = len(json_data)
+
+    for i, submission in enumerate(json_data[:amount_shown]):
         if submission['accepted']:
             accepted_emoji = "[bright_green]:heavy_check_mark:[/bright_green]"
         else:
             accepted_emoji = "[bright_red]:heavy_multiplication_x:[/bright_red]"
 
         status = submission['status']
         if submission['status'] in ("memory limit exceeded", "geheugenlimiet overschreden"):
@@ -309,28 +305,33 @@
             f"\t{accepted_emoji}  [link={submission['url'].rstrip('.json')}]#{len(json_data) - i: <2}[/link]"
             f"\t{status}\t"
         )
     # Newline for clarity
     print()
 
 
-def print_all_submissions(connection: http.client.HTTPSConnection, headers: dict, json_data: dict):
+def print_all_submissions(connection: http.client.HTTPSConnection, headers: dict, json_data: dict, settings: dict):
     """
     Print out a list of the latest 30 submissions for the user, userwide (not tied to an exercise).
     Makes extra requests to Dodona to get the name of the exercises of the submissions
     :param connection: Connection to Dodona
     :param headers: Headers to send with the connection
     :param json_data: Dictionary with submission info
+    :param settings: Dictionary with settings
     :return:
     """
     pretty_console.console.print(
         "\n[u bright_blue]Most recent submissions:[/]"
     )
 
-    for i, submission in enumerate(json_data):
+    amount_shown = min(settings['amount_sub_global'], len(json_data))
+    if amount_shown == -1:
+        amount_shown = len(json_data)
+
+    for i, submission in enumerate(json_data[:amount_shown]):
         if submission['accepted']:
             accepted_emoji = "[bright_green]:heavy_check_mark:[/bright_green]"
         else:
             accepted_emoji = "[bright_red]:heavy_multiplication_x:[/bright_red]"
 
         status = submission['status']
```

### Comparing `dodonacli-2024.5.16/dodonacli/source/set_data.py` & `dodonacli-2024.5.20/dodonacli/source/set_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,23 +21,39 @@
     if not os.path.exists(config_home):
         os.makedirs(config_home)
 
     with open(config_file_path, 'w') as config_file:
         json.dump(config, config_file)
 
 
+def dump_settings(settings: dict):
+    """
+    Save the settings to their file again.
+    :param settings: Dictionary containing the settings
+    """
+    config_home = get_data.get_config_home()
+    settings_file_path = os.path.join(config_home, "settings.json")
+
+    if not os.path.exists(config_home):
+        os.makedirs(config_home)
+
+    with open(settings_file_path, 'w') as settings_file:
+        json.dump(settings, settings_file, indent=4)
+
+
 def post_solution(content: str, connection: http.client.HTTPSConnection, headers: dict, course_id: str,
-                  exercise_id: str):
+                  exercise_id: str, settings):
     """
     Post the solution in content to Dodona and print the result
     :param content: str with the solution to post to Dodona
     :param connection: HTTPSConnection object that connects to www.dodona.be
     :param headers: dict with extra info for connection, mainly authorization needed
     :param course_id:
     :param exercise_id:
+    :param settings: dict with settings
     """
     # Make dict with info needed to post the solution and dump it in a json object
     payload = {
         "submission": {
             "code": content,
             "course_id": course_id,
             "exercise_id": exercise_id
@@ -46,61 +62,74 @@
     json_payload = json.dumps(payload)
 
     # Connect to Dodona and post the solution
     connection.request("POST", "/submissions.json", json_payload, headers=headers)
     res = connection.getresponse()
     status = res.status
     if status == 422:
-        pretty_console.console.print(
-            "\n[i]Patience, young padawan.\n"
-            "A cooldown, Dodona servers have, to prevent DDOS attacks, hmm, yes.[/]\n"
+        pretty_print.custom_print(
+            "[i]Patience, young padawan.\n"
+            "A cooldown, Dodona servers have, to prevent DDOS attacks, hmm, yes.[/]",
+            settings, pretty=True
         )
         return
 
     elif status != 200:
-        print("\nError connection to Dodona: " + str(res.status))
-        print("Reason: " + res.reason + '\n')
+        pretty_print.custom_print(
+            "Error connection to Dodona: " + str(res.status) + '\n'
+            + "Reason: " + res.reason,
+            settings, pretty=True
+        )
         return
 
     # Read out the result
     data = res.read()
     json_data = json.loads(data)
 
     # The Dodona servers take some time to test the solution, so we'll have to keeping asking for an answer.
     json_data['status'] = "running"
 
     # Spinner animation effect while waiting
-    print()
-    waiting = rich.status.Status("Posting your solution, please wait while the servers evaluate your code.",
-                                 spinner=select_spinner())
+    print('\n' * settings['new_lines_above'], end='')
+
+    # Disable the new_lines_above here for the further prints, but need more than just that settings,
+    # that's why I don't just make a new dict with only 'new_lines_below' in
+    settings['new_lines_above'] = 0
+
+    waiting = rich.status.Status(
+        "Posting your solution, please wait while the servers evaluate your code.",
+        spinner=select_spinner()
+    )
     waiting.start()
     wait_interval = 0
 
     while json_data['status'] in ("running", "queued"):
         # Aks the servers for the result with an increasing interval, from 1s to 5s, as the website does
         time.sleep(wait_interval)
         if wait_interval < 5:
             wait_interval += 1
 
         connection.request("GET", "/submissions/" + str(json_data['id']) + ".json", headers=headers)
         res = connection.getresponse()
         if res.status != 200:
             print("Error connection to Dodona: " + str(res.status))
-            print("Reason: " + res.reason)
+            print("Reason: " + res.reason, end='\n' * settings['new_lines_below'])
             return
 
         json_data: dict[str, str] = json.loads(res.read())
 
     waiting.stop()
     connection.close()
 
     # Print out the results
-    pretty_print.print_result(json.loads(json_data['result']))
-    pretty_console.console.print(json_data['url'][:json_data['url'].rfind('.')])
-    print()
+    pretty_print.print_result(
+        json.loads(json_data['result']),
+        json_data['url'][:json_data['url'].rfind('.')],
+        settings
+    )
 
 
 def select_spinner() -> str:
     """
     Select a random spinner-name from a preselected list with good animations.
     During Christmas season (11th of Decembre - 8th of January) it always returns the same Christmas spinner.
     :return: Name of Rich spinner
@@ -125,24 +154,28 @@
 
     if is_christmas_season:
         return christmas_spinner
 
     return random.choice(selection_spinners)
 
 
-def save_to_file(name: str, submission_id: int, content: str, extension: str = ""):
+def save_to_file(name: str, submission_id: int, content: str, settings: dict, extension: str = ""):
     """
     Save code to a file in the users current working directory.
     The resulting file name: {name}_{id}{extension}
     :param name: Name of the file
     :param submission_id: ID to add to the name of file
     :param content: Content to save in the file
+    :param settings: dict with settings
     :param extension: Optional file-extension, has to include the '.'
     """
     name = name.replace(' ', '-')
     file_name = f"{name}_{submission_id}{extension}"
 
     with open(file_name, "w") as code_file:
         code_file.write(content)
 
-    print(f"\nCode from your submission for {name} is now saved in:\n"
-          f"\t{name}_{submission_id}{extension}\n")
+    pretty_print.custom_print(
+        f"Code from your submission for {name} is now saved in:\n"
+        f"\t{name}_{submission_id}{extension}",
+        settings, pretty=True
+    )
```

### Comparing `dodonacli-2024.5.16/dodonacli/source/submission_data_handler.py` & `dodonacli-2024.5.20/dodonacli/source/submission_data_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,91 @@
-def submission_data_handler(submission_data: dict) -> str:
+def submission_data_handler(submission_data: dict, settings: dict) -> str:
     result = ""
-    result += submission_tabs_handler(submission_data)
+    result += submission_tabs_handler(submission_data, settings)
     result += submission_code_annotations(submission_data)
     return result
 
 
-def submission_tabs_handler(submission_data: dict) -> str:
+def submission_tabs_handler(submission_data: dict, settings: dict) -> str:
     """
     Handle all tabs, group together those that were accepted and delegate the failed tabs
     :param submission_data: dictionary with the results of a submission
+    :param settings: dictionary with settings
     :return: formatted string with info per tab
     """
     failed_tabs = []
     correct_tabs = []
     for tab in submission_data['groups']:
         if tab['badgeCount'] > 0:
             failed_tabs.append(tab)
         else:
             correct_tabs.append(tab)
 
+    if settings['amount_feedback_tab'] == -1:
+        amount_failed_display = len(failed_tabs)
+    else:
+        amount_failed_display = min(settings['amount_feedback_tab'], len(failed_tabs))
+
     result = "[bold bright_red]Wrong tabs[/]:"
-    result += ''.join(failed_tab_handler(failed_tab) for failed_tab in failed_tabs)
+    result += ''.join(failed_tab_handler(failed_tab, settings) for failed_tab in failed_tabs[:amount_failed_display])
 
     if len(correct_tabs) > 0:
         result += "\n\n[bold bright_green]Correct tabs:[/] "
         result += ', '.join([tab['description'] for tab in correct_tabs])
 
+    if amount_failed_display < len(failed_tabs):
+        result += "\n[bold bright_red]Other failed tabs:[/] "
+        result += ', '.join([tab['description'] for tab in failed_tabs[amount_failed_display:]])
+
     return result
 
 
-def failed_tab_handler(tab: dict) -> str:
+def failed_tab_handler(tab: dict, settings: dict) -> str:
     """
-    Handle failed tabs by delegating the first 3 failed contexts
+    Handle failed tabs by delegating the first n failed contexts
     :param tab: dictionary with a failed tab
+    :param settings: dictionary with settings
     :return: formatted string with failed tab things
     """
     result = f"\n[bold bright_red] \u00B7 [/][u]{str(tab['description']).capitalize()} ({tab['badgeCount']}):[/]"
     contexts = tab['groups']
     index = 0
     amount_failed = 0
 
-    while index < len(contexts) and amount_failed < 3:
+    while index < len(contexts) and amount_failed < settings['amount_feedback_context']:
         context = contexts[index]
         if context['accepted']:
             index += 1
             continue
-        result += failed_context_handler(context)
+        result += failed_context_handler(context, settings)
         amount_failed += 1
         index += 1
     return result
 
 
-def failed_context_handler(context: dict) -> str:
+def failed_context_handler(context: dict, settings: dict) -> str:
+    """
+    Handle failed context by delegating the first n failed contexts
+    :param context: dictionary with a failed context
+    :param settings: dictionary with settings
+    :return: formatted string with failed tab things
+    """
     result = ""
-    # if 'data' in context:
-    #     result += f"\n\t[bright_red]\u00B7[/] {context['data']['statements'].strip()}:"
-    # elif 'description' in context:
-    #     result += f"\n\t[bright_red]\u00B7[/] {context['description']['description']}:"
 
     test_cases = context['groups']
     index = 0
     amount_failed = 0
 
     context_content = []
 
-    while index < len(test_cases) and amount_failed < 3:
+    while index < len(test_cases) and amount_failed < settings['amount_feedback_testcase']:
         test_case = test_cases[index]
 
         if 'tests' in test_case:
-            context_content.extend(failed_tests_handler(test_case))
+            context_content.extend(failed_tests_handler(test_case, settings))
         else:
             if test_case['accepted']:
                 emoji = '[bright_green]:heavy_check_mark:[/] '
             else:
                 emoji = "[bright_red]:heavy_multiplication_x:[/] "
             context_content.append(emoji + test_case['description']['description'].rstrip())
 
@@ -86,15 +99,21 @@
         result += f"\n   \u2570 {context_content[-1]}\n"
     else:
         result += "\n   - " + context_content[0] + "\n"
 
     return result
 
 
-def failed_tests_handler(test_case: dict) -> list:
+def failed_tests_handler(test_case: dict, settings: dict) -> list:
+    """
+    Handle failed test_case by displaying all tests
+    :param test_case: dictionary with a failed context
+    :param settings: dictionary with settings
+    :return: formatted string with failed tab things
+    """
     result = []
     if 'data' in test_case:
         result.append(test_case['data']['statements'].rstrip())
     elif 'description' in test_case:
         result.append(test_case['description']['description'].rstrip())
 
     tests = test_case['tests']
@@ -103,15 +122,15 @@
         return result
     else:
         result[-1] = "[bright_red]:heavy_multiplication_x:[/] " + result[-1]
 
     index = 0
     amount_failed = 0
 
-    while index < len(tests) and amount_failed < 3:
+    while index < len(tests) and amount_failed < settings['amount_feedback_test']:
         test = tests[index]
         if not test['accepted']:
             result.append("\t    Expected:\t" + test['expected'].rstrip())
             result.append("\t    Actual:  \t" + test['generated'].rstrip())
         amount_failed += 1
         index += 1
 
@@ -126,17 +145,7 @@
     """
     result = ""
     if 'annotations' in submission_data and len(submission_data['annotations']) > 0:
         result = "\n\n[bold]Code annotations:[/]"
         for annotation in submission_data['annotations']:
             result += f"\n- Row {annotation['row']}: {annotation['text']}"
     return result
-
-
-if __name__ == '__main__':
-    import json
-    import pretty_console
-
-    with open(f'/home/bram/tijdelijk{input()}.json', 'r') as test_file:
-        test_data: dict = json.load(test_file)
-
-    pretty_console.console.print(submission_data_handler(test_data))
```

### Comparing `dodonacli-2024.5.16/dodonacli/source/syntax_checker.py` & `dodonacli-2024.5.20/dodonacli/source/syntax_checker.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.16/dodonacli_completion_script.sh` & `dodonacli-2024.5.20/dodonacli_completion_script.sh`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     if [ "$3" == "sub" ]; then
         mapfile -t COMPREPLY < <(compgen -W "load display --help" -- "$2")
 
     elif [ "$3" == "display" ]; then
         mapfile -t COMPREPLY < <(compgen -W "--force --help" -- "$2")
 
     elif [ "$3" == "info" ]; then
-        mapfile -t COMPREPLY < <(compgen -W "version changelog completion github check-update --help" -- "$2")
+        mapfile -t COMPREPLY < <(compgen -W "version changelog completion github check-update man-page --help" -- "$2")
 
     elif [ "$3" == "select" ]; then
         mapfile -t COMPREPLY < <(compgen -W "--other --hidden --help" -- "$2")
 
     elif [ "$3" == "next" ]; then
         mapfile -t COMPREPLY < <(compgen -W "--reverse --unsolved --help" -- "$2")
```

### Comparing `dodonacli-2024.5.16/man-page/dodonacli.1` & `dodonacli-2024.5.20/man-page/dodonacli.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '\" t
-.TH DODONACLI 14/05/2024
+.TH DODONACLI 19/05/2024
 .SH NAME
 dodonacli \- a 3rd party Command Line Interface for Dodona
 
 .SH SYNOPSIS
 .B dodona
 [display|info|next|post|select|status|sub|tutorial|up] [--help]
 
 .SH DESCRIPTION
-This documents the usage of a Command Line Interface made for Dodona. 
+This documents the usage of a Command Line Interface made for Dodona.
 .B DodonaCLI
 connects to Dodona to enable you to read, submit and get (minimal) feedback on exercises.
 You are able to switch courses, series and exercises, as long as you have acces to it on the official Dodona website.
 
 .SH SUBCOMMANDS
 .IP display
 Displays the courses/series/exercises you can select. When used while an exercise is selected, it will link you to the exercise page of the Dodona website. It can be used in combination with the flags
@@ -33,19 +33,19 @@
 Posts the file given as an extra argument to the currently selected exercise. This will return if the tests are passed, or information about the wrong tests. You can also use the
 .BR [-c|--check]
 flag to check your solutionfile for syntax-errors before uploading. This is currently supported for Bash, Java, JavaScript and Python. There is also the
 .BR [-l|--link]
 flag to post your solutionfile directly to the exercise specified in a link on the first line of the file. This link has to be written in a comment!
 
 .IP select
-Select a course/series/exercise of those available when using 
+Select a course/series/exercise of those available when using
 .BR dodona
 .BR display.
-Requires an extra argument 
-.BR [id|name] 
+Requires an extra argument
+.BR [id|name]
 where name can be a distinct part of the cours/series/exercise. If the name is not distinct, it will select the first item it matches with (case-insensitive). It is not guarenteed that this matching happens in the same order as displayed, but often it is.
 
 .IP status
 Show the current selected course/series/exercise. If there is nothing selected for a category, it will be displayed as
 .B None.
 
 .IP sub
@@ -54,22 +54,22 @@
 .IP tutorial
 Starts an interactive tutorial to learn how the CLI works.
 
 .IP up
 Deselects the current course/series/exercise and goes to the layer above. Optional arguments are [all|top|1|2|3], which indicate how many "levels" you'll deselect.
 
 .IP \-\-help
-Can be used with every option to get an help page for the command, if you use 
+Can be used with every option to get an help page for the command, if you use
 .B dodona
 or
 .B dodona --help
 you get the help page of the main command.
 
 .SH EXAMPLE USAGE
-.PP 
+.PP
 dodona display
 .RS 4
 Shows the available courses
 .RE
 
 .PP
 dodona select 1234
@@ -91,15 +91,15 @@
 
 .PP
 dodona select 'Exercise 1'
 .RS 4
 Selects  the exercise with the name: "Exercise 1"
 .RE
 
-.PP 
+.PP
 dodona post test.py
 .RS 4
 Submits the document test.py to the currently selected exercise, and displays feedback.
 .RE
 
 .PP
 dodona sub [view]
@@ -109,14 +109,19 @@
 
 .PP
 dodona up 2
 .RS 4
 Goes up 2 layers, in this case it would deselect the current exercise and series.
 .RE
 
+.SH SETTINGS
+DodonaCLI has settings stored in settings.json, alongside its config file. It's important to note that while it is fine to edit the settings-file manually (while keeping the type of values the same), it is absolutely
+.BR NOT
+advised to edit the config.json file! There will be a subcommand to more easily edit the settings, later.
+
 .SH AUTHORS
 .PP
 DodonaCLI: Bram Windey (windey.bram@gmail.com)
 
 Man-page: Kiandro De Waegenaere & Bram windey
 
 .SH COPYRIGHT
```

### Comparing `dodonacli-2024.5.16/pyproject.toml` & `dodonacli-2024.5.20/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DodonaCLI"
-version = '2024.5.16'
+version = '2024.5.20'
 authors = [
     { name = "Bram Windey", email = "windey.bram@gmail.com" },
 ]
 description = "A CLI tool for Dodona"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
```

