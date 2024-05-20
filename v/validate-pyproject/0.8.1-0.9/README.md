# Comparing `tmp/validate-pyproject-0.8.1.tar.gz` & `tmp/validate-pyproject-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validate-pyproject-0.8.1.tar", last modified: Tue May 17 16:43:29 2022, max compression
+gzip compressed data, was "validate-pyproject-0.9.tar", last modified: Wed May 18 11:44:59 2022, max compression
```

## Comparing `validate-pyproject-0.8.1.tar` & `validate-pyproject-0.9.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     8448 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.873190 validate-pyproject-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.877190 validate-pyproject-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.projections.json
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11762 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15922 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8058 2022-05-17 16:43:29.893190 validate-pyproject-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7088 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.881190 validate-pyproject-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.881190 validate-pyproject-0.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/_static/custom-adjustments.css
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11143 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/dev-guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/json-schemas.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-05-17 16:43:29.893190 validate-pyproject-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.873190 validate-pyproject-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.881190 validate-pyproject-0.8.1/src/validate_pyproject/
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.881190 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.881190 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8769 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29451 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/draft04.py
--rw-r--r--   0 runner    (1001) docker     (121)     7661 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/draft06.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/draft07.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12576 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/indent.py
--rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/_vendor/vendoring_instructions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8721 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     8488 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    11263 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/extra_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)     8647 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/src/validate_pyproject/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/plugins/distutils.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)    11372 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/plugins/setuptools.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/NOTICE.template
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/api-notice.template
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/cli-notice.template
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/main_file.template
--rw-r--r--   0 runner    (1001) docker     (121)    11087 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/project_metadata.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/pyproject_toml.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/src/validate_pyproject/vendoring/
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/vendoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/vendoring/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/src/validate_pyproject/vendoring/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.881190 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8058 2022-05-17 16:43:29.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-05-17 16:43:29.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 16:43:29.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-17 16:43:29.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-17 16:43:27.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-17 16:43:29.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-17 16:43:29.000000 validate-pyproject-0.8.1/src/validate_pyproject.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.873190 validate-pyproject-0.8.1/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/atoml/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/atoml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/atoml/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/flit/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/flit/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/flit/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/pdm/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pdm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pdm/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/pep_text/
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pep_text/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/01-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/02-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/03-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/04-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/05-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/06-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/pretend-setuptools/07-pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/simple/dynamic-version.toml
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/simple/minimal.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/examples/trampolim/
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/trampolim/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/examples/trampolim/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.877190 validate-pyproject-0.8.1/tests/invalid-examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.885190 validate-pyproject-0.8.1/tests/invalid-examples/pdm/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pdm/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pdm/invalid-version/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pdm/invalid-version/errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pdm/invalid-version/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pdm/redefining-as-dynamic/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pdm/redefining-as-dynamic/errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4317 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pdm/redefining-as-dynamic/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.877190 validate-pyproject-0.8.1/tests/invalid-examples/pep621/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pep621/missing-fields/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/missing-fields/missing-version-with-dynamic.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/missing-fields/missing-version-with-dynamic.toml
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/missing-fields/missing-version.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/missing-fields/missing-version.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/author_instead_of_authors.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/author_instead_of_authors.toml
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/requires_instead_of_dependencies.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/requires_instead_of_dependencies.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.877190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/cmdclass/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/cmdclass/invalid-value.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/cmdclass/invalid-value.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/dependencies/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/dependencies/invalid-extra-name.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/dependencies/invalid-extra-name.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/package-dir/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/package-dir/invalid-name.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/package-dir/invalid-name.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/packages/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/packages/missing-find-arguments.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/packages/missing-find-arguments.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.877190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/both-text-and-file.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/both-text-and-file.toml
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/empty.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/empty.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-as-array.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-as-array.toml
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-without-content-type.errors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-without-content-type.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/json_schema_summary/
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/array-contains.example
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/array-no-items.example
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/array-prefix-items.example
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/array-simple.example
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/if-then-else.example
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/if-then-else2.example
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/not.example
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/object-no-properties.example
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/object-pattern-properties.example
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/object-property-names.example
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/json_schema_summary/oneof.example
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-17 16:43:29.889190 validate-pyproject-0.8.1/tests/pre_compile/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/pre_compile/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4525 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)    12629 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_json_schema_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_pre_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tests/test_vendoring.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-05-17 16:41:40.000000 validate-pyproject-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     8448 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.projections.json
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-05-18 11:43:16.000000 validate-pyproject-0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-18 11:43:16.000000 validate-pyproject-0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-05-18 11:43:16.000000 validate-pyproject-0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11762 2022-05-18 11:43:16.000000 validate-pyproject-0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15922 2022-05-18 11:43:16.000000 validate-pyproject-0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-05-18 11:43:16.000000 validate-pyproject-0.9/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-05-18 11:44:59.944159 validate-pyproject-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7088 2022-05-18 11:43:16.000000 validate-pyproject-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/_static/custom-adjustments.css
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11143 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4252 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/json-schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-18 11:43:16.000000 validate-pyproject-0.9/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-05-18 11:43:16.000000 validate-pyproject-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-05-18 11:44:59.944159 validate-pyproject-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-05-18 11:43:16.000000 validate-pyproject-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/src/validate_pyproject/
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/src/validate_pyproject/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     8769 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29451 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/draft04.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7661 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/draft06.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/draft07.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12576 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/indent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5527 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/_vendor/vendoring_instructions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8721 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8606 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11263 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/extra_validations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8647 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/src/validate_pyproject/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)     4183 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/plugins/distutils.schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11372 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/plugins/setuptools.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/src/validate_pyproject/pre_compile/
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/NOTICE.template
+-rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/api-notice.template
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/cli-notice.template
+-rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pre_compile/main_file.template
+-rw-r--r--   0 runner    (1001) docker     (121)    11087 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/project_metadata.schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/pyproject_toml.schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/src/validate_pyproject/vendoring/
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/vendoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/vendoring/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-05-18 11:43:16.000000 validate-pyproject-0.9/src/validate_pyproject/vendoring/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.936159 validate-pyproject-0.9/src/validate_pyproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-05-18 11:44:59.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-05-18 11:44:59.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 11:44:59.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-18 11:44:59.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 11:44:57.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-05-18 11:44:59.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-18 11:44:59.000000 validate-pyproject-0.9/src/validate_pyproject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/atoml/
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/atoml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/atoml/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/flit/
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/flit/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      946 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/flit/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/pdm/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pdm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pdm/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/pep_text/
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pep_text/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/pretend-setuptools/
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/01-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/02-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/03-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/04-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/05-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/06-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/pretend-setuptools/07-pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/simple/dynamic-version.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/simple/minimal.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/examples/trampolim/
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/trampolim/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/examples/trampolim/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/tests/invalid-examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/invalid-examples/pdm/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pdm/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/invalid-examples/pdm/invalid-version/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pdm/invalid-version/errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pdm/invalid-version/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/invalid-examples/pdm/redefining-as-dynamic/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pdm/redefining-as-dynamic/errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4317 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pdm/redefining-as-dynamic/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/tests/invalid-examples/pep621/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.940159 validate-pyproject-0.9/tests/invalid-examples/pep621/missing-fields/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/missing-fields/missing-version-with-dynamic.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/missing-fields/missing-version-with-dynamic.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/missing-fields/missing-version.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/missing-fields/missing-version.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/author_instead_of_authors.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/author_instead_of_authors.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/requires_instead_of_dependencies.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/requires_instead_of_dependencies.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/cmdclass/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/cmdclass/invalid-value.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/cmdclass/invalid-value.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/dependencies/invalid-extra-name.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/dependencies/invalid-extra-name.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/package-dir/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/package-dir/invalid-name.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/package-dir/invalid-name.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/packages/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/packages/missing-find-arguments.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/packages/missing-find-arguments.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.932159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/both-text-and-file.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/both-text-and-file.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/empty.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/empty.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-as-array.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-as-array.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-without-content-type.errors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-without-content-type.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/json_schema_summary/
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/array-contains.example
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/array-no-items.example
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/array-prefix-items.example
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/array-simple.example
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/if-then-else.example
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/if-then-else2.example
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/not.example
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/object-no-properties.example
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/object-pattern-properties.example
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/object-property-names.example
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/json_schema_summary/oneof.example
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 11:44:59.944159 validate-pyproject-0.9/tests/pre_compile/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/pre_compile/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4540 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4369 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12629 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_json_schema_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6528 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_pre_compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tests/test_vendoring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-18 11:43:16.000000 validate-pyproject-0.9/tox.ini
```

### Comparing `validate-pyproject-0.8.1/.cirrus.yml` & `validate-pyproject-0.9/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/.coveragerc` & `validate-pyproject-0.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/.github/workflows/ci.yml` & `validate-pyproject-0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/.gitignore` & `validate-pyproject-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/.pre-commit-config.yaml` & `validate-pyproject-0.9/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,16 @@
 
 - repo: https://github.com/PyCQA/flake8
   rev: 4.0.1
   hooks:
   - id: flake8
     additional_dependencies: [flake8-bugbear]
 
-
 - repo: local  # self-test for `validate-pyproject` hook
   hooks:
   - id: validate-pyproject
     name: Validate pyproject.toml
     language: python
-    files: ^tests/examples/pretend-setuptools/07-pyproject.toml$
+    files: ^tests/examples/.*pyproject\.toml$
     entry: validate-pyproject
     additional_dependencies:
-      - validate-pyproject[all]
+      - validate-pyproject[all]>=0.8
```

### Comparing `validate-pyproject-0.8.1/.projections.json` & `validate-pyproject-0.9/.projections.json`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/CHANGELOG.rst` & `validate-pyproject-0.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 0.9
+===========
+
+- Use ``tomllib`` from the standard library in Python 3.11+, #42
+
 Version 0.8.1
 =============
 
 - Workaround typecheck inconsistencies between different Python versions
 - Publish :pep:`561` type hints, #43
 
 Version 0.8
```

### Comparing `validate-pyproject-0.8.1/CONTRIBUTING.rst` & `validate-pyproject-0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/LICENSE.txt` & `validate-pyproject-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/NOTICE.txt` & `validate-pyproject-0.9/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/PKG-INFO` & `validate-pyproject-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validate-pyproject
-Version: 0.8.1
+Version: 0.9
 Summary: Validation library and CLI tool for checking on 'pyproject.toml' files using JSON Schema
 Home-page: https://github.com/abravalheri/validate-pyproject/
 Author: Anderson Bravalheri
 Author-email: andersonbravalheri@gmail.com
 License: MPL-2.0 and MIT and BSD-3-Clause
 Project-URL: Documentation, https://validate-pyproject.readthedocs.io/
 Project-URL: Source, https://github.com/abravalheri/validate-pyproject
```

### Comparing `validate-pyproject-0.8.1/README.rst` & `validate-pyproject-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/Makefile` & `validate-pyproject-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/_static/custom-adjustments.css` & `validate-pyproject-0.9/docs/_static/custom-adjustments.css`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/conf.py` & `validate-pyproject-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/dev-guide.rst` & `validate-pyproject-0.9/docs/dev-guide.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/embedding.rst` & `validate-pyproject-0.9/docs/embedding.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/faq.rst` & `validate-pyproject-0.9/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/index.rst` & `validate-pyproject-0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/json-schemas.rst` & `validate-pyproject-0.9/docs/json-schemas.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/docs/schemas.rst` & `validate-pyproject-0.9/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/setup.cfg` & `validate-pyproject-0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 all = 
-	tomli>=1.2.1
+	tomli>=1.2.1; python_version<"3.11"
 	packaging>=20.4
 	trove-classifiers>=2021.10.20
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 typecheck =
```

### Comparing `validate-pyproject-0.8.1/setup.py` & `validate-pyproject-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/__init__.py` & `validate-pyproject-0.9/src/validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/LICENSE` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/LICENSE`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/__init__.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/draft04.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/draft04.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/draft06.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/draft06.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/draft07.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/draft07.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/exceptions.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/generator.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/generator.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/indent.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/indent.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/fastjsonschema/ref_resolver.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/_vendor/vendoring_instructions.rst` & `validate-pyproject-0.9/src/validate_pyproject/_vendor/vendoring_instructions.rst`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/api.py` & `validate-pyproject-0.9/src/validate_pyproject/api.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/cli.py` & `validate-pyproject-0.9/src/validate_pyproject/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,25 @@
 from .plugins import PluginWrapper
 from .plugins import list_from_entry_points as list_plugins_from_entry_points
 
 _logger = logging.getLogger(__package__)
 T = TypeVar("T", bound=NamedTuple)
 
 
-try:
-    from tomli import TOMLDecodeError, loads
+try:  # pragma: no cover
+    if sys.version_info[:2] >= (3, 11):
+        from tomllib import TOMLDecodeError, loads
+    else:
+        from tomli import TOMLDecodeError, loads
 except ImportError:  # pragma: no cover
     try:
         from toml import TomlDecodeError as TOMLDecodeError  # type: ignore
         from toml import loads  # type: ignore
     except ImportError as ex:
-        raise ImportError("Please install a TOML parser (e.g. `tomli`)") from ex
+        raise ImportError("Please install `tomli` (TOML parser)") from ex
 
 _REGULAR_EXCEPTIONS = (ValidationError, TOMLDecodeError)
 
 
 @contextmanager
 def critical_logging():
     """Make sure the logging level is set even before parsing the CLI args"""
```

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/error_reporting.py` & `validate-pyproject-0.9/src/validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/errors.py` & `validate-pyproject-0.9/src/validate_pyproject/errors.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/extra_validations.py` & `validate-pyproject-0.9/src/validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/formats.py` & `validate-pyproject-0.9/src/validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/plugins/__init__.py` & `validate-pyproject-0.9/src/validate_pyproject/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/plugins/distutils.schema.json` & `validate-pyproject-0.9/src/validate_pyproject/plugins/distutils.schema.json`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/plugins/setuptools.schema.json` & `validate-pyproject-0.9/src/validate_pyproject/plugins/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/NOTICE.template` & `validate-pyproject-0.9/src/validate_pyproject/pre_compile/NOTICE.template`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/__init__.py` & `validate-pyproject-0.9/src/validate_pyproject/pre_compile/__init__.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/cli.py` & `validate-pyproject-0.9/src/validate_pyproject/pre_compile/cli.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/pre_compile/main_file.template` & `validate-pyproject-0.9/src/validate_pyproject/pre_compile/main_file.template`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/project_metadata.schema.json` & `validate-pyproject-0.9/src/validate_pyproject/project_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/pyproject_toml.schema.json` & `validate-pyproject-0.9/src/validate_pyproject/pyproject_toml.schema.json`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/types.py` & `validate-pyproject-0.9/src/validate_pyproject/types.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject/vendoring/__init__.py` & `validate-pyproject-0.9/src/validate_pyproject/vendoring/__init__.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject.egg-info/PKG-INFO` & `validate-pyproject-0.9/src/validate_pyproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validate-pyproject
-Version: 0.8.1
+Version: 0.9
 Summary: Validation library and CLI tool for checking on 'pyproject.toml' files using JSON Schema
 Home-page: https://github.com/abravalheri/validate-pyproject/
 Author: Anderson Bravalheri
 Author-email: andersonbravalheri@gmail.com
 License: MPL-2.0 and MIT and BSD-3-Clause
 Project-URL: Documentation, https://validate-pyproject.readthedocs.io/
 Project-URL: Source, https://github.com/abravalheri/validate-pyproject
```

### Comparing `validate-pyproject-0.8.1/src/validate_pyproject.egg-info/SOURCES.txt` & `validate-pyproject-0.9/src/validate_pyproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/atoml/LICENSE` & `validate-pyproject-0.9/tests/examples/atoml/LICENSE`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/atoml/pyproject.toml` & `validate-pyproject-0.9/tests/examples/atoml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/flit/LICENSE` & `validate-pyproject-0.9/tests/examples/flit/LICENSE`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/flit/pyproject.toml` & `validate-pyproject-0.9/tests/examples/flit/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pdm/LICENSE` & `validate-pyproject-0.9/tests/examples/pdm/LICENSE`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pdm/pyproject.toml` & `validate-pyproject-0.9/tests/examples/pdm/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pep_text/pyproject.toml` & `validate-pyproject-0.9/tests/examples/pep_text/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/01-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/01-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/02-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/02-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/03-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/03-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/04-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/04-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/05-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/05-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/06-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/06-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/pretend-setuptools/07-pyproject.toml` & `validate-pyproject-0.9/tests/examples/pretend-setuptools/07-pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/trampolim/LICENSE` & `validate-pyproject-0.9/tests/examples/trampolim/LICENSE`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/examples/trampolim/pyproject.toml` & `validate-pyproject-0.9/tests/examples/trampolim/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pdm/LICENSE` & `validate-pyproject-0.9/tests/invalid-examples/pdm/LICENSE`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pdm/invalid-version/pyproject.toml` & `validate-pyproject-0.9/tests/invalid-examples/pdm/invalid-version/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pdm/redefining-as-dynamic/pyproject.toml` & `validate-pyproject-0.9/tests/invalid-examples/pdm/redefining-as-dynamic/pyproject.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/author_instead_of_authors.toml` & `validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/author_instead_of_authors.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pep621/non-standardised-project-fields/requires_instead_of_dependencies.toml` & `validate-pyproject-0.9/tests/invalid-examples/pep621/non-standardised-project-fields/requires_instead_of_dependencies.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/cmdclass/invalid-value.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/cmdclass/invalid-value.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/package-dir/invalid-name.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/package-dir/invalid-name.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/packages/missing-find-arguments.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/packages/missing-find-arguments.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/both-text-and-file.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/both-text-and-file.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/license/empty.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/license/empty.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-as-array.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-as-array.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-without-content-type.toml` & `validate-pyproject-0.9/tests/invalid-examples/pretend-setuptools/pep621/readme/readme-without-content-type.toml`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/json_schema_summary/if-then-else.example` & `validate-pyproject-0.9/tests/json_schema_summary/if-then-else.example`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/json_schema_summary/not.example` & `validate-pyproject-0.9/tests/json_schema_summary/not.example`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/json_schema_summary/oneof.example` & `validate-pyproject-0.9/tests/json_schema_summary/oneof.example`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/test_api.py` & `validate-pyproject-0.9/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections.abc import Mapping
 from functools import partial, wraps
 
 import pytest
-import tomli
 from validate_pyproject._vendor import fastjsonschema as FJS
 
 from validate_pyproject import api, errors, plugins, types
 
+from .helpers import toml_
+
 PYPA_SPECS = "https://packaging.python.org/en/latest/specifications"
 
 
 def test_load():
     spec = api.load("pyproject_toml")
     assert isinstance(spec, Mapping)
 
@@ -80,15 +81,15 @@
     [tool.setuptools]
     zip-safe = false
     packages = {find = {}}
     """
 
     @property
     def valid_example(self):
-        return tomli.loads(self.example_toml)
+        return toml_.loads(self.example_toml)
 
     @property
     def invalid_example(self):
         example = self.valid_example
         example["tool"]["setuptools"]["zip-safe"] = {"hello": "world"}
         return example
```

### Comparing `validate-pyproject-0.8.1/tests/test_cli.py` & `validate-pyproject-0.9/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import inspect
 import logging
+import sys
 from pathlib import Path
 from uuid import uuid4
 
 import pytest
 from validate_pyproject._vendor.fastjsonschema import JsonSchemaValueException
 
 from validate_pyproject import cli, plugins
@@ -157,7 +159,14 @@
     captured = capsys.readouterr().out.lower()
     captured = captured.replace("invalid file:", repl)
     number_invalid = captured.count(repl)
     number_valid = captured.count("valid file:")
     captured = captured.replace(repl, "invalid file:")
     assert number_valid == N
     assert number_invalid == N + 3
+
+
+@pytest.mark.skipif(sys.version_info[:2] < (3, 11), reason="requires 3.11+")
+def test_parser_is_tomllib():
+    """Make sure Python >= 3.11 uses tomllib instead of tomli"""
+    module_name = inspect.getmodule(cli.loads).__name__
+    assert module_name.startswith("tomllib")
```

### Comparing `validate-pyproject-0.8.1/tests/test_error_reporting.py` & `validate-pyproject-0.9/tests/test_error_reporting.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/test_examples.py` & `validate-pyproject-0.9/tests/test_examples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import logging
 
 import pytest
-import tomli
 from validate_pyproject._vendor.fastjsonschema import JsonSchemaValueException
 
 from validate_pyproject import api, cli
 
-from .helpers import EXAMPLES, INVALID, error_file, examples, invalid_examples
+from .helpers import EXAMPLES, INVALID, error_file, examples, invalid_examples, toml_
 
 
 @pytest.mark.parametrize("example", examples())
 def test_examples_api(example):
-    toml_equivalent = tomli.loads((EXAMPLES / example).read_text())
+    toml_equivalent = toml_.loads((EXAMPLES / example).read_text())
     validator = api.Validator()
     return validator(toml_equivalent) is not None
 
 
 @pytest.mark.parametrize("example", examples())
 def test_examples_cli(example):
     assert cli.run(["--dump-json", str(EXAMPLES / example)]) == 0  # no errors
 
 
 @pytest.mark.parametrize("example", invalid_examples())
 def test_invalid_examples_api(example):
     example_file = INVALID / example
     expected_error = error_file(example_file).read_text("utf-8")
-    toml_equivalent = tomli.loads(example_file.read_text())
+    toml_equivalent = toml_.loads(example_file.read_text())
     validator = api.Validator()
     with pytest.raises(JsonSchemaValueException) as exc_info:
         validator(toml_equivalent)
     exception_message = str(exc_info.value)
     for error in expected_error.splitlines():
         assert error in exception_message
```

### Comparing `validate-pyproject-0.8.1/tests/test_formats.py` & `validate-pyproject-0.9/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/test_json_schema_summary.py` & `validate-pyproject-0.9/tests/test_json_schema_summary.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/test_plugins.py` & `validate-pyproject-0.9/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `validate-pyproject-0.8.1/tests/test_pre_compile.py` & `validate-pyproject-0.9/tests/test_pre_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import shutil
 import subprocess
 import sys
 from inspect import cleandoc
 from pathlib import Path
 
 import pytest
-import tomli
 from validate_pyproject._vendor.fastjsonschema import JsonSchemaValueException
 
 from validate_pyproject.pre_compile import cli, pre_compile
 
-from .helpers import EXAMPLES, INVALID, error_file, examples, invalid_examples
+from .helpers import EXAMPLES, INVALID, error_file, examples, invalid_examples, toml_
 
 MAIN_FILE = "hello_world.py"  # Let's use something different that `__init__.py`
 
 
 def _pre_compile_checks(path: Path):
     assert (path / "__init__.py").exists()
     assert (path / "__init__.py").read_text() == ""
@@ -135,25 +134,25 @@
 
     return _validate
 
 
 @pytest.mark.parametrize("example", examples())
 @pytest.mark.parametrize("pre_compiled", _PRE_COMPILED)
 def test_examples_api(tmp_path, pre_compiled_validate, example, pre_compiled):
-    toml_equivalent = tomli.loads((EXAMPLES / example).read_text())
+    toml_equivalent = toml_.loads((EXAMPLES / example).read_text())
     pre_compiled_path = pre_compiled(Path(tmp_path))
     return pre_compiled_validate(pre_compiled_path, toml_equivalent) is not None
 
 
 @pytest.mark.parametrize("example", invalid_examples())
 @pytest.mark.parametrize("pre_compiled", _PRE_COMPILED)
 def test_invalid_examples_api(tmp_path, pre_compiled_validate, example, pre_compiled):
     example_file = INVALID / example
     expected_error = error_file(example_file).read_text("utf-8")
-    toml_equivalent = tomli.loads(example_file.read_text())
+    toml_equivalent = toml_.loads(example_file.read_text())
     pre_compiled_path = pre_compiled(Path(tmp_path))
     with pytest.raises(JsonSchemaValueException) as exc_info:
         pre_compiled_validate(pre_compiled_path, toml_equivalent)
     exception_message = str(exc_info.value)
     print("rule", "=", exc_info.value.rule)
     print("rule_definition", "=", exc_info.value.rule_definition)
     print("definition", "=", exc_info.value.definition)
```

### Comparing `validate-pyproject-0.8.1/tox.ini` & `validate-pyproject-0.9/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -68,19 +68,21 @@
     linkcheck: Check for broken links in the documentation
 setenv =
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
     linkcheck: BUILD = linkcheck
+extras =
+    all
 deps =
     -r {toxinidir}/docs/requirements.txt
     # ^  requirements.txt shared with Read The Docs
 commands =
-    sphinx-build --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
+    sphinx-build -v -T -j auto --color -b {env:BUILD} -d "{env:BUILDDIR}/doctrees" "{env:DOCSDIR}" "{env:BUILDDIR}/{env:BUILD}" {posargs}
 
 
 [testenv:publish]
 description =
     Publish the package you have been developing to a package index server.
     By default, it uses testpypi. If you really want to publish your package
     to be publicly accessible in PyPI, use the `-- --repository pypi` option.
```

