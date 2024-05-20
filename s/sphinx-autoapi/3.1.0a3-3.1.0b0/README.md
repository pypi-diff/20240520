# Comparing `tmp/sphinx-autoapi-3.1.0a3.tar.gz` & `tmp/sphinx_autoapi-3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-autoapi-3.1.0a3.tar", last modified: Fri Feb 16 22:25:49 2024, max compression
+gzip compressed data, was "sphinx_autoapi-3.1b0.tar", last modified: Fri Apr 12 16:55:39 2024, max compression
```

## Comparing `sphinx-autoapi-3.1.0a3.tar` & `sphinx_autoapi-3.1b0.tar`

### file list

```diff
@@ -1,168 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.141608 sphinx-autoapi-3.1.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)    21049 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-02-16 22:25:49.141608 sphinx-autoapi-3.1.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.121608 sphinx-autoapi-3.1.0a3/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/documenters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/inheritance_diagrams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.121608 sphinx-autoapi-3.1.0a3/autoapi/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.121608 sphinx-autoapi-3.1.0a3/autoapi/mappers/python/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19433 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/python/astroid_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/python/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/python/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/mappers/python/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.121608 sphinx-autoapi-3.1.0a3/autoapi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.121608 sphinx-autoapi-3.1.0a3/autoapi/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/base/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/autoapi/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/autoapi/templates/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-16 22:25:49.141608 sphinx-autoapi-3.1.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-02-16 22:25:49.000000 sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-16 22:25:49.000000 sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 22:25:49.000000 sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-16 22:25:49.000000 sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-16 22:25:49.000000 sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/python/py310unionpipe/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py310unionpipe/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/python/py310unionpipe/example/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py310unionpipe/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py310unionpipe/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/python/py38positionalparams/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py38positionalparams/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/python/py38positionalparams/example/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py38positionalparams/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py38positionalparams/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.125608 sphinx-autoapi-3.1.0a3/tests/python/py3example/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3example/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/py3example/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3example/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3example/example/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.113608 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/namespace/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/namespace/example/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/namespace/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/namespace/sibling/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/namespace/sibling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/namespace/sibling/sub_sibling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyannotationcommentsexample/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyannotationcommentsexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyannotationcommentsexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyannotationcommentsexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyannotationcommentsexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/example/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/example/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyemptyexample/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyemptyexample/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyemptyexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyexample/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyexample/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyexample/manualapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyexample/null.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.129608 sphinx-autoapi-3.1.0a3/tests/python/pyiexample/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pyiexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample/example/example.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pyiexample2/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample2/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pyiexample2/example/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample2/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample2/example/example.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyiexample2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/confpy/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/confpy/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/manualapi.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/_private_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/binary_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/subpackage/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/subpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/subpackage/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/unicode_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildall/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildall/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildall/simple/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildall/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildcard/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildcard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.133608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildchain/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildwildchain/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/wildwildchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/_private_submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/submodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/subpackage/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/subpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/subpackage/submodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/python/pyskipexample/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyskipexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/python/pyskipexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyskipexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/pyskipexample/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    39628 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/test_own_page_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    41044 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/python/test_pyintegration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/templateexample/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/templateexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/templateexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/templateexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/templateexample/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.117608 sphinx-autoapi-3.1.0a3/tests/templateexample/template_overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/templateexample/template_overrides/python/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/templateexample/template_overrides/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/test_astroid_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/toctreeexample/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/toctreeexample/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:25:49.137608 sphinx-autoapi-3.1.0a3/tests/toctreeexample/example/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/toctreeexample/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-16 22:25:39.000000 sphinx-autoapi-3.1.0a3/tests/toctreeexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.483732 sphinx_autoapi-3.1b0/
+-rw-r--r--   0 runner    (1001) docker     (127)    21226 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-12 16:55:39.483732 sphinx_autoapi-3.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.463732 sphinx_autoapi-3.1b0/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_astroid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16244 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/documenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/inheritance_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.463732 sphinx_autoapi-3.1b0/autoapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.463732 sphinx_autoapi-3.1b0/autoapi/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/autoapi/templates/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 16:55:39.483732 sphinx_autoapi-3.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 16:55:39.000000 sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/pep695/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pep695/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/pep695/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pep695/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pep695/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py310unionpipe/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py38positionalparams/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py3example/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.467732 sphinx_autoapi-3.1b0/tests/python/py3example/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/example/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.455732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/sibling/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/sibling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/namespace/sibling/sub_sibling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/example/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyemptyexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyemptyexample/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyemptyexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/manualapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyexample/null.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyiexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.471732 sphinx_autoapi-3.1b0/tests/python/pyiexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/example/example.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyiexample2/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyiexample2/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/example/example.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyiexample2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/submodule_foo/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/example/submodule_foo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyisubmoduleinit/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/confpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/confpy/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/manualapi.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/_private_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/binary_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/subpackage/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/unicode_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.475732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildall/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildcard/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildcard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildwildchain/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/wildwildchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackageexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/_private_submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pyskipexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyskipexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/python/pyskipexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyskipexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/pyskipexample/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    41176 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/test_own_page_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42840 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/python/test_pyintegration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/templateexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/templateexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.459732 sphinx_autoapi-3.1b0/tests/templateexample/template_overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/templateexample/template_overrides/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/templateexample/template_overrides/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/test_astroid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/toctreeexample/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/toctreeexample/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:55:39.479732 sphinx_autoapi-3.1b0/tests/toctreeexample/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/toctreeexample/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 16:55:35.000000 sphinx_autoapi-3.1b0/tests/toctreeexample/index.rst
```

### Comparing `sphinx-autoapi-3.1.0a3/CHANGELOG.rst` & `sphinx_autoapi-3.1b0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Changelog
 =========
 
 Versions follow `Semantic Versioning <https://semver.org/>`_ (``<major>.<minor>.<patch>``).
 
 .. towncrier release notes start
 
-v3.1.0a3 (2024-02-16)
----------------------
+v3.1.0.b0 (2024-04-12)
+----------------------
 
-Bugfixes
+Features
 ^^^^^^^^
 
-- Rename "single page output" to "own page output". (#226)
+- Objects can render to their own page (#226)
+- Render PEP-695 type aliases as TypeAlias assignments. (#414)
+
+
+Bugfixes
+^^^^^^^^
 
-- Also added tests for own page output. (#226)
+- Values are always rendered for TypeAlises and PEP-695 type aliases. (#224)
+- Fix submodule with `__init__.pyi` documented as `__init__` instead of submodule name (#398)
+- Fix IndexError when a module docstring contains only a heading (#412)
+- Preserve strings inside Literal type annotations (#423)
+- Stopped using xrefs in page titles (#427)
+- Fix emitting ignore event twice for methods.
 
-- Fix some inherited members always being rendered. (#226)
 
-- Own page members of an entity are linked to after the docstring
-  of the parent entity. (#226)
+Misc
+^^^^
 
-- Fix entities below the "class" level that have their own page
-  from rendering incorrectly. (#226)
+- #388
 
 
 v3.0.0 (2023-09-26)
 -------------------
 
 Bugfixes
 ^^^^^^^^
```

### Comparing `sphinx-autoapi-3.1.0a3/LICENSE.rst` & `sphinx_autoapi-3.1b0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/PKG-INFO` & `sphinx_autoapi-3.1b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-autoapi
-Version: 3.1.0a3
+Version: 3.1.0b0
 Summary: Sphinx API documentation generator
 Home-page: http://github.com/readthedocs/sphinx-autoapi
 Author: Eric Holscher
 Author-email: eric@ericholscher.com
 Maintainer: Ashley Whetter
 Maintainer-email: ashley@awhetter.co.uk
 License: MIT
@@ -60,21 +60,22 @@
 Sphinx AutoAPI is a Sphinx extension for generating complete API documentation
 without needing to load, run, or import the project being documented.
 
 In contrast to the traditional `Sphinx autodoc <https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html>`_,
 which requires manual authoring and uses code imports,
 AutoAPI finds and generates documentation by parsing source code.
 
+For more information, see `the full documentation <https://sphinx-autoapi.readthedocs.org>`_.
+
 Getting Started
 ---------------
 
 The following steps will walk through how to add AutoAPI to an existing Sphinx project.
 For instructions on how to set up a Sphinx project,
-see Sphinx's documentation on
-`Getting Started <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.
+see `Sphinx's documentation <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.
 
 Installation
 ~~~~~~~~~~~~
 
 AutoAPI can be installed through pip:
 
 .. code-block:: bash
```

### Comparing `sphinx-autoapi-3.1.0a3/README.rst` & `sphinx_autoapi-3.1b0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,22 @@
 Sphinx AutoAPI is a Sphinx extension for generating complete API documentation
 without needing to load, run, or import the project being documented.
 
 In contrast to the traditional `Sphinx autodoc <https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html>`_,
 which requires manual authoring and uses code imports,
 AutoAPI finds and generates documentation by parsing source code.
 
+For more information, see `the full documentation <https://sphinx-autoapi.readthedocs.org>`_.
+
 Getting Started
 ---------------
 
 The following steps will walk through how to add AutoAPI to an existing Sphinx project.
 For instructions on how to set up a Sphinx project,
-see Sphinx's documentation on
-`Getting Started <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.
+see `Sphinx's documentation <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.
 
 Installation
 ~~~~~~~~~~~~
 
 AutoAPI can be installed through pip:
 
 .. code-block:: bash
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/directives.py` & `sphinx_autoapi-3.1b0/autoapi/directives.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from docutils.parsers.rst import Directive
 from docutils import nodes
 
 from sphinx.ext.autosummary import Autosummary, mangle_signature
 from sphinx.util.nodes import nested_parse_with_titles
 
-from .mappers.python.objects import PythonFunction
+from ._objects import PythonFunction
 
 
 class AutoapiSummary(Autosummary):
     """A version of autosummary that uses static analysis."""
 
     def get_items(self, names):
         items = []
@@ -44,23 +44,24 @@
     """Nested parsing to remove the first heading of included rST
 
     This is used to handle the case where we like to remove user supplied
     headings from module docstrings. This is required to reduce the number of
     duplicate headings on sections.
     """
 
-    has_content = 1
+    has_content = True
     required_arguments = 0
     optional_arguments = 0
     final_argument_whitespace = False
 
     def run(self):
         node = nodes.container()
         node.document = self.state.document
         nested_parse_with_titles(self.state, self.content, node)
         try:
-            title_node = node[0][0]
-            if isinstance(title_node, nodes.title):
-                del node[0][0]
+            if isinstance(node[0], nodes.section) and isinstance(
+                node[0][0], nodes.title
+            ):
+                node.children = node[0][1:] + node.children[1:]
         except IndexError:
             pass
         return node.children
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/documenters.py` & `sphinx_autoapi-3.1b0/autoapi/documenters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 
 from sphinx.ext import autodoc
 
-from .mappers.python import (
+from ._objects import (
     PythonFunction,
     PythonClass,
     PythonMethod,
     PythonProperty,
     PythonData,
     PythonAttribute,
     PythonException,
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/extension.py` & `sphinx_autoapi-3.1b0/autoapi/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from sphinx.errors import ExtensionError
 import sphinx.util.logging
 from docutils.parsers.rst import directives
 
 from . import documenters
 from .directives import AutoapiSummary, NestedParse
 from .inheritance_diagrams import AutoapiInheritanceDiagram
-from .mappers import PythonSphinxMapper
+from ._mapper import Mapper
 from .settings import API_ROOT
 
 LOGGER = sphinx.util.logging.getLogger(__name__)
 
 _DEFAULT_FILE_PATTERNS = ["*.py", "*.pyi"]
 _DEFAULT_IGNORE_PATTERNS = ["*migrations*"]
 _DEFAULT_OPTIONS = [
@@ -107,15 +107,15 @@
         elif app.srcdir != os.getcwd():
             warnings.warn(
                 "autoapi_template_dir will be expected to be "
                 "relative to the Sphinx source directory instead of "
                 "relative to where sphinx-build is run\n",
                 RemovedInAutoAPI3Warning,
             )
-    sphinx_mapper_obj = PythonSphinxMapper(
+    sphinx_mapper_obj = Mapper(
         app, template_dir=template_dir, dir_root=normalized_root, url_root=url_root
     )
 
     if app.config.autoapi_file_patterns:
         file_patterns = app.config.autoapi_file_patterns
     else:
         file_patterns = _DEFAULT_FILE_PATTERNS
@@ -163,15 +163,15 @@
 
 def doctree_read(app, doctree):
     """Inject AutoAPI into the TOC Tree dynamically."""
 
     if app.env.docname == "index":
         all_docs = set()
         insert = True
-        nodes = list(doctree.traverse(toctree))
+        nodes = list(doctree.findall(toctree))
         toc_entry = f"{app.config.autoapi_root}/index"
         add_entry = (
             nodes
             and app.config.autoapi_generate_api_docs
             and app.config.autoapi_add_toctree_entry
         )
         if not add_entry:
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/inheritance_diagrams.py` & `sphinx_autoapi-3.1b0/autoapi/inheritance_diagrams.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/mappers/python/astroid_utils.py` & `sphinx_autoapi-3.1b0/autoapi/_astroid_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import builtins
 import itertools
 import re
 
 import astroid
 import astroid.nodes
-
 import astroid.nodes.node_classes
-import sphinx.util.logging
-
-_LOGGER = sphinx.util.logging.getLogger(__name__)
 
 
 def resolve_import_alias(name, import_names):
     """Resolve a name from an aliased import to its original name.
 
     :param name: The potentially aliased name to resolve.
     :type name: str
@@ -116,64 +112,77 @@
     Returns:
         iterable(str): The full names.
     """
     for base in node.bases:
         yield _resolve_annotation(base)
 
 
-def _get_const_values(node):
-    value = None
+def _get_const_value(node):
+    if isinstance(node, astroid.nodes.Const):
+        if isinstance(node.value, str) and "\n" in node.value:
+            return '"""{0}"""'.format(node.value)
+
+    class NotConstException(Exception):
+        pass
+
+    def _inner(node):
+        if isinstance(node, (astroid.nodes.List, astroid.nodes.Tuple)):
+            new_value = []
+            for element in node.elts:
+                new_value.append(_inner(element))
+
+            if isinstance(node, astroid.nodes.Tuple):
+                return tuple(new_value)
+
+            return new_value
+        elif isinstance(node, astroid.nodes.Const):
+            # Don't allow multi-line strings inside a data structure.
+            if isinstance(node.value, str) and "\n" in node.value:
+                raise NotConstException()
 
-    if isinstance(node, (astroid.nodes.List, astroid.nodes.Tuple)):
-        new_value = []
-        for element in node.elts:
-            if isinstance(element, astroid.nodes.Const):
-                new_value.append(element.value)
-            elif isinstance(element, (astroid.nodes.List, astroid.nodes.Tuple)):
-                new_value.append(_get_const_values(element))
-            else:
-                break
-        else:
-            value = new_value
+            return node.value
 
-        if isinstance(node, astroid.nodes.Tuple):
-            value = tuple(new_value)
-    elif isinstance(node, astroid.nodes.Const):
-        value = node.value
+        raise NotConstException()
 
-    return value
+    try:
+        result = _inner(node)
+    except NotConstException:
+        return None
+
+    return repr(result)
 
 
 def get_assign_value(node):
     """Get the name and value of the assignment of the given node.
 
     Assignments to multiple names are ignored, as per PEP 257.
 
     Args:
         node (astroid.nodes.Assign or astroid.nodes.AnnAssign): The node
             to get the assignment value from.
 
     Returns:
-        tuple(str, object or None) or None: The name that is assigned
-        to, and the value assigned to the name (if it can be converted).
+        tuple(str, str or None) or None: The name that is assigned
+        to, and the string representation of the value assigned to the name
+        (if it can be converted).
     """
     try:
         targets = node.targets
     except AttributeError:
         targets = [node.target]
 
     if len(targets) == 1:
         target = targets[0]
         if isinstance(target, astroid.nodes.AssignName):
             name = target.name
         elif isinstance(target, astroid.nodes.AssignAttr):
             name = target.attrname
         else:
             return None
-        return (name, _get_const_values(node.value))
+        return (name, _get_const_value(node.value))
 
     return None
 
 
 def get_assign_annotation(node):
     """Get the type annotation of the assignment of the given node.
 
@@ -412,15 +421,28 @@
         resolved = resolve_qualname(annotation, annotation.as_string())
     elif isinstance(annotation, astroid.Subscript):
         value = _resolve_annotation(annotation.value)
         slice_node = annotation.slice
         # astroid.Index was removed in astroid v3
         if hasattr(astroid, "Index") and isinstance(slice_node, astroid.Index):
             slice_node = slice_node.value
-        if isinstance(slice_node, astroid.Tuple):
+        if value == "Literal":
+            if isinstance(slice_node, astroid.Tuple):
+                elts = slice_node.elts
+            else:
+                elts = [slice_node]
+            slice_ = ", ".join(
+                (
+                    elt.as_string()
+                    if isinstance(elt, astroid.Const)
+                    else _resolve_annotation(elt)
+                )
+                for elt in elts
+            )
+        elif isinstance(slice_node, astroid.Tuple):
             slice_ = ", ".join(_resolve_annotation(elt) for elt in slice_node.elts)
         else:
             slice_ = _resolve_annotation(slice_node)
         resolved = f"{value}[{slice_}]"
     elif isinstance(annotation, astroid.Tuple):
         resolved = (
             "(" + ", ".join(_resolve_annotation(elt) for elt in annotation.elts) + ")"
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/mappers/python/mapper.py` & `sphinx_autoapi-3.1b0/autoapi/_mapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import collections
 import copy
+import fnmatch
 import operator
 import os
 import re
 
+from jinja2 import Environment, FileSystemLoader
+import sphinx
 import sphinx.environment
 from sphinx.errors import ExtensionError
 import sphinx.util
+import sphinx.util.logging
 from sphinx.util.console import colorize
 from sphinx.util.display import status_iterator
 import sphinx.util.docstrings
-import sphinx.util.logging
+from sphinx.util.osutil import ensuredir
 
-from ..base import SphinxMapperBase
-from .parser import Parser
-from .objects import (
+from ._parser import Parser
+from ._objects import (
     PythonClass,
     PythonFunction,
     PythonModule,
     PythonMethod,
     PythonPackage,
     PythonProperty,
     PythonAttribute,
     PythonData,
     PythonException,
     TopLevelPythonPythonMapper,
 )
+from .settings import OWN_PAGE_LEVELS, TEMPLATE_DIR
 
 LOGGER = sphinx.util.logging.getLogger(__name__)
 
 
 def _expand_wildcard_placeholder(original_module, originals_map, placeholder):
     """Expand a wildcard placeholder to a sequence of named placeholders.
 
@@ -215,21 +219,19 @@
         elif sub_target:
             result += f":py:obj:`{sub_target}`\\ "
 
     # Strip off the extra "\ "
     return result[:-2]
 
 
-class PythonSphinxMapper(SphinxMapperBase):
-    """AutoAPI domain handler for Python
-
-    Parses directly from Python files.
+class Mapper:
+    """Base class for mapping `PythonMapperBase` objects to Sphinx.
 
     Args:
-        app: Sphinx application passed in as part of the extension
+        app: Sphinx application instance
     """
 
     _OBJ_MAP = {
         cls.type: cls
         for cls in (
             PythonClass,
             PythonFunction,
@@ -240,21 +242,150 @@
             PythonAttribute,
             PythonData,
             PythonException,
         )
     }
 
     def __init__(self, app, template_dir=None, dir_root=None, url_root=None):
-        super().__init__(app, template_dir, dir_root, url_root)
+        self.app = app
+
+        template_paths = [TEMPLATE_DIR]
+
+        if template_dir:
+            # Put at the front so it's loaded first
+            template_paths.insert(0, template_dir)
+
+        self.jinja_env = Environment(
+            loader=FileSystemLoader(template_paths),
+            trim_blocks=True,
+            lstrip_blocks=True,
+        )
+
+        def _wrapped_prepare(value):
+            return value
+
+        self.jinja_env.filters["prepare_docstring"] = _wrapped_prepare
+        if self.app.config.autoapi_prepare_jinja_env:
+            self.app.config.autoapi_prepare_jinja_env(self.jinja_env)
+
+        own_page_level = self.app.config.autoapi_own_page_level
+        desired_page_level = OWN_PAGE_LEVELS.index(own_page_level)
+        self.own_page_types = set(OWN_PAGE_LEVELS[: desired_page_level + 1])
+
+        self.dir_root = dir_root
+        self.url_root = url_root
+
+        # Mapping of {filepath -> raw data}
+        self.paths = collections.OrderedDict()
+        # Mapping of {object id -> Python Object}
+        self.objects_to_render = collections.OrderedDict()
+        # Mapping of {object id -> Python Object}
+        self.all_objects = collections.OrderedDict()
+        # Mapping of {namespace id -> Python Object}
+        self.namespaces = collections.OrderedDict()
 
         self.jinja_env.filters["link_objs"] = _link_objs
         self._use_implicit_namespace = (
             self.app.config.autoapi_python_use_implicit_namespaces
         )
 
+    @staticmethod
+    def find_files(patterns, dirs, ignore):
+        if not ignore:
+            ignore = []
+
+        pattern_regexes = []
+        for pattern in patterns:
+            regex = re.compile(fnmatch.translate(pattern).replace(".*", "(.*)"))
+            pattern_regexes.append((pattern, regex))
+
+        for _dir in dirs:
+            for root, _, filenames in os.walk(_dir):
+                seen = set()
+                for pattern, pattern_re in pattern_regexes:
+                    for filename in fnmatch.filter(filenames, pattern):
+                        skip = False
+
+                        match = re.match(pattern_re, filename)
+                        norm_name = match.groups()
+                        if norm_name in seen:
+                            continue
+
+                        # Skip ignored files
+                        for ignore_pattern in ignore:
+                            if fnmatch.fnmatch(
+                                os.path.join(root, filename), ignore_pattern
+                            ):
+                                LOGGER.info(
+                                    colorize("bold", "[AutoAPI] ")
+                                    + colorize(
+                                        "darkgreen", f"Ignoring {root}/{filename}"
+                                    )
+                                )
+                                skip = True
+
+                        if skip:
+                            continue
+
+                        # Make sure the path is full
+                        if not os.path.isabs(filename):
+                            filename = os.path.join(root, filename)
+
+                        yield filename
+                        seen.add(norm_name)
+
+    def add_object(self, obj):
+        """Add object to local and app environment storage
+
+        Args:
+            obj: Instance of a AutoAPI object
+        """
+        display = obj.display
+        if display and obj.type in self.own_page_types:
+            self.objects_to_render[obj.id] = obj
+
+        self.all_objects[obj.id] = obj
+        child_stack = list(obj.children)
+        while child_stack:
+            child = child_stack.pop()
+            self.all_objects[child.id] = child
+            if display and child.type in self.own_page_types:
+                self.objects_to_render[child.id] = child
+            child_stack.extend(getattr(child, "children", ()))
+
+    def output_rst(self, source_suffix):
+        for _, obj in status_iterator(
+            self.objects_to_render.items(),
+            colorize("bold", "[AutoAPI] ") + "Rendering Data... ",
+            length=len(self.objects_to_render),
+            verbosity=1,
+            stringify_func=(lambda x: x[0]),
+        ):
+            rst = obj.render(is_own_page=True)
+            if not rst:
+                continue
+
+            output_dir = obj.output_dir(self.dir_root)
+            ensuredir(output_dir)
+            output_path = output_dir / obj.output_filename()
+            path = f"{output_path}{source_suffix}"
+            with open(path, "wb+") as detail_file:
+                detail_file.write(rst.encode("utf-8"))
+
+        if self.app.config.autoapi_add_toctree_entry:
+            self._output_top_rst()
+
+    def _output_top_rst(self):
+        # Render Top Index
+        top_level_index = os.path.join(self.dir_root, "index.rst")
+        pages = [obj for obj in self.objects_to_render.values() if obj.display]
+        with open(top_level_index, "wb") as top_level_file:
+            content = self.jinja_env.get_template("index.rst")
+            top_level_file.write(content.render(pages=pages).encode("utf-8"))
+
     def _need_to_load(self, files):
         last_files = getattr(self.app.env, "autoapi_source_files", [])
         self.app.env.autoapi_source_files = files
 
         last_mtime = getattr(self.app.env, "autoapi_max_mtime", 0)
         this_mtime = max(os.path.getmtime(file) for _, file in files)
         self.app.env.autoapi_max_mtime = this_mtime
@@ -268,14 +399,15 @@
         return last_files != files or not last_mtime or last_mtime < this_mtime
 
     def _find_files(self, patterns, dirs, ignore):
         for dir_ in dirs:
             dir_root = dir_
             if (
                 os.path.exists(os.path.join(dir_, "__init__.py"))
+                or os.path.exists(os.path.join(dir_, "__init__.pyi"))
                 or self._use_implicit_namespace
             ):
                 dir_root = os.path.abspath(os.path.join(dir_, os.pardir))
 
             for path in self.find_files(patterns=patterns, dirs=[dir_], ignore=ignore):
                 yield dir_root, path
 
@@ -338,19 +470,40 @@
             modules[module["name"]] = (module, children)
 
         resolved = set()
         for module_name in modules:
             visit_path = collections.OrderedDict()
             _resolve_module_placeholders(modules, module_name, visit_path, resolved)
 
+    def _hide_yo_kids(self):
+        """For all direct children of a module/package, hide them if needed."""
+        for module in self.paths.values():
+            if module["all"] is not None:
+                all_names = set(module["all"])
+                for child in module["children"]:
+                    if child["qual_name"] not in all_names:
+                        child["hide"] = True
+            elif module["type"] == "module":
+                for child in module["children"]:
+                    if child.get("imported"):
+                        child["hide"] = True
+
     def map(self, options=None):
         self._resolve_placeholders()
+        self._hide_yo_kids()
         self.app.env.autoapi_annotations = {}
 
-        super().map(options)
+        for _, data in status_iterator(
+            self.paths.items(),
+            colorize("bold", "[AutoAPI] ") + "Mapping Data... ",
+            length=len(self.paths),
+            stringify_func=(lambda x: x[0]),
+        ):
+            for obj in self.create_class(data, options=options):
+                self.add_object(obj)
 
         top_level_objects = {
             obj.id: obj
             for obj in self.all_objects.values()
             if isinstance(obj, TopLevelPythonPythonMapper)
         }
         parents = {obj.name: obj for obj in top_level_objects.values()}
@@ -364,15 +517,15 @@
         for obj in top_level_objects.values():
             obj.submodules.sort()
             obj.subpackages.sort()
 
         self.app.env.autoapi_objects = self.objects_to_render
         self.app.env.autoapi_all_objects = self.all_objects
 
-    def create_class(self, data, options=None, **kwargs):
+    def create_class(self, data, options=None):
         """Create a class from the passed in data
 
         Args:
             data: dictionary data of parser output
         """
         try:
             cls = self._OBJ_MAP[data["type"]]
@@ -383,21 +536,18 @@
             obj = cls(
                 data,
                 class_content=self.app.config.autoapi_python_class_content,
                 options=self.app.config.autoapi_options,
                 jinja_env=self.jinja_env,
                 app=self.app,
                 url_root=self.url_root,
-                **kwargs,
             )
 
             for child_data in data.get("children", []):
-                for child_obj in self.create_class(
-                    child_data, options=options, **kwargs
-                ):
+                for child_obj in self.create_class(child_data, options=options):
                     obj.children.append(child_obj)
 
             # Some objects require children to establish their docstring
             # or type annotations (eg classes with inheritance),
             # so do this after all children have been created.
             lines = obj.docstring.splitlines()
             if lines:
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/mappers/python/objects.py` & `sphinx_autoapi-3.1b0/autoapi/_objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations
+
 import functools
 import pathlib
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
+import sphinx
+import sphinx.util
 import sphinx.util.logging
 
-from ..base import PythonMapperBase
-
+from .settings import OWN_PAGE_LEVELS
 
 LOGGER = sphinx.util.logging.getLogger(__name__)
 
 
 def _format_args(args_info, include_annotations=True, ignore_self=None):
     result = []
 
@@ -23,306 +26,354 @@
             + ((" = {}" if annotation else "={}").format(default) if default else "")
         )
         result.append(formatted)
 
     return ", ".join(result)
 
 
-class PythonPythonMapper(PythonMapperBase):
-    """A base class for all types of representations of Python objects.
+class PythonObject:
+    """A class representing an entity from the parsed source code.
+
+    This class turns the dictionaries output by the parser into an object.
 
-    Attributes:
-        name (str): The name given to this object.
-        id (str): A unique identifier for this object.
-        children (list(PythonPythonMapper)): The members of this object.
+    Args:
+        obj: JSON object representing this object
+        jinja_env: A template environment for rendering this object
     """
 
-    language = "python"
-    is_callable = False
     member_order = 0
+    """The ordering of objects when doing "groupwise" sorting."""
     type: str
 
-    def __init__(self, obj, class_content="class", **kwargs) -> None:
-        super().__init__(obj, **kwargs)
-
-        self.name = obj["name"]
-        self.qual_name = obj["qual_name"]
-        self.id = obj.get("full_name", self.name)
-
-        # Optional
-        self.children: List[PythonPythonMapper] = []
-        self._docstring = obj["doc"]
-        self._docstring_resolved = False
-        self.imported = "original_path" in obj
-        self.inherited = obj.get("inherited", False)
-        """Whether this was inherited from an ancestor of the parent class.
-
-        :type: bool
-        """
+    def __init__(
+        self, obj, jinja_env, app, url_root, options=None, class_content="class"
+    ):
+        self.app = app
+        self.obj = obj
+        self.options = options
+        self.jinja_env = jinja_env
+        self.url_root = url_root
+
+        self.name: str = obj["name"]
+        """The name of the object, as named in the parsed source code.
+
+        This name will have no periods in it.
+        """
+        self.qual_name: str = obj["qual_name"]
+        """The qualified name for this object."""
+        self.id: str = obj.get("full_name", self.name)
+        """A globally unique identifier for this object.
+
+        This is the same as the fully qualified name of the object.
+        """
+
+        self.children: List[PythonObject] = []
+        """The members of this object.
+
+        For example, the classes and functions defined in the parent module.
+        """
+        self._docstring: str = obj["doc"]
+        self.imported: bool = "original_path" in obj
+        """Whether this object was imported from another module."""
+        self.inherited: bool = obj.get("inherited", False)
+        """Whether this was inherited from an ancestor of the parent class."""
+        self._hide = obj.get("hide", False)
 
         # For later
         self._class_content = class_content
-
         self._display_cache: Optional[bool] = None
 
+    def __getstate__(self):
+        """Obtains serialisable data for pickling."""
+        __dict__ = self.__dict__.copy()
+        __dict__.update(app=None, jinja_env=None)  # clear unpickable attributes
+        return __dict__
+
+    def render(self, **kwargs):
+        LOGGER.log("VERBOSE", "Rendering %s", self.id)
+
+        template = self.jinja_env.get_template(f"python/{self.type}.rst")
+
+        ctx = {}
+        ctx.update(**self.get_context_data())
+        ctx.update(**kwargs)
+        return template.render(**ctx)
+
+    @property
+    def rendered(self):
+        """Shortcut to render an object in templates."""
+        return self.render()
+
+    def get_context_data(self):
+        own_page_level = self.app.config.autoapi_own_page_level
+        desired_page_level = OWN_PAGE_LEVELS.index(own_page_level)
+        own_page_types = set(OWN_PAGE_LEVELS[: desired_page_level + 1])
+
+        return {
+            "autoapi_options": self.app.config.autoapi_options,
+            "include_summaries": self.app.config.autoapi_include_summaries,
+            "obj": self,
+            "own_page_types": own_page_types,
+            "sphinx_version": sphinx.version_info,
+        }
+
+    def __lt__(self, other):
+        """Object sorting comparison"""
+        if not isinstance(other, PythonObject):
+            return NotImplemented
+
+        return self.id < other.id
+
+    def __str__(self) -> str:
+        return f"<{self.__class__.__name__} {self.id}>"
+
+    @property
+    def short_name(self) -> str:
+        """Shorten name property"""
+        return self.name.split(".")[-1]
+
+    def output_dir(self, root):
+        """The directory to render this object."""
+        module = self.id[: -(len("." + self.qual_name))]
+        parts = [root] + module.split(".")
+        return pathlib.PurePosixPath(*parts)
+
+    def output_filename(self) -> str:
+        """The name of the file to render into, without a file suffix."""
+        filename = self.qual_name
+        if filename == "index":
+            filename = ".index"
+
+        return filename
+
+    @property
+    def include_path(self) -> str:
+        """Return 'absolute' path without regarding OS path separator
+
+        This is used in ``toctree`` directives, as Sphinx always expects Unix
+        path separators
+        """
+        return str(self.output_dir(self.url_root) / self.output_filename())
+
     @property
-    def docstring(self):
+    def docstring(self) -> str:
         """The docstring for this object.
 
         If a docstring did not exist on the object,
         this will be the empty string.
 
-        For classes this will also depend on the
+        For classes, this will also depend on the
         :confval:`autoapi_python_class_content` option.
-
-        :type: str
         """
         return self._docstring
 
     @docstring.setter
-    def docstring(self, value):
+    def docstring(self, value: str) -> None:
         self._docstring = value
         self._docstring_resolved = True
 
     @property
-    def is_top_level_object(self):
+    def is_top_level_object(self) -> bool:
         """Whether this object is at the very top level (True) or not (False).
 
         This will be False for subpackages and submodules.
-
-        :type: bool
         """
         return "." not in self.id
 
     @property
-    def is_undoc_member(self):
-        """Whether this object has a docstring (False) or not (True).
-
-        :type: bool
-        """
+    def is_undoc_member(self) -> bool:
+        """Whether this object has a docstring (False) or not (True)."""
         return not bool(self.docstring)
 
     @property
-    def is_private_member(self):
-        """Whether this object is private (True) or not (False).
-
-        :type: bool
-        """
+    def is_private_member(self) -> bool:
+        """Whether this object is private (True) or not (False)."""
         return self.short_name.startswith("_") and not self.short_name.endswith("__")
 
     @property
-    def is_special_member(self):
-        """Whether this object is a special member (True) or not (False).
-
-        :type: bool
-        """
+    def is_special_member(self) -> bool:
+        """Whether this object is a special member (True) or not (False)."""
         return self.short_name.startswith("__") and self.short_name.endswith("__")
 
     @property
-    def display(self):
+    def display(self) -> bool:
         """Whether this object should be displayed in documentation.
 
         This attribute depends on the configuration options given in
         :confval:`autoapi_options` and the result of :event:`autoapi-skip-member`.
-
-        :type: bool
         """
         if self._display_cache is None:
             self._display_cache = not self._ask_ignore(self._should_skip())
 
         return self._display_cache
 
     @property
-    def summary(self):
+    def summary(self) -> str:
         """The summary line of the docstring.
 
         The summary line is the first non-empty line, as-per :pep:`257`.
         This will be the empty string if the object does not have a docstring.
-
-        :type: str
         """
         for line in self.docstring.splitlines():
             line = line.strip()
             if line:
                 return line
 
         return ""
 
-    def _should_skip(self):  # type: () -> bool
+    def _should_skip(self) -> bool:
         skip_undoc_member = self.is_undoc_member and "undoc-members" not in self.options
         skip_private_member = (
             self.is_private_member and "private-members" not in self.options
         )
         skip_special_member = (
             self.is_special_member and "special-members" not in self.options
         )
         skip_imported_member = self.imported and "imported-members" not in self.options
         skip_inherited_member = (
             self.inherited and "inherited-members" not in self.options
         )
 
         return (
-            skip_undoc_member
+            self._hide
+            or skip_undoc_member
             or skip_private_member
             or skip_special_member
             or skip_imported_member
             or skip_inherited_member
         )
 
-    def _ask_ignore(self, skip):  # type: (bool) -> bool
+    def _ask_ignore(self, skip: bool) -> bool:
         ask_result = self.app.emit_firstresult(
             "autoapi-skip-member", self.type, self.id, self, skip, self.options
         )
 
         return ask_result if ask_result is not None else skip
 
-    def _children_of_type(self, type_):
+    def _children_of_type(self, type_: str) -> List[PythonObject]:
         return list(child for child in self.children if child.type == type_)
 
 
-class PythonFunction(PythonPythonMapper):
+class PythonFunction(PythonObject):
     """The representation of a function."""
 
     type = "function"
-    is_callable = True
     member_order = 30
 
-    def __init__(self, obj, **kwargs):
-        super().__init__(obj, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
         autodoc_typehints = getattr(self.app.config, "autodoc_typehints", "signature")
         show_annotations = autodoc_typehints != "none" and not (
-            autodoc_typehints == "description" and not obj["overloads"]
+            autodoc_typehints == "description" and not self.obj["overloads"]
         )
-        self.args = _format_args(obj["args"], show_annotations)
-        """The arguments to this object, formatted as a string.
-
-        :type: str
-        """
+        self.args: str = _format_args(self.obj["args"], show_annotations)
+        """The arguments to this object, formatted as a string."""
 
-        self.return_annotation = obj["return_annotation"] if show_annotations else None
+        self.return_annotation: Optional[str] = (
+            self.obj["return_annotation"] if show_annotations else None
+        )
         """The type annotation for the return type of this function.
 
         This will be ``None`` if an annotation
         or annotation comment was not given.
-
-        :type: str or None
         """
-        self.properties = obj["properties"]
+        self.properties: List[str] = self.obj["properties"]
         """The properties that describe what type of function this is.
 
-        Can be only be: async
-
-        :type: list(str)
+        Can be only be: async.
         """
-        self.overloads = [
+        self.overloads: List[Tuple[str, str]] = [
             (_format_args(args), return_annotation)
-            for args, return_annotation in obj["overloads"]
+            for args, return_annotation in self.obj["overloads"]
         ]
         """The overloaded signatures of this function.
 
         Each tuple is a tuple of ``(args, return_annotation)``
-
-        :type: list(tuple(str, str))
         """
 
 
 class PythonMethod(PythonFunction):
     """The representation of a method."""
 
     type = "method"
-    is_callable = True
     member_order = 50
 
-    def __init__(self, obj, **kwargs):
-        super().__init__(obj, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        self.properties = obj["properties"]
+        self.properties: List[str] = self.obj["properties"]
         """The properties that describe what type of method this is.
 
-        Can be any of: abstractmethod, async, classmethod, property, staticmethod
-
-        :type: list(str)
+        Can be any of: abstractmethod, async, classmethod, property, staticmethod.
         """
 
-    def _should_skip(self):  # type: () -> bool
-        skip = super()._should_skip() or self.name in (
+    def _should_skip(self) -> bool:
+        return super()._should_skip() or self.name in (
             "__new__",
             "__init__",
         )
-        return self._ask_ignore(skip)
 
 
-class PythonProperty(PythonPythonMapper):
+class PythonProperty(PythonObject):
     """The representation of a property on a class."""
 
     type = "property"
     member_order = 60
 
-    def __init__(self, obj, **kwargs):
-        super().__init__(obj, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        self.annotation = obj["return_annotation"]
-        """The type annotation of this property.
-
-        :type: str or None
-        """
-        self.properties = obj["properties"]
+        self.annotation: Optional[str] = self.obj["return_annotation"]
+        """The type annotation of this property."""
+        self.properties: List[str] = self.obj["properties"]
         """The properties that describe what type of property this is.
 
-        Can be any of: abstractmethod, classmethod
-
-        :type: list(str)
+        Can be any of: abstractmethod, classmethod.
         """
 
 
-class PythonData(PythonPythonMapper):
+class PythonData(PythonObject):
     """Global, module level data."""
 
     type = "data"
     member_order = 40
 
-    def __init__(self, obj, **kwargs):
-        super().__init__(obj, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        self.value = obj.get("value")
+        self.value: Optional[str] = self.obj.get("value")
         """The value of this attribute.
 
         This will be ``None`` if the value is not constant.
-
-        :type: str or None
         """
-        self.annotation = obj.get("annotation")
+        self.annotation: Optional[str] = self.obj.get("annotation")
         """The type annotation of this attribute.
 
         This will be ``None`` if an annotation
         or annotation comment was not given.
-
-        :type: str or None
         """
 
 
 class PythonAttribute(PythonData):
     """An object/class level attribute."""
 
     type = "attribute"
     member_order = 60
 
 
-class TopLevelPythonPythonMapper(PythonPythonMapper):
+class TopLevelPythonPythonMapper(PythonObject):
     """A common base class for modules and packages."""
 
-    _RENDER_LOG_LEVEL = "VERBOSE"
-
-    def __init__(self, obj, **kwargs):
-        super().__init__(obj, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
         self.subpackages = []
         self.submodules = []
-        self.all = obj["all"]
+        self.all = self.obj["all"]
         """The contents of ``__all__`` if assigned to.
 
         Only constants are included.
         This will be ``None`` if no ``__all__`` was set.
 
         :type: list(str) or None
         """
@@ -342,15 +393,15 @@
         :type: list(PythonClass)
         """
         return self._children_of_type("class")
 
     def output_dir(self, root):
         """The path to the file to render into, without a file suffix."""
         parts = [root] + self.name.split(".")
-        return pathlib.PosixPath(*parts)
+        return pathlib.PurePosixPath(*parts)
 
     def output_filename(self):
         """The path to the file to render into, without a file suffix."""
         return "index"
 
 
 class PythonModule(TopLevelPythonPythonMapper):
@@ -361,35 +412,31 @@
 
 class PythonPackage(TopLevelPythonPythonMapper):
     """The representation of a package."""
 
     type = "package"
 
 
-class PythonClass(PythonPythonMapper):
+class PythonClass(PythonObject):
     """The representation of a class."""
 
     type = "class"
     member_order = 20
 
-    def __init__(self, obj, **kwargs):
-        super().__init__(obj, **kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-        self.bases = obj["bases"]
-        """The fully qualified names of all base classes.
+        self.bases: List[str] = self.obj["bases"]
+        """The fully qualified names of all base classes."""
 
-        :type: list(str)
-        """
+        self._docstring_resolved: bool = False
 
     @property
-    def args(self):
-        """The arguments to this object, formatted as a string.
-
-        :type: str
-        """
+    def args(self) -> str:
+        """The arguments to this object, formatted as a string."""
         args = ""
 
         if self.constructor:
             autodoc_typehints = getattr(
                 self.app.config, "autodoc_typehints", "signature"
             )
             show_annotations = autodoc_typehints != "none" and not (
@@ -397,15 +444,15 @@
             )
             args_data = self.constructor.obj["args"]
             args = _format_args(args_data, show_annotations, ignore_self="self")
 
         return args
 
     @property
-    def overloads(self):
+    def overloads(self) -> List[Tuple[str, str]]:
         overloads = []
 
         if self.constructor:
             overload_data = self.constructor.obj["overloads"]
             autodoc_typehints = getattr(
                 self.app.config, "autodoc_typehints", "signature"
             )
@@ -417,31 +464,32 @@
                 )
                 for args, return_annotation in overload_data
             ]
 
         return overloads
 
     @property
-    def docstring(self):
-        docstring = super().docstring
+    def docstring(self) -> str:
+        docstring = self._docstring
 
         if not self._docstring_resolved and self._class_content in ("both", "init"):
             constructor_docstring = self.constructor_docstring
 
             if constructor_docstring:
                 if self._class_content == "both":
                     docstring = f"{docstring}\n{constructor_docstring}"
                 else:
                     docstring = constructor_docstring
 
         return docstring
 
     @docstring.setter
-    def docstring(self, value):
-        super(PythonClass, self.__class__).docstring.fset(self, value)
+    def docstring(self, value: str) -> None:
+        self._docstring = value
+        self._docstring_resolved = True
 
     @property
     def methods(self):
         return self._children_of_type("method")
 
     @property
     def properties(self):
@@ -461,15 +509,15 @@
         for child in self.children:
             if child.short_name == "__init__":
                 return child
 
         return None
 
     @property
-    def constructor_docstring(self):
+    def constructor_docstring(self) -> str:
         docstring = ""
 
         constructor = self.constructor
         if constructor and constructor.docstring:
             docstring = constructor.docstring
         else:
             for child in self.children:
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/mappers/python/parser.py` & `sphinx_autoapi-3.1b0/autoapi/_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 import os
 
 import astroid
 import astroid.builder
 import sphinx.util.docstrings
 
-from . import astroid_utils
+from . import _astroid_utils
 
 
 def _prepare_docstring(doc):
     return "\n".join(sphinx.util.docstrings.prepare_docstring(doc))
 
 
 class Parser:
@@ -24,15 +24,15 @@
 
     def _get_full_name(self, name):
         return ".".join(self._full_name_stack + [name])
 
     def _parse_file(self, file_path, condition):
         directory, filename = os.path.split(file_path)
         module_parts = []
-        if filename != "__init__.py":
+        if filename != "__init__.py" and filename != "__init__.pyi":
             module_part = os.path.splitext(filename)[0]
             module_parts = [module_part]
         module_parts = collections.deque(module_parts)
         while directory and condition(directory):
             directory, module_part = os.path.split(directory)
             if module_part:
                 module_parts.appendleft(module_part)
@@ -40,15 +40,18 @@
         module_name = ".".join(module_parts)
         node = astroid.builder.AstroidBuilder().file_build(file_path, module_name)
         return self.parse(node)
 
     def parse_file(self, file_path):
         return self._parse_file(
             file_path,
-            lambda directory: os.path.isfile(os.path.join(directory, "__init__.py")),
+            lambda directory: (
+                os.path.isfile(os.path.join(directory, "__init__.py"))
+                or os.path.isfile(os.path.join(directory, "__init__.pyi"))
+            ),
         )
 
     def parse_file_in_namespace(self, file_path, dir_root):
         return self._parse_file(
             file_path, lambda directory: os.path.abspath(directory) != dir_root
         )
 
@@ -73,25 +76,27 @@
             doc_node.value, astroid.nodes.Const
         ):
             doc = doc_node.value.value
 
         type_ = "data"
         if isinstance(
             node.scope(), astroid.nodes.ClassDef
-        ) or astroid_utils.is_constructor(node.scope()):
+        ) or _astroid_utils.is_constructor(node.scope()):
             type_ = "attribute"
 
-        assign_value = astroid_utils.get_assign_value(node)
+        assign_value = _astroid_utils.get_assign_value(node)
         if not assign_value:
             return []
 
         target = assign_value[0]
         value = assign_value[1]
 
-        annotation = astroid_utils.get_assign_annotation(node)
+        annotation = _astroid_utils.get_assign_annotation(node)
+        if annotation in ("TypeAlias", "typing.TypeAlias"):
+            value = node.value.as_string()
 
         data = {
             "type": type_,
             "name": target,
             "qual_name": self._get_qual_name(target),
             "full_name": self._get_full_name(target),
             "doc": _prepare_docstring(doc),
@@ -101,26 +106,26 @@
             "annotation": annotation,
         }
 
         return [data]
 
     def parse_classdef(self, node, data=None):
         type_ = "class"
-        if astroid_utils.is_exception(node):
+        if _astroid_utils.is_exception(node):
             type_ = "exception"
 
-        basenames = list(astroid_utils.get_full_basenames(node))
+        basenames = list(_astroid_utils.get_full_basenames(node))
 
         data = {
             "type": type_,
             "name": node.name,
             "qual_name": self._get_qual_name(node.name),
             "full_name": self._get_full_name(node.name),
             "bases": basenames,
-            "doc": _prepare_docstring(astroid_utils.get_class_docstring(node)),
+            "doc": _prepare_docstring(_astroid_utils.get_class_docstring(node)),
             "from_line_no": node.fromlineno,
             "to_line_no": node.tolineno,
             "children": [],
         }
 
         self._qual_name_stack.append(node.name)
         self._full_name_stack.append(node.name)
@@ -133,15 +138,15 @@
                 "builtins.object",
                 "builtins.type",
             ):
                 continue
             for child in base.get_children():
                 name = getattr(child, "name", None)
                 if isinstance(child, (astroid.Assign, astroid.AnnAssign)):
-                    assign_value = astroid_utils.get_assign_value(child)
+                    assign_value = _astroid_utils.get_assign_value(child)
                     if not assign_value:
                         continue
                     name = assign_value[0]
 
                 if not name or name in overridden:
                     continue
                 seen.add(name)
@@ -157,26 +162,26 @@
 
         return [data]
 
     def parse_asyncfunctiondef(self, node):
         return self.parse_functiondef(node)
 
     def parse_functiondef(self, node):
-        if astroid_utils.is_decorated_with_property_setter(node):
+        if _astroid_utils.is_decorated_with_property_setter(node):
             return []
 
         type_ = "method"
         properties = []
 
         if node.type == "function":
             type_ = "function"
 
             if isinstance(node, astroid.AsyncFunctionDef):
                 properties.append("async")
-        elif astroid_utils.is_decorated_with_property(node):
+        elif _astroid_utils.is_decorated_with_property(node):
             type_ = "property"
             if node.type == "classmethod":
                 properties.append(node.type)
             if node.is_abstract(pass_is_abstract=False):
                 properties.append("abstractmethod")
         else:
             # "__new__" method is implicit classmethod
@@ -188,21 +193,21 @@
                 properties.append("async")
 
         data = {
             "type": type_,
             "name": node.name,
             "qual_name": self._get_qual_name(node.name),
             "full_name": self._get_full_name(node.name),
-            "args": astroid_utils.get_args_info(node.args),
-            "doc": _prepare_docstring(astroid_utils.get_func_docstring(node)),
+            "args": _astroid_utils.get_args_info(node.args),
+            "doc": _prepare_docstring(_astroid_utils.get_func_docstring(node)),
             "from_line_no": node.fromlineno,
             "to_line_no": node.tolineno,
-            "return_annotation": astroid_utils.get_return_annotation(node),
+            "return_annotation": _astroid_utils.get_return_annotation(node),
             "properties": properties,
-            "is_overload": astroid_utils.is_decorated_with_overload(node),
+            "is_overload": _astroid_utils.is_decorated_with_overload(node),
             "overloads": [],
         }
 
         result = [data]
 
         if node.name == "__init__":
             for child in node.get_children():
@@ -213,15 +218,15 @@
         return result
 
     def _parse_local_import_from(self, node):
         result = []
 
         for import_name, alias in node.names:
             is_wildcard = (alias or import_name) == "*"
-            original_path = astroid_utils.get_full_import_name(
+            original_path = _astroid_utils.get_full_import_name(
                 node, alias or import_name
             )
             name = original_path if is_wildcard else (alias or import_name)
             qual_name = self._get_qual_name(alias or import_name)
             full_name = self._get_full_name(alias or import_name)
 
             data = {
@@ -252,29 +257,58 @@
             "name": node.name,
             "qual_name": node.name,
             "full_name": node.name,
             "doc": _prepare_docstring(node.doc_node.value if node.doc_node else ""),
             "children": [],
             "file_path": path,
             "encoding": node.file_encoding,
-            "all": astroid_utils.get_module_all(node),
+            "all": _astroid_utils.get_module_all(node),
         }
 
         overloads = {}
         top_name = node.name.split(".", 1)[0]
         for child in node.get_children():
-            if astroid_utils.is_local_import_from(child, top_name):
+            if _astroid_utils.is_local_import_from(child, top_name):
                 child_data = self._parse_local_import_from(child)
             else:
                 child_data = self.parse(child)
 
             data["children"].extend(_parse_child(node, child_data, overloads))
 
         return data
 
+    def parse_typealias(self, node):
+        doc = ""
+        doc_node = node.next_sibling()
+        if isinstance(doc_node, astroid.nodes.Expr) and isinstance(
+            doc_node.value, astroid.nodes.Const
+        ):
+            doc = doc_node.value.value
+
+        if isinstance(node.name, astroid.nodes.AssignName):
+            name = node.name.name
+        elif isinstance(node.name, astroid.nodes.AssignAttr):
+            name = node.name.attrname
+        else:
+            return []
+
+        data = {
+            "type": "data",
+            "name": name,
+            "qual_name": self._get_qual_name(name),
+            "full_name": self._get_full_name(name),
+            "doc": _prepare_docstring(doc),
+            "value": node.value.as_string(),
+            "from_line_no": node.fromlineno,
+            "to_line_no": node.tolineno,
+            "annotation": "TypeAlias",
+        }
+
+        return [data]
+
     def parse(self, node):
         data = {}
 
         node_type = node.__class__.__name__.lower()
         parse_func = getattr(self, "parse_" + node_type, None)
         if parse_func:
             data = parse_func(node)
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/templates/python/class.rst` & `sphinx_autoapi-3.1b0/autoapi/templates/python/class.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% if obj.display %}
    {% if is_own_page %}
-:class:`{{ obj.id }}`
-========={{ "=" * obj.id | length }}
+{{ obj.id }}
+{{ "=" * obj.id | length }}
 
    {% endif %}
    {% set visible_children = obj.children|selectattr("display")|list %}
    {% set own_page_children = visible_children|selectattr("type", "in", own_page_types)|list %}
    {% if is_own_page and own_page_children %}
 .. toctree::
    :hidden:
@@ -44,15 +44,15 @@
    {% for obj_item in visible_children %}
       {% if obj_item.type not in own_page_types %}
 
    {{ obj_item.render()|indent(3) }}
       {% endif %}
    {% endfor %}
    {% if is_own_page and own_page_children %}
-      {% set visible_attributes = own_page_children|selectattr("type", "in", ("attribute", "property"))|list %}
+      {% set visible_attributes = own_page_children|selectattr("type", "equalto", "attribute")|list %}
       {% if visible_attributes %}
 Attributes
 ----------
 
 .. autoapisummary::
 
          {% for attribute in visible_attributes %}
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/templates/python/data.rst` & `sphinx_autoapi-3.1b0/autoapi/templates/python/function.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,21 @@
 {% if obj.display %}
    {% if is_own_page %}
-:py:{{ obj.type|truncate(4, True, "", 0) }}:`{{ obj.id }}`
-==========={{ "=" * obj.id | length }}
+{{ obj.id }}
+{{ "=" * obj.id | length }}
 
    {% endif %}
-.. py:{{ obj.type }}:: {% if is_own_page %}{{ obj.id }}{% else %}{{ obj.name }}{% endif %}
-   {% if obj.annotation is not none %}
+.. py:function:: {% if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ obj.args }}){% if obj.return_annotation is not none %} -> {{ obj.return_annotation }}{% endif %}
+   {% for (args, return_annotation) in obj.overloads %}
 
-   :type: {% if obj.annotation %} {{ obj.annotation }}{% endif %}
-   {% endif %}
-   {% if obj.value is not none %}
-
-      {% if obj.value is string and obj.value.splitlines()|count > 1 %}
-   :value: Multiline-String
-
-   .. raw:: html
-
-      <details><summary>Show Value</summary>
-
-   .. code-block:: python
+                 {%+ if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ args }}){% if return_annotation is not none %} -> {{ return_annotation }}{% endif %}
+   {% endfor %}
+   {% for property in obj.properties %}
 
-      """{{ obj.value|indent(width=6,blank=true) }}"""
-
-   .. raw:: html
-
-      </details>
-
-      {% else %}
-         {% if obj.value is string %}
-   :value: {{ "%r" % obj.value|string|truncate(100) }}
-         {% else %}
-   :value: {{ obj.value|string|truncate(100) }}
-         {% endif %}
-      {% endif %}
-   {% endif %}
+   :{{ property }}:
+   {% endfor %}
 
    {% if obj.docstring %}
 
    {{ obj.docstring|indent(3) }}
    {% endif %}
 {% endif %}
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/templates/python/function.rst` & `sphinx_autoapi-3.1b0/autoapi/templates/python/method.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% if obj.display %}
    {% if is_own_page %}
-:py:func:`{{ obj.id }}`
-==========={{ "=" * obj.id | length }}
+{{ obj.id }}
+{{ "=" * obj.id | length }}
 
    {% endif %}
-.. py:function:: {% if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ obj.args }}){% if obj.return_annotation is not none %} -> {{ obj.return_annotation }}{% endif %}
+.. py:method:: {% if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ obj.args }}){% if obj.return_annotation is not none %} -> {{ obj.return_annotation }}{% endif %}
    {% for (args, return_annotation) in obj.overloads %}
 
-                 {%+ if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ args }}){% if return_annotation is not none %} -> {{ return_annotation }}{% endif %}
+               {%+ if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ args }}){% if return_annotation is not none %} -> {{ return_annotation }}{% endif %}
    {% endfor %}
    {% for property in obj.properties %}
 
    :{{ property }}:
    {% endfor %}
 
    {% if obj.docstring %}
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/templates/python/method.rst` & `sphinx_autoapi-3.1b0/autoapi/templates/python/data.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 {% if obj.display %}
    {% if is_own_page %}
-:py:meth:`{{ obj.id }}`
-==========={{ "=" * obj.id | length }}
+{{ obj.id }}
+{{ "=" * obj.id | length }}
 
    {% endif %}
-.. py:method:: {% if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ obj.args }}){% if obj.return_annotation is not none %} -> {{ obj.return_annotation }}{% endif %}
-   {% for (args, return_annotation) in obj.overloads %}
+.. py:{{ obj.type }}:: {% if is_own_page %}{{ obj.id }}{% else %}{{ obj.name }}{% endif %}
+   {% if obj.annotation is not none %}
 
-               {%+ if is_own_page %}{{ obj.id }}{% else %}{{ obj.short_name }}{% endif %}({{ args }}){% if return_annotation is not none %} -> {{ return_annotation }}{% endif %}
-   {% endfor %}
-   {% for property in obj.properties %}
+   :type: {% if obj.annotation %} {{ obj.annotation }}{% endif %}
+   {% endif %}
+   {% if obj.value is not none %}
+
+      {% if obj.value.splitlines()|count > 1 %}
+   :value: Multiline-String
+
+   .. raw:: html
+
+      <details><summary>Show Value</summary>
+
+   .. code-block:: python
 
-   :{{ property }}:
-   {% endfor %}
+      {{ obj.value|indent(width=6,blank=true) }}
+
+   .. raw:: html
+
+      </details>
+
+      {% else %}
+   :value: {{ obj.value|truncate(100) }}
+      {% endif %}
+   {% endif %}
 
    {% if obj.docstring %}
 
    {{ obj.docstring|indent(3) }}
    {% endif %}
 {% endif %}
```

### Comparing `sphinx-autoapi-3.1.0a3/autoapi/templates/python/module.rst` & `sphinx_autoapi-3.1b0/autoapi/templates/python/module.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% if obj.display %}
    {% if is_own_page %}
-:py:mod:`{{ obj.id }}`
-=========={{ "=" * obj.id|length }}
+{{ obj.id }}
+{{ "=" * obj.id|length }}
 
 .. py:module:: {{ obj.name }}
 
       {% if obj.docstring %}
 .. autoapi-nested-parse::
 
    {{ obj.docstring|indent(3) }}
@@ -41,21 +41,15 @@
    {{ submodule.include_path }}
             {% endfor %}
 
 
          {% endif %}
       {% endblock %}
       {% block content %}
-         {% if obj.all is not none %}
-            {% set visible_children = obj.children|selectattr("short_name", "in", obj.all)|list %}
-         {% elif obj.type is equalto("package") %}
-            {% set visible_children = obj.children|selectattr("display")|list %}
-         {% else %}
-            {% set visible_children = obj.children|selectattr("display")|rejectattr("imported")|list %}
-         {% endif %}
+         {% set visible_children = obj.children|selectattr("display")|list %}
          {% if visible_children %}
             {% set visible_attributes = visible_children|selectattr("type", "equalto", "data")|list %}
             {% if visible_attributes %}
                {% if "attribute" in own_page_types or "show-module-summary" in autoapi_options %}
 Attributes
 ----------
```

### Comparing `sphinx-autoapi-3.1.0a3/setup.cfg` & `sphinx_autoapi-3.1b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/PKG-INFO` & `sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-autoapi
-Version: 3.1.0a3
+Version: 3.1.0b0
 Summary: Sphinx API documentation generator
 Home-page: http://github.com/readthedocs/sphinx-autoapi
 Author: Eric Holscher
 Author-email: eric@ericholscher.com
 Maintainer: Ashley Whetter
 Maintainer-email: ashley@awhetter.co.uk
 License: MIT
@@ -60,21 +60,22 @@
 Sphinx AutoAPI is a Sphinx extension for generating complete API documentation
 without needing to load, run, or import the project being documented.
 
 In contrast to the traditional `Sphinx autodoc <https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html>`_,
 which requires manual authoring and uses code imports,
 AutoAPI finds and generates documentation by parsing source code.
 
+For more information, see `the full documentation <https://sphinx-autoapi.readthedocs.org>`_.
+
 Getting Started
 ---------------
 
 The following steps will walk through how to add AutoAPI to an existing Sphinx project.
 For instructions on how to set up a Sphinx project,
-see Sphinx's documentation on
-`Getting Started <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.
+see `Sphinx's documentation <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_.
 
 Installation
 ~~~~~~~~~~~~
 
 AutoAPI can be installed through pip:
 
 .. code-block:: bash
```

### Comparing `sphinx-autoapi-3.1.0a3/sphinx_autoapi.egg-info/SOURCES.txt` & `sphinx_autoapi-3.1b0/sphinx_autoapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 LICENSE.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 autoapi/__init__.py
+autoapi/_astroid_utils.py
+autoapi/_mapper.py
+autoapi/_objects.py
+autoapi/_parser.py
 autoapi/directives.py
 autoapi/documenters.py
 autoapi/extension.py
 autoapi/inheritance_diagrams.py
 autoapi/settings.py
-autoapi/mappers/__init__.py
-autoapi/mappers/base.py
-autoapi/mappers/python/__init__.py
-autoapi/mappers/python/astroid_utils.py
-autoapi/mappers/python/mapper.py
-autoapi/mappers/python/objects.py
-autoapi/mappers/python/parser.py
 autoapi/templates/index.rst
-autoapi/templates/base/base.rst
 autoapi/templates/python/attribute.rst
 autoapi/templates/python/class.rst
 autoapi/templates/python/data.rst
 autoapi/templates/python/exception.rst
 autoapi/templates/python/function.rst
 autoapi/templates/python/method.rst
 autoapi/templates/python/module.rst
@@ -36,14 +32,17 @@
 sphinx_autoapi.egg-info/top_level.txt
 tests/test_astroid_utils.py
 tests/test_integration.py
 tests/python/conftest.py
 tests/python/test_own_page_option.py
 tests/python/test_parser.py
 tests/python/test_pyintegration.py
+tests/python/pep695/conf.py
+tests/python/pep695/index.rst
+tests/python/pep695/example/example.py
 tests/python/py310unionpipe/conf.py
 tests/python/py310unionpipe/index.rst
 tests/python/py310unionpipe/example/example.py
 tests/python/py38positionalparams/conf.py
 tests/python/py38positionalparams/index.rst
 tests/python/py38positionalparams/example/example.py
 tests/python/py3example/conf.py
@@ -73,14 +72,18 @@
 tests/python/pyiexample/index.rst
 tests/python/pyiexample/example/example.py
 tests/python/pyiexample/example/example.pyi
 tests/python/pyiexample2/conf.py
 tests/python/pyiexample2/index.rst
 tests/python/pyiexample2/example/example.py
 tests/python/pyiexample2/example/example.pyi
+tests/python/pyisubmoduleinit/conf.py
+tests/python/pyisubmoduleinit/index.rst
+tests/python/pyisubmoduleinit/example/example.py
+tests/python/pyisubmoduleinit/example/submodule_foo/__init__.pyi
 tests/python/pymovedconfpy/index.rst
 tests/python/pymovedconfpy/manualapi.rst
 tests/python/pymovedconfpy/confpy/conf.py
 tests/python/pymovedconfpy/example/example.py
 tests/python/pypackagecomplex/conf.py
 tests/python/pypackagecomplex/index.rst
 tests/python/pypackagecomplex/complex/__init__.py
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/conftest.py` & `sphinx_autoapi-3.1b0/tests/python/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/py310unionpipe/conf.py` & `sphinx_autoapi-3.1b0/tests/python/pep695/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/py38positionalparams/example/example.py` & `sphinx_autoapi-3.1b0/tests/python/py38positionalparams/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/py3example/conf.py` & `sphinx_autoapi-3.1b0/tests/python/py3example/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/py3example/example/example.py` & `sphinx_autoapi-3.1b0/tests/python/py3example/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/py3implicitnamespace/conf.py` & `sphinx_autoapi-3.1b0/tests/python/py3implicitnamespace/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyannotationcommentsexample/example/example.py` & `sphinx_autoapi-3.1b0/tests/python/pyannotationcommentsexample/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyautodoc_typehints/conf.py` & `sphinx_autoapi-3.1b0/tests/python/pyautodoc_typehints/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyemptyexample/conf.py` & `sphinx_autoapi-3.1b0/tests/python/pyemptyexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyexample/conf.py` & `sphinx_autoapi-3.1b0/tests/python/pyexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyexample/example/example.py` & `sphinx_autoapi-3.1b0/tests/python/pyexample/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyiexample/example/example.pyi` & `sphinx_autoapi-3.1b0/tests/python/pyiexample/example/example.pyi`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/confpy/conf.py` & `sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/confpy/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pymovedconfpy/example/example.py` & `sphinx_autoapi-3.1b0/tests/python/pymovedconfpy/example/example.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pypackagecomplex/complex/foo.py` & `sphinx_autoapi-3.1b0/tests/python/pypackagecomplex/complex/foo.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/__init__.py` & `sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/subpackage/submodule.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-"""This is a docstring."""
+"""Example module
 
-from . import submodule
+This is a description
+"""
 
 DATA = 42
 
 
 def function(foo, bar):
     """A module level function"""
 
 
+def _private_function():
+    """A function that shouldn't get rendered."""
+
+
+def not_in_all_function():
+    """A function that doesn't exist in __all__ when imported."""
+
+
 class Class(object):
     """This is a class."""
 
     class_var = 42
     """Class var docstring"""
 
     class NestedClass(object):
         """A nested class just to test things out"""
 
         @classmethod
         def a_classmethod():
             """A class method"""
             return True
 
-    @property
-    def my_property(self):
-        """A property."""
-        return 42
-
     def method_okay(self, foo=None, bar=None):
         """This method should parse okay"""
         return True
 
 
 class MyException(Exception):
     """This is an exception."""
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/submodule.py` & `sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/submodule.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 """Example module
 
 This is a description
 """
 
+from .subpackage.submodule import function as aliased_function
+from .subpackage.submodule import not_in_all_function
+
+__all__ = (
+    "aliased_function",
+    "Class",
+    "DATA",
+    "function",
+    "MyException",
+)
+
 DATA = 42
 
 
 def function(foo, bar):
     """A module level function"""
 
 
@@ -20,19 +31,14 @@
         """A nested class just to test things out"""
 
         @classmethod
         def a_classmethod():
             """A class method"""
             return True
 
-    @property
-    def my_property(self):
-        """A property."""
-        return 42
-
     def method_okay(self, foo=None, bar=None):
         """This method should parse okay"""
         return True
 
     def method_multiline(self, foo=None, bar=None, baz=None):
         """This is on multiple lines, but should parse okay too
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pypackageexample/package/subpackage/submodule.py` & `sphinx_autoapi-3.1b0/tests/python/pypackageexample/package/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,20 @@
-"""Example module
+"""This is a docstring."""
 
-This is a description
-"""
+from . import submodule
+from .subpackage.submodule import function as aliased_function
+from .subpackage.submodule import not_in_all_function
+
+__all__ = (
+    "aliased_function",
+    "Class",
+    "DATA",
+    "function",
+    "MyException",
+)
 
 DATA = 42
 
 
 def function(foo, bar):
     """A module level function"""
 
@@ -20,19 +29,14 @@
         """A nested class just to test things out"""
 
         @classmethod
         def a_classmethod():
             """A class method"""
             return True
 
-    @property
-    def my_property(self):
-        """A property."""
-        return 42
-
     def method_okay(self, foo=None, bar=None):
         """This method should parse okay"""
         return True
 
 
 class MyException(Exception):
     """This is an exception."""
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/pyskipexample/conf.py` & `sphinx_autoapi-3.1b0/tests/python/pyskipexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/test_own_page_option.py` & `sphinx_autoapi-3.1b0/tests/python/test_own_page_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         assert contents.find(id="package.Class")
         assert contents.find(id="package.Class.class_var")
         assert contents.find(id="package.Class.NestedClass")
         assert contents.find(id="package.Class.method_okay")
         assert contents.find(id="package.Class.NestedClass")
         assert contents.find(id="package.Class.NestedClass.a_classmethod")
         assert contents.find(id="package.function")
+        assert contents.find(id="package.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.not_in_all_function")
 
     def test_subpackage(self, parse):
         subpackage_path = "_build/html/autoapi/package/subpackage/index.html"
         subpackage_file = parse(subpackage_path)
 
         docstring = subpackage_file.find("p")
         assert docstring.text == "This is a docstring."
@@ -73,14 +77,18 @@
         assert not subpackage_file.find(id="classes")
         assert not subpackage_file.find(id="functions")
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
         contents = subpackage_file.find(id="package-contents")
         assert contents.find(id="package.subpackage.function")
+        assert contents.find(id="package.subpackage.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.subpackage.not_in_all_function")
 
     def test_module(self, parse):
         submodule_path = "_build/html/autoapi/package/submodule/index.html"
         submodule_file = parse(submodule_path)
 
         docstring = submodule_file.find("p")
         assert docstring.text == "Example module"
@@ -104,14 +112,18 @@
         assert contents.find(id="package.submodule.Class")
         assert contents.find(id="package.submodule.Class.class_var")
         assert contents.find(id="package.submodule.Class.NestedClass")
         assert contents.find(id="package.submodule.Class.method_okay")
         assert contents.find(id="package.submodule.Class.NestedClass")
         assert contents.find(id="package.submodule.Class.NestedClass.a_classmethod")
         assert contents.find(id="package.submodule.function")
+        assert contents.find(id="package.submodule.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.submodule.not_in_all_function")
 
     def test_rendered_only_expected_pages(self):
         _, dirs, files = next(os.walk("_build/html/autoapi/package"))
         assert sorted(dirs) == ["submodule", "subpackage"]
         assert files == ["index.html"]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/submodule"))
@@ -191,14 +203,18 @@
         assert not contents.find(id="package.Class")
         assert not contents.find(id="package.Class.class_var")
         assert not contents.find(id="package.Class.NestedClass")
         assert not contents.find(id="package.Class.method_okay")
         assert not contents.find(id="package.Class.NestedClass")
         assert not contents.find(id="package.Class.NestedClass.a_classmethod")
         assert contents.find(id="package.function")
+        assert contents.find(id="package.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.not_in_all_function")
 
     def test_module(self, parse):
         submodule_path = "_build/html/autoapi/package/submodule/index.html"
         submodule_file = parse(submodule_path)
 
         docstring = submodule_file.find("p")
         assert docstring.text == "Example module"
@@ -226,14 +242,18 @@
         assert not contents.find(id="package.submodule.Class")
         assert not contents.find(id="package.submodule.Class.class_var")
         assert not contents.find(id="package.submodule.Class.NestedClass")
         assert not contents.find(id="package.submodule.Class.method_okay")
         assert not contents.find(id="package.submodule.Class.NestedClass")
         assert not contents.find(id="package.submodule.Class.NestedClass.a_classmethod")
         assert contents.find(id="package.submodule.function")
+        assert contents.find(id="package.submodule.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.submodule.not_in_all_function")
 
     def test_class(self, parse):
         class_path = "_build/html/autoapi/package/Class.html"
         class_file = parse(class_path)
 
         class_sig = class_file.find(id="package.Class")
         assert class_sig
@@ -250,15 +270,14 @@
         assert not class_file.find(id="attributes")
         assert not class_file.find(id="exceptions")
         assert not class_file.find(id="methods")
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
         assert class_.find(id="package.Class.class_var")
-        assert class_.find(id="package.Class.my_property")
         assert class_.find(id="package.Class.method_okay")
 
         nested_class_path = "_build/html/autoapi/package/Class.NestedClass.html"
         nested_class_file = parse(nested_class_path)
 
         nested_class_sig = nested_class_file.find(id="package.Class.NestedClass")
         assert nested_class_sig
@@ -396,14 +415,18 @@
         assert not contents.find(id="package.Class")
         assert not contents.find(id="package.Class.class_var")
         assert not contents.find(id="package.Class.NestedClass")
         assert not contents.find(id="package.Class.method_okay")
         assert not contents.find(id="package.Class.NestedClass")
         assert not contents.find(id="package.Class.NestedClass.a_classmethod")
         assert not contents.find(id="package.function")
+        assert not contents.find(id="package.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.not_in_all_function")
 
     def test_module(self, parse):
         submodule_path = "_build/html/autoapi/package/submodule/index.html"
         submodule_file = parse(submodule_path)
 
         docstring = submodule_file.find("p")
         assert docstring.text == "Example module"
@@ -433,14 +456,18 @@
         assert not contents.find(id="package.submodule.Class")
         assert not contents.find(id="package.submodule.Class.class_var")
         assert not contents.find(id="package.submodule.Class.NestedClass")
         assert not contents.find(id="package.submodule.Class.method_okay")
         assert not contents.find(id="package.submodule.Class.NestedClass")
         assert not contents.find(id="package.submodule.Class.NestedClass.a_classmethod")
         assert not contents.find(id="package.submodule.function")
+        assert not contents.find(id="package.submodule.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.submodule.not_in_all_function")
 
     def test_class(self, parse):
         class_path = "_build/html/autoapi/package/Class.html"
         class_file = parse(class_path)
 
         class_sig = class_file.find(id="package.Class")
         assert class_sig
@@ -457,15 +484,14 @@
         assert not class_file.find(id="attributes")
         assert not class_file.find(id="exceptions")
         assert not class_file.find(id="methods")
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
         assert class_.find(id="package.Class.class_var")
-        assert class_.find(id="package.Class.my_property")
         assert class_.find(id="package.Class.method_okay")
 
     def test_function(self, parse):
         function_path = "_build/html/autoapi/package/function.html"
         function_file = parse(function_path)
 
         function_sig = function_file.find(id="package.function")
@@ -478,42 +504,45 @@
     def test_rendered_only_expected_pages(self):
         _, dirs, files = next(os.walk("_build/html/autoapi/package"))
         assert sorted(dirs) == ["submodule", "subpackage"]
         assert sorted(files) == [
             "Class.NestedClass.html",
             "Class.html",
             "MyException.html",
+            "aliased_function.html",
             "function.html",
             "index.html",
         ]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/submodule"))
         assert not dirs
         assert sorted(files) == [
             "Class.NestedClass.html",
             "Class.html",
             "MyException.html",
+            "aliased_function.html",
             "function.html",
             "index.html",
         ]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/subpackage"))
         assert dirs == ["submodule"]
-        assert sorted(files) == ["function.html", "index.html"]
+        assert sorted(files) == ["aliased_function.html", "function.html", "index.html"]
 
         _, dirs, files = next(
             os.walk("_build/html/autoapi/package/subpackage/submodule")
         )
         assert not dirs
         assert sorted(files) == [
             "Class.NestedClass.html",
             "Class.html",
             "MyException.html",
             "function.html",
             "index.html",
+            "not_in_all_function.html",
         ]
 
     def test_index(self, parse):
         index_path = "_build/html/autoapi/index.html"
         index_file = parse(index_path)
 
         top_links = index_file.find_all(class_="toctree-l1")
@@ -576,14 +605,18 @@
         assert not contents.find(id="package.Class")
         assert not contents.find(id="package.Class.class_var")
         assert not contents.find(id="package.Class.NestedClass")
         assert not contents.find(id="package.Class.method_okay")
         assert not contents.find(id="package.Class.NestedClass")
         assert not contents.find(id="package.Class.NestedClass.a_classmethod")
         assert not contents.find(id="package.function")
+        assert not contents.find(id="package.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.not_in_all_function")
 
     def test_module(self, parse):
         submodule_path = "_build/html/autoapi/package/submodule/index.html"
         submodule_file = parse(submodule_path)
 
         docstring = submodule_file.find("p")
         assert docstring.text == "Example module"
@@ -613,14 +646,18 @@
         assert not contents.find(id="package.submodule.Class")
         assert not contents.find(id="package.submodule.Class.class_var")
         assert not contents.find(id="package.submodule.Class.NestedClass")
         assert not contents.find(id="package.submodule.Class.method_okay")
         assert not contents.find(id="package.submodule.Class.NestedClass")
         assert not contents.find(id="package.submodule.Class.NestedClass.a_classmethod")
         assert not contents.find(id="package.submodule.function")
+        assert not contents.find(id="package.submodule.aliased_function")
+
+        # Hidden children are never rendered.
+        assert not contents.find(id="package.submodule.not_in_all_function")
 
     def test_class(self, parse):
         class_path = "_build/html/autoapi/package/Class.html"
         class_file = parse(class_path)
 
         class_sig = class_file.find(id="package.Class")
         assert class_sig
@@ -639,15 +676,14 @@
         # There should not be links to the children without their own page
         assert not class_file.find(id="attributes")
         assert not class_file.find(id="exceptions")
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
         assert class_.find(id="package.Class.class_var")
-        assert class_.find(id="package.Class.my_property")
         assert not class_.find(id="package.Class.method_okay")
 
     def test_function(self, parse):
         function_path = "_build/html/autoapi/package/function.html"
         function_file = parse(function_path)
 
         function_sig = function_file.find(id="package.function")
@@ -673,14 +709,15 @@
         assert sorted(dirs) == ["submodule", "subpackage"]
         assert sorted(files) == [
             "Class.NestedClass.a_classmethod.html",
             "Class.NestedClass.html",
             "Class.html",
             "Class.method_okay.html",
             "MyException.html",
+            "aliased_function.html",
             "function.html",
             "index.html",
         ]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/submodule"))
         assert not dirs
         assert sorted(files) == [
@@ -689,34 +726,36 @@
             "Class.html",
             "Class.method_google_docs.html",
             "Class.method_multiline.html",
             "Class.method_okay.html",
             "Class.method_sphinx_docs.html",
             "Class.method_tricky.html",
             "MyException.html",
+            "aliased_function.html",
             "function.html",
             "index.html",
         ]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/subpackage"))
         assert dirs == ["submodule"]
-        assert sorted(files) == ["function.html", "index.html"]
+        assert sorted(files) == ["aliased_function.html", "function.html", "index.html"]
 
         _, dirs, files = next(
             os.walk("_build/html/autoapi/package/subpackage/submodule")
         )
         assert not dirs
         assert sorted(files) == [
             "Class.NestedClass.a_classmethod.html",
             "Class.NestedClass.html",
             "Class.html",
             "Class.method_okay.html",
             "MyException.html",
             "function.html",
             "index.html",
+            "not_in_all_function.html",
         ]
 
     def test_index(self, parse):
         index_path = "_build/html/autoapi/index.html"
         index_file = parse(index_path)
 
         top_links = index_file.find_all(class_="toctree-l1")
@@ -740,14 +779,15 @@
                     "undoc-members",
                     "show-inheritance",
                     "imported-members",
                 ],
             },
         )
 
+    # TODO: Include a test for a property
     def test_package(self, parse):
         package_path = "_build/html/autoapi/package/index.html"
         package_file = parse(package_path)
 
         docstring = package_file.find("p")
         assert docstring.text == "This is a docstring."
 
@@ -772,14 +812,15 @@
         assert attributes.find("a", title="package.DATA")
 
         # There should not be links to the children without their own page
         pass  # there are no children without their own page
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
+        # Hidden children are never rendered.
         assert not package_file.find(id="package-contents")
 
     def test_module(self, parse):
         submodule_path = "_build/html/autoapi/package/submodule/index.html"
         submodule_file = parse(submodule_path)
 
         docstring = submodule_file.find("p")
@@ -802,14 +843,15 @@
 
         # There should not be links to the children without their own page
         assert not submodule_file.find(id="submodules")
         assert not submodule_file.find(id="subpackages")
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
+        # Hidden children are never rendered.
         assert not submodule_file.find(id="module-contents")
 
     def test_class(self, parse):
         class_path = "_build/html/autoapi/package/Class.html"
         class_file = parse(class_path)
 
         class_sig = class_file.find(id="package.Class")
@@ -824,23 +866,21 @@
         assert classes.find("a", title="package.Class.NestedClass")
         methods = class_file.find(id="methods")
         assert methods
         assert methods.find("a", title="package.Class.method_okay")
         attributes = class_file.find(id="attributes")
         assert attributes
         assert attributes.find("a", title="package.Class.class_var")
-        assert attributes.find("a", title="package.Class.my_property")
 
         # There should not be links to the children without their own page
         assert not class_file.find(id="exceptions")
 
         # Children without their own page should be rendered on this page,
         # and children with their own page should not be rendered on this page.
         assert not class_.find(id="package.Class.class_var")
-        assert not class_.find(id="package.Class.my_property")
         assert not class_.find(id="package.Class.method_okay")
 
     def test_function(self, parse):
         function_path = "_build/html/autoapi/package/function.html"
         function_file = parse(function_path)
 
         function_sig = function_file.find(id="package.function")
@@ -871,33 +911,26 @@
     def test_attribute(self, parse):
         attribute_path = "_build/html/autoapi/package/Class.class_var.html"
         attribute_file = parse(attribute_path)
 
         attribute_sig = attribute_file.find(id="package.Class.class_var")
         assert attribute_sig
 
-    def test_property(self, parse):
-        property_path = "_build/html/autoapi/package/Class.my_property.html"
-        property_file = parse(property_path)
-
-        property_sig = property_file.find(id="package.Class.my_property")
-        assert property_sig
-
     def test_rendered_only_expected_pages(self):
         _, dirs, files = next(os.walk("_build/html/autoapi/package"))
         assert sorted(dirs) == ["submodule", "subpackage"]
         assert sorted(files) == [
             "Class.NestedClass.a_classmethod.html",
             "Class.NestedClass.html",
             "Class.class_var.html",
             "Class.html",
             "Class.method_okay.html",
-            "Class.my_property.html",
             "DATA.html",
             "MyException.html",
+            "aliased_function.html",
             "function.html",
             "index.html",
         ]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/submodule"))
         assert not dirs
         assert sorted(files) == [
@@ -906,40 +939,40 @@
             "Class.class_var.html",
             "Class.html",
             "Class.method_google_docs.html",
             "Class.method_multiline.html",
             "Class.method_okay.html",
             "Class.method_sphinx_docs.html",
             "Class.method_tricky.html",
-            "Class.my_property.html",
             "DATA.html",
             "MyException.html",
+            "aliased_function.html",
             "function.html",
             "index.html",
         ]
 
         _, dirs, files = next(os.walk("_build/html/autoapi/package/subpackage"))
         assert dirs == ["submodule"]
-        assert sorted(files) == ["function.html", "index.html"]
+        assert sorted(files) == ["aliased_function.html", "function.html", "index.html"]
 
         _, dirs, files = next(
             os.walk("_build/html/autoapi/package/subpackage/submodule")
         )
         assert not dirs
         assert sorted(files) == [
             "Class.NestedClass.a_classmethod.html",
             "Class.NestedClass.html",
             "Class.class_var.html",
             "Class.html",
             "Class.method_okay.html",
-            "Class.my_property.html",
             "DATA.html",
             "MyException.html",
             "function.html",
             "index.html",
+            "not_in_all_function.html",
         ]
 
     def test_index(self, parse):
         index_path = "_build/html/autoapi/index.html"
         index_file = parse(index_path)
 
         top_links = index_file.find_all(class_="toctree-l1")
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/test_parser.py` & `sphinx_autoapi-3.1b0/tests/python/test_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-# coding=utf8
-
 """Test Python parser"""
 
-from io import StringIO
-import sys
-from textwrap import dedent
-
 import astroid
-import pytest
 
-from autoapi.mappers.python.parser import Parser
+from autoapi._parser import Parser
 
 
 class TestPythonParser:
     def parse(self, source):
         node = astroid.extract_node(source)
         return Parser().parse(node)
 
@@ -28,41 +21,41 @@
 
     def test_parses_all(self):
         source = """
         __all__ = ['Foo', 5.0]
         """
         data = self.parse(source)[0]
         assert data["name"] == "__all__"
-        assert data["value"] == ["Foo", 5.0]
+        assert data["value"] == "['Foo', 5.0]"
 
     def test_parses_all_multiline(self):
         source = """
         __all__ = [
             'foo',
             'bar',
         ]
         """
         data = self.parse(source)[0]
-        assert data["value"] == ["foo", "bar"]
+        assert data["value"] == "['foo', 'bar']"
 
     def test_parses_name(self):
         source = "foo.bar"
         assert self.parse(source) == {}
 
     def test_parses_list(self):
         name = "__all__"
-        value = [1, 2, 3, 4]
+        value = "[1, 2, 3, 4]"
         source = "{} = {}".format(name, value)
         data = self.parse(source)[0]
         assert data["name"] == name
         assert data["value"] == value
 
     def test_parses_nested_list(self):
         name = "__all__"
-        value = [[1, 2], [3, 4]]
+        value = "[[1, 2], [3, 4]]"
         source = "{} = {}".format(name, value)
         data = self.parse(source)[0]
         assert data["name"] == name
         assert data["value"] == value
 
     def test_arguments(self):
         """Argument parsing of source"""
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/python/test_pyintegration.py` & `sphinx_autoapi-3.1b0/tests/python/test_pyintegration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import os
 import pathlib
 import sys
 from unittest.mock import Mock, call
 
 import autoapi.settings
-from autoapi.mappers.python import (
+from autoapi._objects import (
     PythonClass,
     PythonData,
     PythonFunction,
     PythonMethod,
     PythonModule,
 )
 from packaging import version
@@ -240,14 +240,28 @@
         # Are py files preferred
         assert "DoNotFindThis" not in example_file
 
         foo_sig = example_file.find(id="example.Foo")
         assert foo_sig
 
 
+class TestStubInitModuleInSubmodule:
+    @pytest.fixture(autouse=True, scope="class")
+    def built(self, builder):
+        builder("pyisubmoduleinit", warningiserror=True)
+
+    def test_integration(self, parse):
+        example_file = parse("_build/html/autoapi/example/index.html")
+
+        # Documentation should list
+        # submodule_foo instead of __init__
+        assert example_file.find(title="submodule_foo")
+        assert not example_file.find(title="__init__")
+
+
 class TestPy3Module:
     @pytest.fixture(autouse=True, scope="class")
     def built(self, builder):
         builder("py3example")
 
     def test_integration(self, parse):
         example_file = parse("_build/html/autoapi/example/index.html")
@@ -569,14 +583,42 @@
         assert len(args) == 1
         links = args[0].select("span > a")
         assert len(links) == 2
         assert links[0].text == "pathlib.Path"
         assert links[1].text == "None"
 
 
+@pytest.mark.skipif(
+    sys.version_info < (3, 12), reason="PEP-695 support requires Python >=3.12"
+)
+class TestPEP695:
+    @pytest.fixture(autouse=True, scope="class")
+    def built(self, builder):
+        builder("pep695", warningiserror=True)
+
+    def test_integration(self, parse):
+        example_file = parse("_build/html/autoapi/example/index.html")
+
+        alias = example_file.find(id="example.MyTypeAliasA")
+        properties = alias.find_all(class_="property")
+        assert len(properties) == 2
+        annotation = properties[0].text
+        assert annotation == ": TypeAlias"
+        value = properties[1].text
+        assert value == " = tuple[str, int]"
+
+        alias = example_file.find(id="example.MyTypeAliasB")
+        properties = alias.find_all(class_="property")
+        assert len(properties) == 2
+        annotation = properties[0].text
+        assert annotation == ": TypeAlias"
+        value = properties[1].text
+        assert value == " = tuple[str, int]"
+
+
 def test_napoleon_integration_loaded(builder, parse):
     confoverrides = {
         "exclude_patterns": ["manualapi.rst"],
         "extensions": [
             "autoapi.extension",
             "sphinx.ext.autodoc",
             "sphinx.ext.napoleon",
@@ -931,14 +973,21 @@
         assert foo_file.find(id="complex.foo.PublicClass")
 
     def test_parses_unicode_file(self, parse):
         foo_file = parse("_build/html/autoapi/complex/unicode_data/index.html")
 
         assert foo_file.find(id="complex.unicode_data.unicode_str")
 
+    def test_nested_parse_directive(self, parse):
+        package_file = parse("_build/html/autoapi/complex/index.html")
+
+        complex = package_file.find(id="complex")
+        assert "This heading will be removed" not in complex.parent.text
+        assert complex.parent.find("section")["id"] != "this-heading-will-be-removed"
+
 
 class TestComplexPackageParallel(TestComplexPackage):
     @pytest.fixture(autouse=True, scope="class")
     def built(self, builder):
         builder("pypackagecomplex", parallel=2)
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/templateexample/conf.py` & `sphinx_autoapi-3.1b0/tests/templateexample/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-autoapi-3.1.0a3/tests/test_astroid_utils.py` & `sphinx_autoapi-3.1b0/tests/test_astroid_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 
 import astroid
-from autoapi.mappers.python import astroid_utils, objects
+from autoapi import _astroid_utils
+from autoapi import _objects
 import pytest
 
 
 def generate_module_names():
     for i in range(1, 5):
         yield ".".join("module{}".format(j) for j in range(i))
 
@@ -66,44 +67,51 @@
         {}
         class ThisClass({}): #@
             pass
         """.format(
             import_, basename
         )
         node = astroid.extract_node(source)
-        basenames = astroid_utils.resolve_qualname(node.bases[0], node.basenames[0])
+        basenames = _astroid_utils.resolve_qualname(node.bases[0], node.basenames[0])
         assert basenames == expected
 
     @pytest.mark.parametrize(
         ("import_", "basename", "expected"), list(imported_call_cases())
     )
     def test_can_get_full_function_basename(self, import_, basename, expected):
         source = """
         {}
         class ThisClass({}): #@
             pass
         """.format(
             import_, basename
         )
         node = astroid.extract_node(source)
-        basenames = astroid_utils.resolve_qualname(node.bases[0], node.basenames[0])
+        basenames = _astroid_utils.resolve_qualname(node.bases[0], node.basenames[0])
         assert basenames == expected
 
     @pytest.mark.parametrize(
         ("source", "expected"),
         [
-            ('a = "a"', ("a", "a")),
-            ("a = 1", ("a", 1)),
+            ('a = "a"', ("a", "'a'")),
+            ("a = 1", ("a", "1")),
             ("a, b, c = (1, 2, 3)", None),
             ("a = b = 1", None),
+            ("a = [1, 2, [3, 4]]", ("a", "[1, 2, [3, 4]]")),
+            ("a = [1, 2, variable[subscript]]", ("a", None)),
+            ('a = """multiline\nstring"""', ("a", '"""multiline\nstring"""')),
+            ('a = ["""multiline\nstring"""]', ("a", None)),
+            ("a = (1, 2, 3)", ("a", "(1, 2, 3)")),
+            ("a = (1, 'two', 3)", ("a", "(1, 'two', 3)")),
+            ("a = None", ("a", "None")),
         ],
     )
     def test_can_get_assign_values(self, source, expected):
         node = astroid.extract_node(source)
-        value = astroid_utils.get_assign_value(node)
+        value = _astroid_utils.get_assign_value(node)
         assert value == expected
 
     @pytest.mark.parametrize(
         "signature,expected",
         [
             (
                 "a: bool, b: int = 5",
@@ -156,29 +164,29 @@
             def func({}) -> str: #@
                 pass
         """.format(
                 signature
             )
         )
 
-        annotations = astroid_utils.get_args_info(node.args)
+        annotations = _astroid_utils.get_args_info(node.args)
         assert annotations == expected
 
     def test_parse_split_type_comments(self):
         node = astroid.extract_node(
             """
             def func(
                 a, # type: int
                 b, # type: int
             ): # type: (...) -> str
                 pass
         """
         )
 
-        annotations = astroid_utils.get_args_info(node.args)
+        annotations = _astroid_utils.get_args_info(node.args)
 
         expected = [
             (None, "a", "int", None),
             (None, "b", "int", None),
         ]
         assert annotations == expected
 
@@ -205,22 +213,25 @@
                 "*, a: int, b: int",
                 marks=pytest.mark.skipif(
                     sys.version_info[:2] < (3, 8), reason="Uses Python 3.8+ syntax"
                 ),
             ),
             ("a: int, *args, b: str, **kwargs", "a: int, *args, b: str, **kwargs"),
             ("a: 'A'", "a: A"),
+            ("a: Literal[1]", "a: Literal[1]"),
+            ("a: Literal['x']", "a: Literal['x']"),
+            ("a: Literal['x', 'y', 'z']", "a: Literal['x', 'y', 'z']"),
         ],
     )
     def test_format_args(self, signature, expected):
         node = astroid.extract_node(
             """
             def func({}) -> str: #@
                 pass
         """.format(
                 signature
             )
         )
 
-        args_info = astroid_utils.get_args_info(node.args)
-        formatted = objects._format_args(args_info)
+        args_info = _astroid_utils.get_args_info(node.args)
+        formatted = _objects._format_args(args_info)
         assert formatted == expected
```

### Comparing `sphinx-autoapi-3.1.0a3/tests/test_integration.py` & `sphinx_autoapi-3.1b0/tests/test_integration.py`

 * *Files identical despite different names*

