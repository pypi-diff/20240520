# Comparing `tmp/pybloomfiltermmap3-0.5.7.tar.gz` & `tmp/pybloomfiltermmap3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybloomfiltermmap3-0.5.7.tar", last modified: Thu Feb 16 20:28:03 2023, max compression
+gzip compressed data, was "pybloomfiltermmap3-0.6.0.tar", last modified: Mon May 20 16:47:46 2024, max compression
```

## Comparing `pybloomfiltermmap3-0.5.7.tar` & `pybloomfiltermmap3-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 prashant   (501) staff       (20)        0 2023-02-16 20:28:03.272575 pybloomfiltermmap3-0.5.7/
--rw-r--r--   0 prashant   (501) staff       (20)      611 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.5.7/AUTHORS
--rw-r--r--   0 prashant   (501) staff       (20)     4456 2023-02-16 20:25:28.000000 pybloomfiltermmap3-0.5.7/CHANGELOG
--rw-r--r--   0 prashant   (501) staff       (20)     1130 2023-02-16 20:11:31.000000 pybloomfiltermmap3-0.5.7/LICENSE
--rw-r--r--   0 prashant   (501) staff       (20)      124 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/MANIFEST.in
--rw-r--r--   0 prashant   (501) staff       (20)     5611 2023-02-16 20:28:03.271898 pybloomfiltermmap3-0.5.7/PKG-INFO
--rw-r--r--   0 prashant   (501) staff       (20)     4098 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.5.7/README.markdown
-drwxr-xr-x   0 prashant   (501) staff       (20)        0 2023-02-16 20:28:03.233259 pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/
--rw-r--r--   0 prashant   (501) staff       (20)     5611 2023-02-16 20:28:02.000000 pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/PKG-INFO
--rw-r--r--   0 prashant   (501) staff       (20)      827 2023-02-16 20:28:03.000000 pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/SOURCES.txt
--rw-r--r--   0 prashant   (501) staff       (20)        1 2023-02-16 20:28:02.000000 pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/dependency_links.txt
--rw-r--r--   0 prashant   (501) staff       (20)       14 2023-02-16 20:28:03.000000 pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/top_level.txt
--rw-r--r--   0 prashant   (501) staff       (20)       38 2023-02-16 20:28:03.273031 pybloomfiltermmap3-0.5.7/setup.cfg
--rw-r--r--   0 prashant   (501) staff       (20)     2562 2023-02-16 20:25:33.000000 pybloomfiltermmap3-0.5.7/setup.py
-drwxr-xr-x   0 prashant   (501) staff       (20)        0 2023-02-16 20:28:03.248117 pybloomfiltermmap3-0.5.7/src/
--rw-r--r--   0 prashant   (501) staff       (20)      357 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/Makefile
--rw-r--r--   0 prashant   (501) staff       (20)     8053 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/MurmurHash3.c
--rw-r--r--   0 prashant   (501) staff       (20)     1125 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/MurmurHash3.h
--rw-r--r--   0 prashant   (501) staff       (20)     6106 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/bloomfilter.c
--rw-r--r--   0 prashant   (501) staff       (20)     2647 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/bloomfilter.h
--rw-r--r--   0 prashant   (501) staff       (20)     2263 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.5.7/src/cbloomfilter.pxd
--rw-r--r--   0 prashant   (501) staff       (20)    13342 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/md5.c
--rw-r--r--   0 prashant   (501) staff       (20)     3359 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/md5.h
--rw-r--r--   0 prashant   (501) staff       (20)    14472 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.5.7/src/mmapbitarray.c
--rw-r--r--   0 prashant   (501) staff       (20)     2737 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.5.7/src/mmapbitarray.h
--rw-r--r--   0 prashant   (501) staff       (20)      339 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/primetester.c
--rw-r--r--   0 prashant   (501) staff       (20)      119 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/primetester.h
--rw-r--r--   0 prashant   (501) staff       (20)   573524 2023-02-16 20:26:40.000000 pybloomfiltermmap3-0.5.7/src/pybloomfilter.c
--rw-r--r--   0 prashant   (501) staff       (20)    19983 2023-02-16 20:26:22.000000 pybloomfiltermmap3-0.5.7/src/pybloomfilter.pyx
--rw-r--r--   0 prashant   (501) staff       (20)     1786 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/src/superfast.h
-drwxr-xr-x   0 prashant   (501) staff       (20)        0 2023-02-16 20:28:03.251896 pybloomfiltermmap3-0.5.7/tests/
--rw-r--r--   0 prashant   (501) staff       (20)      771 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/__init__.py
-drwxr-xr-x   0 prashant   (501) staff       (20)        0 2023-02-16 20:28:03.255924 pybloomfiltermmap3-0.5.7/tests/__pycache__/
--rw-r--r--   0 prashant   (501) staff       (20)     1085 2020-08-21 16:08:13.000000 pybloomfiltermmap3-0.5.7/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 prashant   (501) staff       (20)     5823 2020-08-21 16:08:13.000000 pybloomfiltermmap3-0.5.7/tests/__pycache__/accuracytest.cpython-38.pyc
--rw-r--r--   0 prashant   (501) staff       (20)    14010 2021-10-28 18:14:18.000000 pybloomfiltermmap3-0.5.7/tests/__pycache__/simpletest.cpython-38.pyc
--rw-r--r--   0 prashant   (501) staff       (20)     5931 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/accuracytest.py
-drwxr-xr-x   0 prashant   (501) staff       (20)        0 2023-02-16 20:28:03.265008 pybloomfiltermmap3-0.5.7/tests/comparisons/
--rw-r--r--   0 prashant   (501) staff       (20)        0 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/comparisons/__init__.py
--rwxr-xr-x   0 prashant   (501) staff       (20)     1921 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/comparisons/accuracytest.py
--rwxr-xr-x   0 prashant   (501) staff       (20)     2190 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/comparisons/speedtest.py
--rw-r--r--   0 prashant   (501) staff       (20)   210719 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/comparisons/testwords
--rw-r--r--   0 prashant   (501) staff       (20)   931708 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.5.7/tests/comparisons/words
--rwxr-xr-x   0 prashant   (501) staff       (20)    15094 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.5.7/tests/simpletest.py
+drwxr-xr-x   0 prashant   (501) staff       (20)        0 2024-05-20 16:47:46.650866 pybloomfiltermmap3-0.6.0/
+-rw-r--r--   0 prashant   (501) staff       (20)      652 2024-05-20 16:46:46.000000 pybloomfiltermmap3-0.6.0/AUTHORS
+-rw-r--r--   0 prashant   (501) staff       (20)     4666 2024-05-20 16:45:22.000000 pybloomfiltermmap3-0.6.0/CHANGELOG
+-rw-r--r--   0 prashant   (501) staff       (20)     1130 2023-02-16 20:11:31.000000 pybloomfiltermmap3-0.6.0/LICENSE
+-rw-r--r--   0 prashant   (501) staff       (20)      118 2024-05-20 16:25:10.000000 pybloomfiltermmap3-0.6.0/MANIFEST.in
+-rw-r--r--   0 prashant   (501) staff       (20)     5635 2024-05-20 16:47:46.650743 pybloomfiltermmap3-0.6.0/PKG-INFO
+-rw-r--r--   0 prashant   (501) staff       (20)     4821 2024-05-20 16:25:10.000000 pybloomfiltermmap3-0.6.0/README.md
+drwxr-xr-x   0 prashant   (501) staff       (20)        0 2024-05-20 16:47:46.642542 pybloomfiltermmap3-0.6.0/pybloomfiltermmap3.egg-info/
+-rw-r--r--   0 prashant   (501) staff       (20)     5635 2024-05-20 16:47:46.000000 pybloomfiltermmap3-0.6.0/pybloomfiltermmap3.egg-info/PKG-INFO
+-rw-r--r--   0 prashant   (501) staff       (20)      956 2024-05-20 16:47:46.000000 pybloomfiltermmap3-0.6.0/pybloomfiltermmap3.egg-info/SOURCES.txt
+-rw-r--r--   0 prashant   (501) staff       (20)        1 2024-05-20 16:47:46.000000 pybloomfiltermmap3-0.6.0/pybloomfiltermmap3.egg-info/dependency_links.txt
+-rw-r--r--   0 prashant   (501) staff       (20)       14 2024-05-20 16:47:46.000000 pybloomfiltermmap3-0.6.0/pybloomfiltermmap3.egg-info/top_level.txt
+-rw-r--r--   0 prashant   (501) staff       (20)       38 2024-05-20 16:47:46.650913 pybloomfiltermmap3-0.6.0/setup.cfg
+-rw-r--r--   0 prashant   (501) staff       (20)     2556 2024-05-20 16:45:48.000000 pybloomfiltermmap3-0.6.0/setup.py
+drwxr-xr-x   0 prashant   (501) staff       (20)        0 2024-05-20 16:47:46.645332 pybloomfiltermmap3-0.6.0/src/
+-rw-r--r--   0 prashant   (501) staff       (20)      357 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/Makefile
+-rw-r--r--   0 prashant   (501) staff       (20)     8053 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/MurmurHash3.c
+-rw-r--r--   0 prashant   (501) staff       (20)     1125 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/MurmurHash3.h
+-rw-r--r--   0 prashant   (501) staff       (20)     6197 2024-05-20 16:25:10.000000 pybloomfiltermmap3-0.6.0/src/bloomfilter.c
+-rw-r--r--   0 prashant   (501) staff       (20)     2666 2024-05-20 16:25:10.000000 pybloomfiltermmap3-0.6.0/src/bloomfilter.h
+-rw-r--r--   0 prashant   (501) staff       (20)     2276 2024-05-20 16:25:10.000000 pybloomfiltermmap3-0.6.0/src/cbloomfilter.pxd
+-rw-r--r--   0 prashant   (501) staff       (20)    13342 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/md5.c
+-rw-r--r--   0 prashant   (501) staff       (20)     3359 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/md5.h
+-rw-r--r--   0 prashant   (501) staff       (20)    14472 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.6.0/src/mmapbitarray.c
+-rw-r--r--   0 prashant   (501) staff       (20)     2737 2021-10-28 18:02:49.000000 pybloomfiltermmap3-0.6.0/src/mmapbitarray.h
+-rw-r--r--   0 prashant   (501) staff       (20)      339 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/primetester.c
+-rw-r--r--   0 prashant   (501) staff       (20)      119 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/primetester.h
+-rw-r--r--   0 prashant   (501) staff       (20)   583804 2024-05-20 16:47:40.000000 pybloomfiltermmap3-0.6.0/src/pybloomfilter.c
+-rw-r--r--   0 prashant   (501) staff       (20)    21561 2024-05-20 16:38:35.000000 pybloomfiltermmap3-0.6.0/src/pybloomfilter.pyx
+-rw-r--r--   0 prashant   (501) staff       (20)     1786 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/src/superfast.h
+drwxr-xr-x   0 prashant   (501) staff       (20)        0 2024-05-20 16:47:46.646037 pybloomfiltermmap3-0.6.0/tests/
+-rw-r--r--   0 prashant   (501) staff       (20)      771 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/__init__.py
+drwxr-xr-x   0 prashant   (501) staff       (20)        0 2024-05-20 16:47:46.647869 pybloomfiltermmap3-0.6.0/tests/__pycache__/
+-rw-r--r--   0 prashant   (501) staff       (20)     2030 2024-05-20 16:27:19.000000 pybloomfiltermmap3-0.6.0/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 prashant   (501) staff       (20)     1085 2020-08-21 16:08:13.000000 pybloomfiltermmap3-0.6.0/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 prashant   (501) staff       (20)    10286 2024-05-20 16:27:19.000000 pybloomfiltermmap3-0.6.0/tests/__pycache__/accuracytest.cpython-311.pyc
+-rw-r--r--   0 prashant   (501) staff       (20)     5823 2020-08-21 16:08:13.000000 pybloomfiltermmap3-0.6.0/tests/__pycache__/accuracytest.cpython-38.pyc
+-rw-r--r--   0 prashant   (501) staff       (20)    28576 2024-05-20 16:27:20.000000 pybloomfiltermmap3-0.6.0/tests/__pycache__/simpletest.cpython-311.pyc
+-rw-r--r--   0 prashant   (501) staff       (20)    14010 2021-10-28 18:14:18.000000 pybloomfiltermmap3-0.6.0/tests/__pycache__/simpletest.cpython-38.pyc
+-rw-r--r--   0 prashant   (501) staff       (20)     5931 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/accuracytest.py
+drwxr-xr-x   0 prashant   (501) staff       (20)        0 2024-05-20 16:47:46.649589 pybloomfiltermmap3-0.6.0/tests/comparisons/
+-rw-r--r--   0 prashant   (501) staff       (20)        0 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/comparisons/__init__.py
+-rwxr-xr-x   0 prashant   (501) staff       (20)     1921 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/comparisons/accuracytest.py
+-rwxr-xr-x   0 prashant   (501) staff       (20)     2190 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/comparisons/speedtest.py
+-rw-r--r--   0 prashant   (501) staff       (20)   210719 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/comparisons/testwords
+-rw-r--r--   0 prashant   (501) staff       (20)   931708 2020-08-21 16:06:31.000000 pybloomfiltermmap3-0.6.0/tests/comparisons/words
+-rwxr-xr-x   0 prashant   (501) staff       (20)    15527 2024-05-20 16:25:10.000000 pybloomfiltermmap3-0.6.0/tests/simpletest.py
```

### Comparing `pybloomfiltermmap3-0.5.7/CHANGELOG` & `pybloomfiltermmap3-0.6.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_,
 and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
+`0.6.0`_ (2023-02-16)
+---------------------
+.. _0.6.0: https://github.com/prashnts/pybloomfiltermmap3/releases/tag/0.6.0
+
+Added
+^^^^^
+- In-memory bloom filters are now pickleable. Thanks @stevesimmons (#44)!
+
+
 `0.5.7`_ (2023-02-16)
 ---------------------
 .. _0.5.7: https://github.com/prashnts/pybloomfiltermmap3/releases/tag/0.5.7
 
 Fixes
 ^^^^^
 - Ensure installation in Python 3.10+ doesn't fail.
```

### Comparing `pybloomfiltermmap3-0.5.7/LICENSE` & `pybloomfiltermmap3-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/PKG-INFO` & `pybloomfiltermmap3-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,129 @@
-Metadata-Version: 2.1
-Name: pybloomfiltermmap3
-Version: 0.5.7
-Summary: A fast implementation of Bloom filter for Python 3 built on mmap
-Home-page: https://github.com/prashnts/pybloomfiltermmap3
-Author: Prashant Sinha
-Author-email: prashant@noop.pw
-License: MIT License
-Description: # pybloomfiltermmap3
-        
-        [pybloomfiltermmap3](https://github.com/prashnts/pybloomfiltermmap3) is a Python 3 compatible fork of [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) by [@axiak](https://github.com/axiak).
-        
-        The goal of `pybloomfiltermmap3` is simple: to provide a fast, simple, scalable, correct library for Bloom filters in Python.
-        
-        [![Build Status](https://travis-ci.org/PrashntS/pybloomfiltermmap3.svg?branch=master)](https://travis-ci.org/PrashntS/pybloomfiltermmap3)
-        [![Documentation Status](https://readthedocs.org/projects/pybloomfiltermmap3/badge/?version=latest)](https://pybloomfiltermmap3.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
-        [![PyPI](https://img.shields.io/pypi/dw/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
-        [![PyPI](https://img.shields.io/pypi/pyversions/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
-        
-        
-        ## Why pybloomfiltermmap3?
-        
-        There are a couple reasons to use this module:
-        
-        * It natively uses [mmaped files](http://en.wikipedia.org/wiki/Mmap).
-        * It is fast (see [benchmarks](http://axiak.github.io/pybloomfiltermmap/#benchmarks)).
-        * It natively does the set things you want a Bloom filter to do.
-        
-        
-        ## Quickstart
-        
-        After you install, the interface to use is a cross between a file
-        interface and an ste interface. As an example:
-        ```python
-            >>> import pybloomfilter
-            >>> fruit = pybloomfilter.BloomFilter(100000, 0.1, '/tmp/words.bloom')
-            >>> fruit.update(('apple', 'pear', 'orange', 'apple'))
-            >>> len(fruit)
-            3
-            >>> 'mike' in fruit
-            False
-            >>> 'apple' in fruit
-            True
-        ```
-        
-        To create an in-memory filter, simply omit the file location:
-        ```python
-            >>> cakes = pybloomfilter.BloomFilter(10000, 0.1)
-        ```
-        *Caveat*: it is currently not possible to persist this filter later.
-        
-        
-        ## Docs
-        
-        Current docs are available at [pybloomfiltermmap3.rtfd.io](https://pybloomfiltermmap3.readthedocs.io/en/latest).
-        
-        
-        ## Install
-        
-        To install:
-        
-        ```shell
-            $ pip install pybloomfiltermmap3
-        ```
-        
-        and you should be set.
-        
-        ### Note to Python 2 to < 3.5 users
-        
-        This library is specifically meant for Python 3.5 and above. [As of 2020](https://www.python.org/doc/sunset-python-2/), we strongly advise you to switch to an actively maintained distribution of Python 3. If for any reason your current environment is restricted to Python 2, please see [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap). Please note that the latter is not actively maintained and will lack bug fixes and new features.
-        
-        
-        ## History and Future
-        
-        [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) is an excellent Bloom filter implementation for Python 2 by [@axiak](https://github.com/axiak) and contributors. I, [@prashnts](https://github.com/prashnts), made initial changes to add support for Python 3 sometime in 2016 as the current [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) on `PyPI`. Since then, with the help of contributors, there have been incremental improvements and bug fixes while maintaining the API from versions `0.4.x` and below.
-        
-        Some new features and changes were first introduced in version `0.5.0`. From this point on, the goal is to reach stability, as well as add a few more APIs to expand upon the use cases. While we can't guarantee that we won't change the current interface, the transition from versions `0.4.x` and below should be quick one liners. Please open an issue if we broke your build!
-        
-        Suggestions, bug reports, and / or patches are welcome!
-        
-        
-        ## Contributions and development
-        
-        When contributing, you should set up an appropriate Python 3 environment and install the dependencies listed in `requirements-dev.txt`.
-        Package installation depends on a generated `pybloomfilter.c` file, which requires Cython module to be in your current environment.
-        
-        
-        ## Maintainers
-        
-        * [Prashant Sinha](https://github.com/prashnts)
-        * [Vytautas Mizgiris](https://github.com/vmizg)
-        
-        
-        ## License
-        
-        See the LICENSE file. It's under the MIT License.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5, <4
-Description-Content-Type: text/markdown
+# pybloomfiltermmap3
+
+[pybloomfiltermmap3](https://github.com/prashnts/pybloomfiltermmap3) is a Python 3 compatible fork of [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) by [@axiak](https://github.com/axiak).
+
+The goal of `pybloomfiltermmap3` is simple: to provide a fast, simple, scalable, correct library for Bloom filters in Python.
+
+[![Build Status](https://travis-ci.org/PrashntS/pybloomfiltermmap3.svg?branch=master)](https://travis-ci.org/PrashntS/pybloomfiltermmap3)
+[![Documentation Status](https://readthedocs.org/projects/pybloomfiltermmap3/badge/?version=latest)](https://pybloomfiltermmap3.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
+[![PyPI](https://img.shields.io/pypi/dw/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
+[![PyPI](https://img.shields.io/pypi/pyversions/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
+
+## Why pybloomfiltermmap3?
+
+There are a couple reasons to use this module:
+
+- It natively uses [mmapped files](http://en.wikipedia.org/wiki/Mmap).
+- It is fast (see [benchmarks](http://axiak.github.io/pybloomfiltermmap/#benchmarks)).
+- It natively does the set things you want a Bloom filter to do.
+
+## Quickstart
+
+After you install, the interface to use is a cross between a file
+interface and an ste interface. As an example:
+
+```python
+    >>> import pybloomfilter
+    >>> fruit = pybloomfilter.BloomFilter(100000, 0.1, '/tmp/words.bloom')
+    >>> fruit.update(('apple', 'pear', 'orange', 'apple'))
+    >>> len(fruit)
+    3
+    >>> 'mike' in fruit
+    False
+    >>> 'apple' in fruit
+    True
+```
+
+To create an in-memory filter, simply omit the file location:
+
+```python
+    >>> fruit = pybloomfilter.BloomFilter(10000, 0.1)
+    >>> fruit.add('apple')
+    >>> 'apple' in fruit
+    True
+```
+
+These in-memory filters can be pickled and reloaded:
+
+```python
+    >>> import pickle
+    >>> pickled_fruit = pickle.dumps(fruit)
+    >>> unpickled_fruit = pickle.loads(pickled_fruit)
+    >>> 'apple' in unpickled_fruit
+    True
+```
+
+_Caveat_: it is currently not possible to persist this filter later as an mmap file.
+
+## Docs
+
+Current docs are available at [pybloomfiltermmap3.rtfd.io](https://pybloomfiltermmap3.readthedocs.io/en/latest).
+
+## Install
+
+To install:
+
+```bash
+pip install pybloomfiltermmap3
+```
+
+and you should be set.
+
+### Note to Python 2 to < 3.5 users
+
+This library is specifically meant for Python 3.5 and above. [As of 2020](https://www.python.org/doc/sunset-python-2/), we strongly advise you to switch to an actively maintained distribution of Python 3. If for any reason your current environment is restricted to Python 2, please see [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap). Please note that the latter is not actively maintained and will lack bug fixes and new features.
+
+## History and Future
+
+[pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) is an excellent Bloom filter implementation for Python 2 by [@axiak](https://github.com/axiak) and contributors. I, [@prashnts](https://github.com/prashnts), made initial changes to add support for Python 3 sometime in 2016 as the current [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) on `PyPI`. Since then, with the help of contributors, there have been incremental improvements and bug fixes while maintaining the API from versions `0.4.x` and below.
+
+Some new features and changes were first introduced in version `0.5.0`. From this point on, the goal is to reach stability, as well as add a few more APIs to expand upon the use cases. While we can't guarantee that we won't change the current interface, the transition from versions `0.4.x` and below should be quick one liners. Please open an issue if we broke your build!
+
+Suggestions, bug reports, and / or patches are welcome!
+
+## Contributions and development
+
+When contributing, you should set up an appropriate Python 3 environment and install the dependencies listed in `requirements-dev.txt`.
+Package installation depends on a generated `pybloomfilter.c` file, which requires Cython module to be in your current environment.
+
+### Environment setup
+
+```bash
+# Installs the venv and python3-dev packages
+sudo apt install python3.10-venv python3-dev
+
+# Creates a virtual env called "env"
+python -m venv env
+
+# Activates the created virtual env
+source ./env/bin/activate
+```
+
+### Dependencies
+
+```bash
+python -m pip install --upgrade pip
+pip install cython
+```
+
+### Build
+
+```bash
+python setup.py develop
+```
+
+### Test
+
+```bash
+python setup.py test
+```
+
+## Maintainers
+
+- [Prashant Sinha](https://github.com/prashnts)
+- [Vytautas Mizgiris](https://github.com/vmizg)
+
+## License
+
+See the LICENSE file. It's under the MIT License.
```

### Comparing `pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/PKG-INFO` & `pybloomfiltermmap3-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,151 @@
 Metadata-Version: 2.1
 Name: pybloomfiltermmap3
-Version: 0.5.7
+Version: 0.6.0
 Summary: A fast implementation of Bloom filter for Python 3 built on mmap
 Home-page: https://github.com/prashnts/pybloomfiltermmap3
 Author: Prashant Sinha
 Author-email: prashant@noop.pw
 License: MIT License
-Description: # pybloomfiltermmap3
-        
-        [pybloomfiltermmap3](https://github.com/prashnts/pybloomfiltermmap3) is a Python 3 compatible fork of [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) by [@axiak](https://github.com/axiak).
-        
-        The goal of `pybloomfiltermmap3` is simple: to provide a fast, simple, scalable, correct library for Bloom filters in Python.
-        
-        [![Build Status](https://travis-ci.org/PrashntS/pybloomfiltermmap3.svg?branch=master)](https://travis-ci.org/PrashntS/pybloomfiltermmap3)
-        [![Documentation Status](https://readthedocs.org/projects/pybloomfiltermmap3/badge/?version=latest)](https://pybloomfiltermmap3.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
-        [![PyPI](https://img.shields.io/pypi/dw/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
-        [![PyPI](https://img.shields.io/pypi/pyversions/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
-        
-        
-        ## Why pybloomfiltermmap3?
-        
-        There are a couple reasons to use this module:
-        
-        * It natively uses [mmaped files](http://en.wikipedia.org/wiki/Mmap).
-        * It is fast (see [benchmarks](http://axiak.github.io/pybloomfiltermmap/#benchmarks)).
-        * It natively does the set things you want a Bloom filter to do.
-        
-        
-        ## Quickstart
-        
-        After you install, the interface to use is a cross between a file
-        interface and an ste interface. As an example:
-        ```python
-            >>> import pybloomfilter
-            >>> fruit = pybloomfilter.BloomFilter(100000, 0.1, '/tmp/words.bloom')
-            >>> fruit.update(('apple', 'pear', 'orange', 'apple'))
-            >>> len(fruit)
-            3
-            >>> 'mike' in fruit
-            False
-            >>> 'apple' in fruit
-            True
-        ```
-        
-        To create an in-memory filter, simply omit the file location:
-        ```python
-            >>> cakes = pybloomfilter.BloomFilter(10000, 0.1)
-        ```
-        *Caveat*: it is currently not possible to persist this filter later.
-        
-        
-        ## Docs
-        
-        Current docs are available at [pybloomfiltermmap3.rtfd.io](https://pybloomfiltermmap3.readthedocs.io/en/latest).
-        
-        
-        ## Install
-        
-        To install:
-        
-        ```shell
-            $ pip install pybloomfiltermmap3
-        ```
-        
-        and you should be set.
-        
-        ### Note to Python 2 to < 3.5 users
-        
-        This library is specifically meant for Python 3.5 and above. [As of 2020](https://www.python.org/doc/sunset-python-2/), we strongly advise you to switch to an actively maintained distribution of Python 3. If for any reason your current environment is restricted to Python 2, please see [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap). Please note that the latter is not actively maintained and will lack bug fixes and new features.
-        
-        
-        ## History and Future
-        
-        [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) is an excellent Bloom filter implementation for Python 2 by [@axiak](https://github.com/axiak) and contributors. I, [@prashnts](https://github.com/prashnts), made initial changes to add support for Python 3 sometime in 2016 as the current [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) on `PyPI`. Since then, with the help of contributors, there have been incremental improvements and bug fixes while maintaining the API from versions `0.4.x` and below.
-        
-        Some new features and changes were first introduced in version `0.5.0`. From this point on, the goal is to reach stability, as well as add a few more APIs to expand upon the use cases. While we can't guarantee that we won't change the current interface, the transition from versions `0.4.x` and below should be quick one liners. Please open an issue if we broke your build!
-        
-        Suggestions, bug reports, and / or patches are welcome!
-        
-        
-        ## Contributions and development
-        
-        When contributing, you should set up an appropriate Python 3 environment and install the dependencies listed in `requirements-dev.txt`.
-        Package installation depends on a generated `pybloomfilter.c` file, which requires Cython module to be in your current environment.
-        
-        
-        ## Maintainers
-        
-        * [Prashant Sinha](https://github.com/prashnts)
-        * [Vytautas Mizgiris](https://github.com/vmizg)
-        
-        
-        ## License
-        
-        See the LICENSE file. It's under the MIT License.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# pybloomfiltermmap3
+
+[pybloomfiltermmap3](https://github.com/prashnts/pybloomfiltermmap3) is a Python 3 compatible fork of [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) by [@axiak](https://github.com/axiak).
+
+The goal of `pybloomfiltermmap3` is simple: to provide a fast, simple, scalable, correct library for Bloom filters in Python.
+
+[![Build Status](https://travis-ci.org/PrashntS/pybloomfiltermmap3.svg?branch=master)](https://travis-ci.org/PrashntS/pybloomfiltermmap3)
+[![Documentation Status](https://readthedocs.org/projects/pybloomfiltermmap3/badge/?version=latest)](https://pybloomfiltermmap3.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
+[![PyPI](https://img.shields.io/pypi/dw/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
+[![PyPI](https://img.shields.io/pypi/pyversions/pybloomfiltermmap3.svg)](https://pypi.python.org/pypi/pybloomfiltermmap3)
+
+## Why pybloomfiltermmap3?
+
+There are a couple reasons to use this module:
+
+- It natively uses [mmapped files](http://en.wikipedia.org/wiki/Mmap).
+- It is fast (see [benchmarks](http://axiak.github.io/pybloomfiltermmap/#benchmarks)).
+- It natively does the set things you want a Bloom filter to do.
+
+## Quickstart
+
+After you install, the interface to use is a cross between a file
+interface and an ste interface. As an example:
+
+```python
+    >>> import pybloomfilter
+    >>> fruit = pybloomfilter.BloomFilter(100000, 0.1, '/tmp/words.bloom')
+    >>> fruit.update(('apple', 'pear', 'orange', 'apple'))
+    >>> len(fruit)
+    3
+    >>> 'mike' in fruit
+    False
+    >>> 'apple' in fruit
+    True
+```
+
+To create an in-memory filter, simply omit the file location:
+
+```python
+    >>> fruit = pybloomfilter.BloomFilter(10000, 0.1)
+    >>> fruit.add('apple')
+    >>> 'apple' in fruit
+    True
+```
+
+These in-memory filters can be pickled and reloaded:
+
+```python
+    >>> import pickle
+    >>> pickled_fruit = pickle.dumps(fruit)
+    >>> unpickled_fruit = pickle.loads(pickled_fruit)
+    >>> 'apple' in unpickled_fruit
+    True
+```
+
+_Caveat_: it is currently not possible to persist this filter later as an mmap file.
+
+## Docs
+
+Current docs are available at [pybloomfiltermmap3.rtfd.io](https://pybloomfiltermmap3.readthedocs.io/en/latest).
+
+## Install
+
+To install:
+
+```bash
+pip install pybloomfiltermmap3
+```
+
+and you should be set.
+
+### Note to Python 2 to < 3.5 users
+
+This library is specifically meant for Python 3.5 and above. [As of 2020](https://www.python.org/doc/sunset-python-2/), we strongly advise you to switch to an actively maintained distribution of Python 3. If for any reason your current environment is restricted to Python 2, please see [pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap). Please note that the latter is not actively maintained and will lack bug fixes and new features.
+
+## History and Future
+
+[pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) is an excellent Bloom filter implementation for Python 2 by [@axiak](https://github.com/axiak) and contributors. I, [@prashnts](https://github.com/prashnts), made initial changes to add support for Python 3 sometime in 2016 as the current [pybloomfiltermmap3](https://pypi.org/project/pybloomfiltermmap3/) on `PyPI`. Since then, with the help of contributors, there have been incremental improvements and bug fixes while maintaining the API from versions `0.4.x` and below.
+
+Some new features and changes were first introduced in version `0.5.0`. From this point on, the goal is to reach stability, as well as add a few more APIs to expand upon the use cases. While we can't guarantee that we won't change the current interface, the transition from versions `0.4.x` and below should be quick one liners. Please open an issue if we broke your build!
+
+Suggestions, bug reports, and / or patches are welcome!
+
+## Contributions and development
+
+When contributing, you should set up an appropriate Python 3 environment and install the dependencies listed in `requirements-dev.txt`.
+Package installation depends on a generated `pybloomfilter.c` file, which requires Cython module to be in your current environment.
+
+### Environment setup
+
+```bash
+# Installs the venv and python3-dev packages
+sudo apt install python3.10-venv python3-dev
+
+# Creates a virtual env called "env"
+python -m venv env
+
+# Activates the created virtual env
+source ./env/bin/activate
+```
+
+### Dependencies
+
+```bash
+python -m pip install --upgrade pip
+pip install cython
+```
+
+### Build
+
+```bash
+python setup.py develop
+```
+
+### Test
+
+```bash
+python setup.py test
+```
+
+## Maintainers
+
+- [Prashant Sinha](https://github.com/prashnts)
+- [Vytautas Mizgiris](https://github.com/vmizg)
+
+## License
+
+See the LICENSE file. It's under the MIT License.
```

### Comparing `pybloomfiltermmap3-0.5.7/pybloomfiltermmap3.egg-info/SOURCES.txt` & `pybloomfiltermmap3-0.6.0/pybloomfiltermmap3.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 CHANGELOG
 LICENSE
 MANIFEST.in
-README.markdown
+README.md
 setup.py
 pybloomfiltermmap3.egg-info/PKG-INFO
 pybloomfiltermmap3.egg-info/SOURCES.txt
 pybloomfiltermmap3.egg-info/dependency_links.txt
 pybloomfiltermmap3.egg-info/top_level.txt
 src/Makefile
 src/MurmurHash3.c
@@ -22,15 +22,18 @@
 src/primetester.h
 src/pybloomfilter.c
 src/pybloomfilter.pyx
 src/superfast.h
 tests/__init__.py
 tests/accuracytest.py
 tests/simpletest.py
+tests/__pycache__/__init__.cpython-311.pyc
 tests/__pycache__/__init__.cpython-38.pyc
+tests/__pycache__/accuracytest.cpython-311.pyc
 tests/__pycache__/accuracytest.cpython-38.pyc
+tests/__pycache__/simpletest.cpython-311.pyc
 tests/__pycache__/simpletest.cpython-38.pyc
 tests/comparisons/__init__.py
 tests/comparisons/accuracytest.py
 tests/comparisons/speedtest.py
 tests/comparisons/testwords
 tests/comparisons/words
```

### Comparing `pybloomfiltermmap3-0.5.7/setup.py` & `pybloomfiltermmap3-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 5):
     raise SystemError("This package is for Python 3.5 and above.")
 
 here = os.path.dirname(__file__)
 
 # Get the long description from the README file
-with open(os.path.join(here, "README.markdown"), encoding="utf-8") as fp:
+with open(os.path.join(here, "README.md"), encoding="utf-8") as fp:
     long_description = fp.read()
 
 setup_kwargs = {}
 
 ext_files = [
     "src/mmapbitarray.c",
     "src/bloomfilter.c",
@@ -53,15 +53,15 @@
     # Note that we let the exception bubble up if `pybloomfilter.c` doesn't exist.
     ext_files.append("src/pybloomfilter.c")
 
 ext_modules = [Extension("pybloomfilter", ext_files)]
 
 setup(
     name="pybloomfiltermmap3",
-    version="0.5.7",
+    version="0.6.0",
     author="Prashant Sinha",
     author_email="prashant@noop.pw",
     url="https://github.com/prashnts/pybloomfiltermmap3",
     description="A fast implementation of Bloom filter for Python 3 built on mmap",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT License",
```

### Comparing `pybloomfiltermmap3-0.5.7/src/MurmurHash3.c` & `pybloomfiltermmap3-0.6.0/src/MurmurHash3.c`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/src/MurmurHash3.h` & `pybloomfiltermmap3-0.6.0/src/MurmurHash3.h`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/src/bloomfilter.c` & `pybloomfiltermmap3-0.6.0/src/bloomfilter.c`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include <stdio.h>
 #include <fcntl.h>
 #include "md5.h"
 
 #include "bloomfilter.h"
 
 BloomFilter *bloomfilter_Create_Malloc(size_t max_num_elem, double error_rate,
-                                BTYPE num_bits, int *hash_seeds, int num_hashes)
+                                BTYPE num_bits, int *hash_seeds, int num_hashes, const char *data)
 {
     BloomFilter * bf = (BloomFilter *)malloc(sizeof(BloomFilter));
     MBArray * array;
 
     if (!bf) {
         return NULL;
     }
@@ -31,14 +31,17 @@
     memset(bf->hash_seeds, 0, sizeof(uint32_t) * 256);
     memcpy(bf->hash_seeds, hash_seeds, sizeof(uint32_t) * num_hashes);
     array = mbarray_Create_Malloc(num_bits);
     if (!array) {
         bloomfilter_Destroy(bf);
         return NULL;
     }
+    if (data) {
+        memcpy(array->vector, data, num_bits / 8);
+    }
 
     bf->array = array;
 
     return bf;
 }
```

### Comparing `pybloomfiltermmap3-0.5.7/src/bloomfilter.h` & `pybloomfiltermmap3-0.6.0/src/bloomfilter.h`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     char * shash;
 } Key;
 
 typedef struct _BloomFilter BloomFilter;
 
 /* Create a bloom filter without a memory-mapped file backing it */
 BloomFilter *bloomfilter_Create_Malloc(size_t max_num_elem, double error_rate,
-                                BTYPE num_bits, int *hash_seeds, int num_hashes);
+                                BTYPE num_bits, int *hash_seeds, int num_hashes, const char * data);
 
 /* Create a bloom filter with a memory-mapped file backing it */
 BloomFilter *bloomfilter_Create_Mmap(size_t max_num_elem, double error_rate,
                                 const char * file, BTYPE num_bits, int oflags, int perms,
                                 int *hash_seeds, int num_hashes);
 
 void bloomfilter_Destroy(BloomFilter * bf);
```

### Comparing `pybloomfiltermmap3-0.5.7/src/cbloomfilter.pxd` & `pybloomfiltermmap3-0.6.0/src/cbloomfilter.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,14 @@
                                       double error_rate,
                                       char * fname, long num_bits,
                                       int oflags, int perms,
                                       int * hash_seeds, int num_hashes)
      BloomFilter * bloomfilter_Create_Malloc(long max_num_elem,
                                       double error_rate,
                                       long num_bits,
-                                      int * hash_seeds, int num_hashes)
+                                      int * hash_seeds, int num_hashes, char * data)
      void bloomfilter_Destroy(BloomFilter * bf)
      int bloomfilter_Add(BloomFilter * bf, Key * key)
      int bloomfilter_Test(BloomFilter * bf, Key * key)
      int bloomfilter_Update(BloomFilter * bf, char * data, int size)
      int bloomfilter_Clear(BloomFilter * bf)
      BloomFilter * bloomfilter_Copy_Template(BloomFilter * src, char * filename, int perms)
```

### Comparing `pybloomfiltermmap3-0.5.7/src/md5.c` & `pybloomfiltermmap3-0.6.0/src/md5.c`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/src/md5.h` & `pybloomfiltermmap3-0.6.0/src/md5.h`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/src/mmapbitarray.c` & `pybloomfiltermmap3-0.6.0/src/mmapbitarray.c`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/src/mmapbitarray.h` & `pybloomfiltermmap3-0.6.0/src/mmapbitarray.h`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/src/pybloomfilter.c` & `pybloomfiltermmap3-0.6.0/src/pybloomfilter.c`

 * *Files 4% similar despite different names*

```diff
@@ -953,24 +953,23 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
   "src/pybloomfilter.pyx",
-  "stringsource",
   "type.pxd",
   "bool.pxd",
   "complex.pxd",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_obj_13pybloomfilter_BloomFilter;
 
-/* "pybloomfilter.pyx":48
+/* "pybloomfilter.pyx":47
  * 
  * 
  * cdef class BloomFilter:             # <<<<<<<<<<<<<<
  *     """
  *     Creates a new BloomFilter object with a given capacity and error_rate.
  */
 struct __pyx_obj_13pybloomfilter_BloomFilter {
@@ -1179,21 +1178,14 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
-/* PyObjectFormat.proto */
-#if CYTHON_USE_UNICODE_WRITER
-static PyObject* __Pyx_PyObject_Format(PyObject* s, PyObject* f);
-#else
-#define __Pyx_PyObject_Format(s, f) PyObject_Format(s, f)
-#endif
-
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1225,14 +1217,21 @@
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* PyObjectFormat.proto */
+#if CYTHON_USE_UNICODE_WRITER
+static PyObject* __Pyx_PyObject_Format(PyObject* s, PyObject* f);
+#else
+#define __Pyx_PyObject_Format(s, f) PyObject_Format(s, f)
+#endif
+
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
@@ -1314,28 +1313,14 @@
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
-/* SetupReduce.proto */
-static int __Pyx_setup_reduce(PyObject* type_obj);
-
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
@@ -1349,14 +1334,22 @@
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* ClassMethod.proto */
 #include "descrobject.h"
 static CYTHON_UNUSED PyObject* __Pyx_Method_ClassMethod(PyObject *method);
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
 /* GetNameInClass.proto */
 #define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
 static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
@@ -1519,27 +1512,27 @@
 static PyObject *__pyx_builtin_OSError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_round;
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_PendingDeprecationWarning;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_open;
-static PyObject *__pyx_builtin_TypeError;
 static const char __pyx_k_[] = "+";
+static const char __pyx_k_B[] = "B";
 static const char __pyx_k_I[] = "I";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_d[] = "d";
 static const char __pyx_k_e[] = "e";
 static const char __pyx_k_f[] = "f";
 static const char __pyx_k_r[] = "r";
 static const char __pyx_k_w[] = "w";
-static const char __pyx_k__2[] = ": ";
-static const char __pyx_k__3[] = "";
-static const char __pyx_k__6[] = "<";
-static const char __pyx_k__7[] = ">";
+static const char __pyx_k__4[] = ": ";
+static const char __pyx_k__5[] = "";
+static const char __pyx_k__8[] = "<";
+static const char __pyx_k__9[] = ">";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_rw[] = "rw";
 static const char __pyx_k_add[] = "add";
 static const char __pyx_k_big[] = "big";
 static const char __pyx_k_eno[] = "eno";
 static const char __pyx_k_log[] = "log";
@@ -1586,15 +1579,14 @@
 static const char __pyx_k_exists[] = "exists";
 static const char __pyx_k_extend[] = "extend";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "_name";
 static const char __pyx_k_object[] = "object";
 static const char __pyx_k_open_2[] = "_open";
 static const char __pyx_k_random[] = "random";
-static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_shutil[] = "shutil";
 static const char __pyx_k_signed[] = "signed";
 static const char __pyx_k_string[] = "string";
 static const char __pyx_k_unlink[] = "unlink";
 static const char __pyx_k_Invalid[] = "Invalid ";
 static const char __pyx_k_OSError[] = "OSError";
 static const char __pyx_k_O_CREAT[] = "O_CREAT";
@@ -1603,70 +1595,67 @@
 static const char __pyx_k_tobytes[] = "tobytes";
 static const char __pyx_k_O_BINARY[] = "O_BINARY";
 static const char __pyx_k_O_RDONLY[] = "O_RDONLY";
 static const char __pyx_k_capacity[] = "capacity";
 static const char __pyx_k_compress[] = "compress";
 static const char __pyx_k_endswith[] = "endswith";
 static const char __pyx_k_filename[] = "filename";
-static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_num_bits[] = "num_bits";
-static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_strerror[] = "strerror";
 static const char __pyx_k_warnings[] = "warnings";
-static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_VERSION_2[] = "__VERSION__";
 static const char __pyx_k_b64decode[] = "b64decode";
 static const char __pyx_k_b64encode[] = "b64encode";
 static const char __pyx_k_bit_count[] = "bit_count";
 static const char __pyx_k_byteorder[] = "byteorder";
 static const char __pyx_k_frombytes[] = "frombytes";
 static const char __pyx_k_read_only[] = "read_only";
-static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_approx_len[] = "approx_len";
 static const char __pyx_k_bit_length[] = "bit_length";
 static const char __pyx_k_capacity_2[] = " capacity: ";
+static const char __pyx_k_data_array[] = "data_array";
 static const char __pyx_k_decompress[] = "decompress";
 static const char __pyx_k_error_rate[] = "error_rate";
 static const char __pyx_k_from_bytes[] = "from_bytes";
 static const char __pyx_k_hash_seeds[] = "hash_seeds";
 static const char __pyx_k_num_hashes[] = "num_hashes";
 static const char __pyx_k_BloomFilter[] = "BloomFilter";
 static const char __pyx_k_assert_open[] = "_assert_open";
 static const char __pyx_k_from_base64[] = "from_base64";
 static const char __pyx_k_getrandbits[] = "getrandbits";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_intersection[] = "intersection";
 static const char __pyx_k_num_hashes_2[] = ", num_hashes: ";
 static const char __pyx_k_Michael_Axiak[] = "Michael Axiak";
-static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_assert_writable[] = "_assert_writable";
-static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_assert_comparable[] = "_assert_comparable";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_NotImplementedError[] = "NotImplementedError";
 static const char __pyx_k_PendingDeprecationWarning[] = "PendingDeprecationWarning";
-static const char __pyx_k_BloomFilter_union_line_445[] = "BloomFilter.union (line 445)";
+static const char __pyx_k_BloomFilter_union_line_483[] = "BloomFilter.union (line 483)";
 static const char __pyx_k_I_O_operation_on_closed_file[] = "I/O operation on closed file";
+static const char __pyx_k_hash_seeds_must_be_specified_if[] = "hash_seeds must be specified if a data_array is provided.";
 static const char __pyx_k_Cannot_access_name_on_an_in_memo[] = "Cannot access .name on an in-memory %s";
 static const char __pyx_k_Cannot_call_copy_on_an_in_memory[] = "Cannot call .copy on an in-memory %s";
 static const char __pyx_k_Insufficient_permissions_for_fil[] = "Insufficient permissions for file %s";
 static const char __pyx_k_Performs_a_set_OR_with_another_c[] = "Performs a set OR with another comparable filter. You can (only) construct\n        comparable filters with :meth:`BloomFilter.copy_template` above.\n\n        The computation will occur *in place*. That is, calling::\n\n            >>> bf.union(bf2)\n\n        is a way of adding *all* the elements of ``bf2`` to ``bf``.\n\n        *NB: Calling this function will render future calls to len()\n        invalid.*\n\n        :param BloomFilter other: filter to perform the union with\n        :rtype: :class:`BloomFilter`\n        ";
 static const char __pyx_k_Some_problem_occured_while_tryin[] = "Some problem occured while trying to add key.";
 static const char __pyx_k_The_two_s_objects_are_not_the_sa[] = "The two %s objects are not the same type (hint: use copy_template)";
 static const char __pyx_k_Write_operation_on_read_only_fil[] = "Write operation on read-only file";
+static const char __pyx_k_data_array_cannot_be_used_for_an[] = "data_array cannot be used for an mmapped filter.";
 static const char __pyx_k_error_rate_allowable_range_0_0_1[] = "error_rate allowable range (0.0, 1.0) ";
 static const char __pyx_k_invalid_hash_seed_s_must_be_0_an[] = "invalid hash seed '%s', must be >= 0 and up to 32 bits in size";
 static const char __pyx_k_name_will_be_deprecated_in_futur[] = "name will be deprecated in future versions, use filename instead";
-static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static PyObject *__pyx_kp_u_;
 static PyObject *__pyx_kp_u_0_3f;
 static PyObject *__pyx_n_s_AUTHOR;
+static PyObject *__pyx_n_u_B;
 static PyObject *__pyx_n_s_BloomFilter;
-static PyObject *__pyx_kp_u_BloomFilter_union_line_445;
+static PyObject *__pyx_kp_u_BloomFilter_union_line_483;
 static PyObject *__pyx_kp_u_Cannot_access_name_on_an_in_memo;
 static PyObject *__pyx_kp_u_Cannot_call_copy_on_an_in_memory;
 static PyObject *__pyx_n_s_ENOENT;
 static PyObject *__pyx_n_s_F_OK;
 static PyObject *__pyx_n_u_I;
 static PyObject *__pyx_kp_u_I_O_operation_on_closed_file;
 static PyObject *__pyx_kp_u_Insufficient_permissions_for_fil;
@@ -1681,24 +1670,23 @@
 static PyObject *__pyx_n_s_O_RDWR;
 static PyObject *__pyx_n_s_PendingDeprecationWarning;
 static PyObject *__pyx_kp_u_Performs_a_set_OR_with_another_c;
 static PyObject *__pyx_n_s_R_OK;
 static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_kp_u_Some_problem_occured_while_tryin;
 static PyObject *__pyx_kp_u_The_two_s_objects_are_not_the_sa;
-static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_VERSION;
 static PyObject *__pyx_n_s_VERSION_2;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_W_OK;
 static PyObject *__pyx_kp_u_Write_operation_on_read_only_fil;
-static PyObject *__pyx_kp_u__2;
-static PyObject *__pyx_kp_u__3;
-static PyObject *__pyx_kp_u__6;
-static PyObject *__pyx_kp_u__7;
+static PyObject *__pyx_kp_u__4;
+static PyObject *__pyx_kp_u__5;
+static PyObject *__pyx_kp_u__8;
+static PyObject *__pyx_kp_u__9;
 static PyObject *__pyx_n_s_access;
 static PyObject *__pyx_n_s_add;
 static PyObject *__pyx_n_s_approx_len;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_assert_comparable;
 static PyObject *__pyx_n_s_assert_open;
 static PyObject *__pyx_n_s_assert_writable;
@@ -1716,14 +1704,16 @@
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_compress;
 static PyObject *__pyx_n_s_copy;
 static PyObject *__pyx_n_s_create;
 static PyObject *__pyx_n_u_d;
+static PyObject *__pyx_n_s_data_array;
+static PyObject *__pyx_kp_u_data_array_cannot_be_used_for_an;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_decompress;
 static PyObject *__pyx_n_s_e;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_endswith;
 static PyObject *__pyx_n_s_eno;
 static PyObject *__pyx_n_s_errno;
@@ -1736,28 +1726,27 @@
 static PyObject *__pyx_kp_u_file;
 static PyObject *__pyx_n_s_filename;
 static PyObject *__pyx_n_s_floor;
 static PyObject *__pyx_n_s_from_base64;
 static PyObject *__pyx_n_s_from_bytes;
 static PyObject *__pyx_n_s_frombytes;
 static PyObject *__pyx_n_s_getrandbits;
-static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_hash_seeds;
+static PyObject *__pyx_kp_u_hash_seeds_must_be_specified_if;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_intersection;
 static PyObject *__pyx_kp_u_invalid_hash_seed_s_must_be_0_an;
 static PyObject *__pyx_n_s_log;
 static PyObject *__pyx_n_s_log2;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_math;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_kp_u_name_will_be_deprecated_in_futur;
-static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_num_bits;
 static PyObject *__pyx_n_s_num_hashes;
 static PyObject *__pyx_kp_u_num_hashes_2;
 static PyObject *__pyx_n_s_object;
 static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_n_s_open_2;
 static PyObject *__pyx_n_s_os;
@@ -1765,23 +1754,18 @@
 static PyObject *__pyx_n_s_perm;
 static PyObject *__pyx_n_u_r;
 static PyObject *__pyx_n_s_random;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_u_rb;
 static PyObject *__pyx_n_s_read;
 static PyObject *__pyx_n_s_read_only;
-static PyObject *__pyx_n_s_reduce;
-static PyObject *__pyx_n_s_reduce_cython;
-static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_replace;
 static PyObject *__pyx_n_s_repr;
 static PyObject *__pyx_n_s_round;
 static PyObject *__pyx_n_u_rw;
-static PyObject *__pyx_n_s_setstate;
-static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shutil;
 static PyObject *__pyx_n_s_signed;
 static PyObject *__pyx_n_s_strerror;
 static PyObject *__pyx_n_s_string;
 static PyObject *__pyx_n_s_sys;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_tobytes;
@@ -1789,75 +1773,74 @@
 static PyObject *__pyx_n_s_unlink;
 static PyObject *__pyx_n_u_w;
 static PyObject *__pyx_kp_u_w_2;
 static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warnings;
 static PyObject *__pyx_n_s_write;
 static PyObject *__pyx_n_s_zlib;
-static int __pyx_pf_13pybloomfilter_11BloomFilter___cinit__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_2_create(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_4_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode); /* proto */
-static void __pyx_pf_13pybloomfilter_11BloomFilter_6__dealloc__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter___reduce__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static int __pyx_pf_13pybloomfilter_11BloomFilter_2__cinit__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds, PyObject *__pyx_v_data_array); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_4_create(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds, PyObject *__pyx_v_data_array); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_6_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode); /* proto */
+static void __pyx_pf_13pybloomfilter_11BloomFilter_8__dealloc__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_9bit_array___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10data_array___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10hash_seeds___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_8capacity___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10error_rate___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10num_hashes___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_8num_bits___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_9bit_count___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10approx_len___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_8_name(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10_name(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_4name___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_8filename___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_9read_only___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10fileno(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_12__repr__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_14__str__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_16sync(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_18clear_all(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static int __pyx_pf_13pybloomfilter_11BloomFilter_20__contains__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_22copy_template(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_24copy(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_26add(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_28update(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_iterable); /* proto */
-static Py_ssize_t __pyx_pf_13pybloomfilter_11BloomFilter_30__len__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_32close(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_34union(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_36__ior__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_38intersection(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_40__iand__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_42_assert_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_44_assert_writable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_46_assert_comparable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_48to_base64(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_50from_base64(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_string, PyObject *__pyx_v_perm); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_52open(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_54__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_56__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_12fileno(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_14__repr__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_16__str__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_18sync(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_20clear_all(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static int __pyx_pf_13pybloomfilter_11BloomFilter_22__contains__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_24copy_template(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_26copy(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_28add(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_30update(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_iterable); /* proto */
+static Py_ssize_t __pyx_pf_13pybloomfilter_11BloomFilter_32__len__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_34close(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_36union(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_38__ior__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_40intersection(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_42__iand__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_44_assert_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_46_assert_writable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_48_assert_comparable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_50to_base64(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_52from_base64(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_string, PyObject *__pyx_v_perm); /* proto */
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_54open(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode); /* proto */
 static PyObject *__pyx_tp_new_13pybloomfilter_BloomFilter(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_4;
-static PyObject *__pyx_int_5;
-static PyObject *__pyx_int_7;
+static PyObject *__pyx_int_6;
 static PyObject *__pyx_int_9;
 static PyObject *__pyx_int_32;
 static PyObject *__pyx_int_493;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 /* Late includes */
 
-/* "pybloomfilter.pyx":28
+/* "pybloomfilter.pyx":27
  * 
  * 
  * cdef _construct_access(mode):             # <<<<<<<<<<<<<<
  *     result = os.F_OK
  *     if 'w' in mode:
  */
 
@@ -1870,118 +1853,118 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_construct_access", 0);
 
-  /* "pybloomfilter.pyx":29
+  /* "pybloomfilter.pyx":28
  * 
  * cdef _construct_access(mode):
  *     result = os.F_OK             # <<<<<<<<<<<<<<
  *     if 'w' in mode:
  *         result |= os.W_OK
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_F_OK); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_F_OK); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_result = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":30
+  /* "pybloomfilter.pyx":29
  * cdef _construct_access(mode):
  *     result = os.F_OK
  *     if 'w' in mode:             # <<<<<<<<<<<<<<
  *         result |= os.W_OK
  *     if 'r' in mode:
  */
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_w, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_w, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 29, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":31
+    /* "pybloomfilter.pyx":30
  *     result = os.F_OK
  *     if 'w' in mode:
  *         result |= os.W_OK             # <<<<<<<<<<<<<<
  *     if 'r' in mode:
  *         result |= os.R_OK
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_W_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_W_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":30
+    /* "pybloomfilter.pyx":29
  * cdef _construct_access(mode):
  *     result = os.F_OK
  *     if 'w' in mode:             # <<<<<<<<<<<<<<
  *         result |= os.W_OK
  *     if 'r' in mode:
  */
   }
 
-  /* "pybloomfilter.pyx":32
+  /* "pybloomfilter.pyx":31
  *     if 'w' in mode:
  *         result |= os.W_OK
  *     if 'r' in mode:             # <<<<<<<<<<<<<<
  *         result |= os.R_OK
  *     return result
  */
-  __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_r, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_r, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 31, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_4 != 0);
   if (__pyx_t_3) {
 
-    /* "pybloomfilter.pyx":33
+    /* "pybloomfilter.pyx":32
  *         result |= os.W_OK
  *     if 'r' in mode:
  *         result |= os.R_OK             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_R_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_R_OK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":32
+    /* "pybloomfilter.pyx":31
  *     if 'w' in mode:
  *         result |= os.W_OK
  *     if 'r' in mode:             # <<<<<<<<<<<<<<
  *         result |= os.R_OK
  *     return result
  */
   }
 
-  /* "pybloomfilter.pyx":34
+  /* "pybloomfilter.pyx":33
  *     if 'r' in mode:
  *         result |= os.R_OK
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":28
+  /* "pybloomfilter.pyx":27
  * 
  * 
  * cdef _construct_access(mode):             # <<<<<<<<<<<<<<
  *     result = os.F_OK
  *     if 'w' in mode:
  */
 
@@ -1994,15 +1977,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":37
+/* "pybloomfilter.pyx":36
  * 
  * 
  * cdef _construct_mode(mode):             # <<<<<<<<<<<<<<
  *     result = os.O_RDONLY
  *     if 'w' in mode:
  */
 
@@ -2017,185 +2000,185 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_construct_mode", 0);
 
-  /* "pybloomfilter.pyx":38
+  /* "pybloomfilter.pyx":37
  * 
  * cdef _construct_mode(mode):
  *     result = os.O_RDONLY             # <<<<<<<<<<<<<<
  *     if 'w' in mode:
  *         result |= os.O_RDWR
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_O_RDONLY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_O_RDONLY); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_result = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":39
+  /* "pybloomfilter.pyx":38
  * cdef _construct_mode(mode):
  *     result = os.O_RDONLY
  *     if 'w' in mode:             # <<<<<<<<<<<<<<
  *         result |= os.O_RDWR
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):
  */
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_w, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_w, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":40
+    /* "pybloomfilter.pyx":39
  *     result = os.O_RDONLY
  *     if 'w' in mode:
  *         result |= os.O_RDWR             # <<<<<<<<<<<<<<
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):
  *         result |= os.O_BINARY
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_O_RDWR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_O_RDWR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":39
+    /* "pybloomfilter.pyx":38
  * cdef _construct_mode(mode):
  *     result = os.O_RDONLY
  *     if 'w' in mode:             # <<<<<<<<<<<<<<
  *         result |= os.O_RDWR
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):
  */
   }
 
-  /* "pybloomfilter.pyx":41
+  /* "pybloomfilter.pyx":40
  *     if 'w' in mode:
  *         result |= os.O_RDWR
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):             # <<<<<<<<<<<<<<
  *         result |= os.O_BINARY
  *     if mode.endswith('+'):
  */
-  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_b, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_b, __pyx_v_mode, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 40, __pyx_L1_error)
   __pyx_t_5 = (__pyx_t_3 != 0);
   if (__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L5_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_HasAttr(__pyx_t_2, __pyx_n_u_O_BINARY); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_HasAttr(__pyx_t_2, __pyx_n_u_O_BINARY); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_3 = (__pyx_t_5 != 0);
   __pyx_t_4 = __pyx_t_3;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":42
+    /* "pybloomfilter.pyx":41
  *         result |= os.O_RDWR
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):
  *         result |= os.O_BINARY             # <<<<<<<<<<<<<<
  *     if mode.endswith('+'):
  *         result |= os.O_CREAT
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_O_BINARY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_O_BINARY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":41
+    /* "pybloomfilter.pyx":40
  *     if 'w' in mode:
  *         result |= os.O_RDWR
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):             # <<<<<<<<<<<<<<
  *         result |= os.O_BINARY
  *     if mode.endswith('+'):
  */
   }
 
-  /* "pybloomfilter.pyx":43
+  /* "pybloomfilter.pyx":42
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):
  *         result |= os.O_BINARY
  *     if mode.endswith('+'):             # <<<<<<<<<<<<<<
  *         result |= os.O_CREAT
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_endswith); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_endswith); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_kp_u_) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":44
+    /* "pybloomfilter.pyx":43
  *         result |= os.O_BINARY
  *     if mode.endswith('+'):
  *         result |= os.O_CREAT             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_O_CREAT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_O_CREAT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceOr(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":43
+    /* "pybloomfilter.pyx":42
  *     if 'b' in mode and hasattr(os, 'O_BINARY'):
  *         result |= os.O_BINARY
  *     if mode.endswith('+'):             # <<<<<<<<<<<<<<
  *         result |= os.O_CREAT
  *     return result
  */
   }
 
-  /* "pybloomfilter.pyx":45
+  /* "pybloomfilter.pyx":44
  *     if mode.endswith('+'):
  *         result |= os.O_CREAT
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":37
+  /* "pybloomfilter.pyx":36
  * 
  * 
  * cdef _construct_mode(mode):             # <<<<<<<<<<<<<<
  *     result = os.O_RDONLY
  *     if 'w' in mode:
  */
 
@@ -2209,46 +2192,180 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":83
+/* "pybloomfilter.pyx":85
+ *     cdef int _oflags
+ * 
+ *     def __reduce__(self):             # <<<<<<<<<<<<<<
+ *         """Makes an in-memory BloomFilter pickleable."""
+ *         callable = BloomFilter
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_1__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter___reduce__[] = "Makes an in-memory BloomFilter pickleable.";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_1__reduce__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter___reduce__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter___reduce__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+  PyTypeObject *__pyx_v_callable = NULL;
+  PyObject *__pyx_v_args = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce__", 0);
+
+  /* "pybloomfilter.pyx":87
+ *     def __reduce__(self):
+ *         """Makes an in-memory BloomFilter pickleable."""
+ *         callable = BloomFilter             # <<<<<<<<<<<<<<
+ *         args = (self.capacity, self.error_rate, None, None, self.hash_seeds, self.data_array)
+ *         return (callable, args)
+ */
+  __Pyx_INCREF(((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter));
+  __pyx_v_callable = __pyx_ptype_13pybloomfilter_BloomFilter;
+
+  /* "pybloomfilter.pyx":88
+ *         """Makes an in-memory BloomFilter pickleable."""
+ *         callable = BloomFilter
+ *         args = (self.capacity, self.error_rate, None, None, self.hash_seeds, self.data_array)             # <<<<<<<<<<<<<<
+ *         return (callable, args)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_capacity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_hash_seeds); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_data_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  PyTuple_SET_ITEM(__pyx_t_5, 2, Py_None);
+  __Pyx_INCREF(Py_None);
+  __Pyx_GIVEREF(Py_None);
+  PyTuple_SET_ITEM(__pyx_t_5, 3, Py_None);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_5, 4, __pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 5, __pyx_t_4);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_4 = 0;
+  __pyx_v_args = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
+
+  /* "pybloomfilter.pyx":89
+ *         callable = BloomFilter
+ *         args = (self.capacity, self.error_rate, None, None, self.hash_seeds, self.data_array)
+ *         return (callable, args)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_INCREF(((PyObject *)__pyx_v_callable));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_callable));
+  PyTuple_SET_ITEM(__pyx_t_5, 0, ((PyObject *)__pyx_v_callable));
+  __Pyx_INCREF(__pyx_v_args);
+  __Pyx_GIVEREF(__pyx_v_args);
+  PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_args);
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "pybloomfilter.pyx":85
  *     cdef int _oflags
  * 
- *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):             # <<<<<<<<<<<<<<
+ *     def __reduce__(self):             # <<<<<<<<<<<<<<
+ *         """Makes an in-memory BloomFilter pickleable."""
+ *         callable = BloomFilter
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("pybloomfilter.BloomFilter.__reduce__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_callable);
+  __Pyx_XDECREF(__pyx_v_args);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pybloomfilter.pyx":92
+ * 
+ * 
+ *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):             # <<<<<<<<<<<<<<
  *         self._closed = 0
  *         self._in_memory = 0
  */
 
 /* Python wrapper */
-static int __pyx_pw_13pybloomfilter_11BloomFilter_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_13pybloomfilter_11BloomFilter_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_13pybloomfilter_11BloomFilter_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_13pybloomfilter_11BloomFilter_3__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_capacity = 0;
   PyObject *__pyx_v_error_rate = 0;
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_perm = 0;
   PyObject *__pyx_v_hash_seeds = 0;
+  PyObject *__pyx_v_data_array = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_capacity,&__pyx_n_s_error_rate,&__pyx_n_s_filename,&__pyx_n_s_perm,&__pyx_n_s_hash_seeds,0};
-    PyObject* values[5] = {0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_capacity,&__pyx_n_s_error_rate,&__pyx_n_s_filename,&__pyx_n_s_perm,&__pyx_n_s_hash_seeds,&__pyx_n_s_data_array,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
     values[2] = ((PyObject *)Py_None);
     values[3] = ((PyObject *)__pyx_int_493);
     values[4] = ((PyObject *)Py_None);
+    values[5] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -2263,15 +2380,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_capacity)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_rate)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 5, 1); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 6, 1); __PYX_ERR(0, 92, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -2283,20 +2400,28 @@
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hash_seeds);
           if (value) { values[4] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data_array);
+          if (value) { values[5] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -2306,117 +2431,118 @@
       }
     }
     __pyx_v_capacity = values[0];
     __pyx_v_error_rate = values[1];
     __pyx_v_filename = values[2];
     __pyx_v_perm = values[3];
     __pyx_v_hash_seeds = values[4];
+    __pyx_v_data_array = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 83, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 92, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybloomfilter.BloomFilter.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter___cinit__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_2__cinit__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds, __pyx_v_data_array);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_13pybloomfilter_11BloomFilter___cinit__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds) {
+static int __pyx_pf_13pybloomfilter_11BloomFilter_2__cinit__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds, PyObject *__pyx_v_data_array) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "pybloomfilter.pyx":84
+  /* "pybloomfilter.pyx":93
  * 
- *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):
+ *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):
  *         self._closed = 0             # <<<<<<<<<<<<<<
  *         self._in_memory = 0
  *         self._oflags = os.O_RDWR
  */
   __pyx_v_self->_closed = 0;
 
-  /* "pybloomfilter.pyx":85
- *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):
+  /* "pybloomfilter.pyx":94
+ *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):
  *         self._closed = 0
  *         self._in_memory = 0             # <<<<<<<<<<<<<<
  *         self._oflags = os.O_RDWR
  * 
  */
   __pyx_v_self->_in_memory = 0;
 
-  /* "pybloomfilter.pyx":86
+  /* "pybloomfilter.pyx":95
  *         self._closed = 0
  *         self._in_memory = 0
  *         self._oflags = os.O_RDWR             # <<<<<<<<<<<<<<
  * 
  *         if capacity is NoConstruct:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_O_RDWR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_O_RDWR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_self->_oflags = __pyx_t_3;
 
-  /* "pybloomfilter.pyx":88
+  /* "pybloomfilter.pyx":97
  *         self._oflags = os.O_RDWR
  * 
  *         if capacity is NoConstruct:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   __pyx_t_4 = (__pyx_v_capacity == __pyx_v_13pybloomfilter_NoConstruct);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "pybloomfilter.pyx":89
+    /* "pybloomfilter.pyx":98
  * 
  *         if capacity is NoConstruct:
  *             return             # <<<<<<<<<<<<<<
  * 
- *         self._create(capacity, error_rate, filename, perm, hash_seeds)
+ *         self._create(capacity, error_rate, filename, perm, hash_seeds, data_array)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "pybloomfilter.pyx":88
+    /* "pybloomfilter.pyx":97
  *         self._oflags = os.O_RDWR
  * 
  *         if capacity is NoConstruct:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   }
 
-  /* "pybloomfilter.pyx":91
+  /* "pybloomfilter.pyx":100
  *             return
  * 
- *         self._create(capacity, error_rate, filename, perm, hash_seeds)             # <<<<<<<<<<<<<<
+ *         self._create(capacity, error_rate, filename, perm, hash_seeds, data_array)             # <<<<<<<<<<<<<<
+ * 
  * 
- *     def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_create); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_create); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = NULL;
   __pyx_t_3 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -2424,30 +2550,30 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_3 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_6, __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_3, 5+__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+    PyObject *__pyx_temp[7] = {__pyx_t_6, __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds, __pyx_v_data_array};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_3, 6+__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_2);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_6, __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_3, 5+__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+    PyObject *__pyx_temp[7] = {__pyx_t_6, __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds, __pyx_v_data_array};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_3, 6+__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_2);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(5+__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(6+__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_v_capacity);
     __Pyx_GIVEREF(__pyx_v_capacity);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_3, __pyx_v_capacity);
@@ -2459,25 +2585,28 @@
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_3, __pyx_v_filename);
     __Pyx_INCREF(__pyx_v_perm);
     __Pyx_GIVEREF(__pyx_v_perm);
     PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_3, __pyx_v_perm);
     __Pyx_INCREF(__pyx_v_hash_seeds);
     __Pyx_GIVEREF(__pyx_v_hash_seeds);
     PyTuple_SET_ITEM(__pyx_t_7, 4+__pyx_t_3, __pyx_v_hash_seeds);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __Pyx_INCREF(__pyx_v_data_array);
+    __Pyx_GIVEREF(__pyx_v_data_array);
+    PyTuple_SET_ITEM(__pyx_t_7, 5+__pyx_t_3, __pyx_v_data_array);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":83
- *     cdef int _oflags
+  /* "pybloomfilter.pyx":92
  * 
- *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):             # <<<<<<<<<<<<<<
+ * 
+ *     def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):             # <<<<<<<<<<<<<<
  *         self._closed = 0
  *         self._in_memory = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -2489,46 +2618,50 @@
   __Pyx_AddTraceback("pybloomfilter.BloomFilter.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":93
- *         self._create(capacity, error_rate, filename, perm, hash_seeds)
+/* "pybloomfilter.pyx":103
+ * 
  * 
- *     def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):             # <<<<<<<<<<<<<<
+ *     def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):             # <<<<<<<<<<<<<<
  *         cdef char * seeds
- *         cdef long long num_bits
+ *         cdef char * data = NULL
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_3_create(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_3_create(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_5_create(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_5_create(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_capacity = 0;
   PyObject *__pyx_v_error_rate = 0;
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_perm = 0;
   PyObject *__pyx_v_hash_seeds = 0;
+  PyObject *__pyx_v_data_array = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_create (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_capacity,&__pyx_n_s_error_rate,&__pyx_n_s_filename,&__pyx_n_s_perm,&__pyx_n_s_hash_seeds,0};
-    PyObject* values[5] = {0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_capacity,&__pyx_n_s_error_rate,&__pyx_n_s_filename,&__pyx_n_s_perm,&__pyx_n_s_hash_seeds,&__pyx_n_s_data_array,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
     values[2] = ((PyObject *)Py_None);
     values[3] = ((PyObject *)__pyx_int_493);
     values[4] = ((PyObject *)Py_None);
+    values[5] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -2543,15 +2676,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_capacity)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_error_rate)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_create", 0, 2, 5, 1); __PYX_ERR(0, 93, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_create", 0, 2, 6, 1); __PYX_ERR(0, 103, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -2563,20 +2696,28 @@
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hash_seeds);
           if (value) { values[4] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data_array);
+          if (value) { values[5] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_create") < 0)) __PYX_ERR(0, 93, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_create") < 0)) __PYX_ERR(0, 103, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
@@ -2586,32 +2727,34 @@
       }
     }
     __pyx_v_capacity = values[0];
     __pyx_v_error_rate = values[1];
     __pyx_v_filename = values[2];
     __pyx_v_perm = values[3];
     __pyx_v_hash_seeds = values[4];
+    __pyx_v_data_array = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_create", 0, 2, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 93, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_create", 0, 2, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 103, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybloomfilter.BloomFilter._create", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_2_create(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_4_create(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_capacity, __pyx_v_error_rate, __pyx_v_filename, __pyx_v_perm, __pyx_v_hash_seeds, __pyx_v_data_array);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_2_create(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_4_create(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_capacity, PyObject *__pyx_v_error_rate, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm, PyObject *__pyx_v_hash_seeds, PyObject *__pyx_v_data_array) {
   char *__pyx_v_seeds;
+  char *__pyx_v_data;
   PY_LONG_LONG __pyx_v_num_bits;
   PyObject *__pyx_v_array_seeds = NULL;
   PyObject *__pyx_v_seed = NULL;
   PyObject *__pyx_v_num_hashes = NULL;
   PyObject *__pyx_v_test = NULL;
   PyObject *__pyx_v_bits_per_hash = NULL;
   CYTHON_UNUSED PyObject *__pyx_7genexpr__pyx_v_i = NULL;
@@ -2639,402 +2782,496 @@
   Py_UCS4 __pyx_t_20;
   PyObject *__pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_create", 0);
 
-  /* "pybloomfilter.pyx":99
+  /* "pybloomfilter.pyx":105
+ *     def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):
+ *         cdef char * seeds
+ *         cdef char * data = NULL             # <<<<<<<<<<<<<<
+ *         cdef long long num_bits
+ * 
+ */
+  __pyx_v_data = NULL;
+
+  /* "pybloomfilter.pyx":108
+ *         cdef long long num_bits
+ * 
+ *         if data_array is not None:             # <<<<<<<<<<<<<<
+ *             if filename:
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ */
+  __pyx_t_1 = (__pyx_v_data_array != Py_None);
+  __pyx_t_2 = (__pyx_t_1 != 0);
+  if (__pyx_t_2) {
+
+    /* "pybloomfilter.pyx":109
+ * 
+ *         if data_array is not None:
+ *             if filename:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ *             if hash_seeds is None:
+ */
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 109, __pyx_L1_error)
+    if (unlikely(__pyx_t_2)) {
+
+      /* "pybloomfilter.pyx":110
+ *         if data_array is not None:
+ *             if filename:
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")             # <<<<<<<<<<<<<<
+ *             if hash_seeds is None:
+ *                 raise ValueError("hash_seeds must be specified if a data_array is provided.")
+ */
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __PYX_ERR(0, 110, __pyx_L1_error)
+
+      /* "pybloomfilter.pyx":109
+ * 
+ *         if data_array is not None:
+ *             if filename:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ *             if hash_seeds is None:
+ */
+    }
+
+    /* "pybloomfilter.pyx":111
+ *             if filename:
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ *             if hash_seeds is None:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("hash_seeds must be specified if a data_array is provided.")
+ * 
+ */
+    __pyx_t_2 = (__pyx_v_hash_seeds == Py_None);
+    __pyx_t_1 = (__pyx_t_2 != 0);
+    if (unlikely(__pyx_t_1)) {
+
+      /* "pybloomfilter.pyx":112
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ *             if hash_seeds is None:
+ *                 raise ValueError("hash_seeds must be specified if a data_array is provided.")             # <<<<<<<<<<<<<<
+ * 
+ *         # Make sure that if the filename is defined, that the
+ */
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __PYX_ERR(0, 112, __pyx_L1_error)
+
+      /* "pybloomfilter.pyx":111
+ *             if filename:
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ *             if hash_seeds is None:             # <<<<<<<<<<<<<<
+ *                 raise ValueError("hash_seeds must be specified if a data_array is provided.")
+ * 
+ */
+    }
+
+    /* "pybloomfilter.pyx":108
+ *         cdef long long num_bits
+ * 
+ *         if data_array is not None:             # <<<<<<<<<<<<<<
+ *             if filename:
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ */
+  }
+
+  /* "pybloomfilter.pyx":116
  *         # Make sure that if the filename is defined, that the
  *         # file exists
  *         if filename and os.path.exists(filename):             # <<<<<<<<<<<<<<
  *             os.unlink(filename)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
   if (__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
-    goto __pyx_L4_bool_binop_done;
+    goto __pyx_L7_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_path); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exists); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_filename);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_1 = __pyx_t_2;
-  __pyx_L4_bool_binop_done:;
+  __pyx_L7_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "pybloomfilter.pyx":100
+    /* "pybloomfilter.pyx":117
  *         # file exists
  *         if filename and os.path.exists(filename):
  *             os.unlink(filename)             # <<<<<<<<<<<<<<
  * 
  *         # For why we round down for determining the number of hashes:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 117, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unlink); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_unlink); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 117, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_filename);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pybloomfilter.pyx":99
+    /* "pybloomfilter.pyx":116
  *         # Make sure that if the filename is defined, that the
  *         # file exists
  *         if filename and os.path.exists(filename):             # <<<<<<<<<<<<<<
  *             os.unlink(filename)
  * 
  */
   }
 
-  /* "pybloomfilter.pyx":112
+  /* "pybloomfilter.pyx":129
  *         # hashes is fractional)."
  * 
  *         if not (0 < error_rate < 1):             # <<<<<<<<<<<<<<
  *             raise ValueError("error_rate allowable range (0.0, 1.0) %f" % (error_rate,))
  * 
  */
-  __pyx_t_3 = PyObject_RichCompare(__pyx_int_0, __pyx_v_error_rate, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_int_0, __pyx_v_error_rate, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_3)) {
     __Pyx_DECREF(__pyx_t_3);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_error_rate, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_error_rate, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "pybloomfilter.pyx":113
+    /* "pybloomfilter.pyx":130
  * 
  *         if not (0 < error_rate < 1):
  *             raise ValueError("error_rate allowable range (0.0, 1.0) %f" % (error_rate,))             # <<<<<<<<<<<<<<
  * 
  *         array_seeds = array.array('I')
  */
-    __pyx_t_3 = __Pyx_PyObject_Format(__pyx_v_error_rate, __pyx_n_u_f); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Format(__pyx_v_error_rate, __pyx_n_u_f); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_error_rate_allowable_range_0_0_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_error_rate_allowable_range_0_0_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 113, __pyx_L1_error)
+    __PYX_ERR(0, 130, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":112
+    /* "pybloomfilter.pyx":129
  *         # hashes is fractional)."
  * 
  *         if not (0 < error_rate < 1):             # <<<<<<<<<<<<<<
  *             raise ValueError("error_rate allowable range (0.0, 1.0) %f" % (error_rate,))
  * 
  */
   }
 
-  /* "pybloomfilter.pyx":115
+  /* "pybloomfilter.pyx":132
  *             raise ValueError("error_rate allowable range (0.0, 1.0) %f" % (error_rate,))
  * 
  *         array_seeds = array.array('I')             # <<<<<<<<<<<<<<
  * 
  *         if hash_seeds:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_array); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_u_I) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_I);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_array_seeds = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pybloomfilter.pyx":117
+  /* "pybloomfilter.pyx":134
  *         array_seeds = array.array('I')
  * 
  *         if hash_seeds:             # <<<<<<<<<<<<<<
  *             for seed in hash_seeds:
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_hash_seeds); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_hash_seeds); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "pybloomfilter.pyx":118
+    /* "pybloomfilter.pyx":135
  * 
  *         if hash_seeds:
  *             for seed in hash_seeds:             # <<<<<<<<<<<<<<
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "
  */
     if (likely(PyList_CheckExact(__pyx_v_hash_seeds)) || PyTuple_CheckExact(__pyx_v_hash_seeds)) {
       __pyx_t_3 = __pyx_v_hash_seeds; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_hash_seeds); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 118, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_hash_seeds); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 118, __pyx_L1_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 135, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_7(__pyx_t_3);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 118, __pyx_L1_error)
+            else __PYX_ERR(0, 135, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v_seed, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "pybloomfilter.pyx":119
+      /* "pybloomfilter.pyx":136
  *         if hash_seeds:
  *             for seed in hash_seeds:
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:             # <<<<<<<<<<<<<<
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "
  *                                         "and up to 32 bits in size" % seed)
  */
       __pyx_t_1 = PyInt_Check(__pyx_v_seed); 
       __pyx_t_8 = ((!(__pyx_t_1 != 0)) != 0);
       if (!__pyx_t_8) {
       } else {
         __pyx_t_2 = __pyx_t_8;
-        goto __pyx_L11_bool_binop_done;
+        goto __pyx_L14_bool_binop_done;
       }
-      __pyx_t_4 = PyObject_RichCompare(__pyx_v_seed, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
-      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 119, __pyx_L1_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_v_seed, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (!__pyx_t_8) {
       } else {
         __pyx_t_2 = __pyx_t_8;
-        goto __pyx_L11_bool_binop_done;
+        goto __pyx_L14_bool_binop_done;
       }
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_seed, __pyx_n_s_bit_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_seed, __pyx_n_s_bit_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_int_32, Py_GT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 119, __pyx_L1_error)
+      __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_int_32, Py_GT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 119, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_2 = __pyx_t_8;
-      __pyx_L11_bool_binop_done:;
+      __pyx_L14_bool_binop_done:;
       if (unlikely(__pyx_t_2)) {
 
-        /* "pybloomfilter.pyx":121
+        /* "pybloomfilter.pyx":138
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "
  *                                         "and up to 32 bits in size" % seed)             # <<<<<<<<<<<<<<
  *             num_hashes = len(hash_seeds)
  *             array_seeds.extend(hash_seeds)
  */
-        __pyx_t_5 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_invalid_hash_seed_s_must_be_0_an, __pyx_v_seed); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_invalid_hash_seed_s_must_be_0_an, __pyx_v_seed); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
 
-        /* "pybloomfilter.pyx":120
+        /* "pybloomfilter.pyx":137
  *             for seed in hash_seeds:
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "             # <<<<<<<<<<<<<<
  *                                         "and up to 32 bits in size" % seed)
  *             num_hashes = len(hash_seeds)
  */
-        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_Raise(__pyx_t_4, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __PYX_ERR(0, 120, __pyx_L1_error)
+        __PYX_ERR(0, 137, __pyx_L1_error)
 
-        /* "pybloomfilter.pyx":119
+        /* "pybloomfilter.pyx":136
  *         if hash_seeds:
  *             for seed in hash_seeds:
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:             # <<<<<<<<<<<<<<
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "
  *                                         "and up to 32 bits in size" % seed)
  */
       }
 
-      /* "pybloomfilter.pyx":118
+      /* "pybloomfilter.pyx":135
  * 
  *         if hash_seeds:
  *             for seed in hash_seeds:             # <<<<<<<<<<<<<<
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pybloomfilter.pyx":122
+    /* "pybloomfilter.pyx":139
  *                     raise ValueError("invalid hash seed '%s', must be >= 0 "
  *                                         "and up to 32 bits in size" % seed)
  *             num_hashes = len(hash_seeds)             # <<<<<<<<<<<<<<
  *             array_seeds.extend(hash_seeds)
  *         else:
  */
-    __pyx_t_6 = PyObject_Length(__pyx_v_hash_seeds); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 122, __pyx_L1_error)
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_hash_seeds); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 139, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_num_hashes = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "pybloomfilter.pyx":123
+    /* "pybloomfilter.pyx":140
  *                                         "and up to 32 bits in size" % seed)
  *             num_hashes = len(hash_seeds)
  *             array_seeds.extend(hash_seeds)             # <<<<<<<<<<<<<<
  *         else:
  *             num_hashes = max(math.floor(math.log2(1 / error_rate)), 1)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_array_seeds, __pyx_n_s_extend); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_array_seeds, __pyx_n_s_extend); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_hash_seeds) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_hash_seeds);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pybloomfilter.pyx":117
+    /* "pybloomfilter.pyx":134
  *         array_seeds = array.array('I')
  * 
  *         if hash_seeds:             # <<<<<<<<<<<<<<
  *             for seed in hash_seeds:
  *                 if not isinstance(seed, int) or seed < 0 or seed.bit_length() > 32:
  */
-    goto __pyx_L7;
+    goto __pyx_L10;
   }
 
-  /* "pybloomfilter.pyx":125
+  /* "pybloomfilter.pyx":142
  *             array_seeds.extend(hash_seeds)
  *         else:
  *             num_hashes = max(math.floor(math.log2(1 / error_rate)), 1)             # <<<<<<<<<<<<<<
  *             array_seeds.extend([random.getrandbits(32) for i in range(num_hashes)])
  * 
  */
   /*else*/ {
     __pyx_t_10 = 1;
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_math); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_math); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_floor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_floor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_math); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_math); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_log2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_log2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyNumber_Divide(__pyx_int_1, __pyx_v_error_rate); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyNumber_Divide(__pyx_int_1, __pyx_v_error_rate); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_12 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_12)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_4 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_9);
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_11 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_11)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -3042,272 +3279,272 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_11, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_11 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_11 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_11); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_11); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     if (__pyx_t_2) {
-      __pyx_t_11 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 142, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_5 = __pyx_t_11;
       __pyx_t_11 = 0;
     } else {
       __Pyx_INCREF(__pyx_t_3);
       __pyx_t_5 = __pyx_t_3;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __pyx_t_5;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_num_hashes = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "pybloomfilter.pyx":126
+    /* "pybloomfilter.pyx":143
  *         else:
  *             num_hashes = max(math.floor(math.log2(1 / error_rate)), 1)
  *             array_seeds.extend([random.getrandbits(32) for i in range(num_hashes)])             # <<<<<<<<<<<<<<
  * 
  *         test = array_seeds.tobytes()
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_array_seeds, __pyx_n_s_extend); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_array_seeds, __pyx_n_s_extend); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     { /* enter inner scope */
-      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L16_error)
+      __pyx_t_11 = PyList_New(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 143, __pyx_L19_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_num_hashes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L16_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_num_hashes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L19_error)
       __Pyx_GOTREF(__pyx_t_4);
       if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
         __pyx_t_9 = __pyx_t_4; __Pyx_INCREF(__pyx_t_9); __pyx_t_6 = 0;
         __pyx_t_7 = NULL;
       } else {
-        __pyx_t_6 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 126, __pyx_L16_error)
+        __pyx_t_6 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 143, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_7 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 126, __pyx_L16_error)
+        __pyx_t_7 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L19_error)
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       for (;;) {
         if (likely(!__pyx_t_7)) {
           if (likely(PyList_CheckExact(__pyx_t_9))) {
             if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_9)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 126, __pyx_L16_error)
+            __pyx_t_4 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 143, __pyx_L19_error)
             #else
-            __pyx_t_4 = PySequence_ITEM(__pyx_t_9, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L16_error)
+            __pyx_t_4 = PySequence_ITEM(__pyx_t_9, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
           } else {
             if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_9)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 126, __pyx_L16_error)
+            __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 143, __pyx_L19_error)
             #else
-            __pyx_t_4 = PySequence_ITEM(__pyx_t_9, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L16_error)
+            __pyx_t_4 = PySequence_ITEM(__pyx_t_9, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_4);
             #endif
           }
         } else {
           __pyx_t_4 = __pyx_t_7(__pyx_t_9);
           if (unlikely(!__pyx_t_4)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 126, __pyx_L16_error)
+              else __PYX_ERR(0, 143, __pyx_L19_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_4);
         }
         __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_i, __pyx_t_4);
         __pyx_t_4 = 0;
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_random); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 126, __pyx_L16_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_random); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 143, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_getrandbits); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 126, __pyx_L16_error)
+        __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_getrandbits); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 143, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
           __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
           if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_13, function);
           }
         }
         __pyx_t_4 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_12, __pyx_int_32) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_int_32);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L16_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 126, __pyx_L16_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_11, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 143, __pyx_L19_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_i); __pyx_7genexpr__pyx_v_i = 0;
-      goto __pyx_L19_exit_scope;
-      __pyx_L16_error:;
+      goto __pyx_L22_exit_scope;
+      __pyx_L19_error:;
       __Pyx_XDECREF(__pyx_7genexpr__pyx_v_i); __pyx_7genexpr__pyx_v_i = 0;
       goto __pyx_L1_error;
-      __pyx_L19_exit_scope:;
+      __pyx_L22_exit_scope:;
     } /* exit inner scope */
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_9, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_11);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_L7:;
+  __pyx_L10:;
 
-  /* "pybloomfilter.pyx":128
+  /* "pybloomfilter.pyx":145
  *             array_seeds.extend([random.getrandbits(32) for i in range(num_hashes)])
  * 
  *         test = array_seeds.tobytes()             # <<<<<<<<<<<<<<
  *         seeds = test
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_array_seeds, __pyx_n_s_tobytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_array_seeds, __pyx_n_s_tobytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_test = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pybloomfilter.pyx":129
+  /* "pybloomfilter.pyx":146
  * 
  *         test = array_seeds.tobytes()
  *         seeds = test             # <<<<<<<<<<<<<<
  * 
  *         bits_per_hash = math.ceil(
  */
-  __pyx_t_14 = __Pyx_PyObject_AsWritableString(__pyx_v_test); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_14 = __Pyx_PyObject_AsWritableString(__pyx_v_test); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L1_error)
   __pyx_v_seeds = __pyx_t_14;
 
-  /* "pybloomfilter.pyx":131
+  /* "pybloomfilter.pyx":148
  *         seeds = test
  * 
  *         bits_per_hash = math.ceil(             # <<<<<<<<<<<<<<
  *                 capacity * abs(math.log(error_rate)) /
  *                 (num_hashes * (math.log(2) ** 2)))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_math); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_math); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ceil); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_ceil); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pybloomfilter.pyx":132
+  /* "pybloomfilter.pyx":149
  * 
  *         bits_per_hash = math.ceil(
  *                 capacity * abs(math.log(error_rate)) /             # <<<<<<<<<<<<<<
  *                 (num_hashes * (math.log(2) ** 2)))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_math); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_math); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_log); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_log); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_9, __pyx_v_error_rate) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_error_rate);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyNumber_Absolute(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyNumber_Absolute(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_Multiply(__pyx_v_capacity, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Multiply(__pyx_v_capacity, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pybloomfilter.pyx":133
+  /* "pybloomfilter.pyx":150
  *         bits_per_hash = math.ceil(
  *                 capacity * abs(math.log(error_rate)) /
  *                 (num_hashes * (math.log(2) ** 2)))             # <<<<<<<<<<<<<<
  * 
  *         # Minimum bit vector of 128 bits
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_math); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_math); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_log); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_log); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_13);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_13, function);
     }
   }
   __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_9, __pyx_int_2) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_int_2);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_13 = PyNumber_Power(__pyx_t_4, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_13 = PyNumber_Power(__pyx_t_4, __pyx_int_2, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Multiply(__pyx_v_num_hashes, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_v_num_hashes, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
 
-  /* "pybloomfilter.pyx":132
+  /* "pybloomfilter.pyx":149
  * 
  *         bits_per_hash = math.ceil(
  *                 capacity * abs(math.log(error_rate)) /             # <<<<<<<<<<<<<<
  *                 (num_hashes * (math.log(2) ** 2)))
  * 
  */
-  __pyx_t_13 = __Pyx_PyNumber_Divide(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyNumber_Divide(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_11);
     if (likely(__pyx_t_4)) {
@@ -3316,355 +3553,415 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_11, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_4, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_13);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __pyx_v_bits_per_hash = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pybloomfilter.pyx":136
+  /* "pybloomfilter.pyx":153
  * 
  *         # Minimum bit vector of 128 bits
  *         num_bits = max(num_hashes * bits_per_hash,128)             # <<<<<<<<<<<<<<
  * 
- *         # print("k = %d  m = %d  n = %d   p ~= %.8f" % (
+ *         # Override calculated capacity if we are provided a data array
  */
   __pyx_t_10 = 0x80;
-  __pyx_t_3 = PyNumber_Multiply(__pyx_v_num_hashes, __pyx_v_bits_per_hash); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_v_num_hashes, __pyx_v_bits_per_hash); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_13 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_13, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_13, __pyx_t_3, Py_GT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_2) {
-    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_11 = __pyx_t_4;
     __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_3);
     __pyx_t_11 = __pyx_t_3;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_15 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_11); if (unlikely((__pyx_t_15 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_11); if (unlikely((__pyx_t_15 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __pyx_v_num_bits = __pyx_t_15;
 
-  /* "pybloomfilter.pyx":145
+  /* "pybloomfilter.pyx":156
+ * 
+ *         # Override calculated capacity if we are provided a data array
+ *         if data_array is not None:             # <<<<<<<<<<<<<<
+ *             num_bits = 8 * len(data_array)
+ * 
+ */
+  __pyx_t_2 = (__pyx_v_data_array != Py_None);
+  __pyx_t_8 = (__pyx_t_2 != 0);
+  if (__pyx_t_8) {
+
+    /* "pybloomfilter.pyx":157
+ *         # Override calculated capacity if we are provided a data array
+ *         if data_array is not None:
+ *             num_bits = 8 * len(data_array)             # <<<<<<<<<<<<<<
+ * 
+ *         # print("k = %d  m = %d  n = %d   p ~= %.8f" % (
+ */
+    __pyx_t_6 = PyObject_Length(__pyx_v_data_array); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_v_num_bits = (8 * __pyx_t_6);
+
+    /* "pybloomfilter.pyx":156
+ * 
+ *         # Override calculated capacity if we are provided a data array
+ *         if data_array is not None:             # <<<<<<<<<<<<<<
+ *             num_bits = 8 * len(data_array)
+ * 
+ */
+  }
+
+  /* "pybloomfilter.pyx":166
  *         # If a filename is provided, we should make a mmap-file
  *         # backed bloom filter. Otherwise, it will be malloc
  *         if filename:             # <<<<<<<<<<<<<<
  *             self._bf = cbloomfilter.bloomfilter_Create_Mmap(capacity,
  *                                                     error_rate,
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
-  if (__pyx_t_2) {
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
+  if (__pyx_t_8) {
 
-    /* "pybloomfilter.pyx":146
+    /* "pybloomfilter.pyx":167
  *         # backed bloom filter. Otherwise, it will be malloc
  *         if filename:
  *             self._bf = cbloomfilter.bloomfilter_Create_Mmap(capacity,             # <<<<<<<<<<<<<<
  *                                                     error_rate,
  *                                                     filename.encode(),
  */
-    __pyx_t_10 = __Pyx_PyInt_As_long(__pyx_v_capacity); if (unlikely((__pyx_t_10 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_long(__pyx_v_capacity); if (unlikely((__pyx_t_10 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":147
+    /* "pybloomfilter.pyx":168
  *         if filename:
  *             self._bf = cbloomfilter.bloomfilter_Create_Mmap(capacity,
  *                                                     error_rate,             # <<<<<<<<<<<<<<
  *                                                     filename.encode(),
  *                                                     num_bits,
  */
-    __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_v_error_rate); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 147, __pyx_L1_error)
+    __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_v_error_rate); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":148
+    /* "pybloomfilter.pyx":169
  *             self._bf = cbloomfilter.bloomfilter_Create_Mmap(capacity,
  *                                                     error_rate,
  *                                                     filename.encode(),             # <<<<<<<<<<<<<<
  *                                                     num_bits,
  *                                                     self._oflags | os.O_CREAT,
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 148, __pyx_L1_error)
+    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_14 = __Pyx_PyObject_AsWritableString(__pyx_t_11); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyObject_AsWritableString(__pyx_t_11); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":150
+    /* "pybloomfilter.pyx":171
  *                                                     filename.encode(),
  *                                                     num_bits,
  *                                                     self._oflags | os.O_CREAT,             # <<<<<<<<<<<<<<
  *                                                     perm,
  *                                                     <int *>seeds,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_oflags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_oflags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_os); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_O_CREAT); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_O_CREAT); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Or(__pyx_t_3, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Or(__pyx_t_3, __pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-    __pyx_t_17 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_17 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_17 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 171, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pybloomfilter.pyx":151
+    /* "pybloomfilter.pyx":172
  *                                                     num_bits,
  *                                                     self._oflags | os.O_CREAT,
  *                                                     perm,             # <<<<<<<<<<<<<<
  *                                                     <int *>seeds,
  *                                                     num_hashes)
  */
-    __pyx_t_18 = __Pyx_PyInt_As_int(__pyx_v_perm); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyInt_As_int(__pyx_v_perm); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":153
+    /* "pybloomfilter.pyx":174
  *                                                     perm,
  *                                                     <int *>seeds,
  *                                                     num_hashes)             # <<<<<<<<<<<<<<
  *         else:
  *             self._in_memory = 1
  */
-    __pyx_t_19 = __Pyx_PyInt_As_int(__pyx_v_num_hashes); if (unlikely((__pyx_t_19 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_As_int(__pyx_v_num_hashes); if (unlikely((__pyx_t_19 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 174, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":146
+    /* "pybloomfilter.pyx":167
  *         # backed bloom filter. Otherwise, it will be malloc
  *         if filename:
  *             self._bf = cbloomfilter.bloomfilter_Create_Mmap(capacity,             # <<<<<<<<<<<<<<
  *                                                     error_rate,
  *                                                     filename.encode(),
  */
     __pyx_v_self->_bf = bloomfilter_Create_Mmap(__pyx_t_10, __pyx_t_16, __pyx_t_14, __pyx_v_num_bits, __pyx_t_17, __pyx_t_18, ((int *)__pyx_v_seeds), __pyx_t_19);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-    /* "pybloomfilter.pyx":145
+    /* "pybloomfilter.pyx":166
  *         # If a filename is provided, we should make a mmap-file
  *         # backed bloom filter. Otherwise, it will be malloc
  *         if filename:             # <<<<<<<<<<<<<<
  *             self._bf = cbloomfilter.bloomfilter_Create_Mmap(capacity,
  *                                                     error_rate,
  */
-    goto __pyx_L20;
+    goto __pyx_L24;
   }
 
-  /* "pybloomfilter.pyx":155
+  /* "pybloomfilter.pyx":176
  *                                                     num_hashes)
  *         else:
  *             self._in_memory = 1             # <<<<<<<<<<<<<<
- *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,
- *                                                     error_rate,
+ *             if data_array is not None:
+ *                 data = data_array
  */
   /*else*/ {
     __pyx_v_self->_in_memory = 1;
 
-    /* "pybloomfilter.pyx":156
+    /* "pybloomfilter.pyx":177
  *         else:
  *             self._in_memory = 1
+ *             if data_array is not None:             # <<<<<<<<<<<<<<
+ *                 data = data_array
+ *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,
+ */
+    __pyx_t_8 = (__pyx_v_data_array != Py_None);
+    __pyx_t_2 = (__pyx_t_8 != 0);
+    if (__pyx_t_2) {
+
+      /* "pybloomfilter.pyx":178
+ *             self._in_memory = 1
+ *             if data_array is not None:
+ *                 data = data_array             # <<<<<<<<<<<<<<
+ *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,
+ *                                                     error_rate,
+ */
+      __pyx_t_14 = __Pyx_PyObject_AsWritableString(__pyx_v_data_array); if (unlikely((!__pyx_t_14) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L1_error)
+      __pyx_v_data = __pyx_t_14;
+
+      /* "pybloomfilter.pyx":177
+ *         else:
+ *             self._in_memory = 1
+ *             if data_array is not None:             # <<<<<<<<<<<<<<
+ *                 data = data_array
+ *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,
+ */
+    }
+
+    /* "pybloomfilter.pyx":179
+ *             if data_array is not None:
+ *                 data = data_array
  *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,             # <<<<<<<<<<<<<<
  *                                                     error_rate,
  *                                                     num_bits,
  */
-    __pyx_t_10 = __Pyx_PyInt_As_long(__pyx_v_capacity); if (unlikely((__pyx_t_10 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 156, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_long(__pyx_v_capacity); if (unlikely((__pyx_t_10 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":157
- *             self._in_memory = 1
+    /* "pybloomfilter.pyx":180
+ *                 data = data_array
  *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,
  *                                                     error_rate,             # <<<<<<<<<<<<<<
  *                                                     num_bits,
  *                                                     <int *>seeds,
  */
-    __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_v_error_rate); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
+    __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_v_error_rate); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":160
+    /* "pybloomfilter.pyx":183
  *                                                     num_bits,
  *                                                     <int *>seeds,
- *                                                     num_hashes)             # <<<<<<<<<<<<<<
+ *                                                     num_hashes, <const char *>data)             # <<<<<<<<<<<<<<
  *         if self._bf is NULL:
  *             if filename:
  */
-    __pyx_t_19 = __Pyx_PyInt_As_int(__pyx_v_num_hashes); if (unlikely((__pyx_t_19 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_As_int(__pyx_v_num_hashes); if (unlikely((__pyx_t_19 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":156
- *         else:
- *             self._in_memory = 1
+    /* "pybloomfilter.pyx":179
+ *             if data_array is not None:
+ *                 data = data_array
  *             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,             # <<<<<<<<<<<<<<
  *                                                     error_rate,
  *                                                     num_bits,
  */
-    __pyx_v_self->_bf = bloomfilter_Create_Malloc(__pyx_t_10, __pyx_t_16, __pyx_v_num_bits, ((int *)__pyx_v_seeds), __pyx_t_19);
+    __pyx_v_self->_bf = bloomfilter_Create_Malloc(__pyx_t_10, __pyx_t_16, __pyx_v_num_bits, ((int *)__pyx_v_seeds), __pyx_t_19, ((char const *)__pyx_v_data));
   }
-  __pyx_L20:;
+  __pyx_L24:;
 
-  /* "pybloomfilter.pyx":161
+  /* "pybloomfilter.pyx":184
  *                                                     <int *>seeds,
- *                                                     num_hashes)
+ *                                                     num_hashes, <const char *>data)
  *         if self._bf is NULL:             # <<<<<<<<<<<<<<
  *             if filename:
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),
  */
   __pyx_t_2 = ((__pyx_v_self->_bf == NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "pybloomfilter.pyx":162
- *                                                     num_hashes)
+    /* "pybloomfilter.pyx":185
+ *                                                     num_hashes, <const char *>data)
  *         if self._bf is NULL:
  *             if filename:             # <<<<<<<<<<<<<<
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),
  *                                                     filename))
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_filename); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
     if (unlikely(__pyx_t_2)) {
 
-      /* "pybloomfilter.pyx":163
+      /* "pybloomfilter.pyx":186
  *         if self._bf is NULL:
  *             if filename:
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),             # <<<<<<<<<<<<<<
  *                                                     filename))
  *             else:
  */
-      __pyx_t_11 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_6 = 0;
       __pyx_t_20 = 127;
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strerror); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strerror); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(errno); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_13 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_9, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 163, __pyx_L1_error)
+      if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_13), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_13), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __pyx_t_20 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_20) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_20;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
       __pyx_t_5 = 0;
-      __Pyx_INCREF(__pyx_kp_u__2);
+      __Pyx_INCREF(__pyx_kp_u__4);
       __pyx_t_6 += 2;
-      __Pyx_GIVEREF(__pyx_kp_u__2);
-      PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_u__2);
+      __Pyx_GIVEREF(__pyx_kp_u__4);
+      PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_u__4);
 
-      /* "pybloomfilter.pyx":164
+      /* "pybloomfilter.pyx":187
  *             if filename:
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),
  *                                                     filename))             # <<<<<<<<<<<<<<
  *             else:
  *                 cpython.PyErr_NoMemory()
  */
-      __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filename), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filename), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 187, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_20 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_20) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_20;
       __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "pybloomfilter.pyx":163
+      /* "pybloomfilter.pyx":186
  *         if self._bf is NULL:
  *             if filename:
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),             # <<<<<<<<<<<<<<
  *                                                     filename))
  *             else:
  */
-      __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_6, __pyx_t_20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_6, __pyx_t_20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_11);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_11);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5);
       __pyx_t_11 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 163, __pyx_L1_error)
+      __PYX_ERR(0, 186, __pyx_L1_error)
 
-      /* "pybloomfilter.pyx":162
- *                                                     num_hashes)
+      /* "pybloomfilter.pyx":185
+ *                                                     num_hashes, <const char *>data)
  *         if self._bf is NULL:
  *             if filename:             # <<<<<<<<<<<<<<
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),
  *                                                     filename))
  */
     }
 
-    /* "pybloomfilter.pyx":166
+    /* "pybloomfilter.pyx":189
  *                                                     filename))
  *             else:
  *                 cpython.PyErr_NoMemory()             # <<<<<<<<<<<<<<
  * 
- *     def _open(self, filename, mode="rw"):
+ * 
  */
     /*else*/ {
-      __pyx_t_21 = PyErr_NoMemory(); if (unlikely(__pyx_t_21 == ((PyObject *)NULL))) __PYX_ERR(0, 166, __pyx_L1_error)
+      __pyx_t_21 = PyErr_NoMemory(); if (unlikely(__pyx_t_21 == ((PyObject *)NULL))) __PYX_ERR(0, 189, __pyx_L1_error)
     }
 
-    /* "pybloomfilter.pyx":161
+    /* "pybloomfilter.pyx":184
  *                                                     <int *>seeds,
- *                                                     num_hashes)
+ *                                                     num_hashes, <const char *>data)
  *         if self._bf is NULL:             # <<<<<<<<<<<<<<
  *             if filename:
  *                 raise OSError(errno, '%s: %s' % (os.strerror(errno),
  */
   }
 
-  /* "pybloomfilter.pyx":93
- *         self._create(capacity, error_rate, filename, perm, hash_seeds)
+  /* "pybloomfilter.pyx":103
  * 
- *     def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):             # <<<<<<<<<<<<<<
+ * 
+ *     def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):             # <<<<<<<<<<<<<<
  *         cdef char * seeds
- *         cdef long long num_bits
+ *         cdef char * data = NULL
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
@@ -3684,25 +3981,25 @@
   __Pyx_XDECREF(__pyx_v_bits_per_hash);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":168
- *                 cpython.PyErr_NoMemory()
+/* "pybloomfilter.pyx":192
+ * 
  * 
  *     def _open(self, filename, mode="rw"):             # <<<<<<<<<<<<<<
  *         # Should not overwrite
  *         mode = mode.replace("+", "")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_5_open(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_5_open(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_7_open(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_7_open(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_mode = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3731,15 +4028,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_open") < 0)) __PYX_ERR(0, 168, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_open") < 0)) __PYX_ERR(0, 192, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -3747,28 +4044,28 @@
       }
     }
     __pyx_v_filename = values[0];
     __pyx_v_mode = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_open", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 168, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_open", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 192, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybloomfilter.BloomFilter._open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_4_open(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_filename, __pyx_v_mode);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_6_open(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_filename, __pyx_v_mode);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_4_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_6_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -3781,88 +4078,88 @@
   char *__pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_open", 0);
   __Pyx_INCREF(__pyx_v_mode);
 
-  /* "pybloomfilter.pyx":170
+  /* "pybloomfilter.pyx":194
  *     def _open(self, filename, mode="rw"):
  *         # Should not overwrite
  *         mode = mode.replace("+", "")             # <<<<<<<<<<<<<<
  * 
  *         if not os.path.exists(filename):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_replace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_replace); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_mode, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":172
+  /* "pybloomfilter.pyx":196
  *         mode = mode.replace("+", "")
  * 
  *         if not os.path.exists(filename):             # <<<<<<<<<<<<<<
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),
  *                                                         filename))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_filename);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "pybloomfilter.pyx":173
+    /* "pybloomfilter.pyx":197
  * 
  *         if not os.path.exists(filename):
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),             # <<<<<<<<<<<<<<
  *                                                         filename))
  *         if not os.access(filename, _construct_access(mode)):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_eno); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_eno); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ENOENT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ENOENT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_os); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_os); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_strerror); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_strerror); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_eno); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_eno); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_ENOENT); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_ENOENT); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -3870,92 +4167,92 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_9, function);
       }
     }
     __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_10);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_3), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_3), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_9);
     __pyx_t_9 = 0;
-    __Pyx_INCREF(__pyx_kp_u__2);
+    __Pyx_INCREF(__pyx_kp_u__4);
     __pyx_t_6 += 2;
-    __Pyx_GIVEREF(__pyx_kp_u__2);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_kp_u__2);
+    __Pyx_GIVEREF(__pyx_kp_u__4);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_kp_u__4);
 
-    /* "pybloomfilter.pyx":174
+    /* "pybloomfilter.pyx":198
  *         if not os.path.exists(filename):
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),
  *                                                         filename))             # <<<<<<<<<<<<<<
  *         if not os.access(filename, _construct_access(mode)):
  *             raise OSError("Insufficient permissions for file %s" % filename)
  */
-    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filename), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filename), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_9);
     __pyx_t_9 = 0;
 
-    /* "pybloomfilter.pyx":173
+    /* "pybloomfilter.pyx":197
  * 
  *         if not os.path.exists(filename):
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),             # <<<<<<<<<<<<<<
  *                                                         filename))
  *         if not os.access(filename, _construct_access(mode)):
  */
-    __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_9);
     __pyx_t_1 = 0;
     __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_t_2, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_t_2, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_9, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __PYX_ERR(0, 173, __pyx_L1_error)
+    __PYX_ERR(0, 197, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":172
+    /* "pybloomfilter.pyx":196
  *         mode = mode.replace("+", "")
  * 
  *         if not os.path.exists(filename):             # <<<<<<<<<<<<<<
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),
  *                                                         filename))
  */
   }
 
-  /* "pybloomfilter.pyx":175
+  /* "pybloomfilter.pyx":199
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),
  *                                                         filename))
  *         if not os.access(filename, _construct_access(mode)):             # <<<<<<<<<<<<<<
  *             raise OSError("Insufficient permissions for file %s" % filename)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_access); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_access); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_f_13pybloomfilter__construct_access(__pyx_v_mode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_13pybloomfilter__construct_access(__pyx_v_mode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -3964,211 +4261,211 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_filename, __pyx_t_2};
-    __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_filename, __pyx_t_2};
-    __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_10 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_filename);
     __Pyx_GIVEREF(__pyx_v_filename);
     PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_11, __pyx_v_filename);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_11, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_10, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_4 = ((!__pyx_t_5) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pybloomfilter.pyx":176
+    /* "pybloomfilter.pyx":200
  *                                                         filename))
  *         if not os.access(filename, _construct_access(mode)):
  *             raise OSError("Insufficient permissions for file %s" % filename)             # <<<<<<<<<<<<<<
  * 
  *         self._oflags = _construct_mode(mode)
  */
-    __pyx_t_9 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Insufficient_permissions_for_fil, __pyx_v_filename); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Insufficient_permissions_for_fil, __pyx_v_filename); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_OSError, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_OSError, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 176, __pyx_L1_error)
+    __PYX_ERR(0, 200, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":175
+    /* "pybloomfilter.pyx":199
  *             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),
  *                                                         filename))
  *         if not os.access(filename, _construct_access(mode)):             # <<<<<<<<<<<<<<
  *             raise OSError("Insufficient permissions for file %s" % filename)
  * 
  */
   }
 
-  /* "pybloomfilter.pyx":178
+  /* "pybloomfilter.pyx":202
  *             raise OSError("Insufficient permissions for file %s" % filename)
  * 
  *         self._oflags = _construct_mode(mode)             # <<<<<<<<<<<<<<
  *         self._bf = cbloomfilter.bloomfilter_Create_Mmap(0,
  *                                                 0,
  */
-  __pyx_t_1 = __pyx_f_13pybloomfilter__construct_mode(__pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_13pybloomfilter__construct_mode(__pyx_v_mode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->_oflags = __pyx_t_11;
 
-  /* "pybloomfilter.pyx":181
+  /* "pybloomfilter.pyx":205
  *         self._bf = cbloomfilter.bloomfilter_Create_Mmap(0,
  *                                                 0,
  *                                                 filename.encode(),             # <<<<<<<<<<<<<<
  *                                                 0,
  *                                                 self._oflags,
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_AsWritableString(__pyx_t_1); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 205, __pyx_L1_error)
 
-  /* "pybloomfilter.pyx":179
+  /* "pybloomfilter.pyx":203
  * 
  *         self._oflags = _construct_mode(mode)
  *         self._bf = cbloomfilter.bloomfilter_Create_Mmap(0,             # <<<<<<<<<<<<<<
  *                                                 0,
  *                                                 filename.encode(),
  */
   __pyx_v_self->_bf = bloomfilter_Create_Mmap(0, 0.0, __pyx_t_12, 0, __pyx_v_self->_oflags, 0, NULL, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":186
+  /* "pybloomfilter.pyx":210
  *                                                 0,
  *                                                 NULL, 0)
  *         if self._bf is NULL:             # <<<<<<<<<<<<<<
  *             raise ValueError("Invalid %s file: %s" %
  *                                 (self.__class__.__name__, filename))
  */
   __pyx_t_4 = ((__pyx_v_self->_bf == NULL) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pybloomfilter.pyx":187
+    /* "pybloomfilter.pyx":211
  *                                                 NULL, 0)
  *         if self._bf is NULL:
  *             raise ValueError("Invalid %s file: %s" %             # <<<<<<<<<<<<<<
  *                                 (self.__class__.__name__, filename))
  * 
  */
-    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = 0;
     __pyx_t_7 = 127;
     __Pyx_INCREF(__pyx_kp_u_Invalid);
     __pyx_t_6 += 8;
     __Pyx_GIVEREF(__pyx_kp_u_Invalid);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid);
 
-    /* "pybloomfilter.pyx":188
+    /* "pybloomfilter.pyx":212
  *         if self._bf is NULL:
  *             raise ValueError("Invalid %s file: %s" %
  *                                 (self.__class__.__name__, filename))             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_name); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_10), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_10), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_9);
     __pyx_t_9 = 0;
     __Pyx_INCREF(__pyx_kp_u_file);
     __pyx_t_6 += 7;
     __Pyx_GIVEREF(__pyx_kp_u_file);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_file);
-    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filename), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filename), __pyx_empty_unicode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_9) : __pyx_t_7;
     __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_9);
     __pyx_t_9 = 0;
 
-    /* "pybloomfilter.pyx":187
+    /* "pybloomfilter.pyx":211
  *                                                 NULL, 0)
  *         if self._bf is NULL:
  *             raise ValueError("Invalid %s file: %s" %             # <<<<<<<<<<<<<<
  *                                 (self.__class__.__name__, filename))
  * 
  */
-    __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyUnicode_Join(__pyx_t_1, 4, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 187, __pyx_L1_error)
+    __PYX_ERR(0, 211, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":186
+    /* "pybloomfilter.pyx":210
  *                                                 0,
  *                                                 NULL, 0)
  *         if self._bf is NULL:             # <<<<<<<<<<<<<<
  *             raise ValueError("Invalid %s file: %s" %
  *                                 (self.__class__.__name__, filename))
  */
   }
 
-  /* "pybloomfilter.pyx":168
- *                 cpython.PyErr_NoMemory()
+  /* "pybloomfilter.pyx":192
+ * 
  * 
  *     def _open(self, filename, mode="rw"):             # <<<<<<<<<<<<<<
  *         # Should not overwrite
  *         mode = mode.replace("+", "")
  */
 
   /* function exit code */
@@ -4186,68 +4483,68 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_mode);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":190
+/* "pybloomfilter.pyx":214
  *                                 (self.__class__.__name__, filename))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cbloomfilter.bloomfilter_Destroy(self._bf)
  *         self._bf = NULL
  */
 
 /* Python wrapper */
-static void __pyx_pw_13pybloomfilter_11BloomFilter_7__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_13pybloomfilter_11BloomFilter_7__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_13pybloomfilter_11BloomFilter_9__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_13pybloomfilter_11BloomFilter_9__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_13pybloomfilter_11BloomFilter_6__dealloc__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_pf_13pybloomfilter_11BloomFilter_8__dealloc__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_13pybloomfilter_11BloomFilter_6__dealloc__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static void __pyx_pf_13pybloomfilter_11BloomFilter_8__dealloc__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "pybloomfilter.pyx":191
+  /* "pybloomfilter.pyx":215
  * 
  *     def __dealloc__(self):
  *         cbloomfilter.bloomfilter_Destroy(self._bf)             # <<<<<<<<<<<<<<
  *         self._bf = NULL
  * 
  */
   bloomfilter_Destroy(__pyx_v_self->_bf);
 
-  /* "pybloomfilter.pyx":192
+  /* "pybloomfilter.pyx":216
  *     def __dealloc__(self):
  *         cbloomfilter.bloomfilter_Destroy(self._bf)
  *         self._bf = NULL             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->_bf = NULL;
 
-  /* "pybloomfilter.pyx":190
+  /* "pybloomfilter.pyx":214
  *                                 (self.__class__.__name__, filename))
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         cbloomfilter.bloomfilter_Destroy(self._bf)
  *         self._bf = NULL
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "pybloomfilter.pyx":195
+/* "pybloomfilter.pyx":219
  * 
  *     @property
  *     def bit_array(self):             # <<<<<<<<<<<<<<
  *         """Bit vector representation of the Bloom filter contents.
  *         Returns an integer.
  */
 
@@ -4279,128 +4576,128 @@
   Py_ssize_t __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":199
+  /* "pybloomfilter.pyx":223
  *         Returns an integer.
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         start_pos = self._bf.array.preamblebytes
  *         end_pos = start_pos + self._bf.array.bytes
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":200
+  /* "pybloomfilter.pyx":224
  *         """
  *         self._assert_open()
  *         start_pos = self._bf.array.preamblebytes             # <<<<<<<<<<<<<<
  *         end_pos = start_pos + self._bf.array.bytes
  *         arr = (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->preamblebytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->preamblebytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_start_pos = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":201
+  /* "pybloomfilter.pyx":225
  *         self._assert_open()
  *         start_pos = self._bf.array.preamblebytes
  *         end_pos = start_pos + self._bf.array.bytes             # <<<<<<<<<<<<<<
  *         arr = (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
  *         return int.from_bytes(arr, byteorder="big", signed=False)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_start_pos, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_start_pos, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_end_pos = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":202
+  /* "pybloomfilter.pyx":226
  *         start_pos = self._bf.array.preamblebytes
  *         end_pos = start_pos + self._bf.array.bytes
  *         arr = (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]             # <<<<<<<<<<<<<<
  *         return int.from_bytes(arr, byteorder="big", signed=False)
  * 
  */
   __Pyx_INCREF(__pyx_v_start_pos);
   __pyx_t_2 = __pyx_v_start_pos;
   __pyx_t_5 = (__pyx_t_2 == Py_None);
   if (__pyx_t_5) {
     __pyx_t_4 = 0;
   } else {
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L1_error)
     __pyx_t_4 = __pyx_t_6;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_INCREF(__pyx_v_end_pos);
   __pyx_t_2 = __pyx_v_end_pos;
   __pyx_t_5 = (__pyx_t_2 == Py_None);
   if (__pyx_t_5) {
     __pyx_t_6 = PY_SSIZE_T_MAX;
   } else {
-    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 226, __pyx_L1_error)
     __pyx_t_6 = __pyx_t_7;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((char *)mbarray_CharData(__pyx_v_self->_bf->array)) + __pyx_t_4, __pyx_t_6 - __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(((char *)mbarray_CharData(__pyx_v_self->_bf->array)) + __pyx_t_4, __pyx_t_6 - __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_arr = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":203
+  /* "pybloomfilter.pyx":227
  *         end_pos = start_pos + self._bf.array.bytes
  *         arr = (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
  *         return int.from_bytes(arr, byteorder="big", signed=False)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)(&PyInt_Type)), __pyx_n_s_from_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_arr);
   __Pyx_GIVEREF(__pyx_v_arr);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_arr);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 203, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_byteorder, __pyx_n_u_big) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 203, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 203, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_byteorder, __pyx_n_u_big) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signed, Py_False) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":195
+  /* "pybloomfilter.pyx":219
  * 
  *     @property
  *     def bit_array(self):             # <<<<<<<<<<<<<<
  *         """Bit vector representation of the Bloom filter contents.
  *         Returns an integer.
  */
 
@@ -4417,15 +4714,234 @@
   __Pyx_XDECREF(__pyx_v_end_pos);
   __Pyx_XDECREF(__pyx_v_arr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":206
+/* "pybloomfilter.pyx":230
+ * 
+ *     @property
+ *     def data_array(self):             # <<<<<<<<<<<<<<
+ *         """Bytes array of the Bloom filter contents.
+ *         """
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_10data_array_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_10data_array_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_10data_array___get__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10data_array___get__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+  PyObject *__pyx_v_start_pos = NULL;
+  PyObject *__pyx_v_end_pos = NULL;
+  PyObject *__pyx_v_arr = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  Py_ssize_t __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+
+  /* "pybloomfilter.pyx":233
+ *         """Bytes array of the Bloom filter contents.
+ *         """
+ *         self._assert_open()             # <<<<<<<<<<<<<<
+ *         start_pos = self._bf.array.preamblebytes
+ *         end_pos = start_pos + self._bf.array.bytes
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "pybloomfilter.pyx":234
+ *         """
+ *         self._assert_open()
+ *         start_pos = self._bf.array.preamblebytes             # <<<<<<<<<<<<<<
+ *         end_pos = start_pos + self._bf.array.bytes
+ *         arr = array.array('B')
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->preamblebytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_start_pos = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "pybloomfilter.pyx":235
+ *         self._assert_open()
+ *         start_pos = self._bf.array.preamblebytes
+ *         end_pos = start_pos + self._bf.array.bytes             # <<<<<<<<<<<<<<
+ *         arr = array.array('B')
+ *         arr.frombytes(
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->bytes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyNumber_Add(__pyx_v_start_pos, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_end_pos = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "pybloomfilter.pyx":236
+ *         start_pos = self._bf.array.preamblebytes
+ *         end_pos = start_pos + self._bf.array.bytes
+ *         arr = array.array('B')             # <<<<<<<<<<<<<<
+ *         arr.frombytes(
+ *             (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_n_u_B) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_B);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_v_arr = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "pybloomfilter.pyx":237
+ *         end_pos = start_pos + self._bf.array.bytes
+ *         arr = array.array('B')
+ *         arr.frombytes(             # <<<<<<<<<<<<<<
+ *             (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
+ *         )
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_arr, __pyx_n_s_frombytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
+  /* "pybloomfilter.pyx":238
+ *         arr = array.array('B')
+ *         arr.frombytes(
+ *             (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]             # <<<<<<<<<<<<<<
+ *         )
+ *         return bytes(arr)
+ */
+  __Pyx_INCREF(__pyx_v_start_pos);
+  __pyx_t_1 = __pyx_v_start_pos;
+  __pyx_t_5 = (__pyx_t_1 == Py_None);
+  if (__pyx_t_5) {
+    __pyx_t_4 = 0;
+  } else {
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_4 = __pyx_t_6;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_INCREF(__pyx_v_end_pos);
+  __pyx_t_1 = __pyx_v_end_pos;
+  __pyx_t_5 = (__pyx_t_1 == Py_None);
+  if (__pyx_t_5) {
+    __pyx_t_6 = PY_SSIZE_T_MAX;
+  } else {
+    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 238, __pyx_L1_error)
+    __pyx_t_6 = __pyx_t_7;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((char *)mbarray_CharData(__pyx_v_self->_bf->array)) + __pyx_t_4, __pyx_t_6 - __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_8);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pybloomfilter.pyx":240
+ *             (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
+ *         )
+ *         return bytes(arr)             # <<<<<<<<<<<<<<
+ * 
+ *     @property
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_arr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "pybloomfilter.pyx":230
+ * 
+ *     @property
+ *     def data_array(self):             # <<<<<<<<<<<<<<
+ *         """Bytes array of the Bloom filter contents.
+ *         """
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("pybloomfilter.BloomFilter.data_array.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_start_pos);
+  __Pyx_XDECREF(__pyx_v_end_pos);
+  __Pyx_XDECREF(__pyx_v_arr);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pybloomfilter.pyx":243
  * 
  *     @property
  *     def hash_seeds(self):             # <<<<<<<<<<<<<<
  *         """Integer seeds used for the random hashing. Returns a list of integers."""
  *         self._assert_open()
  */
 
@@ -4454,133 +4970,133 @@
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":208
+  /* "pybloomfilter.pyx":245
  *     def hash_seeds(self):
  *         """Integer seeds used for the random hashing. Returns a list of integers."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         seeds = array.array('I')
  *         seeds.frombytes(
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":209
+  /* "pybloomfilter.pyx":246
  *         """Integer seeds used for the random hashing. Returns a list of integers."""
  *         self._assert_open()
  *         seeds = array.array('I')             # <<<<<<<<<<<<<<
  *         seeds.frombytes(
  *             (<char *>self._bf.hash_seeds)[:4 * self.num_hashes]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_n_u_I) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_I);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_seeds = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":210
+  /* "pybloomfilter.pyx":247
  *         self._assert_open()
  *         seeds = array.array('I')
  *         seeds.frombytes(             # <<<<<<<<<<<<<<
  *             (<char *>self._bf.hash_seeds)[:4 * self.num_hashes]
  *         )
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_seeds, __pyx_n_s_frombytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_seeds, __pyx_n_s_frombytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pybloomfilter.pyx":211
+  /* "pybloomfilter.pyx":248
  *         seeds = array.array('I')
  *         seeds.frombytes(
  *             (<char *>self._bf.hash_seeds)[:4 * self.num_hashes]             # <<<<<<<<<<<<<<
  *         )
  *         return seeds
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_hashes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_hashes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyNumber_Multiply(__pyx_int_4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_int_4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = (__pyx_t_4 == Py_None);
   if (__pyx_t_6) {
     __pyx_t_5 = PY_SSIZE_T_MAX;
   } else {
-    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_4); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_t_4); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
     __pyx_t_5 = __pyx_t_7;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(((char *)__pyx_v_self->_bf->hash_seeds) + 0, __pyx_t_5 - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(((char *)__pyx_v_self->_bf->hash_seeds) + 0, __pyx_t_5 - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":213
+  /* "pybloomfilter.pyx":250
  *             (<char *>self._bf.hash_seeds)[:4 * self.num_hashes]
  *         )
  *         return seeds             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_seeds);
   __pyx_r = __pyx_v_seeds;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":206
+  /* "pybloomfilter.pyx":243
  * 
  *     @property
  *     def hash_seeds(self):             # <<<<<<<<<<<<<<
  *         """Integer seeds used for the random hashing. Returns a list of integers."""
  *         self._assert_open()
  */
 
@@ -4595,15 +5111,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_seeds);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":216
+/* "pybloomfilter.pyx":253
  * 
  *     @property
  *     def capacity(self):             # <<<<<<<<<<<<<<
  *         """The maximum number of elements this filter can contain while keeping
  *         the false positive rate under :attr:`BloomFilter.error_rate`.
  */
 
@@ -4627,55 +5143,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":221
+  /* "pybloomfilter.pyx":258
  *         Returns an integer.
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return self._bf.max_num_elem
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":222
+  /* "pybloomfilter.pyx":259
  *         """
  *         self._assert_open()
  *         return self._bf.max_num_elem             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->max_num_elem); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->max_num_elem); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":216
+  /* "pybloomfilter.pyx":253
  * 
  *     @property
  *     def capacity(self):             # <<<<<<<<<<<<<<
  *         """The maximum number of elements this filter can contain while keeping
  *         the false positive rate under :attr:`BloomFilter.error_rate`.
  */
 
@@ -4688,15 +5204,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":225
+/* "pybloomfilter.pyx":262
  * 
  *     @property
  *     def error_rate(self):             # <<<<<<<<<<<<<<
  *         """The acceptable probability of false positives. Returns a float."""
  *         self._assert_open()
  */
 
@@ -4720,55 +5236,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":227
+  /* "pybloomfilter.pyx":264
  *     def error_rate(self):
  *         """The acceptable probability of false positives. Returns a float."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return self._bf.error_rate
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":228
+  /* "pybloomfilter.pyx":265
  *         """The acceptable probability of false positives. Returns a float."""
  *         self._assert_open()
  *         return self._bf.error_rate             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_bf->error_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_bf->error_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":225
+  /* "pybloomfilter.pyx":262
  * 
  *     @property
  *     def error_rate(self):             # <<<<<<<<<<<<<<
  *         """The acceptable probability of false positives. Returns a float."""
  *         self._assert_open()
  */
 
@@ -4781,15 +5297,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":231
+/* "pybloomfilter.pyx":268
  * 
  *     @property
  *     def num_hashes(self):             # <<<<<<<<<<<<<<
  *         """Number of hash functions used when computing."""
  *         self._assert_open()
  */
 
@@ -4813,55 +5329,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":233
+  /* "pybloomfilter.pyx":270
  *     def num_hashes(self):
  *         """Number of hash functions used when computing."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return self._bf.num_hashes
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":234
+  /* "pybloomfilter.pyx":271
  *         """Number of hash functions used when computing."""
  *         self._assert_open()
  *         return self._bf.num_hashes             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_bf->num_hashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_bf->num_hashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":231
+  /* "pybloomfilter.pyx":268
  * 
  *     @property
  *     def num_hashes(self):             # <<<<<<<<<<<<<<
  *         """Number of hash functions used when computing."""
  *         self._assert_open()
  */
 
@@ -4874,15 +5390,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":237
+/* "pybloomfilter.pyx":274
  * 
  *     @property
  *     def num_bits(self):             # <<<<<<<<<<<<<<
  *         """Number of bits used in the filter as buckets."""
  *         self._assert_open()
  */
 
@@ -4906,55 +5422,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":239
+  /* "pybloomfilter.pyx":276
  *     def num_bits(self):
  *         """Number of bits used in the filter as buckets."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return self._bf.array.bits
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":240
+  /* "pybloomfilter.pyx":277
  *         """Number of bits used in the filter as buckets."""
  *         self._assert_open()
  *         return self._bf.array.bits             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->bits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->_bf->array->bits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":237
+  /* "pybloomfilter.pyx":274
  * 
  *     @property
  *     def num_bits(self):             # <<<<<<<<<<<<<<
  *         """Number of bits used in the filter as buckets."""
  *         self._assert_open()
  */
 
@@ -4967,15 +5483,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":243
+/* "pybloomfilter.pyx":280
  * 
  *     @property
  *     def bit_count(self):             # <<<<<<<<<<<<<<
  *         """Number of bits set to one."""
  *         self._assert_open()
  */
 
@@ -4999,55 +5515,55 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":245
+  /* "pybloomfilter.pyx":282
  *     def bit_count(self):
  *         """Number of bits set to one."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return cbloomfilter.mbarray_BitCount(self._bf.array)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":246
+  /* "pybloomfilter.pyx":283
  *         """Number of bits set to one."""
  *         self._assert_open()
  *         return cbloomfilter.mbarray_BitCount(self._bf.array)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(mbarray_BitCount(__pyx_v_self->_bf->array)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(mbarray_BitCount(__pyx_v_self->_bf->array)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":243
+  /* "pybloomfilter.pyx":280
  * 
  *     @property
  *     def bit_count(self):             # <<<<<<<<<<<<<<
  *         """Number of bits set to one."""
  *         self._assert_open()
  */
 
@@ -5060,15 +5576,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":249
+/* "pybloomfilter.pyx":286
  * 
  *     @property
  *     def approx_len(self):             # <<<<<<<<<<<<<<
  *         """Approximate number of items in the set.
  * 
  */
 
@@ -5101,75 +5617,75 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":256
+  /* "pybloomfilter.pyx":293
  *         - https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1063.3591&rep=rep1&type=pdf
  *         """
  *         m = self.num_bits             # <<<<<<<<<<<<<<
  *         k = self.num_hashes
  *         X = self.bit_count
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_bits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_bits); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_m = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":257
+  /* "pybloomfilter.pyx":294
  *         """
  *         m = self.num_bits
  *         k = self.num_hashes             # <<<<<<<<<<<<<<
  *         X = self.bit_count
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_hashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_num_hashes); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 294, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_k = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":258
+  /* "pybloomfilter.pyx":295
  *         m = self.num_bits
  *         k = self.num_hashes
  *         X = self.bit_count             # <<<<<<<<<<<<<<
  * 
  *         n = -(m / k) * math.log(1 - (X / m), math.e)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_bit_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_bit_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_X = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":260
+  /* "pybloomfilter.pyx":297
  *         X = self.bit_count
  * 
  *         n = -(m / k) * math.log(1 - (X / m), math.e)             # <<<<<<<<<<<<<<
  *         return round(n)
  * 
  */
-  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_m, __pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_m, __pyx_v_k); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Negative(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Negative(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_log); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_log); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_v_X, __pyx_v_m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyNumber_Divide(__pyx_v_X, __pyx_v_m); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_SubtractCObj(__pyx_int_1, __pyx_t_3, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_SubtractCObj(__pyx_int_1, __pyx_t_3, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_math); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_e); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
@@ -5179,70 +5695,70 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_6};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_5, __pyx_t_6};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_6);
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_n = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pybloomfilter.pyx":261
+  /* "pybloomfilter.pyx":298
  * 
  *         n = -(m / k) * math.log(1 - (X / m), math.e)
  *         return round(n)             # <<<<<<<<<<<<<<
  * 
  *     def _name(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_round, __pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_round, __pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":249
+  /* "pybloomfilter.pyx":286
  * 
  *     @property
  *     def approx_len(self):             # <<<<<<<<<<<<<<
  *         """Approximate number of items in the set.
  * 
  */
 
@@ -5263,167 +5779,167 @@
   __Pyx_XDECREF(__pyx_v_X);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":263
+/* "pybloomfilter.pyx":300
  *         return round(n)
  * 
  *     def _name(self):             # <<<<<<<<<<<<<<
  *         self._assert_open()
  *         if self._in_memory:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_9_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_9_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_11_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_11_name(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_8_name(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_10_name(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_8_name(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10_name(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_name", 0);
 
-  /* "pybloomfilter.pyx":264
+  /* "pybloomfilter.pyx":301
  * 
  *     def _name(self):
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         if self._in_memory:
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":265
+  /* "pybloomfilter.pyx":302
  *     def _name(self):
  *         self._assert_open()
  *         if self._in_memory:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'
  *                                         % self.__class__.__name__)
  */
   __pyx_t_4 = (__pyx_v_self->_in_memory != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pybloomfilter.pyx":267
+    /* "pybloomfilter.pyx":304
  *         if self._in_memory:
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'
  *                                         % self.__class__.__name__)             # <<<<<<<<<<<<<<
  *         if self._bf.array.filename is NULL:
  *             return None
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Cannot_access_name_on_an_in_memo, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Cannot_access_name_on_an_in_memo, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":266
+    /* "pybloomfilter.pyx":303
  *         self._assert_open()
  *         if self._in_memory:
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'             # <<<<<<<<<<<<<<
  *                                         % self.__class__.__name__)
  *         if self._bf.array.filename is NULL:
  */
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 266, __pyx_L1_error)
+    __PYX_ERR(0, 303, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":265
+    /* "pybloomfilter.pyx":302
  *     def _name(self):
  *         self._assert_open()
  *         if self._in_memory:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'
  *                                         % self.__class__.__name__)
  */
   }
 
-  /* "pybloomfilter.pyx":268
+  /* "pybloomfilter.pyx":305
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'
  *                                         % self.__class__.__name__)
  *         if self._bf.array.filename is NULL:             # <<<<<<<<<<<<<<
  *             return None
  *         return self._bf.array.filename
  */
   __pyx_t_4 = ((__pyx_v_self->_bf->array->filename == NULL) != 0);
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":269
+    /* "pybloomfilter.pyx":306
  *                                         % self.__class__.__name__)
  *         if self._bf.array.filename is NULL:
  *             return None             # <<<<<<<<<<<<<<
  *         return self._bf.array.filename
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "pybloomfilter.pyx":268
+    /* "pybloomfilter.pyx":305
  *             raise NotImplementedError('Cannot access .name on an in-memory %s'
  *                                         % self.__class__.__name__)
  *         if self._bf.array.filename is NULL:             # <<<<<<<<<<<<<<
  *             return None
  *         return self._bf.array.filename
  */
   }
 
-  /* "pybloomfilter.pyx":270
+  /* "pybloomfilter.pyx":307
  *         if self._bf.array.filename is NULL:
  *             return None
  *         return self._bf.array.filename             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_self->_bf->array->filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 270, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_self->_bf->array->filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":263
+  /* "pybloomfilter.pyx":300
  *         return round(n)
  * 
  *     def _name(self):             # <<<<<<<<<<<<<<
  *         self._assert_open()
  *         if self._in_memory:
  */
 
@@ -5436,15 +5952,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":273
+/* "pybloomfilter.pyx":310
  * 
  *     @property
  *     def name(self):             # <<<<<<<<<<<<<<
  *         """PENDING DEPRECATION - use :meth:`BloomFilter.filename` instead.
  * 
  */
 
@@ -5468,69 +5984,69 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":280
+  /* "pybloomfilter.pyx":317
  *         Returns an encoded string.
  *         """
  *         warnings.warn('name will be deprecated in future versions, use '             # <<<<<<<<<<<<<<
  *                       'filename instead', PendingDeprecationWarning)
  *         return self._name()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_warnings); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":281
+  /* "pybloomfilter.pyx":318
  *         """
  *         warnings.warn('name will be deprecated in future versions, use '
  *                       'filename instead', PendingDeprecationWarning)             # <<<<<<<<<<<<<<
  *         return self._name()
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":282
+  /* "pybloomfilter.pyx":319
  *         warnings.warn('name will be deprecated in future versions, use '
  *                       'filename instead', PendingDeprecationWarning)
  *         return self._name()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":273
+  /* "pybloomfilter.pyx":310
  * 
  *     @property
  *     def name(self):             # <<<<<<<<<<<<<<
  *         """PENDING DEPRECATION - use :meth:`BloomFilter.filename` instead.
  * 
  */
 
@@ -5543,15 +6059,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":285
+/* "pybloomfilter.pyx":322
  * 
  *     @property
  *     def filename(self):             # <<<<<<<<<<<<<<
  *         """File name (compatible with file objects). Does not apply to an in-memory
  *         :class:`BloomFilter` and will raise :class:`ValueError` if accessed.
  */
 
@@ -5576,62 +6092,62 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":290
+  /* "pybloomfilter.pyx":327
  *         Returns a string.
  *         """
  *         return self._name().decode()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":285
+  /* "pybloomfilter.pyx":322
  * 
  *     @property
  *     def filename(self):             # <<<<<<<<<<<<<<
  *         """File name (compatible with file objects). Does not apply to an in-memory
  *         :class:`BloomFilter` and will raise :class:`ValueError` if accessed.
  */
 
@@ -5645,15 +6161,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":293
+/* "pybloomfilter.pyx":330
  * 
  *     @property
  *     def read_only(self):             # <<<<<<<<<<<<<<
  *         """Indicates if the opened :class:`BloomFilter` is read-only.
  *         Always ``False`` for an in-memory :class:`BloomFilter`.
  */
 
@@ -5680,81 +6196,81 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pybloomfilter.pyx":297
+  /* "pybloomfilter.pyx":334
  *         Always ``False`` for an in-memory :class:`BloomFilter`.
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return not self._in_memory and not self._oflags & os.O_RDWR
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":298
+  /* "pybloomfilter.pyx":335
  *         """
  *         self._assert_open()
  *         return not self._in_memory and not self._oflags & os.O_RDWR             # <<<<<<<<<<<<<<
  * 
  *     def fileno(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_4 = (!(__pyx_v_self->_in_memory != 0));
   if (__pyx_t_4) {
   } else {
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->_oflags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->_oflags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_O_RDWR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_O_RDWR); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_And(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_And(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_6 = (!__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":293
+  /* "pybloomfilter.pyx":330
  * 
  *     @property
  *     def read_only(self):             # <<<<<<<<<<<<<<
  *         """Indicates if the opened :class:`BloomFilter` is read-only.
  *         Always ``False`` for an in-memory :class:`BloomFilter`.
  */
 
@@ -5768,88 +6284,88 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":300
+/* "pybloomfilter.pyx":337
  *         return not self._in_memory and not self._oflags & os.O_RDWR
  * 
  *     def fileno(self):             # <<<<<<<<<<<<<<
  *         """Bloom filter file descriptor."""
  *         self._assert_open()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_11fileno(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_10fileno[] = "Bloom filter file descriptor.";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_11fileno(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_13fileno(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_12fileno[] = "Bloom filter file descriptor.";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_13fileno(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fileno (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_10fileno(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_12fileno(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_10fileno(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_12fileno(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fileno", 0);
 
-  /* "pybloomfilter.pyx":302
+  /* "pybloomfilter.pyx":339
  *     def fileno(self):
  *         """Bloom filter file descriptor."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         return self._bf.array.fd
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 302, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":303
+  /* "pybloomfilter.pyx":340
  *         """Bloom filter file descriptor."""
  *         self._assert_open()
  *         return self._bf.array.fd             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_bf->array->fd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_bf->array->fd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":300
+  /* "pybloomfilter.pyx":337
  *         return not self._in_memory and not self._oflags & os.O_RDWR
  * 
  *     def fileno(self):             # <<<<<<<<<<<<<<
  *         """Bloom filter file descriptor."""
  *         self._assert_open()
  */
 
@@ -5862,183 +6378,183 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":305
+/* "pybloomfilter.pyx":342
  *         return self._bf.array.fd
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         self._assert_open()
  *         my_name = self.__class__.__name__
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_13__repr__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_13__repr__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_15__repr__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_15__repr__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_12__repr__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_14__repr__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_12__repr__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_14__repr__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_v_my_name = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   Py_UCS4 __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "pybloomfilter.pyx":306
+  /* "pybloomfilter.pyx":343
  * 
  *     def __repr__(self):
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         my_name = self.__class__.__name__
  *         return '<%s capacity: %d, error: %0.3f, num_hashes: %d>' % (
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":307
+  /* "pybloomfilter.pyx":344
  *     def __repr__(self):
  *         self._assert_open()
  *         my_name = self.__class__.__name__             # <<<<<<<<<<<<<<
  *         return '<%s capacity: %d, error: %0.3f, num_hashes: %d>' % (
  *             my_name, self._bf.max_num_elem, self._bf.error_rate,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_my_name = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":308
+  /* "pybloomfilter.pyx":345
  *         self._assert_open()
  *         my_name = self.__class__.__name__
  *         return '<%s capacity: %d, error: %0.3f, num_hashes: %d>' % (             # <<<<<<<<<<<<<<
  *             my_name, self._bf.max_num_elem, self._bf.error_rate,
  *             self._bf.num_hashes)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = 0;
   __pyx_t_5 = 127;
-  __Pyx_INCREF(__pyx_kp_u__6);
+  __Pyx_INCREF(__pyx_kp_u__8);
   __pyx_t_4 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__6);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__6);
+  __Pyx_GIVEREF(__pyx_kp_u__8);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u__8);
 
-  /* "pybloomfilter.pyx":309
+  /* "pybloomfilter.pyx":346
  *         my_name = self.__class__.__name__
  *         return '<%s capacity: %d, error: %0.3f, num_hashes: %d>' % (
  *             my_name, self._bf.max_num_elem, self._bf.error_rate,             # <<<<<<<<<<<<<<
  *             self._bf.num_hashes)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_my_name), __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_my_name), __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_1) : __pyx_t_5;
   __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
   __Pyx_INCREF(__pyx_kp_u_capacity_2);
   __pyx_t_4 += 11;
   __Pyx_GIVEREF(__pyx_kp_u_capacity_2);
   PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_capacity_2);
-  __pyx_t_1 = __Pyx_PyUnicode_From_long(__pyx_v_self->_bf->max_num_elem, 0, ' ', 'd'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_From_long(__pyx_v_self->_bf->max_num_elem, 0, ' ', 'd'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_1);
   __pyx_t_1 = 0;
   __Pyx_INCREF(__pyx_kp_u_error);
   __pyx_t_4 += 9;
   __Pyx_GIVEREF(__pyx_kp_u_error);
   PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_kp_u_error);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_bf->error_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->_bf->error_rate); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_Format(__pyx_t_1, __pyx_kp_u_0_3f); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Format(__pyx_t_1, __pyx_kp_u_0_3f); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_5) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_5;
   __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_3);
   __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_kp_u_num_hashes_2);
   __pyx_t_4 += 14;
   __Pyx_GIVEREF(__pyx_kp_u_num_hashes_2);
   PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_kp_u_num_hashes_2);
 
-  /* "pybloomfilter.pyx":310
+  /* "pybloomfilter.pyx":347
  *         return '<%s capacity: %d, error: %0.3f, num_hashes: %d>' % (
  *             my_name, self._bf.max_num_elem, self._bf.error_rate,
  *             self._bf.num_hashes)             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_self->_bf->num_hashes, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_From_int(__pyx_v_self->_bf->num_hashes, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_t_3);
   __pyx_t_3 = 0;
-  __Pyx_INCREF(__pyx_kp_u__7);
+  __Pyx_INCREF(__pyx_kp_u__9);
   __pyx_t_4 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__7);
-  PyTuple_SET_ITEM(__pyx_t_2, 8, __pyx_kp_u__7);
+  __Pyx_GIVEREF(__pyx_kp_u__9);
+  PyTuple_SET_ITEM(__pyx_t_2, 8, __pyx_kp_u__9);
 
-  /* "pybloomfilter.pyx":308
+  /* "pybloomfilter.pyx":345
  *         self._assert_open()
  *         my_name = self.__class__.__name__
  *         return '<%s capacity: %d, error: %0.3f, num_hashes: %d>' % (             # <<<<<<<<<<<<<<
  *             my_name, self._bf.max_num_elem, self._bf.error_rate,
  *             self._bf.num_hashes)
  */
-  __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_2, 9, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_2, 9, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":305
+  /* "pybloomfilter.pyx":342
  *         return self._bf.array.fd
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         self._assert_open()
  *         my_name = self.__class__.__name__
  */
 
@@ -6052,76 +6568,76 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_my_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":312
+/* "pybloomfilter.pyx":349
  *             self._bf.num_hashes)
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return self.__repr__()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_15__str__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_15__str__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_17__str__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_17__str__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__str__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_14__str__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_16__str__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_14__str__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_16__str__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "pybloomfilter.pyx":313
+  /* "pybloomfilter.pyx":350
  * 
  *     def __str__(self):
  *         return self.__repr__()             # <<<<<<<<<<<<<<
  * 
  *     def sync(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_repr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_repr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":312
+  /* "pybloomfilter.pyx":349
  *             self._bf.num_hashes)
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return self.__repr__()
  * 
  */
 
@@ -6134,109 +6650,109 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":315
+/* "pybloomfilter.pyx":352
  *         return self.__repr__()
  * 
  *     def sync(self):             # <<<<<<<<<<<<<<
  *         """Forces a ``sync()`` call on the underlying mmap file object. Use this if
  *         you are about to copy the file and you want to be sure you got
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_17sync(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_16sync[] = "Forces a ``sync()`` call on the underlying mmap file object. Use this if\n        you are about to copy the file and you want to be sure you got\n        everything correctly.\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_17sync(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_19sync(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_18sync[] = "Forces a ``sync()`` call on the underlying mmap file object. Use this if\n        you are about to copy the file and you want to be sure you got\n        everything correctly.\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_19sync(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("sync (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_16sync(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_18sync(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_16sync(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_18sync(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sync", 0);
 
-  /* "pybloomfilter.pyx":320
+  /* "pybloomfilter.pyx":357
  *         everything correctly.
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_writable()
  *         cbloomfilter.mbarray_Sync(self._bf.array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":321
+  /* "pybloomfilter.pyx":358
  *         """
  *         self._assert_open()
  *         self._assert_writable()             # <<<<<<<<<<<<<<
  *         cbloomfilter.mbarray_Sync(self._bf.array)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":322
+  /* "pybloomfilter.pyx":359
  *         self._assert_open()
  *         self._assert_writable()
  *         cbloomfilter.mbarray_Sync(self._bf.array)             # <<<<<<<<<<<<<<
  * 
  *     def clear_all(self):
  */
   (void)(mbarray_Sync(__pyx_v_self->_bf->array));
 
-  /* "pybloomfilter.pyx":315
+  /* "pybloomfilter.pyx":352
  *         return self.__repr__()
  * 
  *     def sync(self):             # <<<<<<<<<<<<<<
  *         """Forces a ``sync()`` call on the underlying mmap file object. Use this if
  *         you are about to copy the file and you want to be sure you got
  */
 
@@ -6251,109 +6767,109 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":324
+/* "pybloomfilter.pyx":361
  *         cbloomfilter.mbarray_Sync(self._bf.array)
  * 
  *     def clear_all(self):             # <<<<<<<<<<<<<<
  *         """Removes all elements from the Bloom filter at once."""
  *         self._assert_open()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_19clear_all(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_18clear_all[] = "Removes all elements from the Bloom filter at once.";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_19clear_all(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_21clear_all(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_20clear_all[] = "Removes all elements from the Bloom filter at once.";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_21clear_all(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clear_all (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_18clear_all(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_20clear_all(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_18clear_all(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_20clear_all(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear_all", 0);
 
-  /* "pybloomfilter.pyx":326
+  /* "pybloomfilter.pyx":363
  *     def clear_all(self):
  *         """Removes all elements from the Bloom filter at once."""
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_writable()
  *         cbloomfilter.bloomfilter_Clear(self._bf)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":327
+  /* "pybloomfilter.pyx":364
  *         """Removes all elements from the Bloom filter at once."""
  *         self._assert_open()
  *         self._assert_writable()             # <<<<<<<<<<<<<<
  *         cbloomfilter.bloomfilter_Clear(self._bf)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 364, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":328
+  /* "pybloomfilter.pyx":365
  *         self._assert_open()
  *         self._assert_writable()
  *         cbloomfilter.bloomfilter_Clear(self._bf)             # <<<<<<<<<<<<<<
  * 
  *     def __contains__(self, item_):
  */
   (void)(bloomfilter_Clear(__pyx_v_self->_bf));
 
-  /* "pybloomfilter.pyx":324
+  /* "pybloomfilter.pyx":361
  *         cbloomfilter.mbarray_Sync(self._bf.array)
  * 
  *     def clear_all(self):             # <<<<<<<<<<<<<<
  *         """Removes all elements from the Bloom filter at once."""
  *         self._assert_open()
  */
 
@@ -6368,40 +6884,40 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":330
+/* "pybloomfilter.pyx":367
  *         cbloomfilter.bloomfilter_Clear(self._bf)
  * 
  *     def __contains__(self, item_):             # <<<<<<<<<<<<<<
  *         """Checks to see if item is contained in the filter, with
  *         an acceptable false positive rate of :attr:`BloomFilter.error_rate`.
  */
 
 /* Python wrapper */
-static int __pyx_pw_13pybloomfilter_11BloomFilter_21__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item_); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_20__contains__[] = "Checks to see if item is contained in the filter, with\n        an acceptable false positive rate of :attr:`BloomFilter.error_rate`.\n\n        :param item: hashable object\n        :rtype: bool\n        ";
+static int __pyx_pw_13pybloomfilter_11BloomFilter_23__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item_); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_22__contains__[] = "Checks to see if item is contained in the filter, with\n        an acceptable false positive rate of :attr:`BloomFilter.error_rate`.\n\n        :param item: hashable object\n        :rtype: bool\n        ";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_20__contains__;
+struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_22__contains__;
 #endif
-static int __pyx_pw_13pybloomfilter_11BloomFilter_21__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item_) {
+static int __pyx_pw_13pybloomfilter_11BloomFilter_23__contains__(PyObject *__pyx_v_self, PyObject *__pyx_v_item_) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__contains__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_20__contains__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_item_));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_22__contains__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_item_));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_13pybloomfilter_11BloomFilter_20__contains__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_) {
+static int __pyx_pf_13pybloomfilter_11BloomFilter_22__contains__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_) {
   Key __pyx_v_key;
   PyObject *__pyx_v_item = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -6411,202 +6927,202 @@
   Py_ssize_t __pyx_t_7;
   Py_hash_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__contains__", 0);
 
-  /* "pybloomfilter.pyx":337
+  /* "pybloomfilter.pyx":374
  *         :rtype: bool
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":339
+  /* "pybloomfilter.pyx":376
  *         self._assert_open()
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):             # <<<<<<<<<<<<<<
  *             item = item_.encode()
  *             key.shash = item
  */
   __pyx_t_4 = PyUnicode_Check(__pyx_v_item_); 
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "pybloomfilter.pyx":340
+    /* "pybloomfilter.pyx":377
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):
  *             item = item_.encode()             # <<<<<<<<<<<<<<
  *             key.shash = item
  *             key.nhash = len(item)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_item_, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_item_, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_item = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "pybloomfilter.pyx":341
+    /* "pybloomfilter.pyx":378
  *         if isinstance(item_, str):
  *             item = item_.encode()
  *             key.shash = item             # <<<<<<<<<<<<<<
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):
  */
-    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 378, __pyx_L1_error)
     __pyx_v_key.shash = __pyx_t_6;
 
-    /* "pybloomfilter.pyx":342
+    /* "pybloomfilter.pyx":379
  *             item = item_.encode()
  *             key.shash = item
  *             key.nhash = len(item)             # <<<<<<<<<<<<<<
  *         elif isinstance(item_, bytes):
  *             item = item_
  */
-    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 342, __pyx_L1_error)
+    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 379, __pyx_L1_error)
     __pyx_v_key.nhash = __pyx_t_7;
 
-    /* "pybloomfilter.pyx":339
+    /* "pybloomfilter.pyx":376
  *         self._assert_open()
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):             # <<<<<<<<<<<<<<
  *             item = item_.encode()
  *             key.shash = item
  */
     goto __pyx_L3;
   }
 
-  /* "pybloomfilter.pyx":343
+  /* "pybloomfilter.pyx":380
  *             key.shash = item
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):             # <<<<<<<<<<<<<<
  *             item = item_
  *             key.shash = item
  */
   __pyx_t_5 = PyBytes_Check(__pyx_v_item_); 
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":344
+    /* "pybloomfilter.pyx":381
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):
  *             item = item_             # <<<<<<<<<<<<<<
  *             key.shash = item
  *             key.nhash = len(item)
  */
     __Pyx_INCREF(__pyx_v_item_);
     __pyx_v_item = __pyx_v_item_;
 
-    /* "pybloomfilter.pyx":345
+    /* "pybloomfilter.pyx":382
  *         elif isinstance(item_, bytes):
  *             item = item_
  *             key.shash = item             # <<<<<<<<<<<<<<
  *             key.nhash = len(item)
  *         else:
  */
-    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
     __pyx_v_key.shash = __pyx_t_6;
 
-    /* "pybloomfilter.pyx":346
+    /* "pybloomfilter.pyx":383
  *             item = item_
  *             key.shash = item
  *             key.nhash = len(item)             # <<<<<<<<<<<<<<
  *         else:
- *             item = item_
+ *             # Warning! Only works reliably for objects whose hash is based on value not memory address.
  */
-    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 383, __pyx_L1_error)
     __pyx_v_key.nhash = __pyx_t_7;
 
-    /* "pybloomfilter.pyx":343
+    /* "pybloomfilter.pyx":380
  *             key.shash = item
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):             # <<<<<<<<<<<<<<
  *             item = item_
  *             key.shash = item
  */
     goto __pyx_L3;
   }
 
-  /* "pybloomfilter.pyx":348
- *             key.nhash = len(item)
+  /* "pybloomfilter.pyx":386
  *         else:
+ *             # Warning! Only works reliably for objects whose hash is based on value not memory address.
  *             item = item_             # <<<<<<<<<<<<<<
  *             key.shash = NULL
  *             key.nhash = hash(item)
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_item_);
     __pyx_v_item = __pyx_v_item_;
 
-    /* "pybloomfilter.pyx":349
- *         else:
+    /* "pybloomfilter.pyx":387
+ *             # Warning! Only works reliably for objects whose hash is based on value not memory address.
  *             item = item_
  *             key.shash = NULL             # <<<<<<<<<<<<<<
  *             key.nhash = hash(item)
  *         return cbloomfilter.bloomfilter_Test(self._bf, &key) == 1
  */
     __pyx_v_key.shash = NULL;
 
-    /* "pybloomfilter.pyx":350
+    /* "pybloomfilter.pyx":388
  *             item = item_
  *             key.shash = NULL
  *             key.nhash = hash(item)             # <<<<<<<<<<<<<<
  *         return cbloomfilter.bloomfilter_Test(self._bf, &key) == 1
  * 
  */
-    __pyx_t_8 = PyObject_Hash(__pyx_v_item); if (unlikely(__pyx_t_8 == ((Py_hash_t)-1))) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Hash(__pyx_v_item); if (unlikely(__pyx_t_8 == ((Py_hash_t)-1))) __PYX_ERR(0, 388, __pyx_L1_error)
     __pyx_v_key.nhash = __pyx_t_8;
   }
   __pyx_L3:;
 
-  /* "pybloomfilter.pyx":351
+  /* "pybloomfilter.pyx":389
  *             key.shash = NULL
  *             key.nhash = hash(item)
  *         return cbloomfilter.bloomfilter_Test(self._bf, &key) == 1             # <<<<<<<<<<<<<<
  * 
  *     def copy_template(self, filename, perm=0755):
  */
   __pyx_r = (bloomfilter_Test(__pyx_v_self->_bf, (&__pyx_v_key)) == 1);
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":330
+  /* "pybloomfilter.pyx":367
  *         cbloomfilter.bloomfilter_Clear(self._bf)
  * 
  *     def __contains__(self, item_):             # <<<<<<<<<<<<<<
  *         """Checks to see if item is contained in the filter, with
  *         an acceptable false positive rate of :attr:`BloomFilter.error_rate`.
  */
 
@@ -6619,26 +7135,26 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":353
+/* "pybloomfilter.pyx":391
  *         return cbloomfilter.bloomfilter_Test(self._bf, &key) == 1
  * 
  *     def copy_template(self, filename, perm=0755):             # <<<<<<<<<<<<<<
  *         """Creates a new :class:`BloomFilter` object with the exact same parameters.
  *         Once this is performed, the two filters are comparable, so
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_23copy_template(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_22copy_template[] = "Creates a new :class:`BloomFilter` object with the exact same parameters.\n        Once this is performed, the two filters are comparable, so\n        you can perform set operations using logical operators.\n\n        :param str filename: new filename\n        :param int perm: file access permission flags\n        :rtype: :class:`BloomFilter`\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_23copy_template(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_25copy_template(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_24copy_template[] = "Creates a new :class:`BloomFilter` object with the exact same parameters.\n        Once this is performed, the two filters are comparable, so\n        you can perform set operations using logical operators.\n\n        :param str filename: new filename\n        :param int perm: file access permission flags\n        :rtype: :class:`BloomFilter`\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_25copy_template(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_perm = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6667,15 +7183,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_perm);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "copy_template") < 0)) __PYX_ERR(0, 353, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "copy_template") < 0)) __PYX_ERR(0, 391, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -6683,203 +7199,203 @@
       }
     }
     __pyx_v_filename = values[0];
     __pyx_v_perm = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("copy_template", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 353, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("copy_template", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 391, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybloomfilter.BloomFilter.copy_template", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_22copy_template(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_filename, __pyx_v_perm);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_24copy_template(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), __pyx_v_filename, __pyx_v_perm);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_22copy_template(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_24copy_template(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_perm) {
   struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_copy = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   char *__pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_template", 0);
 
-  /* "pybloomfilter.pyx":362
+  /* "pybloomfilter.pyx":400
  *         :rtype: :class:`BloomFilter`
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         cdef BloomFilter copy = BloomFilter(NoConstruct, 0)
  *         if os.path.exists(filename):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 362, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":363
+  /* "pybloomfilter.pyx":401
  *         """
  *         self._assert_open()
  *         cdef BloomFilter copy = BloomFilter(NoConstruct, 0)             # <<<<<<<<<<<<<<
  *         if os.path.exists(filename):
  *             os.unlink(filename)
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_13pybloomfilter_NoConstruct);
   __Pyx_GIVEREF(__pyx_v_13pybloomfilter_NoConstruct);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_13pybloomfilter_NoConstruct);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_0);
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_copy = ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":364
+  /* "pybloomfilter.pyx":402
  *         self._assert_open()
  *         cdef BloomFilter copy = BloomFilter(NoConstruct, 0)
  *         if os.path.exists(filename):             # <<<<<<<<<<<<<<
  *             os.unlink(filename)
  *         copy._bf = cbloomfilter.bloomfilter_Copy_Template(self._bf, filename.encode(), perm)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_exists); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_filename);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 364, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":365
+    /* "pybloomfilter.pyx":403
  *         cdef BloomFilter copy = BloomFilter(NoConstruct, 0)
  *         if os.path.exists(filename):
  *             os.unlink(filename)             # <<<<<<<<<<<<<<
  *         copy._bf = cbloomfilter.bloomfilter_Copy_Template(self._bf, filename.encode(), perm)
  *         return copy
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_os); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_unlink); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 365, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_unlink); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_filename);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pybloomfilter.pyx":364
+    /* "pybloomfilter.pyx":402
  *         self._assert_open()
  *         cdef BloomFilter copy = BloomFilter(NoConstruct, 0)
  *         if os.path.exists(filename):             # <<<<<<<<<<<<<<
  *             os.unlink(filename)
  *         copy._bf = cbloomfilter.bloomfilter_Copy_Template(self._bf, filename.encode(), perm)
  */
   }
 
-  /* "pybloomfilter.pyx":366
+  /* "pybloomfilter.pyx":404
  *         if os.path.exists(filename):
  *             os.unlink(filename)
  *         copy._bf = cbloomfilter.bloomfilter_Copy_Template(self._bf, filename.encode(), perm)             # <<<<<<<<<<<<<<
  *         return copy
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_perm); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsWritableString(__pyx_t_2); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_perm); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 404, __pyx_L1_error)
   __pyx_v_copy->_bf = bloomfilter_Copy_Template(__pyx_v_self->_bf, __pyx_t_5, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":367
+  /* "pybloomfilter.pyx":405
  *             os.unlink(filename)
  *         copy._bf = cbloomfilter.bloomfilter_Copy_Template(self._bf, filename.encode(), perm)
  *         return copy             # <<<<<<<<<<<<<<
  * 
  *     def copy(self, filename):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_copy));
   __pyx_r = ((PyObject *)__pyx_v_copy);
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":353
+  /* "pybloomfilter.pyx":391
  *         return cbloomfilter.bloomfilter_Test(self._bf, &key) == 1
  * 
  *     def copy_template(self, filename, perm=0755):             # <<<<<<<<<<<<<<
  *         """Creates a new :class:`BloomFilter` object with the exact same parameters.
  *         Once this is performed, the two filters are comparable, so
  */
 
@@ -6893,139 +7409,139 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_copy);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":369
+/* "pybloomfilter.pyx":407
  *         return copy
  * 
  *     def copy(self, filename):             # <<<<<<<<<<<<<<
  *         """Copies the current :class:`BloomFilter` object to another object
  *         with a new filename.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_25copy(PyObject *__pyx_v_self, PyObject *__pyx_v_filename); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_24copy[] = "Copies the current :class:`BloomFilter` object to another object\n        with a new filename.\n\n        :param str filename: new filename\n        :rtype: :class:`BloomFilter`\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_25copy(PyObject *__pyx_v_self, PyObject *__pyx_v_filename) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_27copy(PyObject *__pyx_v_self, PyObject *__pyx_v_filename); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_26copy[] = "Copies the current :class:`BloomFilter` object to another object\n        with a new filename.\n\n        :param str filename: new filename\n        :rtype: :class:`BloomFilter`\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_27copy(PyObject *__pyx_v_self, PyObject *__pyx_v_filename) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_24copy(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_filename));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_26copy(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_filename));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_24copy(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_26copy(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_filename) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "pybloomfilter.pyx":376
+  /* "pybloomfilter.pyx":414
  *         :rtype: :class:`BloomFilter`
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         if self._in_memory:
  *             raise NotImplementedError('Cannot call .copy on an in-memory %s' %
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":377
+  /* "pybloomfilter.pyx":415
  *         """
  *         self._assert_open()
  *         if self._in_memory:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError('Cannot call .copy on an in-memory %s' %
  *                                       self.__class__.__name__)
  */
   __pyx_t_4 = (__pyx_v_self->_in_memory != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pybloomfilter.pyx":379
+    /* "pybloomfilter.pyx":417
  *         if self._in_memory:
  *             raise NotImplementedError('Cannot call .copy on an in-memory %s' %
  *                                       self.__class__.__name__)             # <<<<<<<<<<<<<<
  *         shutil.copy(self._bf.array.filename, filename)
  *         return self.open(filename)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pybloomfilter.pyx":378
+    /* "pybloomfilter.pyx":416
  *         self._assert_open()
  *         if self._in_memory:
  *             raise NotImplementedError('Cannot call .copy on an in-memory %s' %             # <<<<<<<<<<<<<<
  *                                       self.__class__.__name__)
  *         shutil.copy(self._bf.array.filename, filename)
  */
-    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Cannot_call_copy_on_an_in_memory, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Cannot_call_copy_on_an_in_memory, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_NotImplementedError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 378, __pyx_L1_error)
+    __PYX_ERR(0, 416, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":377
+    /* "pybloomfilter.pyx":415
  *         """
  *         self._assert_open()
  *         if self._in_memory:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError('Cannot call .copy on an in-memory %s' %
  *                                       self.__class__.__name__)
  */
   }
 
-  /* "pybloomfilter.pyx":380
+  /* "pybloomfilter.pyx":418
  *             raise NotImplementedError('Cannot call .copy on an in-memory %s' %
  *                                       self.__class__.__name__)
  *         shutil.copy(self._bf.array.filename, filename)             # <<<<<<<<<<<<<<
  *         return self.open(filename)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_shutil); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_shutil); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_copy); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->_bf->array->filename); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 380, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->_bf->array->filename); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7034,78 +7550,78 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_filename};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_filename};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_1);
     __Pyx_INCREF(__pyx_v_filename);
     __Pyx_GIVEREF(__pyx_v_filename);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_filename);
     __pyx_t_1 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 380, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":381
+  /* "pybloomfilter.pyx":419
  *                                       self.__class__.__name__)
  *         shutil.copy(self._bf.array.filename, filename)
  *         return self.open(filename)             # <<<<<<<<<<<<<<
  * 
  *     def add(self, item_):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_open); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_open); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_filename);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 381, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":369
+  /* "pybloomfilter.pyx":407
  *         return copy
  * 
  *     def copy(self, filename):             # <<<<<<<<<<<<<<
  *         """Copies the current :class:`BloomFilter` object to another object
  *         with a new filename.
  */
 
@@ -7120,37 +7636,37 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":383
+/* "pybloomfilter.pyx":421
  *         return self.open(filename)
  * 
  *     def add(self, item_):             # <<<<<<<<<<<<<<
  *         """Adds an item to the Bloom filter. Returns a boolean indicating whether
  *         this item was present in the Bloom filter prior to adding
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_27add(PyObject *__pyx_v_self, PyObject *__pyx_v_item_); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_26add[] = "Adds an item to the Bloom filter. Returns a boolean indicating whether\n        this item was present in the Bloom filter prior to adding\n        (see :meth:`BloomFilter.__contains__`).\n\n        :param item: hashable object\n        :rtype: bool\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_27add(PyObject *__pyx_v_self, PyObject *__pyx_v_item_) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_29add(PyObject *__pyx_v_self, PyObject *__pyx_v_item_); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_28add[] = "Adds an item to the Bloom filter. Returns a boolean indicating whether\n        this item was present in the Bloom filter prior to adding\n        (see :meth:`BloomFilter.__contains__`).\n\n        :param item: hashable object\n        :rtype: bool\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_29add(PyObject *__pyx_v_self, PyObject *__pyx_v_item_) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_26add(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_item_));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_28add(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_item_));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_26add(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_28add(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_item_) {
   Key __pyx_v_key;
   PyObject *__pyx_v_item = NULL;
   int __pyx_v_result;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -7161,277 +7677,277 @@
   Py_ssize_t __pyx_t_7;
   Py_hash_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
 
-  /* "pybloomfilter.pyx":391
+  /* "pybloomfilter.pyx":429
  *         :rtype: bool
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_writable()
  *         cdef cbloomfilter.Key key
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":392
+  /* "pybloomfilter.pyx":430
  *         """
  *         self._assert_open()
  *         self._assert_writable()             # <<<<<<<<<<<<<<
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":394
+  /* "pybloomfilter.pyx":432
  *         self._assert_writable()
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):             # <<<<<<<<<<<<<<
  *             item = item_.encode()
  *             key.shash = item
  */
   __pyx_t_4 = PyUnicode_Check(__pyx_v_item_); 
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "pybloomfilter.pyx":395
+    /* "pybloomfilter.pyx":433
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):
  *             item = item_.encode()             # <<<<<<<<<<<<<<
  *             key.shash = item
  *             key.nhash = len(item)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_item_, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 395, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_item_, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 395, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_item = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "pybloomfilter.pyx":396
+    /* "pybloomfilter.pyx":434
  *         if isinstance(item_, str):
  *             item = item_.encode()
  *             key.shash = item             # <<<<<<<<<<<<<<
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):
  */
-    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 434, __pyx_L1_error)
     __pyx_v_key.shash = __pyx_t_6;
 
-    /* "pybloomfilter.pyx":397
+    /* "pybloomfilter.pyx":435
  *             item = item_.encode()
  *             key.shash = item
  *             key.nhash = len(item)             # <<<<<<<<<<<<<<
  *         elif isinstance(item_, bytes):
  *             item = item_
  */
-    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 397, __pyx_L1_error)
+    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 435, __pyx_L1_error)
     __pyx_v_key.nhash = __pyx_t_7;
 
-    /* "pybloomfilter.pyx":394
+    /* "pybloomfilter.pyx":432
  *         self._assert_writable()
  *         cdef cbloomfilter.Key key
  *         if isinstance(item_, str):             # <<<<<<<<<<<<<<
  *             item = item_.encode()
  *             key.shash = item
  */
     goto __pyx_L3;
   }
 
-  /* "pybloomfilter.pyx":398
+  /* "pybloomfilter.pyx":436
  *             key.shash = item
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):             # <<<<<<<<<<<<<<
  *             item = item_
  *             key.shash = item
  */
   __pyx_t_5 = PyBytes_Check(__pyx_v_item_); 
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":399
+    /* "pybloomfilter.pyx":437
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):
  *             item = item_             # <<<<<<<<<<<<<<
  *             key.shash = item
  *             key.nhash = len(item)
  */
     __Pyx_INCREF(__pyx_v_item_);
     __pyx_v_item = __pyx_v_item_;
 
-    /* "pybloomfilter.pyx":400
+    /* "pybloomfilter.pyx":438
  *         elif isinstance(item_, bytes):
  *             item = item_
  *             key.shash = item             # <<<<<<<<<<<<<<
  *             key.nhash = len(item)
  *         else:
  */
-    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_item); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 438, __pyx_L1_error)
     __pyx_v_key.shash = __pyx_t_6;
 
-    /* "pybloomfilter.pyx":401
+    /* "pybloomfilter.pyx":439
  *             item = item_
  *             key.shash = item
  *             key.nhash = len(item)             # <<<<<<<<<<<<<<
  *         else:
  *             item = item_
  */
-    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_7 = PyObject_Length(__pyx_v_item); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 439, __pyx_L1_error)
     __pyx_v_key.nhash = __pyx_t_7;
 
-    /* "pybloomfilter.pyx":398
+    /* "pybloomfilter.pyx":436
  *             key.shash = item
  *             key.nhash = len(item)
  *         elif isinstance(item_, bytes):             # <<<<<<<<<<<<<<
  *             item = item_
  *             key.shash = item
  */
     goto __pyx_L3;
   }
 
-  /* "pybloomfilter.pyx":403
+  /* "pybloomfilter.pyx":441
  *             key.nhash = len(item)
  *         else:
  *             item = item_             # <<<<<<<<<<<<<<
  *             key.shash = NULL
  *             key.nhash = hash(item)
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_item_);
     __pyx_v_item = __pyx_v_item_;
 
-    /* "pybloomfilter.pyx":404
+    /* "pybloomfilter.pyx":442
  *         else:
  *             item = item_
  *             key.shash = NULL             # <<<<<<<<<<<<<<
  *             key.nhash = hash(item)
  * 
  */
     __pyx_v_key.shash = NULL;
 
-    /* "pybloomfilter.pyx":405
+    /* "pybloomfilter.pyx":443
  *             item = item_
  *             key.shash = NULL
  *             key.nhash = hash(item)             # <<<<<<<<<<<<<<
  * 
  *         result = cbloomfilter.bloomfilter_Add(self._bf, &key)
  */
-    __pyx_t_8 = PyObject_Hash(__pyx_v_item); if (unlikely(__pyx_t_8 == ((Py_hash_t)-1))) __PYX_ERR(0, 405, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Hash(__pyx_v_item); if (unlikely(__pyx_t_8 == ((Py_hash_t)-1))) __PYX_ERR(0, 443, __pyx_L1_error)
     __pyx_v_key.nhash = __pyx_t_8;
   }
   __pyx_L3:;
 
-  /* "pybloomfilter.pyx":407
+  /* "pybloomfilter.pyx":445
  *             key.nhash = hash(item)
  * 
  *         result = cbloomfilter.bloomfilter_Add(self._bf, &key)             # <<<<<<<<<<<<<<
  *         if result == 2:
  *             raise RuntimeError("Some problem occured while trying to add key.")
  */
   __pyx_v_result = bloomfilter_Add(__pyx_v_self->_bf, (&__pyx_v_key));
 
-  /* "pybloomfilter.pyx":408
+  /* "pybloomfilter.pyx":446
  * 
  *         result = cbloomfilter.bloomfilter_Add(self._bf, &key)
  *         if result == 2:             # <<<<<<<<<<<<<<
  *             raise RuntimeError("Some problem occured while trying to add key.")
  *         return bool(result)
  */
   __pyx_t_4 = ((__pyx_v_result == 2) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "pybloomfilter.pyx":409
+    /* "pybloomfilter.pyx":447
  *         result = cbloomfilter.bloomfilter_Add(self._bf, &key)
  *         if result == 2:
  *             raise RuntimeError("Some problem occured while trying to add key.")             # <<<<<<<<<<<<<<
  *         return bool(result)
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 409, __pyx_L1_error)
+    __PYX_ERR(0, 447, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":408
+    /* "pybloomfilter.pyx":446
  * 
  *         result = cbloomfilter.bloomfilter_Add(self._bf, &key)
  *         if result == 2:             # <<<<<<<<<<<<<<
  *             raise RuntimeError("Some problem occured while trying to add key.")
  *         return bool(result)
  */
   }
 
-  /* "pybloomfilter.pyx":410
+  /* "pybloomfilter.pyx":448
  *         if result == 2:
  *             raise RuntimeError("Some problem occured while trying to add key.")
  *         return bool(result)             # <<<<<<<<<<<<<<
  * 
  *     def update(self, iterable):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_result); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_4))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 410, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_4))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":383
+  /* "pybloomfilter.pyx":421
  *         return self.open(filename)
  * 
  *     def add(self, item_):             # <<<<<<<<<<<<<<
  *         """Adds an item to the Bloom filter. Returns a boolean indicating whether
  *         this item was present in the Bloom filter prior to adding
  */
 
@@ -7445,137 +7961,137 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":412
+/* "pybloomfilter.pyx":450
  *         return bool(result)
  * 
  *     def update(self, iterable):             # <<<<<<<<<<<<<<
  *         """Calls :meth:`BloomFilter.add` on all items in the iterable."""
  *         for item in iterable:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_29update(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_28update[] = "Calls :meth:`BloomFilter.add` on all items in the iterable.";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_29update(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_31update(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_30update[] = "Calls :meth:`BloomFilter.add` on all items in the iterable.";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_31update(PyObject *__pyx_v_self, PyObject *__pyx_v_iterable) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("update (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_28update(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_iterable));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_30update(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v_iterable));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_28update(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_iterable) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_30update(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, PyObject *__pyx_v_iterable) {
   PyObject *__pyx_v_item = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("update", 0);
 
-  /* "pybloomfilter.pyx":414
+  /* "pybloomfilter.pyx":452
  *     def update(self, iterable):
  *         """Calls :meth:`BloomFilter.add` on all items in the iterable."""
  *         for item in iterable:             # <<<<<<<<<<<<<<
  *             self.add(item)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_iterable)) || PyTuple_CheckExact(__pyx_v_iterable)) {
     __pyx_t_1 = __pyx_v_iterable; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_iterable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_iterable); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 452, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 452, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 452, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 452, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 414, __pyx_L1_error)
+          else __PYX_ERR(0, 452, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pybloomfilter.pyx":415
+    /* "pybloomfilter.pyx":453
  *         """Calls :meth:`BloomFilter.add` on all items in the iterable."""
  *         for item in iterable:
  *             self.add(item)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_item) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_item);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pybloomfilter.pyx":414
+    /* "pybloomfilter.pyx":452
  *     def update(self, iterable):
  *         """Calls :meth:`BloomFilter.add` on all items in the iterable."""
  *         for item in iterable:             # <<<<<<<<<<<<<<
  *             self.add(item)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":412
+  /* "pybloomfilter.pyx":450
  *         return bool(result)
  * 
  *     def update(self, iterable):             # <<<<<<<<<<<<<<
  *         """Calls :meth:`BloomFilter.add` on all items in the iterable."""
  *         for item in iterable:
  */
 
@@ -7592,122 +8108,122 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":417
+/* "pybloomfilter.pyx":455
  *             self.add(item)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         """Returns the number of distinct elements that have been
  *         added to the :class:`BloomFilter` object, subject to the error
  */
 
 /* Python wrapper */
-static Py_ssize_t __pyx_pw_13pybloomfilter_11BloomFilter_31__len__(PyObject *__pyx_v_self); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_30__len__[] = "Returns the number of distinct elements that have been\n        added to the :class:`BloomFilter` object, subject to the error\n        given in :attr:`BloomFilter.error_rate`.\n\n        The length reported here is exact as long as no set `union` or\n        `intersection` were performed. Otherwise we report an approximation\n        of based on :attr:`BloomFilter.bit_count`.\n\n        :param item: hashable object\n        :rtype: int\n        ";
+static Py_ssize_t __pyx_pw_13pybloomfilter_11BloomFilter_33__len__(PyObject *__pyx_v_self); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_32__len__[] = "Returns the number of distinct elements that have been\n        added to the :class:`BloomFilter` object, subject to the error\n        given in :attr:`BloomFilter.error_rate`.\n\n        The length reported here is exact as long as no set `union` or\n        `intersection` were performed. Otherwise we report an approximation\n        of based on :attr:`BloomFilter.bit_count`.\n\n        :param item: hashable object\n        :rtype: int\n        ";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_30__len__;
+struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_32__len__;
 #endif
-static Py_ssize_t __pyx_pw_13pybloomfilter_11BloomFilter_31__len__(PyObject *__pyx_v_self) {
+static Py_ssize_t __pyx_pw_13pybloomfilter_11BloomFilter_33__len__(PyObject *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_30__len__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_32__len__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static Py_ssize_t __pyx_pf_13pybloomfilter_11BloomFilter_30__len__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static Py_ssize_t __pyx_pf_13pybloomfilter_11BloomFilter_32__len__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "pybloomfilter.pyx":429
+  /* "pybloomfilter.pyx":467
  *         :rtype: int
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         if not self._bf.count_correct:
  *             return self.approx_len
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":430
+  /* "pybloomfilter.pyx":468
  *         """
  *         self._assert_open()
  *         if not self._bf.count_correct:             # <<<<<<<<<<<<<<
  *             return self.approx_len
  *         return self._bf.elem_count
  */
   __pyx_t_4 = ((!(__pyx_v_self->_bf->count_correct != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "pybloomfilter.pyx":431
+    /* "pybloomfilter.pyx":469
  *         self._assert_open()
  *         if not self._bf.count_correct:
  *             return self.approx_len             # <<<<<<<<<<<<<<
  *         return self._bf.elem_count
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_approx_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_approx_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_5;
     goto __pyx_L0;
 
-    /* "pybloomfilter.pyx":430
+    /* "pybloomfilter.pyx":468
  *         """
  *         self._assert_open()
  *         if not self._bf.count_correct:             # <<<<<<<<<<<<<<
  *             return self.approx_len
  *         return self._bf.elem_count
  */
   }
 
-  /* "pybloomfilter.pyx":432
+  /* "pybloomfilter.pyx":470
  *         if not self._bf.count_correct:
  *             return self.approx_len
  *         return self._bf.elem_count             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
   __pyx_r = __pyx_v_self->_bf->elem_count;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":417
+  /* "pybloomfilter.pyx":455
  *             self.add(item)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         """Returns the number of distinct elements that have been
  *         added to the :class:`BloomFilter` object, subject to the error
  */
 
@@ -7719,279 +8235,279 @@
   __Pyx_AddTraceback("pybloomfilter.BloomFilter.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":434
+/* "pybloomfilter.pyx":472
  *         return self._bf.elem_count
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """Closes the currently opened :class:`BloomFilter` file descriptor.
  *         Following accesses to this instance will raise a :class:`ValueError`.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_33close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_32close[] = "Closes the currently opened :class:`BloomFilter` file descriptor.\n        Following accesses to this instance will raise a :class:`ValueError`.\n\n        *Caution*: this will delete an in-memory filter irrecoverably!\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_33close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_35close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_34close[] = "Closes the currently opened :class:`BloomFilter` file descriptor.\n        Following accesses to this instance will raise a :class:`ValueError`.\n\n        *Caution*: this will delete an in-memory filter irrecoverably!\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_35close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_32close(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_34close(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_32close(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_34close(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pybloomfilter.pyx":440
+  /* "pybloomfilter.pyx":478
  *         *Caution*: this will delete an in-memory filter irrecoverably!
  *         """
  *         if self._closed == 0:             # <<<<<<<<<<<<<<
  *             self._closed = 1
  *             cbloomfilter.bloomfilter_Destroy(self._bf)
  */
   __pyx_t_1 = ((__pyx_v_self->_closed == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "pybloomfilter.pyx":441
+    /* "pybloomfilter.pyx":479
  *         """
  *         if self._closed == 0:
  *             self._closed = 1             # <<<<<<<<<<<<<<
  *             cbloomfilter.bloomfilter_Destroy(self._bf)
  *             self._bf = NULL
  */
     __pyx_v_self->_closed = 1;
 
-    /* "pybloomfilter.pyx":442
+    /* "pybloomfilter.pyx":480
  *         if self._closed == 0:
  *             self._closed = 1
  *             cbloomfilter.bloomfilter_Destroy(self._bf)             # <<<<<<<<<<<<<<
  *             self._bf = NULL
  * 
  */
     bloomfilter_Destroy(__pyx_v_self->_bf);
 
-    /* "pybloomfilter.pyx":443
+    /* "pybloomfilter.pyx":481
  *             self._closed = 1
  *             cbloomfilter.bloomfilter_Destroy(self._bf)
  *             self._bf = NULL             # <<<<<<<<<<<<<<
  * 
  *     def union(self, BloomFilter other):
  */
     __pyx_v_self->_bf = NULL;
 
-    /* "pybloomfilter.pyx":440
+    /* "pybloomfilter.pyx":478
  *         *Caution*: this will delete an in-memory filter irrecoverably!
  *         """
  *         if self._closed == 0:             # <<<<<<<<<<<<<<
  *             self._closed = 1
  *             cbloomfilter.bloomfilter_Destroy(self._bf)
  */
   }
 
-  /* "pybloomfilter.pyx":434
+  /* "pybloomfilter.pyx":472
  *         return self._bf.elem_count
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """Closes the currently opened :class:`BloomFilter` file descriptor.
  *         Following accesses to this instance will raise a :class:`ValueError`.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":445
+/* "pybloomfilter.pyx":483
  *             self._bf = NULL
  * 
  *     def union(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """Performs a set OR with another comparable filter. You can (only) construct
  *         comparable filters with :meth:`BloomFilter.copy_template` above.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_35union(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_34union[] = "Performs a set OR with another comparable filter. You can (only) construct\n        comparable filters with :meth:`BloomFilter.copy_template` above.\n\n        The computation will occur *in place*. That is, calling::\n\n            >>> bf.union(bf2)\n\n        is a way of adding *all* the elements of ``bf2`` to ``bf``.\n\n        *NB: Calling this function will render future calls to len()\n        invalid.*\n\n        :param BloomFilter other: filter to perform the union with\n        :rtype: :class:`BloomFilter`\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_35union(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_37union(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_36union[] = "Performs a set OR with another comparable filter. You can (only) construct\n        comparable filters with :meth:`BloomFilter.copy_template` above.\n\n        The computation will occur *in place*. That is, calling::\n\n            >>> bf.union(bf2)\n\n        is a way of adding *all* the elements of ``bf2`` to ``bf``.\n\n        *NB: Calling this function will render future calls to len()\n        invalid.*\n\n        :param BloomFilter other: filter to perform the union with\n        :rtype: :class:`BloomFilter`\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_37union(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("union (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 445, __pyx_L1_error)
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_34union(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_36union(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_34union(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_36union(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("union", 0);
 
-  /* "pybloomfilter.pyx":461
+  /* "pybloomfilter.pyx":499
  *         :rtype: :class:`BloomFilter`
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_writable()
  *         other._assert_open()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":462
+  /* "pybloomfilter.pyx":500
  *         """
  *         self._assert_open()
  *         self._assert_writable()             # <<<<<<<<<<<<<<
  *         other._assert_open()
  *         self._assert_comparable(other)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":463
+  /* "pybloomfilter.pyx":501
  *         self._assert_open()
  *         self._assert_writable()
  *         other._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_comparable(other)
  *         cbloomfilter.mbarray_Or(self._bf.array, other._bf.array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":464
+  /* "pybloomfilter.pyx":502
  *         self._assert_writable()
  *         other._assert_open()
  *         self._assert_comparable(other)             # <<<<<<<<<<<<<<
  *         cbloomfilter.mbarray_Or(self._bf.array, other._bf.array)
  *         self._bf.count_correct = 0
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_comparable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_comparable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_other)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_other));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":465
+  /* "pybloomfilter.pyx":503
  *         other._assert_open()
  *         self._assert_comparable(other)
  *         cbloomfilter.mbarray_Or(self._bf.array, other._bf.array)             # <<<<<<<<<<<<<<
  *         self._bf.count_correct = 0
  *         return self
  */
   (void)(mbarray_Or(__pyx_v_self->_bf->array, __pyx_v_other->_bf->array));
 
-  /* "pybloomfilter.pyx":466
+  /* "pybloomfilter.pyx":504
  *         self._assert_comparable(other)
  *         cbloomfilter.mbarray_Or(self._bf.array, other._bf.array)
  *         self._bf.count_correct = 0             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->_bf->count_correct = 0;
 
-  /* "pybloomfilter.pyx":467
+  /* "pybloomfilter.pyx":505
  *         cbloomfilter.mbarray_Or(self._bf.array, other._bf.array)
  *         self._bf.count_correct = 0
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __ior__(self, BloomFilter other):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":445
+  /* "pybloomfilter.pyx":483
  *             self._bf = NULL
  * 
  *     def union(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """Performs a set OR with another comparable filter. You can (only) construct
  *         comparable filters with :meth:`BloomFilter.copy_template` above.
  */
 
@@ -8004,88 +8520,88 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":469
+/* "pybloomfilter.pyx":507
  *         return self
  * 
  *     def __ior__(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """See :meth:`BloomFilter.union`."""
  *         return self.union(other)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_37__ior__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_36__ior__[] = "See :meth:`BloomFilter.union`.";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_39__ior__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_38__ior__[] = "See :meth:`BloomFilter.union`.";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_36__ior__;
+struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_38__ior__;
 #endif
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_37__ior__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_39__ior__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__ior__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 469, __pyx_L1_error)
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_36__ior__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_38__ior__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_36__ior__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_38__ior__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__ior__", 0);
 
-  /* "pybloomfilter.pyx":471
+  /* "pybloomfilter.pyx":509
  *     def __ior__(self, BloomFilter other):
  *         """See :meth:`BloomFilter.union`."""
  *         return self.union(other)             # <<<<<<<<<<<<<<
  * 
  *     def intersection(self, BloomFilter other):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_union); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_other)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_other));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":469
+  /* "pybloomfilter.pyx":507
  *         return self
  * 
  *     def __ior__(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """See :meth:`BloomFilter.union`."""
  *         return self.union(other)
  */
 
@@ -8098,190 +8614,190 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":473
+/* "pybloomfilter.pyx":511
  *         return self.union(other)
  * 
  *     def intersection(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """The same as :meth:`BloomFilter.union` above except it uses
  *         a set AND instead of a set OR.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_39intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_38intersection[] = "The same as :meth:`BloomFilter.union` above except it uses\n        a set AND instead of a set OR.\n\n        *NB: Calling this function will render future calls to len()\n        invalid.*\n\n        :param BloomFilter other: filter to perform the intersection with\n        :rtype: :class:`BloomFilter`\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_39intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_41intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_40intersection[] = "The same as :meth:`BloomFilter.union` above except it uses\n        a set AND instead of a set OR.\n\n        *NB: Calling this function will render future calls to len()\n        invalid.*\n\n        :param BloomFilter other: filter to perform the intersection with\n        :rtype: :class:`BloomFilter`\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_41intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersection (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 473, __pyx_L1_error)
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_38intersection(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_40intersection(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_38intersection(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_40intersection(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("intersection", 0);
 
-  /* "pybloomfilter.pyx":483
+  /* "pybloomfilter.pyx":521
  *         :rtype: :class:`BloomFilter`
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_writable()
  *         other._assert_open()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":484
+  /* "pybloomfilter.pyx":522
  *         """
  *         self._assert_open()
  *         self._assert_writable()             # <<<<<<<<<<<<<<
  *         other._assert_open()
  *         self._assert_comparable(other)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_writable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":485
+  /* "pybloomfilter.pyx":523
  *         self._assert_open()
  *         self._assert_writable()
  *         other._assert_open()             # <<<<<<<<<<<<<<
  *         self._assert_comparable(other)
  *         cbloomfilter.mbarray_And(self._bf.array, other._bf.array)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 485, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":486
+  /* "pybloomfilter.pyx":524
  *         self._assert_writable()
  *         other._assert_open()
  *         self._assert_comparable(other)             # <<<<<<<<<<<<<<
  *         cbloomfilter.mbarray_And(self._bf.array, other._bf.array)
  *         self._bf.count_correct = 0
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_comparable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_comparable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_other)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_other));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":487
+  /* "pybloomfilter.pyx":525
  *         other._assert_open()
  *         self._assert_comparable(other)
  *         cbloomfilter.mbarray_And(self._bf.array, other._bf.array)             # <<<<<<<<<<<<<<
  *         self._bf.count_correct = 0
  *         return self
  */
   (void)(mbarray_And(__pyx_v_self->_bf->array, __pyx_v_other->_bf->array));
 
-  /* "pybloomfilter.pyx":488
+  /* "pybloomfilter.pyx":526
  *         self._assert_comparable(other)
  *         cbloomfilter.mbarray_And(self._bf.array, other._bf.array)
  *         self._bf.count_correct = 0             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->_bf->count_correct = 0;
 
-  /* "pybloomfilter.pyx":489
+  /* "pybloomfilter.pyx":527
  *         cbloomfilter.mbarray_And(self._bf.array, other._bf.array)
  *         self._bf.count_correct = 0
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __iand__(self, BloomFilter other):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":473
+  /* "pybloomfilter.pyx":511
  *         return self.union(other)
  * 
  *     def intersection(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """The same as :meth:`BloomFilter.union` above except it uses
  *         a set AND instead of a set OR.
  */
 
@@ -8294,88 +8810,88 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":491
+/* "pybloomfilter.pyx":529
  *         return self
  * 
  *     def __iand__(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """See :meth:`BloomFilter.intersection`."""
  *         return self.intersection(other)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_41__iand__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_40__iand__[] = "See :meth:`BloomFilter.intersection`.";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_43__iand__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_42__iand__[] = "See :meth:`BloomFilter.intersection`.";
 #if CYTHON_UPDATE_DESCRIPTOR_DOC
-struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_40__iand__;
+struct wrapperbase __pyx_wrapperbase_13pybloomfilter_11BloomFilter_42__iand__;
 #endif
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_41__iand__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_43__iand__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iand__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 491, __pyx_L1_error)
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_40__iand__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 529, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_42__iand__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_40__iand__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_42__iand__(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iand__", 0);
 
-  /* "pybloomfilter.pyx":493
+  /* "pybloomfilter.pyx":531
  *     def __iand__(self, BloomFilter other):
  *         """See :meth:`BloomFilter.intersection`."""
  *         return self.intersection(other)             # <<<<<<<<<<<<<<
  * 
  *     def _assert_open(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_intersection); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_intersection); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_other)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_other));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":491
+  /* "pybloomfilter.pyx":529
  *         return self
  * 
  *     def __iand__(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         """See :meth:`BloomFilter.intersection`."""
  *         return self.intersection(other)
  */
 
@@ -8388,78 +8904,78 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":495
+/* "pybloomfilter.pyx":533
  *         return self.intersection(other)
  * 
  *     def _assert_open(self):             # <<<<<<<<<<<<<<
  *         if self._closed != 0:
  *             raise ValueError("I/O operation on closed file")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_43_assert_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_43_assert_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_45_assert_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_45_assert_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_assert_open (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_42_assert_open(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_44_assert_open(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_42_assert_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_44_assert_open(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_assert_open", 0);
 
-  /* "pybloomfilter.pyx":496
+  /* "pybloomfilter.pyx":534
  * 
  *     def _assert_open(self):
  *         if self._closed != 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("I/O operation on closed file")
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->_closed != 0) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pybloomfilter.pyx":497
+    /* "pybloomfilter.pyx":535
  *     def _assert_open(self):
  *         if self._closed != 0:
  *             raise ValueError("I/O operation on closed file")             # <<<<<<<<<<<<<<
  * 
  *     def _assert_writable(self):
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 497, __pyx_L1_error)
+    __PYX_ERR(0, 535, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":496
+    /* "pybloomfilter.pyx":534
  * 
  *     def _assert_open(self):
  *         if self._closed != 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("I/O operation on closed file")
  * 
  */
   }
 
-  /* "pybloomfilter.pyx":495
+  /* "pybloomfilter.pyx":533
  *         return self.intersection(other)
  * 
  *     def _assert_open(self):             # <<<<<<<<<<<<<<
  *         if self._closed != 0:
  *             raise ValueError("I/O operation on closed file")
  */
 
@@ -8472,81 +8988,81 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":499
+/* "pybloomfilter.pyx":537
  *             raise ValueError("I/O operation on closed file")
  * 
  *     def _assert_writable(self):             # <<<<<<<<<<<<<<
  *         if self.read_only:
  *             raise ValueError("Write operation on read-only file")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_45_assert_writable(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_45_assert_writable(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_47_assert_writable(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_47_assert_writable(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_assert_writable (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_44_assert_writable(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_46_assert_writable(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_44_assert_writable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_46_assert_writable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_assert_writable", 0);
 
-  /* "pybloomfilter.pyx":500
+  /* "pybloomfilter.pyx":538
  * 
  *     def _assert_writable(self):
  *         if self.read_only:             # <<<<<<<<<<<<<<
  *             raise ValueError("Write operation on read-only file")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_only); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_read_only); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "pybloomfilter.pyx":501
+    /* "pybloomfilter.pyx":539
  *     def _assert_writable(self):
  *         if self.read_only:
  *             raise ValueError("Write operation on read-only file")             # <<<<<<<<<<<<<<
  * 
  *     def _assert_comparable(self, BloomFilter other):
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 501, __pyx_L1_error)
+    __PYX_ERR(0, 539, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":500
+    /* "pybloomfilter.pyx":538
  * 
  *     def _assert_writable(self):
  *         if self.read_only:             # <<<<<<<<<<<<<<
  *             raise ValueError("Write operation on read-only file")
  * 
  */
   }
 
-  /* "pybloomfilter.pyx":499
+  /* "pybloomfilter.pyx":537
  *             raise ValueError("I/O operation on closed file")
  * 
  *     def _assert_writable(self):             # <<<<<<<<<<<<<<
  *         if self.read_only:
  *             raise ValueError("Write operation on read-only file")
  */
 
@@ -8559,163 +9075,163 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":503
+/* "pybloomfilter.pyx":541
  *             raise ValueError("Write operation on read-only file")
  * 
  *     def _assert_comparable(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         error = ValueError("The two %s objects are not the same type (hint: "
  *                            "use copy_template)" % self.__class__.__name__)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_47_assert_comparable(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_47_assert_comparable(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_49_assert_comparable(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_49_assert_comparable(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_assert_comparable (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 503, __pyx_L1_error)
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_46_assert_comparable(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_13pybloomfilter_BloomFilter, 1, "other", 0))) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_48_assert_comparable(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_46_assert_comparable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_48_assert_comparable(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_other) {
   PyObject *__pyx_v_error = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_assert_comparable", 0);
 
-  /* "pybloomfilter.pyx":505
+  /* "pybloomfilter.pyx":543
  *     def _assert_comparable(self, BloomFilter other):
  *         error = ValueError("The two %s objects are not the same type (hint: "
  *                            "use copy_template)" % self.__class__.__name__)             # <<<<<<<<<<<<<<
  *         if self._bf.array.bits != other._bf.array.bits:
  *             raise error
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_The_two_s_objects_are_not_the_sa, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_The_two_s_objects_are_not_the_sa, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":504
+  /* "pybloomfilter.pyx":542
  * 
  *     def _assert_comparable(self, BloomFilter other):
  *         error = ValueError("The two %s objects are not the same type (hint: "             # <<<<<<<<<<<<<<
  *                            "use copy_template)" % self.__class__.__name__)
  *         if self._bf.array.bits != other._bf.array.bits:
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_error = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":506
+  /* "pybloomfilter.pyx":544
  *         error = ValueError("The two %s objects are not the same type (hint: "
  *                            "use copy_template)" % self.__class__.__name__)
  *         if self._bf.array.bits != other._bf.array.bits:             # <<<<<<<<<<<<<<
  *             raise error
  *         if self.hash_seeds != other.hash_seeds:
  */
   __pyx_t_3 = ((__pyx_v_self->_bf->array->bits != __pyx_v_other->_bf->array->bits) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "pybloomfilter.pyx":507
+    /* "pybloomfilter.pyx":545
  *                            "use copy_template)" % self.__class__.__name__)
  *         if self._bf.array.bits != other._bf.array.bits:
  *             raise error             # <<<<<<<<<<<<<<
  *         if self.hash_seeds != other.hash_seeds:
  *             raise error
  */
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(0, 507, __pyx_L1_error)
+    __PYX_ERR(0, 545, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":506
+    /* "pybloomfilter.pyx":544
  *         error = ValueError("The two %s objects are not the same type (hint: "
  *                            "use copy_template)" % self.__class__.__name__)
  *         if self._bf.array.bits != other._bf.array.bits:             # <<<<<<<<<<<<<<
  *             raise error
  *         if self.hash_seeds != other.hash_seeds:
  */
   }
 
-  /* "pybloomfilter.pyx":508
+  /* "pybloomfilter.pyx":546
  *         if self._bf.array.bits != other._bf.array.bits:
  *             raise error
  *         if self.hash_seeds != other.hash_seeds:             # <<<<<<<<<<<<<<
  *             raise error
  *         return
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_hash_seeds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_hash_seeds); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_hash_seeds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_hash_seeds); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "pybloomfilter.pyx":509
+    /* "pybloomfilter.pyx":547
  *             raise error
  *         if self.hash_seeds != other.hash_seeds:
  *             raise error             # <<<<<<<<<<<<<<
  *         return
  * 
  */
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(0, 509, __pyx_L1_error)
+    __PYX_ERR(0, 547, __pyx_L1_error)
 
-    /* "pybloomfilter.pyx":508
+    /* "pybloomfilter.pyx":546
  *         if self._bf.array.bits != other._bf.array.bits:
  *             raise error
  *         if self.hash_seeds != other.hash_seeds:             # <<<<<<<<<<<<<<
  *             raise error
  *         return
  */
   }
 
-  /* "pybloomfilter.pyx":510
+  /* "pybloomfilter.pyx":548
  *         if self.hash_seeds != other.hash_seeds:
  *             raise error
  *         return             # <<<<<<<<<<<<<<
  * 
  *     def to_base64(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":503
+  /* "pybloomfilter.pyx":541
  *             raise ValueError("Write operation on read-only file")
  * 
  *     def _assert_comparable(self, BloomFilter other):             # <<<<<<<<<<<<<<
  *         error = ValueError("The two %s objects are not the same type (hint: "
  *                            "use copy_template)" % self.__class__.__name__)
  */
 
@@ -8729,37 +9245,37 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_error);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":512
+/* "pybloomfilter.pyx":550
  *         return
  * 
  *     def to_base64(self):             # <<<<<<<<<<<<<<
  *         """Creates a compressed, base64 encoded version of the :class:`BloomFilter`.
  *         Since the Bloom filter is efficiently in binary on the file system,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_49to_base64(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_48to_base64[] = "Creates a compressed, base64 encoded version of the :class:`BloomFilter`.\n        Since the Bloom filter is efficiently in binary on the file system,\n        this may not be too useful. I find it useful for debugging so I can\n        copy filters from one terminal to another in their entirety.\n\n        :rtype: base64 encoded string representing filter\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_49to_base64(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_51to_base64(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_50to_base64[] = "Creates a compressed, base64 encoded version of the :class:`BloomFilter`.\n        Since the Bloom filter is efficiently in binary on the file system,\n        this may not be too useful. I find it useful for debugging so I can\n        copy filters from one terminal to another in their entirety.\n\n        :rtype: base64 encoded string representing filter\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_51to_base64(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("to_base64 (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_48to_base64(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_50to_base64(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_48to_base64(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_50to_base64(struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
   PyObject *__pyx_v_bfile = NULL;
   PyObject *__pyx_v_fl_content = NULL;
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -8773,113 +9289,113 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("to_base64", 0);
 
-  /* "pybloomfilter.pyx":520
+  /* "pybloomfilter.pyx":558
  *         :rtype: base64 encoded string representing filter
  *         """
  *         self._assert_open()             # <<<<<<<<<<<<<<
  *         bfile = open(self.filename, "rb")
  *         fl_content = bfile.read()
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_assert_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":521
+  /* "pybloomfilter.pyx":559
  *         """
  *         self._assert_open()
  *         bfile = open(self.filename, "rb")             # <<<<<<<<<<<<<<
  *         fl_content = bfile.read()
  *         result = b64encode(zlib.compress(b64encode(zlib.compress(
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_filename); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_filename); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_rb);
   __Pyx_GIVEREF(__pyx_n_u_rb);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_rb);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_bfile = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":522
+  /* "pybloomfilter.pyx":560
  *         self._assert_open()
  *         bfile = open(self.filename, "rb")
  *         fl_content = bfile.read()             # <<<<<<<<<<<<<<
  *         result = b64encode(zlib.compress(b64encode(zlib.compress(
  *             fl_content, 9))))
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_bfile, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 522, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_bfile, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 522, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_fl_content = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":523
+  /* "pybloomfilter.pyx":561
  *         bfile = open(self.filename, "rb")
  *         fl_content = bfile.read()
  *         result = b64encode(zlib.compress(b64encode(zlib.compress(             # <<<<<<<<<<<<<<
  *             fl_content, 9))))
  *         bfile.close()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_zlib); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_zlib); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_compress); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_compress); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_zlib); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_zlib); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_compress); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_compress); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pybloomfilter.pyx":524
+  /* "pybloomfilter.pyx":562
  *         fl_content = bfile.read()
  *         result = b64encode(zlib.compress(b64encode(zlib.compress(
  *             fl_content, 9))))             # <<<<<<<<<<<<<<
  *         bfile.close()
  *         return result
  */
   __pyx_t_8 = NULL;
@@ -8893,40 +9409,40 @@
       __Pyx_DECREF_SET(__pyx_t_9, function);
       __pyx_t_10 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_9)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_v_fl_content, __pyx_int_9};
-    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 561, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_7);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
     PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_v_fl_content, __pyx_int_9};
-    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 561, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_GOTREF(__pyx_t_7);
   } else
   #endif
   {
-    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 561, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     if (__pyx_t_8) {
       __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_INCREF(__pyx_v_fl_content);
     __Pyx_GIVEREF(__pyx_v_fl_content);
     PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_v_fl_content);
     __Pyx_INCREF(__pyx_int_9);
     __Pyx_GIVEREF(__pyx_int_9);
     PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_int_9);
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_11, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_11, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 561, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   }
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
@@ -8936,15 +9452,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_9, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 523, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -8952,15 +9468,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 523, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8968,59 +9484,59 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 523, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_result = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":525
+  /* "pybloomfilter.pyx":563
  *         result = b64encode(zlib.compress(b64encode(zlib.compress(
  *             fl_content, 9))))
  *         bfile.close()             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_bfile, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_bfile, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 525, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":526
+  /* "pybloomfilter.pyx":564
  *             fl_content, 9))))
  *         bfile.close()
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":512
+  /* "pybloomfilter.pyx":550
  *         return
  * 
  *     def to_base64(self):             # <<<<<<<<<<<<<<
  *         """Creates a compressed, base64 encoded version of the :class:`BloomFilter`.
  *         Since the Bloom filter is efficiently in binary on the file system,
  */
 
@@ -9043,26 +9559,26 @@
   __Pyx_XDECREF(__pyx_v_fl_content);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":529
+/* "pybloomfilter.pyx":567
  * 
  *     @classmethod
  *     def from_base64(cls, filename, string, perm=0755):             # <<<<<<<<<<<<<<
  *         """Unpacks the supplied base64 string (as returned by :meth:`BloomFilter.to_base64`)
  *         into the supplied filename and return a :class:`BloomFilter` object using that
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_51from_base64(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_50from_base64[] = "Unpacks the supplied base64 string (as returned by :meth:`BloomFilter.to_base64`)\n        into the supplied filename and return a :class:`BloomFilter` object using that\n        file.\n\n        :param str filename: new filename\n        :param int perm: file access permission flags\n        :rtype: :class:`BloomFilter`\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_51from_base64(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_53from_base64(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_52from_base64[] = "Unpacks the supplied base64 string (as returned by :meth:`BloomFilter.to_base64`)\n        into the supplied filename and return a :class:`BloomFilter` object using that\n        file.\n\n        :param str filename: new filename\n        :param int perm: file access permission flags\n        :rtype: :class:`BloomFilter`\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_53from_base64(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_string = 0;
   PyObject *__pyx_v_perm = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -9090,25 +9606,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_filename)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_string)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("from_base64", 0, 2, 3, 1); __PYX_ERR(0, 529, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("from_base64", 0, 2, 3, 1); __PYX_ERR(0, 567, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_perm);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "from_base64") < 0)) __PYX_ERR(0, 529, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "from_base64") < 0)) __PYX_ERR(0, 567, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -9118,28 +9634,28 @@
     }
     __pyx_v_filename = values[0];
     __pyx_v_string = values[1];
     __pyx_v_perm = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("from_base64", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 529, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("from_base64", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 567, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybloomfilter.BloomFilter.from_base64", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_50from_base64(((PyTypeObject*)__pyx_v_cls), __pyx_v_filename, __pyx_v_string, __pyx_v_perm);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_52from_base64(((PyTypeObject*)__pyx_v_cls), __pyx_v_filename, __pyx_v_string, __pyx_v_perm);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_50from_base64(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_string, PyObject *__pyx_v_perm) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_52from_base64(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_string, PyObject *__pyx_v_perm) {
   PyObject *__pyx_v_bfile_fp = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -9152,27 +9668,27 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("from_base64", 0);
 
-  /* "pybloomfilter.pyx":538
+  /* "pybloomfilter.pyx":576
  *         :rtype: :class:`BloomFilter`
  *         """
  *         bfile_fp = os.open(filename, _construct_mode("w+"), perm)             # <<<<<<<<<<<<<<
  *         os.write(bfile_fp, zlib.decompress(b64decode(zlib.decompress(
  *             b64decode(string)))))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_open); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_open); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_f_13pybloomfilter__construct_mode(__pyx_kp_u_w_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_13pybloomfilter__construct_mode(__pyx_kp_u_w_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 576, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9181,99 +9697,99 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_filename, __pyx_t_2, __pyx_v_perm};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_filename, __pyx_t_2, __pyx_v_perm};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_filename);
     __Pyx_GIVEREF(__pyx_v_filename);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_filename);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_perm);
     __Pyx_GIVEREF(__pyx_v_perm);
     PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, __pyx_v_perm);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 576, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_bfile_fp = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":539
+  /* "pybloomfilter.pyx":577
  *         """
  *         bfile_fp = os.open(filename, _construct_mode("w+"), perm)
  *         os.write(bfile_fp, zlib.decompress(b64decode(zlib.decompress(             # <<<<<<<<<<<<<<
  *             b64decode(string)))))
  *         os.close(bfile_fp)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_write); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_write); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_zlib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_zlib); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decompress); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decompress); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_zlib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_zlib); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_decompress); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_decompress); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-  /* "pybloomfilter.pyx":540
+  /* "pybloomfilter.pyx":578
  *         bfile_fp = os.open(filename, _construct_mode("w+"), perm)
  *         os.write(bfile_fp, zlib.decompress(b64decode(zlib.decompress(
  *             b64decode(string)))))             # <<<<<<<<<<<<<<
  *         os.close(bfile_fp)
  *         return cls.open(filename)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
       __Pyx_INCREF(__pyx_t_12);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_11, function);
     }
   }
   __pyx_t_9 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_v_string) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_string);
   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -9281,15 +9797,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_8 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_11, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_9);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 539, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -9297,15 +9813,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_2 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_10, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -9313,15 +9829,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_7, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_4)) {
@@ -9331,107 +9847,107 @@
       __Pyx_DECREF_SET(__pyx_t_6, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_bfile_fp, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_bfile_fp, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_2 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_bfile_fp);
     __Pyx_GIVEREF(__pyx_v_bfile_fp);
     PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_5, __pyx_v_bfile_fp);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":541
+  /* "pybloomfilter.pyx":579
  *         os.write(bfile_fp, zlib.decompress(b64decode(zlib.decompress(
  *             b64decode(string)))))
  *         os.close(bfile_fp)             # <<<<<<<<<<<<<<
  *         return cls.open(filename)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_os); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_os); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_v_bfile_fp) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_bfile_fp);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 541, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":542
+  /* "pybloomfilter.pyx":580
  *             b64decode(string)))))
  *         os.close(bfile_fp)
  *         return cls.open(filename)             # <<<<<<<<<<<<<<
  * 
  *     @classmethod
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cls), __pyx_n_s_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_v_filename) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_filename);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":529
+  /* "pybloomfilter.pyx":567
  * 
  *     @classmethod
  *     def from_base64(cls, filename, string, perm=0755):             # <<<<<<<<<<<<<<
  *         """Unpacks the supplied base64 string (as returned by :meth:`BloomFilter.to_base64`)
  *         into the supplied filename and return a :class:`BloomFilter` object using that
  */
 
@@ -9453,26 +9969,26 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_bfile_fp);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybloomfilter.pyx":545
+/* "pybloomfilter.pyx":583
  * 
  *     @classmethod
  *     def open(cls, filename, mode="rw"):             # <<<<<<<<<<<<<<
  *         """Creates a :class:`BloomFilter` object from an existing file.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_53open(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_13pybloomfilter_11BloomFilter_52open[] = "Creates a :class:`BloomFilter` object from an existing file.\n\n        :param str filename: existing filename\n        :param str mode: file access mode\n        :rtype: :class:`BloomFilter`\n        ";
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_53open(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_55open(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_13pybloomfilter_11BloomFilter_54open[] = "Creates a :class:`BloomFilter` object from an existing file.\n\n        :param str filename: existing filename\n        :param str mode: file access mode\n        :rtype: :class:`BloomFilter`\n        ";
+static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_55open(PyObject *__pyx_v_cls, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_filename = 0;
   PyObject *__pyx_v_mode = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -9501,15 +10017,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 545, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 583, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -9517,69 +10033,69 @@
       }
     }
     __pyx_v_filename = values[0];
     __pyx_v_mode = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 545, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 583, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybloomfilter.BloomFilter.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_52open(((PyTypeObject*)__pyx_v_cls), __pyx_v_filename, __pyx_v_mode);
+  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_54open(((PyTypeObject*)__pyx_v_cls), __pyx_v_filename, __pyx_v_mode);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_52open(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode) {
+static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_54open(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_filename, PyObject *__pyx_v_mode) {
   PyObject *__pyx_v_instance = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
-  /* "pybloomfilter.pyx":552
+  /* "pybloomfilter.pyx":590
  *         :rtype: :class:`BloomFilter`
  *         """
  *         instance = cls(NoConstruct, 0)             # <<<<<<<<<<<<<<
  *         instance._open(filename, mode)
  *         return instance
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_13pybloomfilter_NoConstruct);
   __Pyx_GIVEREF(__pyx_v_13pybloomfilter_NoConstruct);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_13pybloomfilter_NoConstruct);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_0);
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_v_cls), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_v_cls), __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_instance = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":553
+  /* "pybloomfilter.pyx":591
  *         """
  *         instance = cls(NoConstruct, 0)
  *         instance._open(filename, mode)             # <<<<<<<<<<<<<<
  *         return instance
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_instance, __pyx_n_s_open_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_instance, __pyx_n_s_open_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -9588,57 +10104,57 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_filename, __pyx_v_mode};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_2);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_filename, __pyx_v_mode};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_2);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_filename);
     __Pyx_GIVEREF(__pyx_v_filename);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_filename);
     __Pyx_INCREF(__pyx_v_mode);
     __Pyx_GIVEREF(__pyx_v_mode);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_mode);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":554
+  /* "pybloomfilter.pyx":592
  *         instance = cls(NoConstruct, 0)
  *         instance._open(filename, mode)
  *         return instance             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_instance);
   __pyx_r = __pyx_v_instance;
   goto __pyx_L0;
 
-  /* "pybloomfilter.pyx":545
+  /* "pybloomfilter.pyx":583
  * 
  *     @classmethod
  *     def open(cls, filename, mode="rw"):             # <<<<<<<<<<<<<<
  *         """Creates a :class:`BloomFilter` object from an existing file.
  * 
  */
 
@@ -9653,136 +10169,23 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_instance);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_55__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_55__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_54__reduce_cython__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_54__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
-
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 2, __pyx_L1_error)
-
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pybloomfilter.BloomFilter.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_57__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_13pybloomfilter_11BloomFilter_57__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_13pybloomfilter_11BloomFilter_56__setstate_cython__(((struct __pyx_obj_13pybloomfilter_BloomFilter *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_13pybloomfilter_11BloomFilter_56__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_13pybloomfilter_BloomFilter *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
-
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 4, __pyx_L1_error)
-
-  /* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pybloomfilter.BloomFilter.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 static PyObject *__pyx_tp_new_13pybloomfilter_BloomFilter(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  if (unlikely(__pyx_pw_13pybloomfilter_11BloomFilter_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_13pybloomfilter_11BloomFilter_3__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_13pybloomfilter_BloomFilter(PyObject *o) {
@@ -9791,25 +10194,29 @@
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_13pybloomfilter_11BloomFilter_7__dealloc__(o);
+    __pyx_pw_13pybloomfilter_11BloomFilter_9__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_getprop_13pybloomfilter_11BloomFilter_bit_array(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_13pybloomfilter_11BloomFilter_9bit_array_1__get__(o);
 }
 
+static PyObject *__pyx_getprop_13pybloomfilter_11BloomFilter_data_array(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_13pybloomfilter_11BloomFilter_10data_array_1__get__(o);
+}
+
 static PyObject *__pyx_getprop_13pybloomfilter_11BloomFilter_hash_seeds(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_13pybloomfilter_11BloomFilter_10hash_seeds_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_13pybloomfilter_11BloomFilter_capacity(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_13pybloomfilter_11BloomFilter_8capacity_1__get__(o);
 }
@@ -9843,40 +10250,40 @@
 }
 
 static PyObject *__pyx_getprop_13pybloomfilter_11BloomFilter_read_only(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_13pybloomfilter_11BloomFilter_9read_only_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_13pybloomfilter_BloomFilter[] = {
-  {"_create", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_3_create, METH_VARARGS|METH_KEYWORDS, 0},
-  {"_open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_5_open, METH_VARARGS|METH_KEYWORDS, 0},
-  {"_name", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_9_name, METH_NOARGS, 0},
-  {"fileno", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_11fileno, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_10fileno},
-  {"sync", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_17sync, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_16sync},
-  {"clear_all", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_19clear_all, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_18clear_all},
-  {"copy_template", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_23copy_template, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13pybloomfilter_11BloomFilter_22copy_template},
-  {"copy", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_25copy, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_24copy},
-  {"add", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_27add, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_26add},
-  {"update", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_29update, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_28update},
-  {"close", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_33close, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_32close},
-  {"union", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_35union, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_34union},
-  {"intersection", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_39intersection, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_38intersection},
-  {"_assert_open", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_43_assert_open, METH_NOARGS, 0},
-  {"_assert_writable", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_45_assert_writable, METH_NOARGS, 0},
-  {"_assert_comparable", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_47_assert_comparable, METH_O, 0},
-  {"to_base64", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_49to_base64, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_48to_base64},
-  {"from_base64", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_51from_base64, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13pybloomfilter_11BloomFilter_50from_base64},
-  {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_53open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13pybloomfilter_11BloomFilter_52open},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_55__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_57__setstate_cython__, METH_O, 0},
+  {"__reduce__", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_1__reduce__, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter___reduce__},
+  {"_create", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_5_create, METH_VARARGS|METH_KEYWORDS, 0},
+  {"_open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_7_open, METH_VARARGS|METH_KEYWORDS, 0},
+  {"_name", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_11_name, METH_NOARGS, 0},
+  {"fileno", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_13fileno, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_12fileno},
+  {"sync", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_19sync, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_18sync},
+  {"clear_all", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_21clear_all, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_20clear_all},
+  {"copy_template", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_25copy_template, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13pybloomfilter_11BloomFilter_24copy_template},
+  {"copy", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_27copy, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_26copy},
+  {"add", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_29add, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_28add},
+  {"update", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_31update, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_30update},
+  {"close", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_35close, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_34close},
+  {"union", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_37union, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_36union},
+  {"intersection", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_41intersection, METH_O, __pyx_doc_13pybloomfilter_11BloomFilter_40intersection},
+  {"_assert_open", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_45_assert_open, METH_NOARGS, 0},
+  {"_assert_writable", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_47_assert_writable, METH_NOARGS, 0},
+  {"_assert_comparable", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_49_assert_comparable, METH_O, 0},
+  {"to_base64", (PyCFunction)__pyx_pw_13pybloomfilter_11BloomFilter_51to_base64, METH_NOARGS, __pyx_doc_13pybloomfilter_11BloomFilter_50to_base64},
+  {"from_base64", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_53from_base64, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13pybloomfilter_11BloomFilter_52from_base64},
+  {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_13pybloomfilter_11BloomFilter_55open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_13pybloomfilter_11BloomFilter_54open},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_13pybloomfilter_BloomFilter[] = {
   {(char *)"bit_array", __pyx_getprop_13pybloomfilter_11BloomFilter_bit_array, 0, (char *)"Bit vector representation of the Bloom filter contents.\n        Returns an integer.\n        ", 0},
+  {(char *)"data_array", __pyx_getprop_13pybloomfilter_11BloomFilter_data_array, 0, (char *)"Bytes array of the Bloom filter contents.\n        ", 0},
   {(char *)"hash_seeds", __pyx_getprop_13pybloomfilter_11BloomFilter_hash_seeds, 0, (char *)"Integer seeds used for the random hashing. Returns a list of integers.", 0},
   {(char *)"capacity", __pyx_getprop_13pybloomfilter_11BloomFilter_capacity, 0, (char *)"The maximum number of elements this filter can contain while keeping\n        the false positive rate under :attr:`BloomFilter.error_rate`.\n        Returns an integer.\n        ", 0},
   {(char *)"error_rate", __pyx_getprop_13pybloomfilter_11BloomFilter_error_rate, 0, (char *)"The acceptable probability of false positives. Returns a float.", 0},
   {(char *)"num_hashes", __pyx_getprop_13pybloomfilter_11BloomFilter_num_hashes, 0, (char *)"Number of hash functions used when computing.", 0},
   {(char *)"num_bits", __pyx_getprop_13pybloomfilter_11BloomFilter_num_bits, 0, (char *)"Number of bits used in the filter as buckets.", 0},
   {(char *)"bit_count", __pyx_getprop_13pybloomfilter_11BloomFilter_bit_count, 0, (char *)"Number of bits set to one.", 0},
   {(char *)"approx_len", __pyx_getprop_13pybloomfilter_11BloomFilter_approx_len, 0, (char *)"Approximate number of items in the set.\n\n        See also:\n        - https://en.wikipedia.org/wiki/Bloom_filter#The_union_and_intersection_of_sets\n        - https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.1063.3591&rep=rep1&type=pdf\n        ", 0},
@@ -9928,45 +10335,45 @@
   #if PY_MAJOR_VERSION < 3 || (CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x03050000)
   0, /*nb_inplace_divide*/
   #endif
   0, /*nb_inplace_remainder*/
   0, /*nb_inplace_power*/
   0, /*nb_inplace_lshift*/
   0, /*nb_inplace_rshift*/
-  __pyx_pw_13pybloomfilter_11BloomFilter_41__iand__, /*nb_inplace_and*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_43__iand__, /*nb_inplace_and*/
   0, /*nb_inplace_xor*/
-  __pyx_pw_13pybloomfilter_11BloomFilter_37__ior__, /*nb_inplace_or*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_39__ior__, /*nb_inplace_or*/
   0, /*nb_floor_divide*/
   0, /*nb_true_divide*/
   0, /*nb_inplace_floor_divide*/
   0, /*nb_inplace_true_divide*/
   0, /*nb_index*/
   #if PY_VERSION_HEX >= 0x03050000
   0, /*nb_matrix_multiply*/
   #endif
   #if PY_VERSION_HEX >= 0x03050000
   0, /*nb_inplace_matrix_multiply*/
   #endif
 };
 
 static PySequenceMethods __pyx_tp_as_sequence_BloomFilter = {
-  __pyx_pw_13pybloomfilter_11BloomFilter_31__len__, /*sq_length*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_33__len__, /*sq_length*/
   0, /*sq_concat*/
   0, /*sq_repeat*/
   0, /*sq_item*/
   0, /*sq_slice*/
   0, /*sq_ass_item*/
   0, /*sq_ass_slice*/
-  __pyx_pw_13pybloomfilter_11BloomFilter_21__contains__, /*sq_contains*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_23__contains__, /*sq_contains*/
   0, /*sq_inplace_concat*/
   0, /*sq_inplace_repeat*/
 };
 
 static PyMappingMethods __pyx_tp_as_mapping_BloomFilter = {
-  __pyx_pw_13pybloomfilter_11BloomFilter_31__len__, /*mp_length*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_33__len__, /*mp_length*/
   0, /*mp_subscript*/
   0, /*mp_ass_subscript*/
 };
 
 static PyTypeObject __pyx_type_13pybloomfilter_BloomFilter = {
   PyVarObject_HEAD_INIT(0, 0)
   "pybloomfilter.BloomFilter", /*tp_name*/
@@ -9983,26 +10390,26 @@
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
   #endif
-  __pyx_pw_13pybloomfilter_11BloomFilter_13__repr__, /*tp_repr*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_15__repr__, /*tp_repr*/
   &__pyx_tp_as_number_BloomFilter, /*tp_as_number*/
   &__pyx_tp_as_sequence_BloomFilter, /*tp_as_sequence*/
   &__pyx_tp_as_mapping_BloomFilter, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
-  __pyx_pw_13pybloomfilter_11BloomFilter_15__str__, /*tp_str*/
+  __pyx_pw_13pybloomfilter_11BloomFilter_17__str__, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
-  "\n    Creates a new BloomFilter object with a given capacity and error_rate.\n\n    :param int capacity: the maximum number of elements this filter\n        can contain while keeping the false positive rate under ``error_rate``.\n    :param float error_rate: false positive probability that will hold\n        given that ``capacity`` is not exceeded.\n    :param str filename: filename to use to create the new Bloom filter.\n        If a filename is not provided, an in-memory Bloom filter will be created.\n    :param str mode: (*not applicable for an in-memory Bloom filter*)\n        file access mode.\n    :param int perm: (*not applicable for an in-memory Bloom filter*)\n        file access permission flags.\n    :param list hash_seeds: optionally specify hash seeds to use for the\n        hashing algorithm. Each hash seed must not exceed 32 bits. The number\n        of hash seeds will determine the number of hashes performed.\n\n    **Note that we do not check capacity.** This is important, because\n    we want to be able to support logical OR and AND (see :meth:`BloomFilter.union`\n    and :meth:`BloomFilter.intersection`). The capacity and error_rate then together\n    serve as a contract -- you add less than capacity items, and the Bloom filter\n    will have an error rate less than error_rate.\n\n    Raises :class:`OSError` if the supplied filename does not exist or if user\n    lacks permission to access such file. Raises :class:`ValueError` if the supplied\n    ``error_rate`` is invalid, ``hash_seeds`` does not contain valid hash seeds, or\n    if the file cannot be read.\n    ", /*tp_doc*/
+  "\n    Creates a new BloomFilter object with a given capacity and error_rate.\n\n    :param int capacity: the maximum number of elements this filter\n        can contain while keeping the false positive rate under ``error_rate``.\n    :param float error_rate: false positive probability that will hold\n        given that ``capacity`` is not exceeded.\n    :param str filename: filename to use to create the new Bloom filter.\n        If a filename is not provided, an in-memory Bloom filter will be created.\n    :param str mode: (*not applicable for an in-memory Bloom filter*)\n        file access mode.\n    :param int perm: (*not applicable for an in-memory Bloom filter*)\n        file access permission flags.\n    :param list hash_seeds: optionally specify hash seeds to use for the\n        hashing algorithm. Each hash seed must not exceed 32 bits. The number\n        of hash seeds will determine the number of hashes performed.\n    :param bytes data_array: optionally specify the filter data array, same as\n        given by BloomFilter.data_array. Only valid for in-memory bloomfilters.\n        If provided, hash_seeds must be given too.\n\n    **Note that we do not check capacity.** This is important, because\n    we want to be able to support logical OR and AND (see :meth:`BloomFilter.union`\n    and :meth:`BloomFilter.intersection`). The capacity and error_rate then together\n    serve as a contract -- you add less than capacity items, and the Bloom filter\n    will have an error rate less than error_rate.\n\n    Raises :class:`OSError` if the supplied filename does not exist or if user\n    lacks permission to access such file. Raises :class:`ValueError` if the supplied\n    ``error_rate`` is invalid, ``hash_seeds`` does not contain valid hash seeds, or\n    if the file cannot be read.\n    ", /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
   __pyx_methods_13pybloomfilter_BloomFilter, /*tp_methods*/
@@ -10084,16 +10491,17 @@
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
   {&__pyx_kp_u_0_3f, __pyx_k_0_3f, sizeof(__pyx_k_0_3f), 0, 1, 0, 0},
   {&__pyx_n_s_AUTHOR, __pyx_k_AUTHOR, sizeof(__pyx_k_AUTHOR), 0, 0, 1, 1},
+  {&__pyx_n_u_B, __pyx_k_B, sizeof(__pyx_k_B), 0, 1, 0, 1},
   {&__pyx_n_s_BloomFilter, __pyx_k_BloomFilter, sizeof(__pyx_k_BloomFilter), 0, 0, 1, 1},
-  {&__pyx_kp_u_BloomFilter_union_line_445, __pyx_k_BloomFilter_union_line_445, sizeof(__pyx_k_BloomFilter_union_line_445), 0, 1, 0, 0},
+  {&__pyx_kp_u_BloomFilter_union_line_483, __pyx_k_BloomFilter_union_line_483, sizeof(__pyx_k_BloomFilter_union_line_483), 0, 1, 0, 0},
   {&__pyx_kp_u_Cannot_access_name_on_an_in_memo, __pyx_k_Cannot_access_name_on_an_in_memo, sizeof(__pyx_k_Cannot_access_name_on_an_in_memo), 0, 1, 0, 0},
   {&__pyx_kp_u_Cannot_call_copy_on_an_in_memory, __pyx_k_Cannot_call_copy_on_an_in_memory, sizeof(__pyx_k_Cannot_call_copy_on_an_in_memory), 0, 1, 0, 0},
   {&__pyx_n_s_ENOENT, __pyx_k_ENOENT, sizeof(__pyx_k_ENOENT), 0, 0, 1, 1},
   {&__pyx_n_s_F_OK, __pyx_k_F_OK, sizeof(__pyx_k_F_OK), 0, 0, 1, 1},
   {&__pyx_n_u_I, __pyx_k_I, sizeof(__pyx_k_I), 0, 1, 0, 1},
   {&__pyx_kp_u_I_O_operation_on_closed_file, __pyx_k_I_O_operation_on_closed_file, sizeof(__pyx_k_I_O_operation_on_closed_file), 0, 1, 0, 0},
   {&__pyx_kp_u_Insufficient_permissions_for_fil, __pyx_k_Insufficient_permissions_for_fil, sizeof(__pyx_k_Insufficient_permissions_for_fil), 0, 1, 0, 0},
@@ -10108,24 +10516,23 @@
   {&__pyx_n_s_O_RDWR, __pyx_k_O_RDWR, sizeof(__pyx_k_O_RDWR), 0, 0, 1, 1},
   {&__pyx_n_s_PendingDeprecationWarning, __pyx_k_PendingDeprecationWarning, sizeof(__pyx_k_PendingDeprecationWarning), 0, 0, 1, 1},
   {&__pyx_kp_u_Performs_a_set_OR_with_another_c, __pyx_k_Performs_a_set_OR_with_another_c, sizeof(__pyx_k_Performs_a_set_OR_with_another_c), 0, 1, 0, 0},
   {&__pyx_n_s_R_OK, __pyx_k_R_OK, sizeof(__pyx_k_R_OK), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_kp_u_Some_problem_occured_while_tryin, __pyx_k_Some_problem_occured_while_tryin, sizeof(__pyx_k_Some_problem_occured_while_tryin), 0, 1, 0, 0},
   {&__pyx_kp_u_The_two_s_objects_are_not_the_sa, __pyx_k_The_two_s_objects_are_not_the_sa, sizeof(__pyx_k_The_two_s_objects_are_not_the_sa), 0, 1, 0, 0},
-  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_VERSION, __pyx_k_VERSION, sizeof(__pyx_k_VERSION), 0, 0, 1, 1},
   {&__pyx_n_s_VERSION_2, __pyx_k_VERSION_2, sizeof(__pyx_k_VERSION_2), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_W_OK, __pyx_k_W_OK, sizeof(__pyx_k_W_OK), 0, 0, 1, 1},
   {&__pyx_kp_u_Write_operation_on_read_only_fil, __pyx_k_Write_operation_on_read_only_fil, sizeof(__pyx_k_Write_operation_on_read_only_fil), 0, 1, 0, 0},
-  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-  {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-  {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
+  {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
+  {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
+  {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
+  {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
   {&__pyx_n_s_access, __pyx_k_access, sizeof(__pyx_k_access), 0, 0, 1, 1},
   {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
   {&__pyx_n_s_approx_len, __pyx_k_approx_len, sizeof(__pyx_k_approx_len), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_assert_comparable, __pyx_k_assert_comparable, sizeof(__pyx_k_assert_comparable), 0, 0, 1, 1},
   {&__pyx_n_s_assert_open, __pyx_k_assert_open, sizeof(__pyx_k_assert_open), 0, 0, 1, 1},
   {&__pyx_n_s_assert_writable, __pyx_k_assert_writable, sizeof(__pyx_k_assert_writable), 0, 0, 1, 1},
@@ -10143,14 +10550,16 @@
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_compress, __pyx_k_compress, sizeof(__pyx_k_compress), 0, 0, 1, 1},
   {&__pyx_n_s_copy, __pyx_k_copy, sizeof(__pyx_k_copy), 0, 0, 1, 1},
   {&__pyx_n_s_create, __pyx_k_create, sizeof(__pyx_k_create), 0, 0, 1, 1},
   {&__pyx_n_u_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 1, 0, 1},
+  {&__pyx_n_s_data_array, __pyx_k_data_array, sizeof(__pyx_k_data_array), 0, 0, 1, 1},
+  {&__pyx_kp_u_data_array_cannot_be_used_for_an, __pyx_k_data_array_cannot_be_used_for_an, sizeof(__pyx_k_data_array_cannot_be_used_for_an), 0, 1, 0, 0},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_decompress, __pyx_k_decompress, sizeof(__pyx_k_decompress), 0, 0, 1, 1},
   {&__pyx_n_s_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_endswith, __pyx_k_endswith, sizeof(__pyx_k_endswith), 0, 0, 1, 1},
   {&__pyx_n_s_eno, __pyx_k_eno, sizeof(__pyx_k_eno), 0, 0, 1, 1},
   {&__pyx_n_s_errno, __pyx_k_errno, sizeof(__pyx_k_errno), 0, 0, 1, 1},
@@ -10163,28 +10572,27 @@
   {&__pyx_kp_u_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 1, 0, 0},
   {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
   {&__pyx_n_s_floor, __pyx_k_floor, sizeof(__pyx_k_floor), 0, 0, 1, 1},
   {&__pyx_n_s_from_base64, __pyx_k_from_base64, sizeof(__pyx_k_from_base64), 0, 0, 1, 1},
   {&__pyx_n_s_from_bytes, __pyx_k_from_bytes, sizeof(__pyx_k_from_bytes), 0, 0, 1, 1},
   {&__pyx_n_s_frombytes, __pyx_k_frombytes, sizeof(__pyx_k_frombytes), 0, 0, 1, 1},
   {&__pyx_n_s_getrandbits, __pyx_k_getrandbits, sizeof(__pyx_k_getrandbits), 0, 0, 1, 1},
-  {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_hash_seeds, __pyx_k_hash_seeds, sizeof(__pyx_k_hash_seeds), 0, 0, 1, 1},
+  {&__pyx_kp_u_hash_seeds_must_be_specified_if, __pyx_k_hash_seeds_must_be_specified_if, sizeof(__pyx_k_hash_seeds_must_be_specified_if), 0, 1, 0, 0},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_intersection, __pyx_k_intersection, sizeof(__pyx_k_intersection), 0, 0, 1, 1},
   {&__pyx_kp_u_invalid_hash_seed_s_must_be_0_an, __pyx_k_invalid_hash_seed_s_must_be_0_an, sizeof(__pyx_k_invalid_hash_seed_s_must_be_0_an), 0, 1, 0, 0},
   {&__pyx_n_s_log, __pyx_k_log, sizeof(__pyx_k_log), 0, 0, 1, 1},
   {&__pyx_n_s_log2, __pyx_k_log2, sizeof(__pyx_k_log2), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_math, __pyx_k_math, sizeof(__pyx_k_math), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_kp_u_name_will_be_deprecated_in_futur, __pyx_k_name_will_be_deprecated_in_futur, sizeof(__pyx_k_name_will_be_deprecated_in_futur), 0, 1, 0, 0},
-  {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_num_bits, __pyx_k_num_bits, sizeof(__pyx_k_num_bits), 0, 0, 1, 1},
   {&__pyx_n_s_num_hashes, __pyx_k_num_hashes, sizeof(__pyx_k_num_hashes), 0, 0, 1, 1},
   {&__pyx_kp_u_num_hashes_2, __pyx_k_num_hashes_2, sizeof(__pyx_k_num_hashes_2), 0, 1, 0, 0},
   {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_n_s_open_2, __pyx_k_open_2, sizeof(__pyx_k_open_2), 0, 0, 1, 1},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
@@ -10192,23 +10600,18 @@
   {&__pyx_n_s_perm, __pyx_k_perm, sizeof(__pyx_k_perm), 0, 0, 1, 1},
   {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
   {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_u_rb, __pyx_k_rb, sizeof(__pyx_k_rb), 0, 1, 0, 1},
   {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
   {&__pyx_n_s_read_only, __pyx_k_read_only, sizeof(__pyx_k_read_only), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_replace, __pyx_k_replace, sizeof(__pyx_k_replace), 0, 0, 1, 1},
   {&__pyx_n_s_repr, __pyx_k_repr, sizeof(__pyx_k_repr), 0, 0, 1, 1},
   {&__pyx_n_s_round, __pyx_k_round, sizeof(__pyx_k_round), 0, 0, 1, 1},
   {&__pyx_n_u_rw, __pyx_k_rw, sizeof(__pyx_k_rw), 0, 1, 0, 1},
-  {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
-  {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shutil, __pyx_k_shutil, sizeof(__pyx_k_shutil), 0, 0, 1, 1},
   {&__pyx_n_s_signed, __pyx_k_signed, sizeof(__pyx_k_signed), 0, 0, 1, 1},
   {&__pyx_n_s_strerror, __pyx_k_strerror, sizeof(__pyx_k_strerror), 0, 0, 1, 1},
   {&__pyx_n_s_string, __pyx_k_string, sizeof(__pyx_k_string), 0, 0, 1, 1},
   {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_tobytes, __pyx_k_tobytes, sizeof(__pyx_k_tobytes), 0, 0, 1, 1},
@@ -10219,115 +10622,117 @@
   {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
   {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {&__pyx_n_s_zlib, __pyx_k_zlib, sizeof(__pyx_k_zlib), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 113, __pyx_L1_error)
-  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(0, 163, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 126, __pyx_L1_error)
-  __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(0, 261, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 266, __pyx_L1_error)
-  __pyx_builtin_PendingDeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_PendingDeprecationWarning); if (!__pyx_builtin_PendingDeprecationWarning) __PYX_ERR(0, 281, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 409, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 521, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(0, 298, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_builtin_PendingDeprecationWarning = __Pyx_GetBuiltinName(__pyx_n_s_PendingDeprecationWarning); if (!__pyx_builtin_PendingDeprecationWarning) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 559, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pybloomfilter.pyx":170
+  /* "pybloomfilter.pyx":110
+ *         if data_array is not None:
+ *             if filename:
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")             # <<<<<<<<<<<<<<
+ *             if hash_seeds is None:
+ *                 raise ValueError("hash_seeds must be specified if a data_array is provided.")
+ */
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_data_array_cannot_be_used_for_an); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "pybloomfilter.pyx":112
+ *                 raise ValueError("data_array cannot be used for an mmapped filter.")
+ *             if hash_seeds is None:
+ *                 raise ValueError("hash_seeds must be specified if a data_array is provided.")             # <<<<<<<<<<<<<<
+ * 
+ *         # Make sure that if the filename is defined, that the
+ */
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_hash_seeds_must_be_specified_if); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+
+  /* "pybloomfilter.pyx":194
  *     def _open(self, filename, mode="rw"):
  *         # Should not overwrite
  *         mode = mode.replace("+", "")             # <<<<<<<<<<<<<<
  * 
  *         if not os.path.exists(filename):
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_kp_u__3); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 170, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_kp_u_, __pyx_kp_u__5); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 194, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "pybloomfilter.pyx":280
+  /* "pybloomfilter.pyx":317
  *         Returns an encoded string.
  *         """
  *         warnings.warn('name will be deprecated in future versions, use '             # <<<<<<<<<<<<<<
  *                       'filename instead', PendingDeprecationWarning)
  *         return self._name()
  */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_kp_u_name_will_be_deprecated_in_futur, __pyx_builtin_PendingDeprecationWarning); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 280, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_kp_u_name_will_be_deprecated_in_futur, __pyx_builtin_PendingDeprecationWarning); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "pybloomfilter.pyx":409
+  /* "pybloomfilter.pyx":447
  *         result = cbloomfilter.bloomfilter_Add(self._bf, &key)
  *         if result == 2:
  *             raise RuntimeError("Some problem occured while trying to add key.")             # <<<<<<<<<<<<<<
  *         return bool(result)
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Some_problem_occured_while_tryin); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 409, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Some_problem_occured_while_tryin); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "pybloomfilter.pyx":497
+  /* "pybloomfilter.pyx":535
  *     def _assert_open(self):
  *         if self._closed != 0:
  *             raise ValueError("I/O operation on closed file")             # <<<<<<<<<<<<<<
  * 
  *     def _assert_writable(self):
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_I_O_operation_on_closed_file); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_I_O_operation_on_closed_file); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "pybloomfilter.pyx":501
+  /* "pybloomfilter.pyx":539
  *     def _assert_writable(self):
  *         if self.read_only:
  *             raise ValueError("Write operation on read-only file")             # <<<<<<<<<<<<<<
  * 
  *     def _assert_comparable(self, BloomFilter other):
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Write_operation_on_read_only_fil); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 501, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_Write_operation_on_read_only_fil); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "pybloomfilter.pyx":3
  * # cython: language_level=3
  * 
- * VERSION = (0, 5, 7)             # <<<<<<<<<<<<<<
+ * VERSION = (0, 6, 0)             # <<<<<<<<<<<<<<
  * AUTHOR = "Michael Axiak"
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_0, __pyx_int_5, __pyx_int_7); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_0, __pyx_int_6, __pyx_int_0); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10335,16 +10740,15 @@
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_7 = PyInt_FromLong(7); if (unlikely(!__pyx_int_7)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_6 = PyInt_FromLong(6); if (unlikely(!__pyx_int_6)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_9 = PyInt_FromLong(9); if (unlikely(!__pyx_int_9)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_493 = PyInt_FromLong(493); if (unlikely(!__pyx_int_493)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -10385,63 +10789,62 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_13pybloomfilter_BloomFilter) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_13pybloomfilter_BloomFilter) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_13pybloomfilter_BloomFilter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_13pybloomfilter_BloomFilter.tp_dictoffset && __pyx_type_13pybloomfilter_BloomFilter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_13pybloomfilter_BloomFilter.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__contains__"); if (unlikely(!wrapper)) __PYX_ERR(0, 48, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__contains__"); if (unlikely(!wrapper)) __PYX_ERR(0, 47, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_20__contains__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_20__contains__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_20__contains__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_20__contains__;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_22__contains__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_22__contains__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_22__contains__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_22__contains__;
     }
   }
   #endif
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__len__"); if (unlikely(!wrapper)) __PYX_ERR(0, 48, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__len__"); if (unlikely(!wrapper)) __PYX_ERR(0, 47, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_30__len__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_30__len__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_30__len__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_30__len__;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_32__len__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_32__len__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_32__len__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_32__len__;
     }
   }
   #endif
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__ior__"); if (unlikely(!wrapper)) __PYX_ERR(0, 48, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__ior__"); if (unlikely(!wrapper)) __PYX_ERR(0, 47, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_36__ior__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_36__ior__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_36__ior__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_36__ior__;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_38__ior__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_38__ior__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_38__ior__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_38__ior__;
     }
   }
   #endif
   #if CYTHON_UPDATE_DESCRIPTOR_DOC
   {
-    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__iand__"); if (unlikely(!wrapper)) __PYX_ERR(0, 48, __pyx_L1_error)
+    PyObject *wrapper = PyObject_GetAttrString((PyObject *)&__pyx_type_13pybloomfilter_BloomFilter, "__iand__"); if (unlikely(!wrapper)) __PYX_ERR(0, 47, __pyx_L1_error)
     if (Py_TYPE(wrapper) == &PyWrapperDescr_Type) {
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_40__iand__ = *((PyWrapperDescrObject *)wrapper)->d_base;
-      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_40__iand__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_40__iand__;
-      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_40__iand__;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_42__iand__ = *((PyWrapperDescrObject *)wrapper)->d_base;
+      __pyx_wrapperbase_13pybloomfilter_11BloomFilter_42__iand__.doc = __pyx_doc_13pybloomfilter_11BloomFilter_42__iand__;
+      ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_13pybloomfilter_11BloomFilter_42__iand__;
     }
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BloomFilter, (PyObject *)&__pyx_type_13pybloomfilter_BloomFilter) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_13pybloomfilter_BloomFilter) < 0) __PYX_ERR(0, 48, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BloomFilter, (PyObject *)&__pyx_type_13pybloomfilter_BloomFilter) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_ptype_13pybloomfilter_BloomFilter = &__pyx_type_13pybloomfilter_BloomFilter;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -10450,34 +10853,34 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10699,247 +11102,247 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "pybloomfilter.pyx":3
  * # cython: language_level=3
  * 
- * VERSION = (0, 5, 7)             # <<<<<<<<<<<<<<
+ * VERSION = (0, 6, 0)             # <<<<<<<<<<<<<<
  * AUTHOR = "Michael Axiak"
  * 
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_VERSION, __pyx_tuple__13) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "pybloomfilter.pyx":4
  * 
- * VERSION = (0, 5, 7)
+ * VERSION = (0, 6, 0)
  * AUTHOR = "Michael Axiak"             # <<<<<<<<<<<<<<
  * 
  * __VERSION__ = VERSION
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_AUTHOR, __pyx_kp_u_Michael_Axiak) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
 
   /* "pybloomfilter.pyx":6
  * AUTHOR = "Michael Axiak"
  * 
  * __VERSION__ = VERSION             # <<<<<<<<<<<<<<
  * 
- * 
+ * cimport cbloomfilter
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_VERSION); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_VERSION_2, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":12
+  /* "pybloomfilter.pyx":11
  * cimport cpython
  * 
  * import array             # <<<<<<<<<<<<<<
  * from base64 import b64encode, b64decode
  * import errno as eno
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_array, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_array, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_array, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_array, __pyx_t_1) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pybloomfilter.pyx":13
+  /* "pybloomfilter.pyx":12
  * 
  * import array
  * from base64 import b64encode, b64decode             # <<<<<<<<<<<<<<
  * import errno as eno
  * import math
  */
-  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_b64encode);
   __Pyx_GIVEREF(__pyx_n_s_b64encode);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_b64encode);
   __Pyx_INCREF(__pyx_n_s_b64decode);
   __Pyx_GIVEREF(__pyx_n_s_b64decode);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_b64decode);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_base64, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_base64, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_b64encode, __pyx_t_1) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_b64encode, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_b64decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_b64decode, __pyx_t_1) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_b64decode, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":14
+  /* "pybloomfilter.pyx":13
  * import array
  * from base64 import b64encode, b64decode
  * import errno as eno             # <<<<<<<<<<<<<<
  * import math
  * import os
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_errno, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_errno, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_eno, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_eno, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":15
+  /* "pybloomfilter.pyx":14
  * from base64 import b64encode, b64decode
  * import errno as eno
  * import math             # <<<<<<<<<<<<<<
  * import os
  * import random
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_math, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_math, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_math, __pyx_t_2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_math, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":16
+  /* "pybloomfilter.pyx":15
  * import errno as eno
  * import math
  * import os             # <<<<<<<<<<<<<<
  * import random
  * import shutil
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_os, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_os, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_os, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_os, __pyx_t_2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":17
+  /* "pybloomfilter.pyx":16
  * import math
  * import os
  * import random             # <<<<<<<<<<<<<<
  * import shutil
  * import sys
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_random, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":18
+  /* "pybloomfilter.pyx":17
  * import os
  * import random
  * import shutil             # <<<<<<<<<<<<<<
  * import sys
  * import warnings
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_shutil, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_shutil, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shutil, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shutil, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":19
+  /* "pybloomfilter.pyx":18
  * import random
  * import shutil
  * import sys             # <<<<<<<<<<<<<<
  * import warnings
  * import zlib
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_sys, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_sys, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":20
+  /* "pybloomfilter.pyx":19
  * import shutil
  * import sys
  * import warnings             # <<<<<<<<<<<<<<
  * import zlib
  * 
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":21
+  /* "pybloomfilter.pyx":20
  * import sys
  * import warnings
  * import zlib             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_zlib, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_zlib, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_zlib, __pyx_t_2) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_zlib, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":25
+  /* "pybloomfilter.pyx":24
  * 
  * cdef extern int errno
  * cdef NoConstruct = object()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(__pyx_builtin_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(__pyx_v_13pybloomfilter_NoConstruct);
   __Pyx_DECREF_SET(__pyx_v_13pybloomfilter_NoConstruct, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pybloomfilter.pyx":529
+  /* "pybloomfilter.pyx":567
  * 
  *     @classmethod
  *     def from_base64(cls, filename, string, perm=0755):             # <<<<<<<<<<<<<<
  *         """Unpacks the supplied base64 string (as returned by :meth:`BloomFilter.to_base64`)
  *         into the supplied filename and return a :class:`BloomFilter` object using that
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter, __pyx_n_s_from_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 529, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter, __pyx_n_s_from_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pybloomfilter.pyx":528
+  /* "pybloomfilter.pyx":566
  *         return result
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def from_base64(cls, filename, string, perm=0755):
  *         """Unpacks the supplied base64 string (as returned by :meth:`BloomFilter.to_base64`)
  */
-  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Method_ClassMethod(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter->tp_dict, __pyx_n_s_from_base64, __pyx_t_1) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter->tp_dict, __pyx_n_s_from_base64, __pyx_t_1) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_ptype_13pybloomfilter_BloomFilter);
 
-  /* "pybloomfilter.pyx":545
+  /* "pybloomfilter.pyx":583
  * 
  *     @classmethod
  *     def open(cls, filename, mode="rw"):             # <<<<<<<<<<<<<<
  *         """Creates a :class:`BloomFilter` object from an existing file.
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter, __pyx_n_s_open); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 545, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter, __pyx_n_s_open); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pybloomfilter.pyx":544
+  /* "pybloomfilter.pyx":582
  *         return cls.open(filename)
  * 
  *     @classmethod             # <<<<<<<<<<<<<<
  *     def open(cls, filename, mode="rw"):
  *         """Creates a :class:`BloomFilter` object from an existing file.
  */
-  __pyx_t_2 = __Pyx_Method_ClassMethod(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 544, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Method_ClassMethod(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 582, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter->tp_dict, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 545, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_13pybloomfilter_BloomFilter->tp_dict, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_13pybloomfilter_BloomFilter);
 
   /* "pybloomfilter.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
- * VERSION = (0, 5, 7)
+ * VERSION = (0, 6, 0)
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_BloomFilter_union_line_445, __pyx_kp_u_Performs_a_set_OR_with_another_c) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_BloomFilter_union_line_483, __pyx_kp_u_Performs_a_set_OR_with_another_c) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -11491,50 +11894,14 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
-/* PyObjectFormat */
-#if CYTHON_USE_UNICODE_WRITER
-static PyObject* __Pyx_PyObject_Format(PyObject* obj, PyObject* format_spec) {
-    int ret;
-    _PyUnicodeWriter writer;
-    if (likely(PyFloat_CheckExact(obj))) {
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x03040000
-        _PyUnicodeWriter_Init(&writer, 0);
-#else
-        _PyUnicodeWriter_Init(&writer);
-#endif
-        ret = _PyFloat_FormatAdvancedWriter(
-            &writer,
-            obj,
-            format_spec, 0, PyUnicode_GET_LENGTH(format_spec));
-    } else if (likely(PyLong_CheckExact(obj))) {
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x03040000
-        _PyUnicodeWriter_Init(&writer, 0);
-#else
-        _PyUnicodeWriter_Init(&writer);
-#endif
-        ret = _PyLong_FormatAdvancedWriter(
-            &writer,
-            obj,
-            format_spec, 0, PyUnicode_GET_LENGTH(format_spec));
-    } else {
-        return PyObject_Format(obj, format_spec);
-    }
-    if (unlikely(ret == -1)) {
-        _PyUnicodeWriter_Dealloc(&writer);
-        return NULL;
-    }
-    return _PyUnicodeWriter_Finish(&writer);
-}
-#endif
-
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
@@ -11710,14 +12077,50 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* PyObjectFormat */
+#if CYTHON_USE_UNICODE_WRITER
+static PyObject* __Pyx_PyObject_Format(PyObject* obj, PyObject* format_spec) {
+    int ret;
+    _PyUnicodeWriter writer;
+    if (likely(PyFloat_CheckExact(obj))) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x03040000
+        _PyUnicodeWriter_Init(&writer, 0);
+#else
+        _PyUnicodeWriter_Init(&writer);
+#endif
+        ret = _PyFloat_FormatAdvancedWriter(
+            &writer,
+            obj,
+            format_spec, 0, PyUnicode_GET_LENGTH(format_spec));
+    } else if (likely(PyLong_CheckExact(obj))) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x03040000
+        _PyUnicodeWriter_Init(&writer, 0);
+#else
+        _PyUnicodeWriter_Init(&writer);
+#endif
+        ret = _PyLong_FormatAdvancedWriter(
+            &writer,
+            obj,
+            format_spec, 0, PyUnicode_GET_LENGTH(format_spec));
+    } else {
+        return PyObject_Format(obj, format_spec);
+    }
+    if (unlikely(ret == -1)) {
+        _PyUnicodeWriter_Dealloc(&writer);
+        return NULL;
+    }
+    return _PyUnicodeWriter_Finish(&writer);
+}
+#endif
+
 /* PyObjectCallNoArg */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
@@ -12280,165 +12683,14 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
-/* SetupReduce */
-static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
-  int ret;
-  PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name);
-  if (likely(name_attr)) {
-      ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
-  } else {
-      ret = -1;
-  }
-  if (unlikely(ret < 0)) {
-      PyErr_Clear();
-      ret = 0;
-  }
-  Py_XDECREF(name_attr);
-  return ret;
-}
-static int __Pyx_setup_reduce(PyObject* type_obj) {
-    int ret = 0;
-    PyObject *object_reduce = NULL;
-    PyObject *object_getstate = NULL;
-    PyObject *object_reduce_ex = NULL;
-    PyObject *reduce = NULL;
-    PyObject *reduce_ex = NULL;
-    PyObject *reduce_cython = NULL;
-    PyObject *setstate = NULL;
-    PyObject *setstate_cython = NULL;
-    PyObject *getstate = NULL;
-#if CYTHON_USE_PYTYPE_LOOKUP
-    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
-#else
-    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
-    if (!getstate && PyErr_Occurred()) {
-        goto __PYX_BAD;
-    }
-#endif
-    if (getstate) {
-#if CYTHON_USE_PYTYPE_LOOKUP
-        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
-#else
-        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
-        if (!object_getstate && PyErr_Occurred()) {
-            goto __PYX_BAD;
-        }
-#endif
-        if (object_getstate != getstate) {
-            goto __PYX_GOOD;
-        }
-    }
-#if CYTHON_USE_PYTYPE_LOOKUP
-    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
-#else
-    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
-#endif
-    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
-    if (reduce_ex == object_reduce_ex) {
-#if CYTHON_USE_PYTYPE_LOOKUP
-        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
-#else
-        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
-#endif
-        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
-        if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
-            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
-            if (likely(reduce_cython)) {
-                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-            } else if (reduce == object_reduce || PyErr_Occurred()) {
-                goto __PYX_BAD;
-            }
-            setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
-            if (!setstate) PyErr_Clear();
-            if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
-                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
-                if (likely(setstate_cython)) {
-                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                } else if (!setstate || PyErr_Occurred()) {
-                    goto __PYX_BAD;
-                }
-            }
-            PyType_Modified((PyTypeObject*)type_obj);
-        }
-    }
-    goto __PYX_GOOD;
-__PYX_BAD:
-    if (!PyErr_Occurred())
-        PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
-    ret = -1;
-__PYX_GOOD:
-#if !CYTHON_USE_PYTYPE_LOOKUP
-    Py_XDECREF(object_reduce);
-    Py_XDECREF(object_reduce_ex);
-    Py_XDECREF(object_getstate);
-    Py_XDECREF(getstate);
-#endif
-    Py_XDECREF(reduce);
-    Py_XDECREF(reduce_ex);
-    Py_XDECREF(reduce_cython);
-    Py_XDECREF(setstate);
-    Py_XDECREF(setstate_cython);
-    return ret;
-}
-
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
     size_t size, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
@@ -12612,14 +12864,39 @@
         return PyClassMethod_New(PyMethod_GET_FUNCTION(method));
     }
     else {
         return PyClassMethod_New(method);
     }
 }
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
 /* GetNameInClass */
 static PyObject *__Pyx_GetGlobalNameAfterAttributeLookup(PyObject *name) {
     PyObject *result;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
```

### Comparing `pybloomfiltermmap3-0.5.7/src/pybloomfilter.pyx` & `pybloomfiltermmap3-0.6.0/src/pybloomfilter.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # cython: language_level=3
 
-VERSION = (0, 5, 7)
+VERSION = (0, 6, 0)
 AUTHOR = "Michael Axiak"
 
 __VERSION__ = VERSION
 
-
 cimport cbloomfilter
 cimport cpython
 
 import array
 from base64 import b64encode, b64decode
 import errno as eno
 import math
@@ -58,14 +57,17 @@
     :param str mode: (*not applicable for an in-memory Bloom filter*)
         file access mode.
     :param int perm: (*not applicable for an in-memory Bloom filter*)
         file access permission flags.
     :param list hash_seeds: optionally specify hash seeds to use for the
         hashing algorithm. Each hash seed must not exceed 32 bits. The number
         of hash seeds will determine the number of hashes performed.
+    :param bytes data_array: optionally specify the filter data array, same as
+        given by BloomFilter.data_array. Only valid for in-memory bloomfilters.
+        If provided, hash_seeds must be given too.
 
     **Note that we do not check capacity.** This is important, because
     we want to be able to support logical OR and AND (see :meth:`BloomFilter.union`
     and :meth:`BloomFilter.intersection`). The capacity and error_rate then together
     serve as a contract -- you add less than capacity items, and the Bloom filter
     will have an error rate less than error_rate.
 
@@ -76,28 +78,43 @@
     """
 
     cdef cbloomfilter.BloomFilter * _bf
     cdef int _closed
     cdef int _in_memory
     cdef int _oflags
 
-    def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):
+    def __reduce__(self):
+        """Makes an in-memory BloomFilter pickleable."""
+        callable = BloomFilter
+        args = (self.capacity, self.error_rate, None, None, self.hash_seeds, self.data_array)
+        return (callable, args)
+
+
+    def __cinit__(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):
         self._closed = 0
         self._in_memory = 0
         self._oflags = os.O_RDWR
 
         if capacity is NoConstruct:
             return
 
-        self._create(capacity, error_rate, filename, perm, hash_seeds)
+        self._create(capacity, error_rate, filename, perm, hash_seeds, data_array)
+
 
-    def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None):
+    def _create(self, capacity, error_rate, filename=None, perm=0755, hash_seeds=None, data_array=None):
         cdef char * seeds
+        cdef char * data = NULL
         cdef long long num_bits
 
+        if data_array is not None:
+            if filename:
+                raise ValueError("data_array cannot be used for an mmapped filter.")
+            if hash_seeds is None:
+                raise ValueError("hash_seeds must be specified if a data_array is provided.")
+             
         # Make sure that if the filename is defined, that the
         # file exists
         if filename and os.path.exists(filename):
             os.unlink(filename)
 
         # For why we round down for determining the number of hashes:
         # http://corte.si/%2Fposts/code/bloom-filter-rules-of-thumb/index.html
@@ -131,14 +148,18 @@
         bits_per_hash = math.ceil(
                 capacity * abs(math.log(error_rate)) /
                 (num_hashes * (math.log(2) ** 2)))
 
         # Minimum bit vector of 128 bits
         num_bits = max(num_hashes * bits_per_hash,128)
 
+        # Override calculated capacity if we are provided a data array
+        if data_array is not None:
+            num_bits = 8 * len(data_array)
+
         # print("k = %d  m = %d  n = %d   p ~= %.8f" % (
         #     num_hashes, num_bits, capacity,
         #     (1.0 - math.exp(- float(num_hashes) * float(capacity) / num_bits))
         #     ** num_hashes))
 
         # If a filename is provided, we should make a mmap-file
         # backed bloom filter. Otherwise, it will be malloc
@@ -149,26 +170,29 @@
                                                     num_bits,
                                                     self._oflags | os.O_CREAT,
                                                     perm,
                                                     <int *>seeds,
                                                     num_hashes)
         else:
             self._in_memory = 1
+            if data_array is not None:
+                data = data_array
             self._bf = cbloomfilter.bloomfilter_Create_Malloc(capacity,
                                                     error_rate,
                                                     num_bits,
                                                     <int *>seeds,
-                                                    num_hashes)
+                                                    num_hashes, <const char *>data)
         if self._bf is NULL:
             if filename:
                 raise OSError(errno, '%s: %s' % (os.strerror(errno),
                                                     filename))
             else:
                 cpython.PyErr_NoMemory()
 
+
     def _open(self, filename, mode="rw"):
         # Should not overwrite
         mode = mode.replace("+", "")
 
         if not os.path.exists(filename):
             raise OSError(eno.ENOENT, '%s: %s' % (os.strerror(eno.ENOENT),
                                                         filename))
@@ -199,14 +223,27 @@
         self._assert_open()
         start_pos = self._bf.array.preamblebytes
         end_pos = start_pos + self._bf.array.bytes
         arr = (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
         return int.from_bytes(arr, byteorder="big", signed=False)
 
     @property
+    def data_array(self):
+        """Bytes array of the Bloom filter contents.
+        """
+        self._assert_open()
+        start_pos = self._bf.array.preamblebytes
+        end_pos = start_pos + self._bf.array.bytes 
+        arr = array.array('B')
+        arr.frombytes(
+            (<char *>cbloomfilter.mbarray_CharData(self._bf.array))[start_pos:end_pos]
+        )
+        return bytes(arr)
+
+    @property
     def hash_seeds(self):
         """Integer seeds used for the random hashing. Returns a list of integers."""
         self._assert_open()
         seeds = array.array('I')
         seeds.frombytes(
             (<char *>self._bf.hash_seeds)[:4 * self.num_hashes]
         )
@@ -341,14 +378,15 @@
             key.shash = item
             key.nhash = len(item)
         elif isinstance(item_, bytes):
             item = item_
             key.shash = item
             key.nhash = len(item)
         else:
+            # Warning! Only works reliably for objects whose hash is based on value not memory address.
             item = item_
             key.shash = NULL
             key.nhash = hash(item)
         return cbloomfilter.bloomfilter_Test(self._bf, &key) == 1
 
     def copy_template(self, filename, perm=0755):
         """Creates a new :class:`BloomFilter` object with the exact same parameters.
```

### Comparing `pybloomfiltermmap3-0.5.7/src/superfast.h` & `pybloomfiltermmap3-0.6.0/src/superfast.h`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/__init__.py` & `pybloomfiltermmap3-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/__pycache__/__init__.cpython-38.pyc` & `pybloomfiltermmap3-0.6.0/tests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/__pycache__/accuracytest.cpython-38.pyc` & `pybloomfiltermmap3-0.6.0/tests/__pycache__/accuracytest.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/__pycache__/simpletest.cpython-38.pyc` & `pybloomfiltermmap3-0.6.0/tests/__pycache__/simpletest.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/accuracytest.py` & `pybloomfiltermmap3-0.6.0/tests/accuracytest.py`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/comparisons/accuracytest.py` & `pybloomfiltermmap3-0.6.0/tests/comparisons/accuracytest.py`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/comparisons/speedtest.py` & `pybloomfiltermmap3-0.6.0/tests/comparisons/speedtest.py`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/comparisons/testwords` & `pybloomfiltermmap3-0.6.0/tests/comparisons/testwords`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/comparisons/words` & `pybloomfiltermmap3-0.6.0/tests/comparisons/words`

 * *Files identical despite different names*

### Comparing `pybloomfiltermmap3-0.5.7/tests/simpletest.py` & `pybloomfiltermmap3-0.6.0/tests/simpletest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import string
 import unittest
 import tempfile
+import pickle
 from random import randint, choice, getrandbits
 
 import pybloomfilter
 
 from tests import with_test_file
 
 
@@ -396,12 +397,25 @@
         union_bf = bf1.copy(self.tempfile.name + '.union')
         union_bf.union(bf2)
 
         assert len(union_bf) == 29  # approximate size
         intersection = len(bf1) + len(bf2) - len(union_bf)
         assert intersection == 11  # approximate size
 
+    def test_pickle(self):
+        bf = pybloomfilter.BloomFilter(100, 0.1)
+        bf.add('apple')
+        assert 'apple' in bf
+        assert 'hello' not in bf
+
+        pickled = pickle.dumps(bf)
+        unpickled = pickle.loads(pickled)
+        assert 'apple' in unpickled
+        assert 'hello' not in unpickled
+
+        # Expecting same hashing sequence
+        self.assertEqual(bf.bit_array, unpickled.bit_array)
 
 def suite():
     suite = unittest.TestSuite()
     suite.addTest(unittest.makeSuite(SimpleTestCase))
     return suite
```

