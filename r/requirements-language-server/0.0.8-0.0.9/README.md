# Comparing `tmp/requirements-language-server-0.0.8.tar.gz` & `tmp/requirements-language-server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements-language-server-0.0.8.tar", last modified: Thu Oct 19 07:33:01 2023, max compression
+gzip compressed data, was "requirements-language-server-0.0.9.tar", last modified: Fri Oct 27 15:12:32 2023, max compression
```

## Comparing `requirements-language-server-0.0.8.tar` & `requirements-language-server-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.722855 requirements-language-server-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2023-10-19 07:33:01.722855 requirements-language-server-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/api/requirements-language-server.md
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      135 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/sdist/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/sdist/_requirements-language-server
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/sdist/requirements-language-server
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/sdist/requirements-language-server.1
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 07:33:01.722855 requirements-language-server-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.714855 requirements-language-server-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/src/requirements_language_server/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.714855 requirements-language-server-0.0.8/src/requirements_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/src/requirements_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/assets/jinja2/template.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/src/requirements_language_server/documents/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/documents/option.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/documents/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/finders.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.722855 requirements-language-server-0.0.8/src/requirements_language_server/tree_sitter_lsp/
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/tree_sitter_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/tree_sitter_lsp/complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/tree_sitter_lsp/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/tree_sitter_lsp/finders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/tree_sitter_lsp/format.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/src/requirements_language_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.718855 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-19 07:33:01.000000 requirements-language-server-0.0.8/src/requirements_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.722855 requirements-language-server-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 07:33:01.722855 requirements-language-server-0.0.8/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      299 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/tests/requirements.txt.in
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-10-19 07:32:50.000000 requirements-language-server-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.145048 requirements-language-server-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.137048 requirements-language-server-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.137048 requirements-language-server-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2023-10-27 15:12:32.145048 requirements-language-server-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/api/requirements-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/requirements/colorize.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      158 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/sdist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/sdist/_requirements-language-server
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2023-10-27 15:12:31.000000 requirements-language-server-0.0.9/sdist/requirements-language-server
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/sdist/requirements-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-27 15:12:32.145048 requirements-language-server-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.137048 requirements-language-server-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/src/requirements_language_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-27 15:12:31.000000 requirements-language-server-0.0.9/src/requirements_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.137048 requirements-language-server-0.0.9/src/requirements_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/src/requirements_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/assets/jinja2/template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/finders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/src/requirements_language_server/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/misc/option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.145048 requirements-language-server-0.0.9/src/requirements_language_server/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/packages/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9667 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/src/requirements_language_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.141048 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11155 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-27 15:12:32.000000 requirements-language-server-0.0.9/src/requirements_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.145048 requirements-language-server-0.0.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 15:12:32.145048 requirements-language-server-0.0.9/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      299 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/tests/requirements.txt.in
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2023-10-27 15:12:18.000000 requirements-language-server-0.0.9/tests/test_utils.py
```

### Comparing `requirements-language-server-0.0.8/.github/workflows/main.yml` & `requirements-language-server-0.0.9/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 # https://github.com/softprops/action-gh-release/issues/236
 permissions:
   contents: write
 
 env:
   PYTHONUTF8: "1"
-  python-version: 3.x
+  # https://github.com/tree-sitter/py-tree-sitter/pull/161
+  python-version: "3.11"
   cache: pip
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
```

### Comparing `requirements-language-server-0.0.8/.gitignore` & `requirements-language-server-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/.pre-commit-config.yaml` & `requirements-language-server-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/LICENSE` & `requirements-language-server-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/PKG-INFO` & `requirements-language-server-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,7 @@
-Metadata-Version: 2.1
-Name: requirements-language-server
-Version: 0.0.8
-Summary: requirements.txt language server
-Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
-License: GPL v3
-Project-URL: Homepage, https://requirements-language-server.readthedocs.io
-Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
-Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
-Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
-Keywords: requirements,language server
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: jinja2
-Requires-Dist: pip-cache
-Requires-Dist: platformdirs
-Requires-Dist: pygls
-Requires-Dist: tomli; python_version < "3.11"
-Requires-Dist: tree-sitter-requirements
-Provides-Extra: dev
-Requires-Dist: pytest-cov; extra == "dev"
-
 # requirements-language-server
 
 [![readthedocs](https://shields.io/readthedocs/requirements-language-server)](https://requirements-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/requirements-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/requirements-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/requirements-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/requirements-language-server/actions)
 [![codecov](https://codecov.io/gh/Freed-Wu/requirements-language-server/branch/main/graph/badge.svg)](https://codecov.io/gh/Freed-Wu/requirements-language-server)
 [![DeepSource](https://deepsource.io/gh/Freed-Wu/requirements-language-server.svg/?show_trend=true)](https://deepsource.io/gh/Freed-Wu/requirements-language-server)
@@ -103,37 +64,49 @@
 
 We recognize `requirements.txt` and `requirements/dev.txt` as PEP508's
 `requirements.txt`s and display errors for all pip's options. For other
 `requirements.txt`s, we recognize them as pip's `requirements.txt`s.
 
 Features:
 
-- [x] diagnostic
-- [x] format: sort packages
-- [x] go to definition: jump to first repeated package
-- [x] go to reference: jump to all other repeated packages
-- [x] document link: open package's pypi homepage
-- [x] document hover & completion:
+- [x] [Goto Definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_definition):
+  jump to first repeated package
+- [x] [Find References](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_references):
+  jump to all other repeated packages
+- [x] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic):
+  - [x] repeated packages
+  - [x] unsorted packages
+  - [x] invalid path
+  - [x] pip's option when PEP508 is enabled
+- [x] [Document Formatting](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_formatting):
+  sort packages
+- [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink):
+  open package's pypi homepage
+- [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
+  - [x] pip's options
+  - [x] package: requires [pip-cache](https://github.com/brunobeltran/pip-cache).
+    Must `pip-cache update` before.
+- [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion):
   - [x] pip's options
   - [x] package: requires [pip-cache](https://github.com/brunobeltran/pip-cache).
     Must `pip-cache update` before.
 
 Other features:
 
-- [x] pre-commit-hooks
+- [x] [pre-commit-hooks](https://pre-commit.com/)
   - [x] linter
   - [x] formatter
 
 ## Screenshots
 
 ### Diagnostic
 
 ![diagnostic](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/13aa466d-62af-423a-a141-880b495750a7)
 
-### Document Hover
+### Hover
 
 ![module](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/0e74a423-b07a-459a-8fb4-10789f245265)
 
 ![option](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/78a7b5ec-a9dd-46c2-b22b-4dc0123b6f0e)
 
 ### Completion
```

### Comparing `requirements-language-server-0.0.8/docs/conf.py` & `requirements-language-server-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/docs/resources/configure.md` & `requirements-language-server-0.0.9/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/docs/resources/install.md` & `requirements-language-server-0.0.9/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/pyproject.toml` & `requirements-language-server-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,17 @@
 "share/bash-completion/completions" = ["sdist/requirements-language-server"]
 "share/zsh/site-functions" = ["sdist/_requirements-language-server"]
 
 [tool.setuptools.dynamic.dependencies]
 file = "requirements.txt"
 
 # begin: scripts/update-pyproject.toml.pl
+[tool.setuptools.dynamic.optional-dependencies.colorize]
+file = "requirements/colorize.txt"
+
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "requirements/dev.txt"
 # end: scripts/update-pyproject.toml.pl
 
 [tool.setuptools_scm]
 write_to = "src/requirements_language_server/_version.py"
```

### Comparing `requirements-language-server-0.0.8/sdist/_requirements-language-server` & `requirements-language-server-0.0.9/sdist/_requirements-language-server`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,14 @@
   _describe 'requirements-language-server commands' _commands
 }
 
 _shtab_requirements_language_server_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   "(- : *)--print-completion[print shell completion script]:print_completion:(bash zsh tcsh)"
   "(- : *)--version[show program\'s version number and exit]"
-  "--print-config[print config value]:print_config:(template cache all)"
-  "--generate-cache[generate cache]"
   "--check[check file\'s errors and warnings]:check:"
   "--format[format files]:format:"
   "--color[when to display color]:color:(auto always never)"
 )
 
 
 _shtab_requirements_language_server() {
```

### Comparing `requirements-language-server-0.0.8/sdist/requirements-language-server` & `requirements-language-server-0.0.9/sdist/requirements-language-server`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
 
 
-_shtab_requirements_language_server_option_strings=('-h' '--help' '--print-completion' '--version' '--print-config' '--generate-cache' '--check' '--format' '--color')
+_shtab_requirements_language_server_option_strings=('-h' '--help' '--print-completion' '--version' '--check' '--format' '--color')
 
 
 
 _shtab_requirements_language_server___print_completion_choices=('bash' 'zsh' 'tcsh')
-_shtab_requirements_language_server___print_config_choices=('template' 'cache' 'all')
 _shtab_requirements_language_server___color_choices=('auto' 'always' 'never')
 
 _shtab_requirements_language_server__h_nargs=0
 _shtab_requirements_language_server___help_nargs=0
 _shtab_requirements_language_server___version_nargs=0
-_shtab_requirements_language_server___generate_cache_nargs=0
 _shtab_requirements_language_server___check_nargs=*
 _shtab_requirements_language_server___format_nargs=*
 
 
 # $1=COMP_WORDS[1]
 _shtab_compgen_files() {
   compgen -f -- $1  # files
```

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server/__main__.py` & `requirements-language-server-0.0.9/src/requirements_language_server/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 r"""This module can be called by
 `python -m <https://docs.python.org/3/library/__main__.html>`_.
 """
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from contextlib import suppress
 from datetime import datetime
 
-from . import CONFIG
 from . import __name__ as NAME
 from . import __version__
 
 NAME = NAME.replace("_", "-")
 VERSION = rf"""{NAME} {__version__}
 Copyright (C) {datetime.now().year}
 Written by Wu Zhenyu
@@ -27,24 +26,14 @@
     )
     with suppress(ImportError):
         import shtab
 
         shtab.add_argument_to(parser)
     parser.add_argument("--version", version=VERSION, action="version")
     parser.add_argument(
-        "--print-config",
-        choices=["template", "cache", "all"],
-        help="print config value",
-    )
-    parser.add_argument(
-        "--generate-cache",
-        action="store_true",
-        help="generate cache",
-    )
-    parser.add_argument(
         "--check",
         nargs="*",
         default=[],
         help="check file's errors and warnings",
     )
     parser.add_argument(
         "--format",
@@ -62,37 +51,31 @@
 
 
 def main() -> None:
     r"""Parse arguments and provide shell completions."""
     parser = get_parser()
     args = parser.parse_args()
 
+    from tree_sitter_lsp.diagnose import check
+    from tree_sitter_lsp.format import format
     from tree_sitter_requirements import parse
 
-    from .tree_sitter_lsp.diagnose import check
-    from .tree_sitter_lsp.format import format
-    from .utils import DIAGNOSTICS_FINDERS, FORMATTING_FINDER
+    from .finders import DIAGNOSTICS_FINDER_CLASSES, FORMATTING_FINDER_CLASSES
+    from .utils import get_filetype
 
-    format(args.format, FORMATTING_FINDER, parse)
-    result = check(args.check, DIAGNOSTICS_FINDERS, parse, args.color)
+    format(args.format, parse, FORMATTING_FINDER_CLASSES, get_filetype)  # type: ignore
+    result = check(
+        args.check,
+        parse,
+        DIAGNOSTICS_FINDER_CLASSES,
+        get_filetype,
+        args.color,
+    )
     if args.format or args.check:
         exit(result)
-    if args.print_config:
-        print(
-            CONFIG.get(
-                args.print_config,
-                "\n".join([k + ": " + v for k, v in CONFIG.items()]),
-            )
-        )
-        return None
-    if args.generate_cache:
-        from .documents.package import generate_cache
-
-        generate_cache()
-        return None
 
     from .server import RequirementsLanguageServer
 
     RequirementsLanguageServer(NAME, __version__).start_io()
 
 
 if __name__ == "__main__":
```

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server/_metainfo.py` & `requirements-language-server-0.0.9/src/requirements_language_server/_metainfo.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server/documents/option.py` & `requirements-language-server-0.0.9/src/requirements_language_server/misc/option.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server/finders.py` & `requirements-language-server-0.0.9/src/requirements_language_server/finders.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,24 @@
 import os
 from typing import Literal
 
 import tree_sitter_requirements as requirements
 from lsprotocol.types import Diagnostic, DiagnosticSeverity
 from pip_cache import get_package_names
 from tree_sitter import Node, Tree
+from tree_sitter_lsp import UNI, Finder
+from tree_sitter_lsp.finders import (
+    ErrorFinder,
+    MissingFinder,
+    RepeatedFinder,
+    TypeFinder,
+    UnsortedFinder,
+)
 
-from .tree_sitter_lsp import UNI, Finder
-from .tree_sitter_lsp.finders import RepeatedFinder, TypeFinder, UnsortedFinder
+from . import FILETYPE
 
 
 class InvalidPackageFinder(Finder):
     r"""Invalidpackagefinder."""
 
     def __init__(
         self,
@@ -140,15 +147,15 @@
 
 
 class RepeatedPackageFinder(RepeatedFinder):
     r"""Repeatedpackagefinder."""
 
     def __init__(
         self,
-        pep508: bool = False,
+        filetype: FILETYPE = "pip",
         message: str = "{{uni.get_text()}}: is repeated on {{_uni}}",
         severity: DiagnosticSeverity = DiagnosticSeverity.Warning,
     ) -> None:
         r"""Init.
 
         :param self:
         :param pep508:
@@ -156,24 +163,24 @@
         :param message:
         :type message: str
         :param severity:
         :type severity: DiagnosticSeverity
         :rtype: None
         """
         super().__init__(message, severity)
-        self.pep508 = pep508
+        self.filetype = filetype
 
     def is_include_node(self, node: Node) -> bool:
         r"""Is include node.
 
         :param node:
         :type node: Node
         :rtype: bool
         """
-        return node.type == "path" and not self.pep508
+        return node.type == "path" and self.filetype == "pip"
 
     def parse(self, code: bytes) -> Tree:
         r"""Parse.
 
         :param code:
         :type code: bytes
         :rtype: Tree
@@ -212,7 +219,20 @@
         r"""Filter.
 
         :param uni:
         :type uni: UNI
         :rtype: bool
         """
         return uni.node.type == "requirement"
+
+
+FORMATTING_FINDER_CLASSES = [UnsortedRequirementFinder]
+
+
+DIAGNOSTICS_FINDER_CLASSES = [
+    ErrorFinder,
+    MissingFinder,
+    InvalidPackageFinder,
+    InvalidPathFinder,
+    RepeatedPackageFinder,
+    UnsortedRequirementFinder,
+]
```

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server/server.py` & `requirements-language-server-0.0.9/src/requirements_language_server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-# type: ignore
 r"""Server
 ==========
 """
 import os
 from typing import Any
 
 import tree_sitter_requirements as requirements
 from lsprotocol.types import (
-    INITIALIZE,
     TEXT_DOCUMENT_COMPLETION,
     TEXT_DOCUMENT_DEFINITION,
     TEXT_DOCUMENT_DID_CHANGE,
     TEXT_DOCUMENT_DID_OPEN,
     TEXT_DOCUMENT_DOCUMENT_LINK,
     TEXT_DOCUMENT_FORMATTING,
     TEXT_DOCUMENT_HOVER,
@@ -21,37 +19,36 @@
     CompletionList,
     CompletionParams,
     DidChangeTextDocumentParams,
     DocumentFormattingParams,
     DocumentLink,
     DocumentLinkParams,
     Hover,
-    InitializeParams,
     Location,
     MarkupContent,
     MarkupKind,
     TextDocumentPositionParams,
     TextEdit,
 )
-from pip_cache import get_package_names
 from pygls.server import LanguageServer
-
-from . import NOT_FOUND, TEMPLATE
-from .documents import get_documents
-from .documents.option import OPTIONS, OPTIONS_WITH_EQUAL
-from .finders import InvalidPackageFinder, RepeatedPackageFinder
-from .tree_sitter_lsp import UNI
-from .tree_sitter_lsp.complete import get_completion_list_by_uri
-from .tree_sitter_lsp.diagnose import get_diagnostics
-from .tree_sitter_lsp.finders import PositionFinder, TypeFinder
-from .utils import (
-    DIAGNOSTICS_FINDERS,
-    DIAGNOSTICS_FINDERS_PEP508,
-    FORMATTING_FINDER,
+from tree_sitter_lsp import UNI
+from tree_sitter_lsp.complete import get_completion_list_by_uri
+from tree_sitter_lsp.diagnose import get_diagnostics
+from tree_sitter_lsp.finders import PositionFinder, TypeFinder
+from tree_sitter_lsp.format import get_text_edits
+
+from . import FILETYPE
+from .finders import (
+    DIAGNOSTICS_FINDER_CLASSES,
+    FORMATTING_FINDER_CLASSES,
+    InvalidPackageFinder,
+    RepeatedPackageFinder,
 )
+from .misc.option import OPTIONS, OPTIONS_WITH_EQUAL
+from .packages import search_document, search_package_names
 
 try:
     import tomllib as tomli
 except ImportError:
     import tomli
 
 
@@ -65,64 +62,50 @@
         :param args:
         :type args: Any
         :param kwargs:
         :type kwargs: Any
         :rtype: None
         """
         super().__init__(*args, **kwargs)
-        self.template = ""
-        self.documents = {}
         self.trees = {}
 
-        @self.feature(INITIALIZE)
-        def initialize(params: InitializeParams) -> None:
-            r"""Initialize.
-
-            :param params:
-            :type params: InitializeParams
-            :rtype: None
-            """
-            opts = params.initialization_options
-            self.template = getattr(opts, "template", TEMPLATE)
-            self.documents = get_documents()
-
         @self.feature(TEXT_DOCUMENT_DID_OPEN)
         @self.feature(TEXT_DOCUMENT_DID_CHANGE)
         def did_change(params: DidChangeTextDocumentParams) -> None:
             r"""Did change.
 
             :param params:
             :type params: DidChangeTextDocumentParams
             :rtype: None
             """
+            filetype = self.get_filetype(params.text_document.uri)
             document = self.workspace.get_document(params.text_document.uri)
             self.trees[document.uri] = requirements.parse(document.source)
-            if self.is_pep508(document.uri):
-                finders = DIAGNOSTICS_FINDERS_PEP508
-            else:
-                finders = DIAGNOSTICS_FINDERS
             diagnostics = get_diagnostics(
-                finders,
                 document.uri,
                 self.trees[document.uri],
+                DIAGNOSTICS_FINDER_CLASSES,
+                filetype,
             )
             self.publish_diagnostics(params.text_document.uri, diagnostics)
 
         @self.feature(TEXT_DOCUMENT_FORMATTING)
         def format(params: DocumentFormattingParams) -> list[TextEdit]:
             r"""Format.
 
             :param params:
             :type params: DocumentFormattingParams
             :rtype: list[TextEdit]
             """
             document = self.workspace.get_document(params.text_document.uri)
-            finder = FORMATTING_FINDER
-            finder.find_all(document.uri, self.trees[document.uri])
-            return finder.get_text_edits()
+            return get_text_edits(
+                document.uri,
+                self.trees[document.uri],
+                FORMATTING_FINDER_CLASSES,  # type: ignore
+            )
 
         @self.feature(TEXT_DOCUMENT_DEFINITION)
         def definition(params: TextDocumentPositionParams) -> list[Location]:
             r"""Get definition.
 
             :param params:
             :type params: TextDocumentPositionParams
@@ -193,59 +176,47 @@
             text = uni.get_text()
             if uni.node.type == "option":
                 return Hover(
                     MarkupContent(MarkupKind.PlainText, OPTIONS.get(text, "")),
                     uni.get_range(),
                 )
             if uni.node.type == "package":
-                doc = self.documents.get(text, NOT_FOUND)
-                # if cache is outdated
-                if doc == NOT_FOUND:
-                    from .documents.package import search_document
-
-                    doc = search_document(text, TEMPLATE)
-                if not doc:
-                    return None
-                return Hover(
-                    MarkupContent(MarkupKind.Markdown, doc),
-                    uni.get_range(),
-                )
+                if doc := search_document(text):
+                    return Hover(
+                        MarkupContent(MarkupKind.Markdown, doc),
+                        uni.get_range(),
+                    )
 
         @self.feature(TEXT_DOCUMENT_COMPLETION)
         def completions(params: CompletionParams) -> CompletionList:
             r"""Completions.
 
             :param params:
             :type params: CompletionParams
             :rtype: CompletionList
             """
             document = self.workspace.get_document(params.text_document.uri)
-            uni = PositionFinder(params.position).find(
+            uni = PositionFinder(params.position, right_equal=True).find(
                 document.uri, self.trees[document.uri]
             )
             if uni is None:
                 return CompletionList(False, [])
             text = uni.get_text()
 
             if uni.node.type == "package":
                 return CompletionList(
                     False,
                     [
                         CompletionItem(
-                            x,
+                            k,
                             kind=CompletionItemKind.Module,
-                            # even if cache is outdated,
-                            # we still don't find because it is too slow
-                            documentation=MarkupContent(
-                                kind=MarkupKind.Markdown,
-                                value=self.documents.get(x, NOT_FOUND),
-                            ),
-                            insert_text=x,
+                            documentation=v,
+                            insert_text=k,
                         )
-                        for x in get_package_names(text)
+                        for k, v in search_package_names(text).items()
                     ],
                 )
             # uni.node.type != "option" due to incomplete
             if text.startswith("-"):
                 return CompletionList(
                     False,
                     [
@@ -258,28 +229,30 @@
                         for x in OPTIONS_WITH_EQUAL
                         if x.startswith(text)
                     ],
                 )
             document = self.workspace.get_document(params.text_document.uri)
             return get_completion_list_by_uri(document.uri, text, "*.txt")
 
-    def is_pep508(self, uri: str) -> bool:
-        r"""Is pep508.
+    def get_filetype(self, uri: str) -> FILETYPE:
+        r"""Get filetype.
 
         :param uri:
         :type uri: str
-        :rtype: bool
+        :rtype: FILETYPE
         """
+        if self.workspace.root_uri is None:
+            return "pip"
         pyproject_uri = os.path.join(self.workspace.root_uri, "pyproject.toml")
         document = self.workspace.get_document(pyproject_uri)
         pyproject_path = UNI.uri2path(document.uri)
         path = UNI.uri2path(uri)
         if path in self.get_dependencies_files(pyproject_path):
-            return True
-        return False
+            return "pep508"
+        return "pip"
 
     @staticmethod
     def get_dependencies_files(pyproject_path: str) -> list[str]:
         r"""Get dependencies files.
 
         :param pyproject_path:
         :type pyproject_path: str
```

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server.egg-info/PKG-INFO` & `requirements-language-server-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-language-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: requirements.txt language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://requirements-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
@@ -23,21 +23,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: jinja2
 Requires-Dist: pip-cache
 Requires-Dist: platformdirs
-Requires-Dist: pygls
 Requires-Dist: tomli; python_version < "3.11"
+Requires-Dist: tree-sitter-lsp>=0.0.3
 Requires-Dist: tree-sitter-requirements
+Provides-Extra: colorize
+Requires-Dist: tree-sitter-lsp[colorize]; extra == "colorize"
 Provides-Extra: dev
 Requires-Dist: pytest-cov; extra == "dev"
 
 # requirements-language-server
 
 [![readthedocs](https://shields.io/readthedocs/requirements-language-server)](https://requirements-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/requirements-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/requirements-language-server/main)
@@ -103,37 +103,49 @@
 
 We recognize `requirements.txt` and `requirements/dev.txt` as PEP508's
 `requirements.txt`s and display errors for all pip's options. For other
 `requirements.txt`s, we recognize them as pip's `requirements.txt`s.
 
 Features:
 
-- [x] diagnostic
-- [x] format: sort packages
-- [x] go to definition: jump to first repeated package
-- [x] go to reference: jump to all other repeated packages
-- [x] document link: open package's pypi homepage
-- [x] document hover & completion:
+- [x] [Goto Definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_definition):
+  jump to first repeated package
+- [x] [Find References](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_references):
+  jump to all other repeated packages
+- [x] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic):
+  - [x] repeated packages
+  - [x] unsorted packages
+  - [x] invalid path
+  - [x] pip's option when PEP508 is enabled
+- [x] [Document Formatting](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_formatting):
+  sort packages
+- [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink):
+  open package's pypi homepage
+- [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
+  - [x] pip's options
+  - [x] package: requires [pip-cache](https://github.com/brunobeltran/pip-cache).
+    Must `pip-cache update` before.
+- [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion):
   - [x] pip's options
   - [x] package: requires [pip-cache](https://github.com/brunobeltran/pip-cache).
     Must `pip-cache update` before.
 
 Other features:
 
-- [x] pre-commit-hooks
+- [x] [pre-commit-hooks](https://pre-commit.com/)
   - [x] linter
   - [x] formatter
 
 ## Screenshots
 
 ### Diagnostic
 
 ![diagnostic](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/13aa466d-62af-423a-a141-880b495750a7)
 
-### Document Hover
+### Hover
 
 ![module](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/0e74a423-b07a-459a-8fb4-10789f245265)
 
 ![option](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/78a7b5ec-a9dd-46c2-b22b-4dc0123b6f0e)
 
 ### Completion
```

### Comparing `requirements-language-server-0.0.8/src/requirements_language_server.egg-info/SOURCES.txt` & `requirements-language-server-0.0.9/src/requirements_language_server.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 docs/api/requirements-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
 docs/resources/requirements.md
+requirements/colorize.txt
 requirements/dev.txt
 sdist/_requirements-language-server
 sdist/requirements-language-server
 sdist/requirements-language-server.1
 src/requirements_language_server/__init__.py
 src/requirements_language_server/__main__.py
 src/requirements_language_server/_metainfo.py
@@ -32,22 +33,18 @@
 src/requirements_language_server.egg-info/PKG-INFO
 src/requirements_language_server.egg-info/SOURCES.txt
 src/requirements_language_server.egg-info/dependency_links.txt
 src/requirements_language_server.egg-info/entry_points.txt
 src/requirements_language_server.egg-info/requires.txt
 src/requirements_language_server.egg-info/top_level.txt
 src/requirements_language_server/assets/jinja2/template.md.j2
-src/requirements_language_server/documents/__init__.py
-src/requirements_language_server/documents/option.py
-src/requirements_language_server/documents/package.py
-src/requirements_language_server/tree_sitter_lsp/__init__.py
-src/requirements_language_server/tree_sitter_lsp/complete.py
-src/requirements_language_server/tree_sitter_lsp/diagnose.py
-src/requirements_language_server/tree_sitter_lsp/finders.py
-src/requirements_language_server/tree_sitter_lsp/format.py
+src/requirements_language_server/misc/__init__.py
+src/requirements_language_server/misc/option.py
+src/requirements_language_server/packages/__init__.py
+src/requirements_language_server/packages/pypi.py
 templates/class.txt
 templates/def.txt
 templates/noarg.txt
 tests/requirements.txt.in
 tests/test_package.py
 tests/test_server.py
 tests/test_utils.py
```

### Comparing `requirements-language-server-0.0.8/tests/test_utils.py` & `requirements-language-server-0.0.9/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 r"""Test utils."""
 import os
 
+from tree_sitter_lsp.diagnose import check
 from tree_sitter_requirements import parse
 
-from requirements_language_server.tree_sitter_lsp.diagnose import check
-from requirements_language_server.utils import DIAGNOSTICS_FINDERS
+from requirements_language_server.finders import DIAGNOSTICS_FINDER_CLASSES
+from requirements_language_server.utils import get_filetype
 
 
 class Test:
     r"""Test."""
 
     @staticmethod
     def test_check() -> None:
         r"""Test check.
 
         :rtype: None
         """
         result = check(
             [os.path.join(os.path.dirname(__file__), "requirements.txt.in")],
-            DIAGNOSTICS_FINDERS,
             parse,
+            DIAGNOSTICS_FINDER_CLASSES,
+            get_filetype,
         )
         assert result > 0
```

