# Comparing `tmp/py-solc-x-2.0.2.tar.gz` & `tmp/py-solc-x-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-solc-x-2.0.2.tar", last modified: Fri Nov 10 22:41:45 2023, max compression
+gzip compressed data, was "py-solc-x-2.0.3.tar", last modified: Mon May 20 14:42:55 2024, max compression
```

## Comparing `py-solc-x-2.0.2.tar` & `py-solc-x-2.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.160489 py-solc-x-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8831 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-11-10 22:41:45.160489 py-solc-x-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/methoddocs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/methoddocs/main.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/methoddocs/wrapper.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.152489 py-solc-x-2.0.2/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/userguides/using-the-compiler.md
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/docs/userguides/version-management.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.156489 py-solc-x-2.0.2/py_solc_x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-11-10 22:41:45.000000 py-solc-x-2.0.2/py_solc_x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-11-10 22:41:45.000000 py-solc-x-2.0.2/py_solc_x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 22:41:45.000000 py-solc-x-2.0.2/py_solc_x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 22:41:45.000000 py-solc-x-2.0.2/py_solc_x.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-11-10 22:41:45.000000 py-solc-x-2.0.2/py_solc_x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-10 22:41:45.000000 py-solc-x-2.0.2/py_solc_x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-10 22:41:45.160489 py-solc-x-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.156489 py-solc-x-2.0.2/solcx/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25821 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    16668 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.156489 py-solc-x-2.0.2/solcx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/utils/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-10 22:41:44.000000 py-solc-x-2.0.2/solcx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/solcx/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.156489 py-solc-x-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.156489 py-solc-x-2.0.2/tests/install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_get_executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_import_solc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_solc_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/install/test_validate_installation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:45.160489 py-solc-x-2.0.2/tests/main/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/test_compile_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/test_compile_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/test_link_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/main/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-11-10 22:41:32.000000 py-solc-x-2.0.2/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.553699 py-solc-x-2.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.553699 py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/methoddocs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/methoddocs/main.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/methoddocs/wrapper.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/userguides/using-the-compiler.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/docs/userguides/version-management.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.557699 py-solc-x-2.0.3/py_solc_x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/py_solc_x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/py_solc_x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/py_solc_x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/py_solc_x.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/py_solc_x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/py_solc_x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/solcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26068 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16668 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/solcx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/utils/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 14:42:55.000000 py-solc-x-2.0.3/solcx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/solcx/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/tests/install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_get_executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_import_solc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_solc_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/install/test_validate_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:55.561699 py-solc-x-2.0.3/tests/main/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/test_compile_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/test_compile_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/test_link_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/main/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-20 14:42:44.000000 py-solc-x-2.0.3/tests/test_wrapper.py
```

### Comparing `py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/bug.md` & `py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/feature.md` & `py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/ISSUE_TEMPLATE/work-item.md` & `py-solc-x-2.0.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/release-drafter.yml` & `py-solc-x-2.0.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/workflows/codeql.yml` & `py-solc-x-2.0.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/workflows/prtitle.yaml` & `py-solc-x-2.0.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/workflows/publish.yaml` & `py-solc-x-2.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/workflows/stale-prs.yml` & `py-solc-x-2.0.3/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.github/workflows/test.yaml` & `py-solc-x-2.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.gitignore` & `py-solc-x-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/.pre-commit-config.yaml` & `py-solc-x-2.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/CHANGELOG.md` & `py-solc-x-2.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/CONTRIBUTING.md` & `py-solc-x-2.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/LICENSE` & `py-solc-x-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/PKG-INFO` & `py-solc-x-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-solc-x
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python wrapper and version management tool for the solc Solidity compiler.
 Home-page: https://github.com/ApeWorX/py-solc-x
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: MIT
 Keywords: ethereum solidity solc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py-solc-x-2.0.2/README.md` & `py-solc-x-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/build_docs.py` & `py-solc-x-2.0.3/build_docs.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/_static/custom.css` & `py-solc-x-2.0.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/_static/custom.js` & `py-solc-x-2.0.3/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/_templates/layout.html` & `py-solc-x-2.0.3/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/conf.py` & `py-solc-x-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/favicon.ico` & `py-solc-x-2.0.3/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/logo.gif` & `py-solc-x-2.0.3/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/userguides/using-the-compiler.md` & `py-solc-x-2.0.3/docs/userguides/using-the-compiler.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/docs/userguides/version-management.md` & `py-solc-x-2.0.3/docs/userguides/version-management.md`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/py_solc_x.egg-info/PKG-INFO` & `py-solc-x-2.0.3/py_solc_x.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-solc-x
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python wrapper and version management tool for the solc Solidity compiler.
 Home-page: https://github.com/ApeWorX/py-solc-x
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: MIT
 Keywords: ethereum solidity solc
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `py-solc-x-2.0.2/py_solc_x.egg-info/SOURCES.txt` & `py-solc-x-2.0.3/py_solc_x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/py_solc_x.egg-info/requires.txt` & `py-solc-x-2.0.3/py_solc_x.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/pyproject.toml` & `py-solc-x-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/setup.py` & `py-solc-x-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/solcx/__init__.py` & `py-solc-x-2.0.3/solcx/__init__.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/solcx/exceptions.py` & `py-solc-x-2.0.3/solcx/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/solcx/install.py` & `py-solc-x-2.0.3/solcx/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,16 +485,17 @@
                 version, filename, show_progress, solcx_binary_path=solcx_binary_path
             )
         elif os_name == "windows":
             _install_solc_windows(
                 version, filename, show_progress, solcx_binary_path=solcx_binary_path
             )
 
+        base_version = version if isinstance(version, str) else version.base_version
         try:
-            _validate_installation(version, solcx_binary_path=solcx_binary_path)
+            _validate_installation(Version(base_version), solcx_binary_path=solcx_binary_path)
         except SolcInstallationError as exc:
             if os_name != "windows":
                 exc.args = (
                     f"{exc.args[0]} If this issue persists, you can try to compile from "
                     f"source code using `solcx.compile_solc('{version}')`.",
                 )
             raise exc
@@ -699,24 +700,28 @@
         raise SolcInstallationError(
             "Downloaded binary would not execute, or returned unexpected output."
         )
 
     installed_version_clean = Version(
         Version(installed_version.replace("-nightly", "")).base_version
     )
-    if installed_version_clean.base_version != version.base_version:
+    base_version = version if isinstance(version, str) else version.base_version
+    if installed_version_clean.base_version != base_version:
         # Without the nightly suffix, it should be the same!
         _unlink_solc(binary_path)
         raise UnexpectedVersionError(
             f"Attempted to install solc v{version}, but got solc v{installed_version}"
         )
-    if installed_version not in (version.base_version, f"{version}"):
+    if installed_version_clean not in (
+        Version(base_version),
+        f"{base_version}",
+    ) or installed_version.endswith("-nightly"):
         # If it does have the nightly suffix, then only warn.
         warnings.warn(
-            f"Installed solc version is v{installed_version}, expecting v{version.base_version}",
+            f"Installed solc version is v{installed_version_clean}, expecting v{base_version}",
             UnexpectedVersionWarning,
         )
 
     if not get_default_solc_binary():
         set_solc_version(version)
 
     LOGGER.info(f"solc {version} successfully installed at: {binary_path}")
```

### Comparing `py-solc-x-2.0.2/solcx/main.py` & `py-solc-x-2.0.3/solcx/main.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/solcx/utils/lock.py` & `py-solc-x-2.0.3/solcx/utils/lock.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/solcx/wrapper.py` & `py-solc-x-2.0.3/solcx/wrapper.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/conftest.py` & `py-solc-x-2.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/conftest.py` & `py-solc-x-2.0.3/tests/install/conftest.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/test_compile.py` & `py-solc-x-2.0.3/tests/install/test_compile.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/test_get_executable.py` & `py-solc-x-2.0.3/tests/install/test_get_executable.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/test_import_solc.py` & `py-solc-x-2.0.3/tests/install/test_import_solc.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/test_install.py` & `py-solc-x-2.0.3/tests/install/test_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import pytest
 
 import solcx
 from solcx.exceptions import SolcInstallationError
 
 
 @pytest.mark.skipif("'--no-install' in sys.argv")
@@ -19,15 +21,18 @@
 def test_install_unknown_version():
     with pytest.raises(SolcInstallationError):
         solcx.install_solc("0.4.99")
 
 
 @pytest.mark.skipif("'--no-install' in sys.argv")
 def test_progress_bar(nosolc):
-    assert solcx.install_solc("0.6.9", show_progress=True).base_version == "0.6.9"
+    # There should be no warnings!
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        assert solcx.install_solc("0.6.9", show_progress=True).base_version == "0.6.9"
 
 
 def test_environment_var_path(monkeypatch, tmp_path):
     install_folder = solcx.get_solcx_install_folder()
     monkeypatch.setenv("SOLCX_BINARY_PATH", tmp_path.as_posix())
     assert solcx.get_solcx_install_folder() != install_folder
```

### Comparing `py-solc-x-2.0.2/tests/install/test_locks.py` & `py-solc-x-2.0.3/tests/install/test_locks.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/test_solc_version.py` & `py-solc-x-2.0.3/tests/install/test_solc_version.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/install/test_validate_installation.py` & `py-solc-x-2.0.3/tests/install/test_validate_installation.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/main/conftest.py` & `py-solc-x-2.0.3/tests/main/conftest.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/main/test_compile_files.py` & `py-solc-x-2.0.3/tests/main/test_compile_files.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/main/test_compile_source.py` & `py-solc-x-2.0.3/tests/main/test_compile_source.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/main/test_compile_standard.py` & `py-solc-x-2.0.3/tests/main/test_compile_standard.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/main/test_link_code.py` & `py-solc-x-2.0.3/tests/main/test_link_code.py`

 * *Files identical despite different names*

### Comparing `py-solc-x-2.0.2/tests/test_wrapper.py` & `py-solc-x-2.0.3/tests/test_wrapper.py`

 * *Files identical despite different names*

