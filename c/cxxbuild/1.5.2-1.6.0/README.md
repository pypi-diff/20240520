# Comparing `tmp/cxxbuild-1.5.2.tar.gz` & `tmp/cxxbuild-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxxbuild-1.5.2.tar", last modified: Fri Jan  5 03:02:10 2024, max compression
+gzip compressed data, was "cxxbuild-1.6.0.tar", last modified: Sun May 19 23:21:37 2024, max compression
```

## Comparing `cxxbuild-1.5.2.tar` & `cxxbuild-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-01-05 03:02:10.836052 cxxbuild-1.5.2/
--rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11953 2024-01-05 03:02:10.832052 cxxbuild-1.5.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     9917 2024-01-05 02:50:12.000000 cxxbuild-1.5.2/README.md
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-01-05 03:02:10.832052 cxxbuild-1.5.2/cxxbuild/
--rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.5.2/cxxbuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45366 2024-01-05 02:50:12.000000 cxxbuild-1.5.2/cxxbuild/cxxbuild.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-01-05 03:02:10.832052 cxxbuild-1.5.2/cxxbuild.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11953 2024-01-05 03:02:10.000000 cxxbuild-1.5.2/cxxbuild.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2024-01-05 03:02:10.000000 cxxbuild-1.5.2/cxxbuild.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-05 03:02:10.000000 cxxbuild-1.5.2/cxxbuild.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-01-05 03:02:10.000000 cxxbuild-1.5.2/cxxbuild.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-01-05 03:02:10.000000 cxxbuild-1.5.2/cxxbuild.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-05 03:02:10.000000 cxxbuild-1.5.2/cxxbuild.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      910 2024-01-05 02:50:12.000000 cxxbuild-1.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-05 03:02:10.836052 cxxbuild-1.5.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      227 2024-01-05 02:50:12.000000 cxxbuild-1.5.2/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:21:37.231684 cxxbuild-1.6.0/
+-rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14541 2024-05-19 23:21:37.231684 cxxbuild-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12505 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/README.md
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:21:37.227684 cxxbuild-1.6.0/cxxbuild/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.0/cxxbuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49679 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/cxxbuild/cxxbuild.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-19 23:21:37.227684 cxxbuild-1.6.0/cxxbuild.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14541 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-19 23:21:37.000000 cxxbuild-1.6.0/cxxbuild.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      910 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 23:21:37.231684 cxxbuild-1.6.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      227 2024-05-19 23:20:26.000000 cxxbuild-1.6.0/setup.py
```

### Comparing `cxxbuild-1.5.2/LICENSE` & `cxxbuild-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cxxbuild-1.5.2/PKG-INFO` & `cxxbuild-1.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,40 @@
-Metadata-Version: 2.1
-Name: cxxbuild
-Version: 1.5.2
-Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
-Author-email: Igor Machado Coelho <igormcoelho@proton.me>
-License: MIT License
-        
-        Copyright (c) 2023 manydeps
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
-Project-URL: Homepage, https://github.com/manydeps/cxxbuild
-Keywords: build,cplusplus,dependencies,cxxdeps,cmake,bazel
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: toml
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: bumpver; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-
 # cxxbuild / cxxdeps
 
 [![Demo on windows, linux and macos](https://github.com/manydeps/cxxbuild/actions/workflows/demo.yml/badge.svg)](https://github.com/manydeps/cxxbuild/actions/workflows/demo.yml)
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
-Version: `cxxbuild version=1.5.2`  Installation: `pip install cxxbuild`
+_**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-cxxbuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
+- Version: `cxxbuild version=1.6.0`
+- Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
+But you MUST follow the canonical organization below:
+
+```
+project1/
+        |
+        | include/
+        |        | package1/
+        |                  | file1.h
+        |                  | file2.hpp
+        |                  | ...
+        | src/
+        |    | file1.cpp
+        |    | file2.c
+        |    | file_main.cpp
+        |    | ...
+        | cxxdeps.txt
+```
 
 The strongest point of this project is the `cxxdeps.txt` format, 
 that allow easy specification of dependencies from different package managers (in similar style of python `requirements.txt` format)
 
 To use it locally, just copy [cxxbuild/cxxbuild.py](cxxbuild/cxxbuild.py) file to your project and execute it: `python3 cxxbuild.py help`
 
 Or, just install it from pip: `pip install cxxbuild`
@@ -77,17 +52,25 @@
 - lint mode (unimplemented): will lint project files
 - test mode (unimplemented): will run project tests
 
 ## Running demos 
 
 
 - Demo 1 [README](demo/project1/README.md): `cxxbuild demo/project1`
+    * Dependencies: fmt, catch2, pthread:!windows, crypto:linux
 - Demo 2 [README](demo/project2/README.md): `cxxbuild demo/project2`
+    * Dependencies: NONE
 - Demo 3 [README](demo/project3/README.md): `cxxbuild demo/project3`
+    * Dependencies: fmt, catch2, pthread:!windows
 - Demo 4 [README](demo/project4/README.md): `cxxbuild demo/project4 --c++20`
+    * Dependencies: catch2
+- Demo 5 [README](demo/project5/README.md): `cxxbuild demo/project5`
+    * Dependencies (cmake-only): fmt, catch2
+- Demo 6 [README](demo/project6/README.md): `cxxbuild demo/project6`
+    * Dependencies (cmake-only): optframe, absl (google abseil)
 
 All of them support both CMake and Bazel build systems,
 for common platforms Linux, Windows and Mac.
 
 ## Test summary for demos
 
 - demo/project1: runs on linux, osx and windows* (bash only) - default c++17 (works with c++11 to c++23)
@@ -156,21 +139,26 @@
 
 An example is:
 
 ```
 fmt == "9.1.0"     [ fmt ]                    git *    https://github.com/fmtlib/fmt.git
 Catch2 == "v3.3.1" [ Catch2::Catch2WithMain ] git test https://github.com/catchorg/Catch2.git
 m
+!std c++17
+!build cmake
+# this is a comment
 ```
 
 This is quite simple and powerful, with few lines describing the following:
 
 - take `fmt` project from git repository in specific version
 - take `Catch2` project from git repository in specific version and use it for tests only
 - take system `-lm` dependency
+- C++ standard `c++17` is used
+- build system `cmake` is used
 
 The `git` part could be any package manager, such as conan and vcpkg, although not implemented yet!
 The `git` can be specified for `cmake` or `bazel`, like `cmake+git` or `bazel+git`.
 
 It can also be `bcr`, for the Bazel Central Registry, or more specifically: `bazel+bcr` (not supported for `cmake+bcr`)
 
 ### Ongoing extensions for cxxdeps
@@ -228,24 +216,70 @@
 
 ### Drawbacks
 
 None that I know, yet :)
 
 Some people may dislike the imposed organization, like `src/` and `tests/`, but it can be changed manually on script. The idea here is to really make a simplistic script, that really works with highly complex setups (such as taking dependencies from remote and dealing with build systems like cmake and bazel). These things are hard to do even for some experienced c++ programmers... so, as long as it is simple and it works, that is fine! If it doesn't work, file an issue!
 
+### Build `!options` on cxxdeps
+
+The `cxxdeps.txt` file allows defining some usual command line parameters with `!` prefix.
+Examples:
+
+- Parameter `--c++20` appears on file as `!std c++20`
+- Parameter `--cmake` appears on file as `!build cmake`
+- Parameter `--bazel` appears on file as `!build bazel`
+- Parameter `--include dir` appears on file as `!include "dir"`
+
+Command-line parameters have priority over `cxxdeps.txt` and can overwrite or complement them (with exception of `!build` parameter that cannot be overwritten).
+
+In the future, the `!options` could be limited by operating system, e.g., `!option:windows`.
+
 ## Related Works
 
 - See [ccbuild from debian](https://packages.debian.org/pt-br/sid/devel/ccbuild)
    * See [bneijt/ccbuild](https://github.com/bneijt/ccbuild)
 - See [Mantle project](https://github.com/jpxor/Mantle) (experimental but with similar ideas)
 
 None of them support dependencies, such as `cxxdeps.txt`, or even build systems such as cmake and bazel.
 
 Hopefully, when this project is fully finished, C++ will be a better place for all of us :)
 
+### Case of Study
+
+In order to check the capabilities of cxxbuild, it was used to build the C/C++ ccbuild tool.
+Unfortunately, few tweaks were necessary in the generated CMakeLists, due to FLEX dependency, 
+but it was quite easy on general. See [Issue 34 on ccbuild project](https://github.com/bneijt/ccbuild/issues/34)
+
+General instructions:
+- Create `cxxdeps.txt` file:
+
+```
+bobcat
+gnutls
+fl
+png
+# apt install flex 
+# apt install libboost-all-dev
+# apt install gnutls-dev
+# apt install libbobcat-dev
+# libpng-dev
+```
+
+- Use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20`
+- Add this to last line of CMakeLists: `add_definitions(-DVERSION="v2.0.7-39-gdf7b35c")`
+- Add this to SOURCES: `${FLEX_SourceScanner_OUTPUTS}`
+- Add these two lines before the SOURCES:
+
+```
+find_package(FLEX)
+FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
+```
+
+And that's it! It builds all avaliable targets and tests for ccbuild.
 
 ## Acknowledgements
 
 Thanks for those trying to use and improve this software.
 Specially, thanks Fellipe Pessanha for early suggesting integrating toml support for cxxdeps.
 
 ### Citation
```

### Comparing `cxxbuild-1.5.2/README.md` & `cxxbuild-1.6.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,83 @@
+Metadata-Version: 2.1
+Name: cxxbuild
+Version: 1.6.0
+Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
+Author-email: Igor Machado Coelho <igormcoelho@proton.me>
+License: MIT License
+        
+        Copyright (c) 2023 manydeps
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/manydeps/cxxbuild
+Keywords: build,cplusplus,dependencies,cxxdeps,cmake,bazel
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: toml
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
 # cxxbuild / cxxdeps
 
 [![Demo on windows, linux and macos](https://github.com/manydeps/cxxbuild/actions/workflows/demo.yml/badge.svg)](https://github.com/manydeps/cxxbuild/actions/workflows/demo.yml)
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
-Version: `cxxbuild version=1.5.2`  Installation: `pip install cxxbuild`
+_**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-cxxbuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
+- Version: `cxxbuild version=1.6.0`
+- Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
+But you MUST follow the canonical organization below:
+
+```
+project1/
+        |
+        | include/
+        |        | package1/
+        |                  | file1.h
+        |                  | file2.hpp
+        |                  | ...
+        | src/
+        |    | file1.cpp
+        |    | file2.c
+        |    | file_main.cpp
+        |    | ...
+        | cxxdeps.txt
+```
 
 The strongest point of this project is the `cxxdeps.txt` format, 
 that allow easy specification of dependencies from different package managers (in similar style of python `requirements.txt` format)
 
 To use it locally, just copy [cxxbuild/cxxbuild.py](cxxbuild/cxxbuild.py) file to your project and execute it: `python3 cxxbuild.py help`
 
 Or, just install it from pip: `pip install cxxbuild`
@@ -34,17 +95,25 @@
 - lint mode (unimplemented): will lint project files
 - test mode (unimplemented): will run project tests
 
 ## Running demos 
 
 
 - Demo 1 [README](demo/project1/README.md): `cxxbuild demo/project1`
+    * Dependencies: fmt, catch2, pthread:!windows, crypto:linux
 - Demo 2 [README](demo/project2/README.md): `cxxbuild demo/project2`
+    * Dependencies: NONE
 - Demo 3 [README](demo/project3/README.md): `cxxbuild demo/project3`
+    * Dependencies: fmt, catch2, pthread:!windows
 - Demo 4 [README](demo/project4/README.md): `cxxbuild demo/project4 --c++20`
+    * Dependencies: catch2
+- Demo 5 [README](demo/project5/README.md): `cxxbuild demo/project5`
+    * Dependencies (cmake-only): fmt, catch2
+- Demo 6 [README](demo/project6/README.md): `cxxbuild demo/project6`
+    * Dependencies (cmake-only): optframe, absl (google abseil)
 
 All of them support both CMake and Bazel build systems,
 for common platforms Linux, Windows and Mac.
 
 ## Test summary for demos
 
 - demo/project1: runs on linux, osx and windows* (bash only) - default c++17 (works with c++11 to c++23)
@@ -113,21 +182,26 @@
 
 An example is:
 
 ```
 fmt == "9.1.0"     [ fmt ]                    git *    https://github.com/fmtlib/fmt.git
 Catch2 == "v3.3.1" [ Catch2::Catch2WithMain ] git test https://github.com/catchorg/Catch2.git
 m
+!std c++17
+!build cmake
+# this is a comment
 ```
 
 This is quite simple and powerful, with few lines describing the following:
 
 - take `fmt` project from git repository in specific version
 - take `Catch2` project from git repository in specific version and use it for tests only
 - take system `-lm` dependency
+- C++ standard `c++17` is used
+- build system `cmake` is used
 
 The `git` part could be any package manager, such as conan and vcpkg, although not implemented yet!
 The `git` can be specified for `cmake` or `bazel`, like `cmake+git` or `bazel+git`.
 
 It can also be `bcr`, for the Bazel Central Registry, or more specifically: `bazel+bcr` (not supported for `cmake+bcr`)
 
 ### Ongoing extensions for cxxdeps
@@ -185,24 +259,70 @@
 
 ### Drawbacks
 
 None that I know, yet :)
 
 Some people may dislike the imposed organization, like `src/` and `tests/`, but it can be changed manually on script. The idea here is to really make a simplistic script, that really works with highly complex setups (such as taking dependencies from remote and dealing with build systems like cmake and bazel). These things are hard to do even for some experienced c++ programmers... so, as long as it is simple and it works, that is fine! If it doesn't work, file an issue!
 
+### Build `!options` on cxxdeps
+
+The `cxxdeps.txt` file allows defining some usual command line parameters with `!` prefix.
+Examples:
+
+- Parameter `--c++20` appears on file as `!std c++20`
+- Parameter `--cmake` appears on file as `!build cmake`
+- Parameter `--bazel` appears on file as `!build bazel`
+- Parameter `--include dir` appears on file as `!include "dir"`
+
+Command-line parameters have priority over `cxxdeps.txt` and can overwrite or complement them (with exception of `!build` parameter that cannot be overwritten).
+
+In the future, the `!options` could be limited by operating system, e.g., `!option:windows`.
+
 ## Related Works
 
 - See [ccbuild from debian](https://packages.debian.org/pt-br/sid/devel/ccbuild)
    * See [bneijt/ccbuild](https://github.com/bneijt/ccbuild)
 - See [Mantle project](https://github.com/jpxor/Mantle) (experimental but with similar ideas)
 
 None of them support dependencies, such as `cxxdeps.txt`, or even build systems such as cmake and bazel.
 
 Hopefully, when this project is fully finished, C++ will be a better place for all of us :)
 
+### Case of Study
+
+In order to check the capabilities of cxxbuild, it was used to build the C/C++ ccbuild tool.
+Unfortunately, few tweaks were necessary in the generated CMakeLists, due to FLEX dependency, 
+but it was quite easy on general. See [Issue 34 on ccbuild project](https://github.com/bneijt/ccbuild/issues/34)
+
+General instructions:
+- Create `cxxdeps.txt` file:
+
+```
+bobcat
+gnutls
+fl
+png
+# apt install flex 
+# apt install libboost-all-dev
+# apt install gnutls-dev
+# apt install libbobcat-dev
+# libpng-dev
+```
+
+- Use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20`
+- Add this to last line of CMakeLists: `add_definitions(-DVERSION="v2.0.7-39-gdf7b35c")`
+- Add this to SOURCES: `${FLEX_SourceScanner_OUTPUTS}`
+- Add these two lines before the SOURCES:
+
+```
+find_package(FLEX)
+FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
+```
+
+And that's it! It builds all avaliable targets and tests for ccbuild.
 
 ## Acknowledgements
 
 Thanks for those trying to use and improve this software.
 Specially, thanks Fellipe Pessanha for early suggesting integrating toml support for cxxdeps.
 
 ### Citation
```

### Comparing `cxxbuild-1.5.2/cxxbuild/cxxbuild.py` & `cxxbuild-1.6.0/cxxbuild/cxxbuild.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 # Copyleft 2023 Igor Machado Coelho
 
 import os
 import sys
 import json
 import subprocess
 
+def version():
+    v = "cxxbuild=1.6.0"
+    return v
 
 def usage():
-    u="""
-cxxbuild=1.5.2
+    u=version()+"""
 Usage:
     cxxbuild [build] [ROOT_PATH] 
       builds with cxxbuild, examples: 
         cxxbuild
         cxxbuild .
         cxxbuild build .
         cxxbuild . --c++20 --bazel
@@ -50,15 +52,15 @@
 def get_cmakelists_from_cxxdeps(root_path, cmakelists, INCLUDE_DIRS, src_main, src_test_main):
     try:
         with open(root_path+'/cxxdeps.txt', 'r') as fd:
             x=fd.readlines()
             #print(x)
             cmakelists.append("# begin dependencies from cxxdeps.txt")
             for l in x:
-                if (len(l) >= 1) and (l[0] != '#'):
+                if (len(l) >= 1) and (l[0] != '#') and (l[0] != '!'):
                     # good line!
                     print(l)
                     fields = l.split()
                     print(fields)
                     # assume all spacing is correct, for now!
                     if len(fields) == 0:
                         # IGNORE (EMPTY LINE!)
@@ -205,15 +207,15 @@
 def get_bazelfiles_from_cxxdeps(root_path, bzl, INCLUDE_DIRS, src_main, src_test_main):
     try:
         with open(root_path+'/cxxdeps.txt', 'r') as fd:
             x=fd.readlines()
             #print(x)
             # cmakelists.append("# begin dependencies from cxxdeps.txt")
             for l in x:
-                if (len(l) >= 1) and (l[0] != '#'):
+                if (len(l) >= 1) and (l[0] != '#') and (l[0] != '!'):
                     # good line!
                     print(l)
                     fields = l.split()
                     print(fields)
                     # assume all spacing is correct, for now!
                     if len(fields) == 0:
                         # IGNORE (EMPTY LINE!)
@@ -843,14 +845,48 @@
     x=subprocess.call(list(filter(None, CMAKE_CMD.split(' '))))
     print('cmake result:', x)
     assert(x == 0)
     x=subprocess.call(list(filter(None, NINJA_CMD.split(' '))))
     print('ninja result:', x)
     assert(x == 0)
 
+def run_bazel(root_path):
+    # ============ build with bazel ===========
+    # STEP 1: check that 'bazel' command exists
+    CHECK_BAZEL_CMD="bazel --version"
+    print("Please install latest bazel with NVM: bash -i -c \"npm install -g @bazel/bazelisk\"")
+    print("   - on windows: choco install bazel")
+    print("   - on macos:   brew install bazelisk")
+    print("or visit bazel website: https://bazel.build/install")
+    print("checking bazel command now...")
+    x=subprocess.call(list(filter(None, CHECK_BAZEL_CMD.split(' '))))
+    print('check result:', x)
+    assert(x == 0)
+    #
+    # STEP 1.5: debug only (TODO: create flag --verbose!)
+    BAZEL_CMD="cat "+root_path+"/MODULE.bazel"
+    print("showing MODULE.bazel... "+BAZEL_CMD)
+    x=subprocess.call(list(filter(None, BAZEL_CMD.split(' '))))
+    print('\nbazel result:', x)
+    assert(x == 0)
+    #
+    BAZEL_CMD="cat "+root_path+"/BUILD.bazel"
+    print("showing BUILD.bazel... "+BAZEL_CMD)
+    x=subprocess.call(list(filter(None, BAZEL_CMD.split(' '))))
+    print('\nbazel result:', x)
+    assert(x == 0)
+    #
+    # STEP 2: build with bazel
+    BAZEL_CMD="bazel build ..."
+    print("building...\n"+BAZEL_CMD)
+    x=subprocess.call(list(filter(None, BAZEL_CMD.split(' '))), cwd=root_path)
+    print('bazel result:', x)
+    assert(x == 0)
+
+
 # detect if it's 'cmd' for windows, but not 'bash'
 def is_cmd():
     return os.name == 'nt' and 'WSL_DISTRO_NAME' not in os.environ
 
 
 def main():
     print("======================================")
@@ -868,56 +904,122 @@
     if "clean" in sys.argv:
         print("'clean' not implemented, yet!")
         exit()
     if "lint" in sys.argv:
         print("'lint' not implemented, yet!")
         exit()
     root_path = sys.argv[1]
+    
     if "build" in sys.argv:
         # must take path explicitly from third argument!
         # example: cxxbuild build .
         if len(sys.argv) > 2:
             root_path = sys.argv[2]
         else:
             usage()
             exit()
 
-    search_src="src"
-    search_tests="tests"
-    search_include="include"
-    INCLUDE_DIRS = []
-    use_cmake=None
-    use_bazel=None
-    cppstd="17"
+    print(version())
+    build_options_args = []
     for i in range(len(sys.argv)):
         if (sys.argv[i] == "--src"):
-            search_src = str(sys.argv[i + 1])
+            build_options_args.append("!src \""+str(sys.argv[i + 1])+"\"")
         if (sys.argv[i] == "--tests"):
-            search_tests = str(sys.argv[i + 1])
+            build_options_args.append("!tests \""+str(sys.argv[i + 1])+"\"")
         if (sys.argv[i] == "--include"):
-            search_include = str(sys.argv[i + 1])
             # force --include to appear
-            INCLUDE_DIRS.append(root_path+"/"+search_include)
+            build_options_args.append("!include \""+search_include+"\"")
         if (sys.argv[i] == "--cmake"):
+            build_options_args.append("!build cmake")
+        if (sys.argv[i] == "--bazel"):
+            build_options_args.append("!build bazel")
+        if (sys.argv[i] == "--c++11"):
+            build_options_args.append("!std c++11")
+        if (sys.argv[i] == "--c++14"):
+            build_options_args.append("!std c++14")
+        if (sys.argv[i] == "--c++17"):
+            build_options_args.append("!std c++17")
+        if (sys.argv[i] == "--c++20"):
+            build_options_args.append("!std c++20")
+        if (sys.argv[i] == "--c++23"):
+            build_options_args.append("!std c++23")
+
+    print("build options from args: "+str(build_options_args))
+    #
+    build_options = []
+    # TODO: convert .toml to .txt here, if necessary!
+    # get more build options for cxxdeps.txt
+    try:
+        with open(root_path+'/cxxdeps.txt', 'r') as fd:
+            x=fd.readlines()
+            for l in x:
+                if (len(l) >= 1) and (l[0] == '!'):
+                    build_options.append(l)
+    except FileNotFoundError:
+        print("File cxxdeps.txt does not exist... ignoring it!")
+    
+    # merge with argument build options (priority is LAST)
+    for op in build_options_args:
+        build_options.append(op)
+
+    print("build options (including cxxdeps): "+str(build_options))
+
+    # begin processing build options
+    search_src="src"
+    search_tests="tests"
+    search_include="include"
+    #
+    use_cmake=None
+    use_bazel=None
+    cppstd="17"
+    INCLUDE_DIRS = []
+    for op in build_options:
+        oplist = op.split()
+        print(op.split())
+        if oplist[0] == '!version':
+            MIN_CXXBUILD_VERSION=oplist[1]
+            current_version = version().split("=")[1]
+            # from setuptools._distutils.version import LooseVersion, StrictVersion
+            # if LooseVersion(current_version) < LooseVersion(MIN_CXXBUILD_VERSION):
+            from packaging.version import Version
+            if Version(current_version) < Version(MIN_CXXBUILD_VERSION):
+                print("Insufficient CXXBUILD version! Please upgrade!")
+                print("Current version: "+current_version)
+                print("Required version (cxxdeps): "+MIN_CXXBUILD_VERSION)
+                print("Aborting...")
+                exit(1)
+        if oplist[0] == '!include':
+            INCLUDE_DIRS.append(oplist[1].strip("\""))
+        if oplist[0] == '!src':
+            search_src = oplist[1].strip("\"")
+        if oplist[0] == '!tests':
+            search_tests = oplist[1].strip("\"")
+        if oplist[0] == '!build' and oplist[1] == 'cmake':
+            if use_bazel == True:
+                print("cxxbuild error: cannot redefine build system 'bazel' to 'cmake'")
+                exit(1)
             use_cmake = True
             use_bazel = False
-        if (sys.argv[i] == "--bazel"):
+        if oplist[0] == '!build' and oplist[1] == 'bazel':
+            if use_cmake == True:
+                print("cxxbuild error: cannot redefine build system 'cmake' to 'bazel'")
+                exit(1)
             use_cmake = False
             use_bazel = True
-        if (sys.argv[i] == "--c++11"):
+        if oplist[0] == '!std' and oplist[1] == 'c++11':
             cppstd="11"
-        if (sys.argv[i] == "--c++14"):
+        if oplist[0] == '!std' and oplist[1] == 'c++14':
             cppstd="14"
-        if (sys.argv[i] == "--c++17"):
+        if oplist[0] == '!std' and oplist[1] == 'c++17':
             cppstd="17"
-        if (sys.argv[i] == "--c++20"):
+        if oplist[0] == '!std' and oplist[1] == 'c++20':
             cppstd="20"
-        if (sys.argv[i] == "--c++23"):
+        if oplist[0] == '!std' and oplist[1] == 'c++23':
             cppstd="23"
-            
+        
     # build system defaults to cmake
     if use_cmake is None:
         use_cmake = True
         use_bazel = False
 
     #
     print("begin build on root_path=",root_path)
@@ -1003,14 +1105,15 @@
             app_name1 = app_name_list[1] + str(COUNT_APP_ID) # concat number
         all_apps.append(app_name1)
         app_name_list[1] = app_name1
         src_main[filepath] = tuple(app_name_list) 
     # ---------------------------------
 
     print("fixed src_main: ", src_main)
+    
 
     # SO... TIME TO FIND INCLUDE FOLDERS
 
     #INCLUDE_DIRS = []
     for root, subdirs, files in os.walk(root_path):
         root = root.removeprefix(root_path).removeprefix("/")
         #print("root: ", root)
@@ -1037,16 +1140,17 @@
         generate_bazelfiles(cppstd, root_path, INCLUDE_DIRS, src_main, src_test_main, src_list, src_test_nomain)
     else:
         assert(False)
 
     if use_cmake == True:
         run_cmake(root_path)
     elif use_bazel == True:
-        print("FINISHED! Please run bazel with command: bazel build ...")
+        run_bazel(root_path)
     else:
+        print("UNKNOWN BUILDER! cxxbuild ERROR...")
         assert(False)
 
     if len(src_main.items()) > 0:
         print("OK: at least one main() has been found!")
     else:
         print("WARNING: no main() has been found!")
```

### Comparing `cxxbuild-1.5.2/cxxbuild.egg-info/PKG-INFO` & `cxxbuild-1.6.0/cxxbuild.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.5.2
+Version: 1.6.0
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,21 +45,39 @@
 
 [![Demo on windows, linux and macos](https://github.com/manydeps/cxxbuild/actions/workflows/demo.yml/badge.svg)](https://github.com/manydeps/cxxbuild/actions/workflows/demo.yml)
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
-Version: `cxxbuild version=1.5.2`  Installation: `pip install cxxbuild`
+_**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-cxxbuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
+- Version: `cxxbuild version=1.6.0`
+- Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
+But you MUST follow the canonical organization below:
+
+```
+project1/
+        |
+        | include/
+        |        | package1/
+        |                  | file1.h
+        |                  | file2.hpp
+        |                  | ...
+        | src/
+        |    | file1.cpp
+        |    | file2.c
+        |    | file_main.cpp
+        |    | ...
+        | cxxdeps.txt
+```
 
 The strongest point of this project is the `cxxdeps.txt` format, 
 that allow easy specification of dependencies from different package managers (in similar style of python `requirements.txt` format)
 
 To use it locally, just copy [cxxbuild/cxxbuild.py](cxxbuild/cxxbuild.py) file to your project and execute it: `python3 cxxbuild.py help`
 
 Or, just install it from pip: `pip install cxxbuild`
@@ -77,17 +95,25 @@
 - lint mode (unimplemented): will lint project files
 - test mode (unimplemented): will run project tests
 
 ## Running demos 
 
 
 - Demo 1 [README](demo/project1/README.md): `cxxbuild demo/project1`
+    * Dependencies: fmt, catch2, pthread:!windows, crypto:linux
 - Demo 2 [README](demo/project2/README.md): `cxxbuild demo/project2`
+    * Dependencies: NONE
 - Demo 3 [README](demo/project3/README.md): `cxxbuild demo/project3`
+    * Dependencies: fmt, catch2, pthread:!windows
 - Demo 4 [README](demo/project4/README.md): `cxxbuild demo/project4 --c++20`
+    * Dependencies: catch2
+- Demo 5 [README](demo/project5/README.md): `cxxbuild demo/project5`
+    * Dependencies (cmake-only): fmt, catch2
+- Demo 6 [README](demo/project6/README.md): `cxxbuild demo/project6`
+    * Dependencies (cmake-only): optframe, absl (google abseil)
 
 All of them support both CMake and Bazel build systems,
 for common platforms Linux, Windows and Mac.
 
 ## Test summary for demos
 
 - demo/project1: runs on linux, osx and windows* (bash only) - default c++17 (works with c++11 to c++23)
@@ -156,21 +182,26 @@
 
 An example is:
 
 ```
 fmt == "9.1.0"     [ fmt ]                    git *    https://github.com/fmtlib/fmt.git
 Catch2 == "v3.3.1" [ Catch2::Catch2WithMain ] git test https://github.com/catchorg/Catch2.git
 m
+!std c++17
+!build cmake
+# this is a comment
 ```
 
 This is quite simple and powerful, with few lines describing the following:
 
 - take `fmt` project from git repository in specific version
 - take `Catch2` project from git repository in specific version and use it for tests only
 - take system `-lm` dependency
+- C++ standard `c++17` is used
+- build system `cmake` is used
 
 The `git` part could be any package manager, such as conan and vcpkg, although not implemented yet!
 The `git` can be specified for `cmake` or `bazel`, like `cmake+git` or `bazel+git`.
 
 It can also be `bcr`, for the Bazel Central Registry, or more specifically: `bazel+bcr` (not supported for `cmake+bcr`)
 
 ### Ongoing extensions for cxxdeps
@@ -228,24 +259,70 @@
 
 ### Drawbacks
 
 None that I know, yet :)
 
 Some people may dislike the imposed organization, like `src/` and `tests/`, but it can be changed manually on script. The idea here is to really make a simplistic script, that really works with highly complex setups (such as taking dependencies from remote and dealing with build systems like cmake and bazel). These things are hard to do even for some experienced c++ programmers... so, as long as it is simple and it works, that is fine! If it doesn't work, file an issue!
 
+### Build `!options` on cxxdeps
+
+The `cxxdeps.txt` file allows defining some usual command line parameters with `!` prefix.
+Examples:
+
+- Parameter `--c++20` appears on file as `!std c++20`
+- Parameter `--cmake` appears on file as `!build cmake`
+- Parameter `--bazel` appears on file as `!build bazel`
+- Parameter `--include dir` appears on file as `!include "dir"`
+
+Command-line parameters have priority over `cxxdeps.txt` and can overwrite or complement them (with exception of `!build` parameter that cannot be overwritten).
+
+In the future, the `!options` could be limited by operating system, e.g., `!option:windows`.
+
 ## Related Works
 
 - See [ccbuild from debian](https://packages.debian.org/pt-br/sid/devel/ccbuild)
    * See [bneijt/ccbuild](https://github.com/bneijt/ccbuild)
 - See [Mantle project](https://github.com/jpxor/Mantle) (experimental but with similar ideas)
 
 None of them support dependencies, such as `cxxdeps.txt`, or even build systems such as cmake and bazel.
 
 Hopefully, when this project is fully finished, C++ will be a better place for all of us :)
 
+### Case of Study
+
+In order to check the capabilities of cxxbuild, it was used to build the C/C++ ccbuild tool.
+Unfortunately, few tweaks were necessary in the generated CMakeLists, due to FLEX dependency, 
+but it was quite easy on general. See [Issue 34 on ccbuild project](https://github.com/bneijt/ccbuild/issues/34)
+
+General instructions:
+- Create `cxxdeps.txt` file:
+
+```
+bobcat
+gnutls
+fl
+png
+# apt install flex 
+# apt install libboost-all-dev
+# apt install gnutls-dev
+# apt install libbobcat-dev
+# libpng-dev
+```
+
+- Use the following build script: `cxxbuild . --tests test --include src --include src/sourceScanner --c++20`
+- Add this to last line of CMakeLists: `add_definitions(-DVERSION="v2.0.7-39-gdf7b35c")`
+- Add this to SOURCES: `${FLEX_SourceScanner_OUTPUTS}`
+- Add these two lines before the SOURCES:
+
+```
+find_package(FLEX)
+FLEX_TARGET(SourceScanner "src/sourceScanner/lexer"  "src/sourceScanner/yylex.cc" )
+```
+
+And that's it! It builds all avaliable targets and tests for ccbuild.
 
 ## Acknowledgements
 
 Thanks for those trying to use and improve this software.
 Specially, thanks Fellipe Pessanha for early suggesting integrating toml support for cxxdeps.
 
 ### Citation
```

### Comparing `cxxbuild-1.5.2/pyproject.toml` & `cxxbuild-1.6.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires=["setuptools", "wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name="cxxbuild"
-version="1.5.2"
+version="1.6.0"
 description="CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!"
 readme="README.md"
 authors=[{ name="Igor Machado Coelho", email="igormcoelho@proton.me" }]
 license={ file="LICENSE" }
 classifiers=[
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

