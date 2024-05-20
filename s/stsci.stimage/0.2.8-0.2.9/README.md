# Comparing `tmp/stsci_stimage-0.2.8.tar.gz` & `tmp/stsci_stimage-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsci_stimage-0.2.8.tar", last modified: Fri Apr 19 19:26:49 2024, max compression
+gzip compressed data, was "stsci_stimage-0.2.9.tar", last modified: Mon May 20 13:27:17 2024, max compression
```

## Comparing `stsci_stimage-0.2.8.tar` & `stsci_stimage-0.2.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.642415 stsci_stimage-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.626416 stsci_stimage-0.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.626416 stsci_stimage-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.github/workflows/test_devdeps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 19:26:49.642415 stsci_stimage-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.626416 stsci_stimage-0.2.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/doc/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.626416 stsci_stimage-0.2.8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/doc/source/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/get_waf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.622416 stsci_stimage-0.2.8/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.626416 stsci_stimage-0.2.8/include/immatch/
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/immatch/geomap.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.630416 stsci_stimage-0.2.8/include/immatch/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/immatch/lib/match_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/immatch/lib/tolerance.h
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/immatch/lib/triangles.h
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/immatch/xyxymatch.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.630416 stsci_stimage-0.2.8/include/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/error.h
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/lintransform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/polynomial.h
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/xybbox.h
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/xycoincide.h
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/lib/xysort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.630416 stsci_stimage-0.2.8/include/surface/
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/surface/cholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/surface/fit.h
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/surface/surface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/include/surface/vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:26:49.642415 stsci_stimage-0.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      950 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.630416 stsci_stimage-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.630416 stsci_stimage-0.2.8/src/immatch/
--rw-r--r--   0 runner    (1001) docker     (127)    50354 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/immatch/geomap.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.634415 stsci_stimage-0.2.8/src/immatch/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/immatch/lib/tolerance.c
--rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/immatch/lib/triangles.c
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/immatch/lib/triangles_vote.c
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/immatch/xyxymatch.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.634415 stsci_stimage-0.2.8/src/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/error.c
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/lintransform.c
--rw-r--r--   0 runner    (1001) docker     (127)    16094 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/polynomial.c
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/util.c
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/xybbox.c
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/xycoincide.c
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/lib/xysort.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.634415 stsci_stimage-0.2.8/src/surface/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/surface/cholesky.c
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/surface/fit.c
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/surface/surface.c
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/surface/vector.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.634415 stsci_stimage-0.2.8/src/wrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.634415 stsci_stimage-0.2.8/src/wrap/immatch/
--rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/wrap/immatch/py_geomap.c
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/wrap/immatch/py_xyxymatch.c
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/wrap/stimage_module.c
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/wrap/wrap_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/wrap/wrap_util.h
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/src/wscript
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.634415 stsci_stimage-0.2.8/stsci/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/stsci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.638415 stsci_stimage-0.2.8/stsci/stimage/
--rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/stsci/stimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci/stimage/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.638415 stsci_stimage-0.2.8/stsci/stimage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/stsci/stimage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/stsci/stimage/tests/test_geomap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/stsci/stimage/tests/test_xyxymatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.642415 stsci_stimage-0.2.8/stsci.stimage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci.stimage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci.stimage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci.stimage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci.stimage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci.stimage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 19:26:49.000000 stsci_stimage-0.2.8/stsci.stimage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:26:49.642415 stsci_stimage-0.2.8/test_c/
--rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_c.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_cholesky.c
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_geomap.c
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_lintransform.c
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_surface.c
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_triangles.c
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_xycoincide.c
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_xysort.c
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_xyxymatch.c
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/test_xyxymatch_triangles.c
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/test_c/wscript
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 19:26:38.000000 stsci_stimage-0.2.8/wscript
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.989071 stsci_stimage-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.973070 stsci_stimage-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.973070 stsci_stimage-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.github/workflows/test_devdeps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-20 13:27:17.989071 stsci_stimage-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.973070 stsci_stimage-0.2.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/doc/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.973070 stsci_stimage-0.2.9/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/doc/source/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/get_waf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.969071 stsci_stimage-0.2.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.973070 stsci_stimage-0.2.9/include/immatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/immatch/geomap.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.977070 stsci_stimage-0.2.9/include/immatch/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/immatch/lib/match_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/immatch/lib/tolerance.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/immatch/lib/triangles.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/immatch/xyxymatch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.977070 stsci_stimage-0.2.9/include/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/error.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/lintransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/polynomial.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/xybbox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/xycoincide.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/lib/xysort.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.977070 stsci_stimage-0.2.9/include/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/surface/cholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/surface/fit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/surface/surface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/include/surface/vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:27:17.989071 stsci_stimage-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.977070 stsci_stimage-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.977070 stsci_stimage-0.2.9/src/immatch/
+-rw-r--r--   0 runner    (1001) docker     (127)    50354 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/immatch/geomap.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.981071 stsci_stimage-0.2.9/src/immatch/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/immatch/lib/tolerance.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/immatch/lib/triangles.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/immatch/lib/triangles_vote.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/immatch/xyxymatch.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.981071 stsci_stimage-0.2.9/src/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/error.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/lintransform.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16094 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/polynomial.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/xybbox.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/xycoincide.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/lib/xysort.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.981071 stsci_stimage-0.2.9/src/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/surface/cholesky.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/surface/fit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/surface/surface.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/surface/vector.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.981071 stsci_stimage-0.2.9/src/wrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.981071 stsci_stimage-0.2.9/src/wrap/immatch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/wrap/immatch/py_geomap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/wrap/immatch/py_xyxymatch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/wrap/stimage_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/wrap/wrap_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/wrap/wrap_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/src/wscript
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.981071 stsci_stimage-0.2.9/stsci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/stsci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.985071 stsci_stimage-0.2.9/stsci/stimage/
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/stsci/stimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci/stimage/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.985071 stsci_stimage-0.2.9/stsci/stimage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/stsci/stimage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/stsci/stimage/tests/test_geomap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/stsci/stimage/tests/test_xyxymatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.985071 stsci_stimage-0.2.9/stsci.stimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci.stimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci.stimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci.stimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci.stimage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci.stimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:27:17.000000 stsci_stimage-0.2.9/stsci.stimage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:27:17.985071 stsci_stimage-0.2.9/test_c/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_cholesky.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_geomap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_lintransform.c
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_surface.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_triangles.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_xycoincide.c
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_xysort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_xyxymatch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/test_xyxymatch_triangles.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/test_c/wscript
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-20 13:27:04.000000 stsci_stimage-0.2.9/wscript
```

### Comparing `stsci_stimage-0.2.8/.github/workflows/build.yml` & `stsci_stimage-0.2.9/.github/workflows/build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -19,9 +19,10 @@
         # Linux wheels
         - cp3*-manylinux_x86_64
         # MacOS wheels
         - cp3*-macosx_x86_64
         # ARM64 wheels
         - cp3*-macosx_arm64
       sdist: true
+      test_command: python -c "from stsci.stimage import xyxymatch, geomap"
     secrets:
       pypi_token: ${{ secrets.PYPI_PASSWORD_STSCI_MAINTAINER }}
```

### Comparing `stsci_stimage-0.2.8/.github/workflows/ci.yml` & `stsci_stimage-0.2.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/.github/workflows/test_devdeps.yml` & `stsci_stimage-0.2.9/.github/workflows/test_devdeps.yml`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/.readthedocs.yaml` & `stsci_stimage-0.2.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/CODE_OF_CONDUCT.md` & `stsci_stimage-0.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/LICENSE` & `stsci_stimage-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/PKG-INFO` & `stsci_stimage-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.stimage
-Version: 0.2.8
+Version: 0.2.9
 Summary: Various image processing functions
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2008-2010 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stsci_stimage-0.2.8/README.md` & `stsci_stimage-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/doc/Makefile` & `stsci_stimage-0.2.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/doc/source/conf.py` & `stsci_stimage-0.2.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/immatch/geomap.h` & `stsci_stimage-0.2.9/include/immatch/geomap.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/immatch/lib/match_util.h` & `stsci_stimage-0.2.9/include/immatch/lib/match_util.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/immatch/lib/tolerance.h` & `stsci_stimage-0.2.9/include/immatch/lib/tolerance.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/immatch/lib/triangles.h` & `stsci_stimage-0.2.9/include/immatch/lib/triangles.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/immatch/xyxymatch.h` & `stsci_stimage-0.2.9/include/immatch/xyxymatch.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/error.h` & `stsci_stimage-0.2.9/include/lib/error.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/lintransform.h` & `stsci_stimage-0.2.9/include/lib/lintransform.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/polynomial.h` & `stsci_stimage-0.2.9/include/lib/polynomial.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/util.h` & `stsci_stimage-0.2.9/include/lib/util.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/xybbox.h` & `stsci_stimage-0.2.9/include/lib/xybbox.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/xycoincide.h` & `stsci_stimage-0.2.9/include/lib/xycoincide.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/lib/xysort.h` & `stsci_stimage-0.2.9/include/lib/xysort.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/surface/cholesky.h` & `stsci_stimage-0.2.9/include/surface/cholesky.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/surface/fit.h` & `stsci_stimage-0.2.9/include/surface/fit.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/surface/surface.h` & `stsci_stimage-0.2.9/include/surface/surface.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/include/surface/vector.h` & `stsci_stimage-0.2.9/include/surface/vector.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/pyproject.toml` & `stsci_stimage-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -61,7 +61,8 @@
 [tool.setuptools.packages.find]
 include = [
     "stsci.stimage",
 ]
 
 [tool.setuptools_scm]
 write_to = "stsci/stimage/_version.py"
+
```

### Comparing `stsci_stimage-0.2.8/src/immatch/geomap.c` & `stsci_stimage-0.2.9/src/immatch/geomap.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/immatch/lib/tolerance.c` & `stsci_stimage-0.2.9/src/immatch/lib/tolerance.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/immatch/lib/triangles.c` & `stsci_stimage-0.2.9/src/immatch/lib/triangles.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/immatch/lib/triangles_vote.c` & `stsci_stimage-0.2.9/src/immatch/lib/triangles_vote.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/immatch/xyxymatch.c` & `stsci_stimage-0.2.9/src/immatch/xyxymatch.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/error.c` & `stsci_stimage-0.2.9/src/lib/error.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/lintransform.c` & `stsci_stimage-0.2.9/src/lib/lintransform.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/polynomial.c` & `stsci_stimage-0.2.9/src/lib/polynomial.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/util.c` & `stsci_stimage-0.2.9/src/lib/util.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/xybbox.c` & `stsci_stimage-0.2.9/src/lib/xybbox.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/xycoincide.c` & `stsci_stimage-0.2.9/src/lib/xycoincide.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/lib/xysort.c` & `stsci_stimage-0.2.9/src/lib/xysort.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/surface/cholesky.c` & `stsci_stimage-0.2.9/src/surface/cholesky.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/surface/fit.c` & `stsci_stimage-0.2.9/src/surface/fit.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/surface/surface.c` & `stsci_stimage-0.2.9/src/surface/surface.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/surface/vector.c` & `stsci_stimage-0.2.9/src/surface/vector.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/wrap/immatch/py_geomap.c` & `stsci_stimage-0.2.9/src/wrap/immatch/py_geomap.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/wrap/immatch/py_xyxymatch.c` & `stsci_stimage-0.2.9/src/wrap/immatch/py_xyxymatch.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/wrap/stimage_module.c` & `stsci_stimage-0.2.9/src/wrap/stimage_module.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/wrap/wrap_util.c` & `stsci_stimage-0.2.9/src/wrap/wrap_util.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/wrap/wrap_util.h` & `stsci_stimage-0.2.9/src/wrap/wrap_util.h`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/src/wscript` & `stsci_stimage-0.2.9/src/wscript`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/stsci/stimage/__init__.py` & `stsci_stimage-0.2.9/stsci/stimage/__init__.py`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/stsci/stimage/tests/test_geomap.py` & `stsci_stimage-0.2.9/stsci/stimage/tests/test_geomap.py`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/stsci/stimage/tests/test_xyxymatch.py` & `stsci_stimage-0.2.9/stsci/stimage/tests/test_xyxymatch.py`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/stsci.stimage.egg-info/PKG-INFO` & `stsci_stimage-0.2.9/stsci.stimage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stsci.stimage
-Version: 0.2.8
+Version: 0.2.9
 Summary: Various image processing functions
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2008-2010 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `stsci_stimage-0.2.8/stsci.stimage.egg-info/SOURCES.txt` & `stsci_stimage-0.2.9/stsci.stimage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_c.py` & `stsci_stimage-0.2.9/test_c/test_c.py`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_geomap.c` & `stsci_stimage-0.2.9/test_c/test_geomap.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_lintransform.c` & `stsci_stimage-0.2.9/test_c/test_lintransform.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_surface.c` & `stsci_stimage-0.2.9/test_c/test_surface.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_triangles.c` & `stsci_stimage-0.2.9/test_c/test_triangles.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_xycoincide.c` & `stsci_stimage-0.2.9/test_c/test_xycoincide.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_xysort.c` & `stsci_stimage-0.2.9/test_c/test_xysort.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_xyxymatch.c` & `stsci_stimage-0.2.9/test_c/test_xyxymatch.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/test_xyxymatch_triangles.c` & `stsci_stimage-0.2.9/test_c/test_xyxymatch_triangles.c`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/test_c/wscript` & `stsci_stimage-0.2.9/test_c/wscript`

 * *Files identical despite different names*

### Comparing `stsci_stimage-0.2.8/wscript` & `stsci_stimage-0.2.9/wscript`

 * *Files identical despite different names*

