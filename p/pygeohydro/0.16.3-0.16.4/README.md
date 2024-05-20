# Comparing `tmp/pygeohydro-0.16.3.tar.gz` & `tmp/pygeohydro-0.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeohydro-0.16.3.tar", last modified: Thu May 16 20:16:18 2024, max compression
+gzip compressed data, was "pygeohydro-0.16.4.tar", last modified: Mon May 20 21:25:48 2024, max compression
```

## Comparing `pygeohydro-0.16.3.tar` & `pygeohydro-0.16.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.721878 pygeohydro-0.16.3/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.713878 pygeohydro-0.16.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.713878 pygeohydro-0.16.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.713878 pygeohydro-0.16.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    36468 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-16 20:16:18.721878 pygeohydro-0.16.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.709878 pygeohydro-0.16.3/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.717878 pygeohydro-0.16.3/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.717878 pygeohydro-0.16.3/pygeohydro/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/nfhl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/nlcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/nwis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37032 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/pygeohydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    24736 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/stnfloodevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/us_abbrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/waterdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pygeohydro/watershed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.721878 pygeohydro-0.16.3/pygeohydro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-16 20:16:18.000000 pygeohydro-0.16.3/pygeohydro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 20:16:18.000000 pygeohydro-0.16.3/pygeohydro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:16:18.000000 pygeohydro-0.16.3/pygeohydro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:16:18.000000 pygeohydro-0.16.3/pygeohydro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 20:16:18.000000 pygeohydro-0.16.3/pygeohydro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 20:16:18.000000 pygeohydro-0.16.3/pygeohydro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:16:18.721878 pygeohydro-0.16.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:16:18.721878 pygeohydro-0.16.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/tests/test_pygeohydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-05-16 20:16:06.000000 pygeohydro-0.16.3/tests/test_stn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.919981 pygeohydro-0.16.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    37149 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-20 21:25:48.919981 pygeohydro-0.16.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.907981 pygeohydro-0.16.4/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.915981 pygeohydro-0.16.4/pygeohydro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/nfhl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/nlcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36883 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/pygeohydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24736 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/stnfloodevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/us_abbrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/waterdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/watershed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.915981 pygeohydro-0.16.4/pygeohydro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:25:48.919981 pygeohydro-0.16.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.915981 pygeohydro-0.16.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/tests/test_pygeohydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/tests/test_stn.py
```

### Comparing `pygeohydro-0.16.3/.github/ISSUE_TEMPLATE/bugreport.yml` & `pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/.github/ISSUE_TEMPLATE/newfeature.yml` & `pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/.github/workflows/codeql-analysis.yml` & `pygeohydro-0.16.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/.github/workflows/release.yml` & `pygeohydro-0.16.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/.github/workflows/test.yml` & `pygeohydro-0.16.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/.gitignore` & `pygeohydro-0.16.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/.pre-commit-config.yaml` & `pygeohydro-0.16.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/CITATION.cff` & `pygeohydro-0.16.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/CODE_OF_CONDUCT.rst` & `pygeohydro-0.16.4/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/CONTRIBUTING.rst` & `pygeohydro-0.16.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/HISTORY.rst` & `pygeohydro-0.16.4/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 =======
 History
 =======
 
+0.16.4 (2024-05-20)
+-------------------
+
+Bug Fixes
+~~~~~~~~~
+- Fix an issue in ``NID.stage_nid_inventory`` where the function was failing
+  when the response status code was 206 (partial content). This issue is fixed
+  by checking the response status code and if it's 206, the function will continue
+  reading the headers and the get the modified date from the response headers.
+  Also, the function incorrectly didn't check if the local database was up-to-date
+  with the remote database when the processed database already existed. Now, the
+  function will check changes in the remote database and re-download the data even if
+  necessary even if the processed database exists.
+
 0.16.3 (2024-05-16)
 -------------------
 
 Internal Changes
 ~~~~~~~~~~~~~~~~
 - More robust handling of failed download links for eHydro data.
   For example, sometimes, eHydro web service uses placeholder as actual
```

### Comparing `pygeohydro-0.16.3/LICENSE` & `pygeohydro-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/PKG-INFO` & `pygeohydro-0.16.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.16.3
+Version: 0.16.4
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
```

### Comparing `pygeohydro-0.16.3/README.rst` & `pygeohydro-0.16.4/README.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/ci/requirements/environment-dev.yml` & `pygeohydro-0.16.4/ci/requirements/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/ci/requirements/environment.yml` & `pygeohydro-0.16.4/ci/requirements/environment.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/noxfile.py` & `pygeohydro-0.16.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/__init__.py` & `pygeohydro-0.16.4/pygeohydro/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/exceptions.py` & `pygeohydro-0.16.4/pygeohydro/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/helpers.py` & `pygeohydro-0.16.4/pygeohydro/helpers.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/nfhl.py` & `pygeohydro-0.16.4/pygeohydro/nfhl.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/nlcd.py` & `pygeohydro-0.16.4/pygeohydro/nlcd.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/nwis.py` & `pygeohydro-0.16.4/pygeohydro/nwis.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/plot.py` & `pygeohydro-0.16.4/pygeohydro/plot.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/print_versions.py` & `pygeohydro-0.16.4/pygeohydro/print_versions.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/pygeohydro.py` & `pygeohydro-0.16.4/pygeohydro/pygeohydro.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,28 +235,30 @@
         }
     )
     return eta
 
 
 def _remote_file_modified(file_path: Path) -> bool:
     """Check if the file is older than the last modification date of the NID web service."""
+    if not file_path.exists():
+        return True
     url = "https://nid.sec.usace.army.mil/api/nation/gpkg"
     # we need to get the redirect URL so that we can get the last modified date, so
     # we need to send a request with the Range header set to 0-0 to avoid downloading
     # the entire file.
     response = requests.get(url, headers={"Range": "bytes=0-0"}, allow_redirects=True, timeout=50)
-    if response.status_code != 200:
+    if response.status_code not in (200, 206):
         raise ServiceError(response.reason, url)
     response = requests.head(response.url, timeout=50)
     if response.status_code != 200:
         raise ServiceError(response.reason, url)
 
     remote_last_modified = datetime.strptime(
         response.headers["Last-Modified"], "%a, %d %b %Y %H:%M:%S GMT"
-    )
+    ).replace(tzinfo=timezone.utc)
     local_last_modified = datetime.fromtimestamp(file_path.stat().st_mtime, tz=timezone.utc)
     return local_last_modified < remote_last_modified
 
 
 class NID:
     """Retrieve data from the National Inventory of Dams web service."""
 
@@ -315,51 +317,51 @@
             "maxStorage": "acre-ft",
             "normalStorage": "acre-ft",
             "surfaceArea": "acre",
             "drainageArea": "square miles",
             "maxDischarge": "cfs",
             "spillwayWidth": "ft",
         }
-        self._nid_inventory_path = Path("cache", "nid_inventory.feather")
+        self._nid_inventory_path = Path("cache", "full_nid_inventory.parquet")
 
     @property
     def nid_inventory_path(self) -> Path:
-        """Path to the NID inventory feather file."""
+        """Path to the NID inventory parquet file."""
         return self._nid_inventory_path
 
     @nid_inventory_path.setter
     def nid_inventory_path(self, value: Path | str) -> None:
         self._nid_inventory_path = Path(value)
         self._nid_inventory_path.parent.mkdir(parents=True, exist_ok=True)
 
     def stage_nid_inventory(self, fname: str | Path | None = None) -> None:
-        """Download the entire NID inventory data and save to a feather file.
+        """Download the entire NID inventory data and save to a parquet file.
 
         Parameters
         ----------
         fname : str, pathlib.Path, optional
             The path to the file to save the data to, defaults to
-            ``./cache/nid_inventory.feather``.
+            ``./cache/full_nid_inventory.parquet``.
         """
         fname = self.nid_inventory_path if fname is None else Path(fname)
-        if fname.suffix != ".feather":
-            fname = fname.with_suffix(".feather")
+        if fname.suffix != ".parquet":
+            fname = fname.with_suffix(".parquet")
 
         self.nid_inventory_path = fname
-        if not self.nid_inventory_path.exists():
-            if _remote_file_modified(fname.with_suffix(".gpkg")):
-                fname.with_suffix(".gpkg").unlink()
+        gpkg_file = fname.with_suffix(".gpkg")
+        if _remote_file_modified(gpkg_file) or not self.nid_inventory_path.exists():
+            gpkg_file.unlink(missing_ok=True)
             url = "https://nid.sec.usace.army.mil/api/nation/gpkg"
-            fname_ = ogc.streaming_download(url, fnames=fname.with_suffix(".gpkg"))
+            fname_ = ogc.streaming_download(url, fnames=gpkg_file)
             if fname_ is None:
                 raise EmptyResponseError
             dams = (
-                gpd.read_file(fname.with_suffix(".gpkg"), engine="pyogrio", use_arrow=True)
+                gpd.read_file(gpkg_file, engine="pyogrio", use_arrow=True)
                 if importlib.util.find_spec("pyogrio")
-                else gpd.read_file(fname.with_suffix(".gpkg"))
+                else gpd.read_file(gpkg_file)
             )
 
             dams = dams.astype(
                 {
                     "name": str,
                     "otherNames": str,
                     "formerNames": str,
@@ -431,18 +433,14 @@
                     "inspectionFrequency": "f4",
                     "hazardId": str,
                     "conditionAssessId": str,
                     "conditionAssessDate": "datetime64[ns]",
                     "eapId": str,
                     "eapLastRevDate": "datetime64[ns]",
                     "websiteUrl": str,
-                    "privateDamId": str,
-                    "politicalPartyId": str,
-                    "id": "int32",
-                    "systemId": "int32",
                     "huc2": str,
                     "huc4": str,
                     "huc6": str,
                     "huc8": str,
                     "zipcode": str,
                     "nation": str,
                     "stateKey": str,
@@ -450,16 +448,15 @@
                     "femaCommunity": str,
                 }
             )
             for c in dams:
                 if (dams[c] == "Yes").any():
                     dams[c] = dams[c] == "Yes"
             dams.loc[dams["yearCompleted"] < 1000, "yearCompleted"] = pd.NA
-            dams.to_feather(fname)
-            fname.with_suffix(".gpkg").unlink()
+            dams.to_parquet(fname)
 
     @property
     def df(self):
         """Entire NID inventory (``csv`` version) as a ``pandas.DataFrame``."""
         fname = self.nid_inventory_path
         par_name = fname.with_suffix(".parquert")
         if par_name.exists():
@@ -472,15 +469,15 @@
         dams.to_parquet(par_name)
         return dams
 
     @property
     def gdf(self):
         """Entire NID inventory (``gpkg`` version) as a ``geopandas.GeoDataFrame``."""
         self.stage_nid_inventory()
-        return gpd.read_feather(self.nid_inventory_path)
+        return gpd.read_parquet(self.nid_inventory_path)
 
     @staticmethod
     def _get_json(
         urls: Sequence[str], params: list[dict[str, str]] | None = None
     ) -> list[dict[str, Any]]:
         """Get JSON response from NID web service.
```

### Comparing `pygeohydro-0.16.3/pygeohydro/stnfloodevents.py` & `pygeohydro-0.16.4/pygeohydro/stnfloodevents.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/us_abbrs.py` & `pygeohydro-0.16.4/pygeohydro/us_abbrs.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/waterdata.py` & `pygeohydro-0.16.4/pygeohydro/waterdata.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro/watershed.py` & `pygeohydro-0.16.4/pygeohydro/watershed.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pygeohydro.egg-info/PKG-INFO` & `pygeohydro-0.16.4/pygeohydro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.16.3
+Version: 0.16.4
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
```

### Comparing `pygeohydro-0.16.3/pygeohydro.egg-info/SOURCES.txt` & `pygeohydro-0.16.4/pygeohydro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/pyproject.toml` & `pygeohydro-0.16.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/tests/test_exceptions.py` & `pygeohydro-0.16.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.3/tests/test_pygeohydro.py` & `pygeohydro-0.16.4/tests/test_pygeohydro.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,16 +190,16 @@
         bbox = geoutils.geometry_reproject(GEOM.bounds, DEF_CRS, ALT_CRS)
         dams_box = self.nid.get_bygeom(bbox, ALT_CRS)
         name = "Pingree Pond"
         assert (dams_geo.name == name).any()
         assert (dams_box.name == "Pingree Pond").any()
 
     def test_nation(self):
-        assert self.nid.df.shape == (91807, 79)
-        assert self.nid.gdf.shape == (91658, 97)
+        assert self.nid.df.shape == (91856, 84)
+        assert self.nid.gdf.shape == (91702, 97)
 
 
 class TestWaterQuality:
     wq: gh.WaterQuality = gh.WaterQuality()
 
     def test_bbox(self):
         stations = self.wq.station_bybbox(
@@ -315,15 +315,15 @@
 def test_sensorthings():
     sensor = gh.SensorThings()
     cond = " and ".join(
         ("properties/monitoringLocationType eq 'Stream'", "properties/stateFIPS eq 'US:04'")
     )
     odata = sensor.odata_helper(conditionals=cond)
     df = sensor.query_byodata(odata)
-    assert df.shape[0] == 197
+    assert df.shape[0] == 72
 
     df = sensor.sensor_info("USGS-09380000")
     assert df["description"].iloc[0] == "Stream"
 
     df = sensor.sensor_property("Datastreams", "USGS-09380000")
     assert df["observationType"].unique()[0] == "Instantaneous"
```

### Comparing `pygeohydro-0.16.3/tests/test_stn.py` & `pygeohydro-0.16.4/tests/test_stn.py`

 * *Files identical despite different names*

