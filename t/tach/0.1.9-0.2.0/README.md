# Comparing `tmp/tach-0.1.9.tar.gz` & `tmp/tach-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.1.9.tar", last modified: Thu May  9 15:44:29 2024, max compression
+gzip compressed data, was "tach-0.2.0.tar", last modified: Mon May 20 02:23:13 2024, max compression
```

## Comparing `tach-0.1.9.tar` & `tach-0.2.0.tar`

### file list

```diff
@@ -1,131 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.881271 tach-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.889271 tach-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-09 15:44:24.000000 tach-0.1.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 15:44:24.000000 tach-0.1.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 15:44:24.000000 tach-0.1.9/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-09 15:44:24.000000 tach-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 15:44:24.000000 tach-0.1.9/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 15:44:24.000000 tach-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-09 15:44:29.905271 tach-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-09 15:44:24.000000 tach-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 15:44:24.000000 tach-0.1.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.889271 tach-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-09 15:44:24.000000 tach-0.1.9/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 15:44:24.000000 tach-0.1.9/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-09 15:44:24.000000 tach-0.1.9/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 15:44:24.000000 tach-0.1.9/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-09 15:44:24.000000 tach-0.1.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-09 15:44:24.000000 tach-0.1.9/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 15:44:24.000000 tach-0.1.9/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-09 15:44:24.000000 tach-0.1.9/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-09 15:44:24.000000 tach-0.1.9/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-09 15:44:24.000000 tach-0.1.9/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-09 15:44:24.000000 tach-0.1.9/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 15:44:24.000000 tach-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:44:29.905271 tach-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.889271 tach-0.1.9/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-09 15:44:24.000000 tach-0.1.9/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-09 15:44:24.000000 tach-0.1.9/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-09 15:44:24.000000 tach-0.1.9/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 15:44:24.000000 tach-0.1.9/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 15:44:24.000000 tach-0.1.9/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 15:44:24.000000 tach-0.1.9/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 15:44:24.000000 tach-0.1.9/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 15:44:24.000000 tach-0.1.9/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 15:44:24.000000 tach-0.1.9/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 15:44:24.000000 tach-0.1.9/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-09 15:44:24.000000 tach-0.1.9/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.893271 tach-0.1.9/tach/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-09 15:44:24.000000 tach-0.1.9/tach/hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-09 15:44:24.000000 tach-0.1.9/tach/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-09 15:44:24.000000 tach-0.1.9/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 15:44:24.000000 tach-0.1.9/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-09 15:44:24.000000 tach-0.1.9/tach/parsing/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 15:44:29.000000 tach-0.1.9/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 15:44:24.000000 tach-0.1.9/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.897271 tach-0.1.9/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.901271 tach-0.1.9/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:44:29.905271 tach-0.1.9/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 15:44:24.000000 tach-0.1.9/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_module_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:44:24.000000 tach-0.1.9/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.676150 tach-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.680150 tach-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-20 02:23:04.000000 tach-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 02:23:04.000000 tach-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 02:23:04.000000 tach-0.2.0/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-20 02:23:04.000000 tach-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 02:23:04.000000 tach-0.2.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 02:23:04.000000 tach-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 02:23:13.696150 tach-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-20 02:23:04.000000 tach-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 02:23:04.000000 tach-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-20 02:23:04.000000 tach-0.2.0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-20 02:23:04.000000 tach-0.2.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-20 02:23:04.000000 tach-0.2.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-20 02:23:04.000000 tach-0.2.0/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 02:23:04.000000 tach-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 02:23:04.000000 tach-0.2.0/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-20 02:23:04.000000 tach-0.2.0/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-20 02:23:04.000000 tach-0.2.0/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-20 02:23:04.000000 tach-0.2.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-20 02:23:04.000000 tach-0.2.0/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-20 02:23:04.000000 tach-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-20 02:23:04.000000 tach-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:23:13.696150 tach-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-20 02:23:04.000000 tach-0.2.0/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-20 02:23:04.000000 tach-0.2.0/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 02:23:04.000000 tach-0.2.0/tach/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-20 02:23:04.000000 tach-0.2.0/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 02:23:04.000000 tach-0.2.0/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 02:23:04.000000 tach-0.2.0/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 02:23:04.000000 tach-0.2.0/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 02:23:04.000000 tach-0.2.0/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 02:23:04.000000 tach-0.2.0/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 02:23:04.000000 tach-0.2.0/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-20 02:23:04.000000 tach-0.2.0/tach/hooks/pre-commit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-20 02:23:04.000000 tach-0.2.0/tach/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 02:23:04.000000 tach-0.2.0/tach/interactive/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-20 02:23:04.000000 tach-0.2.0/tach/interactive/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 02:23:04.000000 tach-0.2.0/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 02:23:04.000000 tach-0.2.0/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-20 02:23:04.000000 tach-0.2.0/tach/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-20 02:23:04.000000 tach-0.2.0/tach/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-20 02:23:04.000000 tach-0.2.0/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_package_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_show.py
```

### Comparing `tach-0.1.9/.github/workflows/ci.yml` & `tach-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/.github/workflows/publish.yml` & `tach-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/.github/workflows/publish_docs.yml` & `tach-0.2.0/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/.gitignore` & `tach-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/LICENSE` & `tach-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/PKG-INFO` & `tach-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,31 +22,35 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: stdlib-list==0.10.0
+Requires-Dist: rich==13.7.1
+Requires-Dist: prompt-toolkit==3.0.43
 
 [![image](https://img.shields.io/pypi/v/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/l/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/pyversions/tach.svg)](https://pypi.Python.org/pypi/tach)
-[![image](https://github.com/Never-Over/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/Never-Over/tach/actions/workflows/ci.yml)
+[![image](https://github.com/gauge-sh/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/gauge-sh/tach/actions/workflows/ci.yml)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # tach
 a Python tool to enforce modular design
 
 
-[Docs](https://never-over.github.io/tach/)
+[Docs](https://gauge-sh.github.io/tach/)
 
-[Discord](https://discord.gg/7crTTJwDv9) - come say hi!
+[Discord](https://discord.gg/DKVksRtuqS) - come say hi!
 
 
- <video loop src="https://github.com/Never-Over/tach/assets/10570340/a9d8d4df-d262-4b2b-b69a-adbc30d069aa">Tach Demo</video> 
+
+https://github.com/gauge-sh/tach/assets/10570340/2f5ed866-124e-4322-afe6-15207727ca38
+
 
 
 ## What is tach?
 `tach` allows you to define boundaries and control dependencies between your Python packages. Each package can also define its public interface.
 
 This enforces a decoupled, modular architecture, and prevents tight coupling.
 If a package tries to import from another package that is not listed as a dependency, tach will report an error.
@@ -56,30 +60,47 @@
 
 ## Installation
 ```bash
 pip install tach
 ```
 
 ## Quickstart
-`tach` comes bundled with a command to set up and define your initial boundaries.
+`tach` comes bundled with a command to interactively define your package boundaries.
+Run the following in the root of your Python project to enter the editor:
+```bash
+tach pkg
+```
+
+The interactive editor allows you to mark which directories should be treated as package boundaries.
+You can navigate with the arrow keys, mark individual packages with `Enter`, and mark all sibling directories
+as packages with `Ctrl + a`.
+
+After identifying your packages, press `Ctrl + s` to initialize the boundaries.
+Each package will receive a `package.yml` with a single tag based on the folder name,
+and a default `tach.yml` file will be created in the current working directory.
+
+If you want to sync your `tach.yml` with the actual dependencies found in your project, you can use `tach sync`:
 ```bash
-tach init
+tach sync [--prune]
 ```
-By running `tach init` from the root of your Python project, `tach` will initialize each top-level Python package. Each package will receive a `package.yml` with a single tag based on the folder name. 
-The tool will take into consideration the usages between packages, and write a matching set of dependencies to `tach.yml` in the project root.
 
-If you'd like to incrementally or individually add new packages to your `tach.yml`, you can use:
+Any dependency errors will be automatically resolved by
+adding the corresponding dependencies to your `tach.yml` file. If you supply `--prune`,
+any dependency constraints in your `tach.yml` which are not necessary will also be removed.
+
+In case you want to start over, `tach clean` lets you delete all `tach` configuration files so that you can re-initialize or configure your packages manually.
 ```bash
-tach add [file_or_path]
+tach clean
 ```
-This will create a boundary around the given file or directory, and update your `tach.yml` with the correct set of dependencies.
 
 
 ## Defining Packages
-To define a package, add a `package.yml` to the corresponding Python package. Add at least one 'tag' to identify the package:
+To define a package, add a `package.yml` to the corresponding Python package. Add at least one 'tag' to identify the package.
+
+Examples:
 ```python
 # core/package.yml
 tags: ["core"]
 ```
 ```python
 # db/package.yml
 tags: ["db"]
@@ -104,17 +125,19 @@
 ```
 With these rules in place, packages with tag `core` can import from packages with tag `db` or `utils`. Packages tagged with `db` can only import from `utils`, and packages tagged with `utils` cannot import from any other packages in the project. 
 
 `tach` will now flag any violation of these boundaries.
 ```bash
 # From the root of your Python project (in this example, `project/`)
 > tach check
-❌ ./utils/helpers.py: Import "core.PublicAPI" is blocked by boundary "core". Tag(s) ["utils"] do not have access to ["core"].
+❌ utils/helpers.py[L10]: Cannot import 'core.PublicAPI'. Tags ['utils'] cannot depend on ['core'].
 ```
 
+NOTE: If your terminal supports hyperlinks, you can click on the failing file path to go directly to the error.
+
 ## Defining Interfaces
 If you want to define a public interface for the package, import and reference each object you want exposed in the package's `__init__.py` and add its name to `__all__`:
 ```python
 # db/__init__.py
 from db.service import PublicAPI
 
 __all__ = ["PublicAPI"]
@@ -127,15 +150,15 @@
 ```
 ```python
 # The only valid import from "db"
 from db import PublicAPI 
 ```
 
 ### Pre-Commit Hook
-`tach` can be installed as a pre-commit hook. See the [docs](https://never-over.github.io/tach/usage/#tach-install) for installation instructions.
+`tach` can be installed as a pre-commit hook. See the [docs](https://gauge-sh.github.io/tach/usage/#tach-install) for installation instructions.
 
 
 ## Advanced
 `tach` supports specific exceptions. You can mark an import with the `tach-ignore` comment:
 ```python
 # tach-ignore
 from db.main import PrivateAPI
```

### Comparing `tach-0.1.9/README.md` & `tach-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [![image](https://img.shields.io/pypi/v/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/l/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/pyversions/tach.svg)](https://pypi.Python.org/pypi/tach)
-[![image](https://github.com/Never-Over/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/Never-Over/tach/actions/workflows/ci.yml)
+[![image](https://github.com/gauge-sh/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/gauge-sh/tach/actions/workflows/ci.yml)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # tach
 a Python tool to enforce modular design
 
 
-[Docs](https://never-over.github.io/tach/)
+[Docs](https://gauge-sh.github.io/tach/)
 
-[Discord](https://discord.gg/7crTTJwDv9) - come say hi!
+[Discord](https://discord.gg/DKVksRtuqS) - come say hi!
 
 
- <video loop src="https://github.com/Never-Over/tach/assets/10570340/a9d8d4df-d262-4b2b-b69a-adbc30d069aa">Tach Demo</video> 
+
+https://github.com/gauge-sh/tach/assets/10570340/2f5ed866-124e-4322-afe6-15207727ca38
+
 
 
 ## What is tach?
 `tach` allows you to define boundaries and control dependencies between your Python packages. Each package can also define its public interface.
 
 This enforces a decoupled, modular architecture, and prevents tight coupling.
 If a package tries to import from another package that is not listed as a dependency, tach will report an error.
@@ -27,30 +29,47 @@
 
 ## Installation
 ```bash
 pip install tach
 ```
 
 ## Quickstart
-`tach` comes bundled with a command to set up and define your initial boundaries.
+`tach` comes bundled with a command to interactively define your package boundaries.
+Run the following in the root of your Python project to enter the editor:
+```bash
+tach pkg
+```
+
+The interactive editor allows you to mark which directories should be treated as package boundaries.
+You can navigate with the arrow keys, mark individual packages with `Enter`, and mark all sibling directories
+as packages with `Ctrl + a`.
+
+After identifying your packages, press `Ctrl + s` to initialize the boundaries.
+Each package will receive a `package.yml` with a single tag based on the folder name,
+and a default `tach.yml` file will be created in the current working directory.
+
+If you want to sync your `tach.yml` with the actual dependencies found in your project, you can use `tach sync`:
 ```bash
-tach init
+tach sync [--prune]
 ```
-By running `tach init` from the root of your Python project, `tach` will initialize each top-level Python package. Each package will receive a `package.yml` with a single tag based on the folder name. 
-The tool will take into consideration the usages between packages, and write a matching set of dependencies to `tach.yml` in the project root.
 
-If you'd like to incrementally or individually add new packages to your `tach.yml`, you can use:
+Any dependency errors will be automatically resolved by
+adding the corresponding dependencies to your `tach.yml` file. If you supply `--prune`,
+any dependency constraints in your `tach.yml` which are not necessary will also be removed.
+
+In case you want to start over, `tach clean` lets you delete all `tach` configuration files so that you can re-initialize or configure your packages manually.
 ```bash
-tach add [file_or_path]
+tach clean
 ```
-This will create a boundary around the given file or directory, and update your `tach.yml` with the correct set of dependencies.
 
 
 ## Defining Packages
-To define a package, add a `package.yml` to the corresponding Python package. Add at least one 'tag' to identify the package:
+To define a package, add a `package.yml` to the corresponding Python package. Add at least one 'tag' to identify the package.
+
+Examples:
 ```python
 # core/package.yml
 tags: ["core"]
 ```
 ```python
 # db/package.yml
 tags: ["db"]
@@ -75,17 +94,19 @@
 ```
 With these rules in place, packages with tag `core` can import from packages with tag `db` or `utils`. Packages tagged with `db` can only import from `utils`, and packages tagged with `utils` cannot import from any other packages in the project. 
 
 `tach` will now flag any violation of these boundaries.
 ```bash
 # From the root of your Python project (in this example, `project/`)
 > tach check
-❌ ./utils/helpers.py: Import "core.PublicAPI" is blocked by boundary "core". Tag(s) ["utils"] do not have access to ["core"].
+❌ utils/helpers.py[L10]: Cannot import 'core.PublicAPI'. Tags ['utils'] cannot depend on ['core'].
 ```
 
+NOTE: If your terminal supports hyperlinks, you can click on the failing file path to go directly to the error.
+
 ## Defining Interfaces
 If you want to define a public interface for the package, import and reference each object you want exposed in the package's `__init__.py` and add its name to `__all__`:
 ```python
 # db/__init__.py
 from db.service import PublicAPI
 
 __all__ = ["PublicAPI"]
@@ -98,15 +119,15 @@
 ```
 ```python
 # The only valid import from "db"
 from db import PublicAPI 
 ```
 
 ### Pre-Commit Hook
-`tach` can be installed as a pre-commit hook. See the [docs](https://never-over.github.io/tach/usage/#tach-install) for installation instructions.
+`tach` can be installed as a pre-commit hook. See the [docs](https://gauge-sh.github.io/tach/usage/#tach-install) for installation instructions.
 
 
 ## Advanced
 `tach` supports specific exceptions. You can mark an import with the `tach-ignore` comment:
 ```python
 # tach-ignore
 from db.main import PrivateAPI
```

### Comparing `tach-0.1.9/docs/favicon.ico` & `tach-0.2.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/docs/index.md` & `tach-0.2.0/docs/index.md`

 * *Files 23% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 If a package tries to import from another package that is not listed as a dependency, `tach` will throw an exception.
 
 When a package is in ['strict mode'](strict-mode.md), if another package tries to import from it without using its public interface, `tach` will throw an exception.
 
 `tach` runs on the CLI, and is ideal for pre-commit hooks and CI checks.
 
 ## Commands
-* [`tach init`](usage.md#tach-init) - Initialize package boundaries in your Python project.
-* [`tach add`](usage.md#tach-add) - Add a new package around a file or directory to your existing config. 
+* [`tach pkg`](usage.md#tach-pkg) - Interactively define package boundaries in your Python project.
 * [`tach check`](usage.md#tach-check) - Check that boundaries are respected.
+* [`tach sync`](usage.md#tach-sync) - Sync constraints with actual dependencies in your Python project.
 * [`tach install`](usage.md#tach-install) - Install `tach` into your development workflow (e.g. pre-commit)
+* [`tach clean`](usage.md#tach-clean) - Delete all existing configuration and start from a clean slate.
```

### Comparing `tach-0.1.9/docs/strict-mode.md` & `tach-0.2.0/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/docs/tach_demo.mp4` & `tach-0.2.0/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/docs/usage.md` & `tach-0.2.0/docs/usage.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,81 +10,108 @@
 
 options:
   -h, --help            show this help message and exit
   -e file_or_path,..., --exclude file_or_path,...
                         Comma separated path list to exclude. tests/, ci/, etc.
 ```
 
+An error will indicate:
 
-## tach init
+- the file path in which the error was detected
+- the tags associated with that file
+- the tags associated with the attempted import
+
+Example:
+```bash
+# From the root of your Python project (in this example, `project/`)
+> tach check
+❌ utils/helpers.py[L10]: Cannot import 'core.PublicAPI'. Tags ['utils'] cannot depend on ['core'].
+```
+
+NOTE: If your terminal supports hyperlinks, you can click on the failing file path to go directly to the error.
+
+
+## tach pkg
 `tach` comes bundled with a command to set up and define your initial boundaries.
 
 ```bash
-usage: tach init [-h] [-e file_or_path,...] [-d depth]
+usage: tach pkg [-h] [-d [DEPTH]] [-e file_or_path,...]
 
-Initialize boundaries with tach
+Configure package boundaries interactively
 
 options:
   -h, --help            show this help message and exit
-  -d [depth], --depth [depth]
-                        The number of child directories to search for packages to initialize
+  -d [DEPTH], --depth [DEPTH]
+                        The number of child directories to search for packages to auto-select
   -e file_or_path,..., --exclude file_or_path,...
-                        Comma separated path list to exclude. tests,ci,...
+                        Comma separated path list to exclude. tests/, ci/, etc.
 ```
 
-By running `tach init` from the root of your Python project, `tach` will create an initial set of `package.yml` files to identify your Python packages.
-
-These initial packages will receive a single 'tag' based on their path from the project root. The packages will _not_ be in strict mode by default, but setting `strict: true` in the `package.yml` file will enable this. See ['Strict Mode'](strict-mode.md) for details.
+Running `tach pkg` will open an interactive editor in your terminal which allows you to mark your package boundaries.
 
-In addition to their tags, the `package.yml` files will contain a `depends_on` key which includes all the dependencies that `tach` was able to detect automatically for the package, which means that after running `tach init`, your project will be in a permissive, but passing state.
+You can navigate with the arrow keys, mark individual packages with `Enter`, and mark all sibling directories
+as packages with `Ctrl + a`.
 
-If `tach init` detects a only a single package in the root of your project where it's run, it will set boundaries within that package as well. Otherwise, it will simply create boundaries and dependencies for all top-level packages. You can optionally specify `-d/--depth`, which will create packages up to the specified number. 
+If you have not configured `tach` in your project before, `tach pkg` will automatically mark an initial set of packages.
+The `--depth` flag controls how many directories `tach` will traverse when suggesting these initial packages.
+You can accept these suggestions immediately with `Ctrl + s`, or you can edit the selections freely before confirming.
 
+Any time you make changes with `tach pkg`, it is recommended to run [`tach sync`](usage.md#tach-sync)
+to automatically set up dependency rules.
 
-## tach add
-`tach` also comes with a convenient command to add new packages and dependencies automatically.
-```bash 
-usage: tach add [-h] [-t tag,...] file_or_path,...
+## tach sync
+`tach` can automatically sync your project configuration (`tach.yml`) with your project's actual dependencies.
 
-Initialize boundaries between top-level modules and write dependencies to `tach.yml`
+```bash
+usage: tach sync [-h] [--prune] [-e file_or_path,...]
 
-positional arguments:
-  file_or_path,...      The path(s) of the file or directory to create a module boundary around. Use a comma-separated list for multiple.
+Sync constraints with actual dependencies in your project.
 
 options:
   -h, --help            show this help message and exit
-  -t tag,..., --tags tag,...
-                        The tag for the module to be initialized with. Use a comma-separated list for multiple.
-```
-`tach add` supports single or multiple paths:
-```bash
-tach add service.py
-tach add service.py,utils 
+  --prune               Prune all existing constraints and re-sync dependencies.
+  -e file_or_path,..., --exclude file_or_path,...
+                        Comma separated path list to exclude. tests/, ci/, etc.
 ```
-You can also optionally specify the tags you would like the new packages to have:
+
+When this command runs, `tach` will analyze the imports in your packages.
+
+Any undeclared dependencies or other dependency errors will be automatically resolved by
+adding the corresponding dependencies to your `tach.yml` file.
+
+If you supply `--prune`,
+any dependency constraints in your `tach.yml` which are not necessary will also be removed.
+
+## tach clean
+If you ever want to remove all configuration for `tach` and start over, you can use `tach clean`:
+
 ```bash
-tach add utils -t shared
-```
-`tach` will take each file or directory and turn it into a python package with a `package.yml`. It will also update your `tach.yml` and attempt to get you to a passing state.
+usage: tach clean [-h] [--force]
+
+Delete existing configuration and start from an empty slate.
 
-Note that if you have [`strict:True`](strict-mode.md) set, you may end up in a failing state due to imports that used to be within a module now crossing a package boundary.
+options:
+  -h, --help  show this help message and exit
+  --force     Do not prompt for confirmation.
+```
 
-If you have relative imports in a file that is turned into a package, they will also likely break due to the creation of the new package. Both issues should be easily solved by hand.
+This will find the nearest `tach` project in parent directories, or simply work from the current directory.
+It will remove `tach.yml` along with any `package.yml` files it finds.
 
 ## tach install
-`tach` can be installed into your development workflow automatically as a pre-commit hook. This means `tach check` will run from the root of your repo before any commit is created.
+`tach` can be installed into your development workflow automatically as a pre-commit hook.
 
 
 ### With pre-commit framework
 If you use the [pre-commit framework](https://github.com/pre-commit/pre-commit), you can add the following to your `.pre-commit-hooks.yaml`:
 
 ```yaml
 repos:
 -   repo: https://github.com/Never-Over/tach
-    rev: v0.1.9  # change this to the latest tag!
+    rev: v0.2.0  # change this to the latest tag!
     hooks:
     -   id: tach
 ```
 
 Note that you should specify the version you are using in the `rev` key.
 
 
@@ -93,8 +120,8 @@
 
 ```bash
 tach install pre-commit
 ```
 
 The command above will install `tach check` as a pre-commit hook, directly into `.git/hooks/pre-commit`.
 
-If that file already exists, you will need to manually add `tach check` to your existing `.git/hooks/pre-commit` file.
+If that file already exists, you will need to manually add `tach check` to your existing `.git/hooks/pre-commit` file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tach-0.1.9/docs/why-tach.md` & `tach-0.2.0/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/mkdocs.yml` & `tach-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/pyproject.toml` & `tach-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -23,15 +23,17 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 dependencies = [
     "pyyaml==6.0.1",
     "pydantic==2.7.1",
-    "stdlib-list==0.10.0"
+    "stdlib-list==0.10.0",
+    "rich==13.7.1",
+    "prompt-toolkit==3.0.43"
 ]
 keywords = ['python', 'module', 'package', 'guard', 'enforcement', 'boundary', 'enforcer', 'domain', 'architecture']
 
 
 [project.urls]
 Homepage = "https://github.com/never-over/tach"
 Issues = "https://github.com/never-over/tach/issues"
```

### Comparing `tach-0.1.9/tach/add.py` & `tach-0.2.0/tach/add.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from datetime import datetime
 from typing import Iterable, Optional
 
 
 from tach import filesystem as fs
-from tach.check import check
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME, PACKAGE_FILE_NAME
 from tach.errors import TachError
 from tach.filesystem import canonical
 from tach.parsing import (
     parse_project_config,
     parse_package_config,
     dump_project_config_to_yaml,
 )
+from tach.sync import sync_dependency_constraints
 
 init_content_template = """# Generated by tach on {timestamp}
 from .main import *
 """
 
 
 def build_init_content():
@@ -51,46 +51,22 @@
 
 
 def update_project_config(root: str, tags: set[str]):
     current_dir = fs.get_cwd()
     try:
         fs.chdir(root)
         project_config = parse_project_config()
-        check_errors = check(
-            root,
-            project_config=project_config,
-            exclude_paths=project_config.exclude,
+
+        sync_dependency_constraints(
+            root, project_config=project_config, filter_tags=tags
         )
-        for error in check_errors:
-            if error.is_tag_error:
-                invalid_tags = set(error.invalid_tags)
-                if error.source_tag in tags:
-                    # A package with one of the added tags caused this error and should update its dependencies
-                    project_config.add_dependencies_to_tag(
-                        error.source_tag, error.invalid_tags
-                    )
-                if invalid_tags & tags:
-                    # A package now depends on one of the added tags and should add the newly added tags
-                    # Note that we should leave pre-existing invalid tags
-                    project_config.add_dependencies_to_tag(
-                        error.source_tag, list(invalid_tags & tags)
-                    )
 
         tach_yml_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
         tach_yml_content = dump_project_config_to_yaml(project_config)
         fs.write_file(tach_yml_path, tach_yml_content)
-
-        check_errors = check(
-            root, project_config=project_config, exclude_paths=project_config.exclude
-        )
-        if check_errors:
-            return (
-                "Could not auto-detect all dependencies, "
-                "use 'tach check' to finish initialization manually."
-            )
     except Exception as e:
         fs.chdir(current_dir)
         raise e
     fs.chdir(current_dir)
 
 
 def validate_path(path: str) -> None:
```

### Comparing `tach-0.1.9/tach/check.py` & `tach-0.2.0/tach/check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,27 @@
 import os
 from dataclasses import dataclass, field
 from typing import Optional
 
 from tach import filesystem as fs
+from tach import errors
 from tach.core import PackageTrie, PackageNode, ProjectConfig
 from tach.parsing import build_package_trie, get_project_imports
 
 
 @dataclass
 class ErrorInfo:
-    location: str = ""
-    import_mod_path: str = ""
-    source_tag: str = ""
+    source_tags: list[str] = field(default_factory=list)
     invalid_tags: list[str] = field(default_factory=list)
     allowed_tags: list[str] = field(default_factory=list)
     exception_message: str = ""
 
     @property
     def is_tag_error(self) -> bool:
-        return all(
-            (self.location, self.import_mod_path, self.source_tag, self.invalid_tags)
-        )
-
-    @property
-    def message(self) -> str:
-        if self.exception_message:
-            return self.exception_message
-        if not self.is_tag_error:
-            return f"Unexpected error: ({[self.location, self.import_mod_path, self.source_tag, self.allowed_tags]})"
-        if not self.allowed_tags:
-            return (
-                f"Import '{self.import_mod_path}' with tags '{self.invalid_tags}' "
-                f"in {self.location} is blocked. "
-                f"Tag '{self.source_tag}' has no allowed dependency tags."
-            )
-        return (
-            f"Import '{self.import_mod_path}' with tags '{self.invalid_tags}' "
-            f"in {self.location} is blocked. "
-            f"Tag '{self.source_tag}' can only depend on tags '{self.allowed_tags}'."
-        )
-
-
-@dataclass
-class CheckResult:
-    ok: bool
-    error_info: Optional[ErrorInfo] = None
-
-    @classmethod
-    def success(cls) -> "CheckResult":
-        return cls(ok=True)
-
-    @classmethod
-    def fail(cls, error_info: ErrorInfo) -> "CheckResult":
-        return cls(ok=False, error_info=error_info)
+        return all((self.source_tags, self.invalid_tags))
 
 
 def is_top_level_package_import(mod_path: str, package: PackageNode) -> bool:
     return mod_path == package.full_path
 
 
 def import_matches_interface_members(mod_path: str, package: PackageNode) -> bool:
@@ -73,131 +38,138 @@
 
 def check_import(
     project_config: ProjectConfig,
     package_trie: PackageTrie,
     import_mod_path: str,
     file_mod_path: str,
     file_nearest_package: Optional[PackageNode] = None,
-) -> CheckResult:
+) -> Optional[ErrorInfo]:
     import_nearest_package = package_trie.find_nearest(import_mod_path)
     if import_nearest_package is None:
         # This shouldn't happen since we intend to filter out any external imports,
         # but we should allow external imports if they have made it here.
-        return CheckResult.success()
+        return None
 
     # Lookup file_mod_path if package not given
     if file_nearest_package is None:
         file_nearest_package = package_trie.find_nearest(file_mod_path)
     # If package not found, we should fail since the implication is that
     # an external package is importing directly from our project
     if file_nearest_package is None:
-        return CheckResult.fail(
-            error_info=ErrorInfo(
-                exception_message=f"Package containing '{file_mod_path}' not found in project."
-            )
+        return ErrorInfo(
+            exception_message=f"Package containing '{file_mod_path}' not found in project.",
         )
 
     # Imports within the same package are always allowed
     if import_nearest_package == file_nearest_package:
-        return CheckResult.success()
+        return None
 
     import_package_config = import_nearest_package.config
     if import_package_config and import_package_config.strict:
         if not is_top_level_package_import(
             import_mod_path, import_nearest_package
         ) and not import_matches_interface_members(
             import_mod_path, import_nearest_package
         ):
             # In strict mode, import must be of the package itself or one of the
             # interface members (defined in __all__)
-            return CheckResult.fail(
-                error_info=ErrorInfo(
-                    location=file_mod_path,
-                    exception_message=(
-                        f"Package '{import_nearest_package.full_path}' is in strict mode. "
-                        "Only imports from the root of this package are allowed. "
-                        f"The import '{import_mod_path}' (in '{file_mod_path}') "
-                        f"is not included in __all__."
-                    ),
-                )
+            return ErrorInfo(
+                exception_message=(
+                    f"Package '{import_nearest_package.full_path}' is in strict mode. "
+                    "Only imports from the root of this package are allowed. "
+                    f"The import '{import_mod_path}' (in '{file_mod_path}') "
+                    f"is not included in __all__."
+                ),
             )
 
     # The import must be explicitly allowed based on the tags and top-level config
     if not file_nearest_package.config or not import_nearest_package.config:
-        return CheckResult.fail(
-            error_info=ErrorInfo(
-                exception_message="Could not find config for packages."
-            )
+        return ErrorInfo(
+            exception_message="Could not find package configuration.",
         )
     file_tags = file_nearest_package.config.tags
     import_tags = import_nearest_package.config.tags
 
     for file_tag in file_tags:
         dependency_tags = project_config.dependencies_for_tag(file_tag)
         if any(
             any(dependency_tag == import_tag for dependency_tag in dependency_tags)
             for import_tag in import_tags
         ):
             # The import has at least one tag which matches at least one expected dependency
             continue
         # This means the import has no tags which the file can depend on
-        return CheckResult.fail(
-            error_info=ErrorInfo(
-                location=file_mod_path,
-                import_mod_path=import_mod_path,
-                source_tag=file_tag,
-                invalid_tags=import_tags,
-                allowed_tags=dependency_tags,
-            )
+        return ErrorInfo(
+            source_tags=file_tags,
+            invalid_tags=import_tags,
+            allowed_tags=dependency_tags,
         )
 
-    return CheckResult.success()
+    return None
+
+
+@dataclass
+class BoundaryError:
+    file_path: str
+    line_number: int
+    import_mod_path: str
+    error_info: ErrorInfo
 
 
 def check(
     root: str,
     project_config: ProjectConfig,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
-) -> list[ErrorInfo]:
+) -> list[BoundaryError]:
     if not os.path.isdir(root):
-        return [
-            ErrorInfo(exception_message=f"The path {root} is not a valid directory.")
-        ]
+        raise errors.TachSetupError(f"The path {root} is not a valid directory.")
 
     # This 'canonicalizes' the path arguments, resolving directory traversal
     root = fs.canonical(root)
-    exclude_paths = list(map(fs.canonical, exclude_paths)) if exclude_paths else None
+
+    if exclude_paths is not None and project_config.exclude is not None:
+        exclude_paths.extend(project_config.exclude)
+    else:
+        exclude_paths = project_config.exclude
 
     package_trie = build_package_trie(
         root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
     )
 
-    errors: list[ErrorInfo] = []
+    boundary_errors: list[BoundaryError] = []
     for file_path in fs.walk_pyfiles(
         root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
     ):
         mod_path = fs.file_to_module_path(file_path)
         nearest_package = package_trie.find_nearest(mod_path)
         if nearest_package is None:
             continue
-        import_mod_paths = get_project_imports(
+
+        # This should only give us imports from within our project
+        # (excluding stdlib, builtins, and 3rd party packages)
+        project_imports = get_project_imports(
             root,
             file_path,
             ignore_type_checking_imports=project_config.ignore_type_checking_imports,
         )
-        # This should only give us imports from within our project
-        # (excluding stdlib, builtins, and 3rd party packages)
-        for import_mod_path in import_mod_paths:
-            check_result = check_import(
+        for project_import in project_imports:
+            check_error = check_import(
                 project_config=project_config,
                 package_trie=package_trie,
-                import_mod_path=import_mod_path,
+                import_mod_path=project_import.mod_path,
                 file_nearest_package=nearest_package,
                 file_mod_path=mod_path,
             )
-            if check_result.ok or check_result.error_info is None:
+            if check_error is None:
                 continue
 
-            errors.append(check_result.error_info)
+            boundary_errors.append(
+                BoundaryError(
+                    file_path=file_path,
+                    import_mod_path=project_import.mod_path,
+                    line_number=project_import.line_number,
+                    error_info=check_error,
+                )
+            )
 
-    return errors
+    return boundary_errors
```

### Comparing `tach-0.1.9/tach/core/package.py` & `tach-0.2.0/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/tach/filesystem/__init__.py` & `tach-0.2.0/tach/filesystem/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from tach.filesystem.service import (
     get_cwd,
     chdir,
     canonical,
     read_file,
     write_file,
+    delete_file,
     parse_ast,
+    walk,
     walk_pyfiles,
     walk_pypackages,
     walk_configured_packages,
     file_to_module_path,
     module_to_file_path,
     is_project_import,
 )
@@ -25,15 +27,17 @@
 
 __all__ = [
     "get_cwd",
     "chdir",
     "canonical",
     "read_file",
     "write_file",
+    "delete_file",
     "parse_ast",
+    "walk",
     "walk_pyfiles",
     "walk_pypackages",
     "walk_configured_packages",
     "file_to_module_path",
     "module_to_file_path",
     "is_project_import",
     "get_project_config_path",
```

### Comparing `tach-0.1.9/tach/filesystem/install.py` & `tach-0.2.0/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/tach/filesystem/project.py` & `tach-0.2.0/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/tach/filesystem/service.py` & `tach-0.2.0/tach/filesystem/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,18 @@
     return _get_file_cache().get(_file_cache_key(path))
 
 
 def _set_cached_file(path: str, file_info: FileInfo):
     _get_file_cache()[_file_cache_key(path)] = file_info
 
 
+def _remove_cached_file(path: str):
+    _get_file_cache().pop(_file_cache_key(path), None)
+
+
 def canonical(path: str) -> str:
     cached_file = _cached_file(path)
     if cached_file and cached_file.canonical_path:
         return cached_file.canonical_path
 
     result = os.path.relpath(os.path.realpath(path), start=get_cwd())
 
@@ -104,14 +108,20 @@
     if cached_file:
         cached_file.content = content
         cached_file.ast = None
     else:
         _set_cached_file(path, FileInfo(path=path, content=content))
 
 
+def delete_file(path: str):
+    _remove_cached_file(path)
+    os.unlink(path)
+    print(f"{BCOLORS.WARNING}Deleted '{canonical(path)}'{BCOLORS.ENDC}")
+
+
 def mark_executable(path: str):
     file_path = Path(path)
     file_path.chmod(
         file_path.stat().st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH
     )
 
 
@@ -139,54 +149,78 @@
         cached_file.ast = ast_result
     else:
         _set_cached_file(path, FileInfo(path=path, content=content, ast=ast_result))
 
     return ast_result
 
 
-def walk_pyfiles(
+def walk(
     root: str,
     depth: Optional[int] = None,
+    exclude_root: bool = True,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
-) -> Generator[str, None, None]:
+) -> Generator[tuple[str, list[str]], None, None]:
     canonical_root = canonical(root)
     base_depth = 0 if canonical_root == "." else canonical_root.count(os.path.sep) + 1
-    for dirpath, _, filenames in os.walk(canonical_root):
+    for dirpath, dirnames, filenames in os.walk(canonical_root):
         dirpath = canonical(dirpath)
         dirpath_for_matching = f"{dirpath}/"
 
-        if dirpath == canonical_root:
+        if exclude_root and dirpath == canonical_root:
             continue
 
-        if exclude_hidden_paths and os.path.basename(dirpath).startswith("."):
+        if exclude_hidden_paths and (
+            os.path.basename(os.path.normpath(dirpath)).startswith(".")
+        ):
+            # This prevents recursing into child directories of hidden paths
+            del dirnames[:]
             continue
 
         if exclude_paths is not None and any(
             re.match(exclude_path, dirpath_for_matching)
             for exclude_path in exclude_paths
         ):
             # Treat excluded paths as invisible
             continue
 
         if depth:
             # Ignore anything past requested depth
             current_depth = dirpath.count(os.path.sep)
             if current_depth >= base_depth + depth:
                 continue
-        for filename in filenames:
+
+        def filter_filename(filename: str) -> bool:
             if exclude_hidden_paths and filename.startswith("."):
-                continue
+                return False
             file_path = os.path.join(dirpath, filename)
             if exclude_paths is not None and any(
                 re.match(exclude_path, file_path) for exclude_path in exclude_paths
             ):
-                continue
+                return False
+            return True
+
+        yield dirpath, list(filter(filter_filename, filenames))
+
+
+def walk_pyfiles(
+    root: str,
+    depth: Optional[int] = None,
+    exclude_paths: Optional[list[str]] = None,
+    exclude_hidden_paths: Optional[bool] = True,
+) -> Generator[str, None, None]:
+    for dirpath, filenames in walk(
+        root,
+        depth=depth,
+        exclude_paths=exclude_paths,
+        exclude_hidden_paths=exclude_hidden_paths,
+    ):
+        for filename in filenames:
             if filename.endswith(".py"):
-                yield file_path
+                yield os.path.join(dirpath, filename)
 
 
 def walk_pypackages(
     root: str,
     depth: Optional[int] = None,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
@@ -203,24 +237,24 @@
 
 
 def walk_configured_packages(
     root: str,
     depth: Optional[int] = None,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
-) -> Generator[str, None, None]:
+) -> Generator[tuple[str, str], None, None]:
     for dirpath in walk_pypackages(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
         exclude_hidden_paths=exclude_hidden_paths,
     ):
         package_yml_path = os.path.join(dirpath, "package.yml")
         if os.path.isfile(package_yml_path):
-            yield dirpath
+            yield dirpath, package_yml_path
 
 
 @lru_cache(maxsize=None)
 def file_to_module_path(file_path: str) -> str:
     # Assuming that the file_path has been 'canonicalized' and does not traverse multiple directories
     file_path = file_path.lstrip("./")
     if file_path == ".":
@@ -247,39 +281,37 @@
             return True
         # If string representation of path is not in parent directory, return False
         if str(p) not in map(str, p.parent.iterdir()):
             return False
         p = p.parent
 
 
-def module_to_file_path(
-    mod_path: str, find_package_init: bool = False
-) -> tuple[str, str]:
+def module_to_file_path(mod_path: str) -> tuple[str, str]:
     # Assumes that the mod_path is correctly formatted and refers to an actual module
     fs_path = mod_path.replace(".", os.path.sep)
 
     # mod_path may refer to a package
-    if path_exists_case_sensitive(Path(fs_path)):
-        return (
-            os.path.join(fs_path, "__init__.py") if find_package_init else fs_path
-        ), ""
+    init_file_path = Path(fs_path) / "__init__.py"
+    if path_exists_case_sensitive(init_file_path):
+        return str(init_file_path), ""
 
     # mod_path may refer to a file module
     file_path = fs_path + ".py"
     if path_exists_case_sensitive(Path(file_path)):
         return file_path, ""
 
     # mod_path may refer to a member within a file module
     last_sep_index = fs_path.rfind(os.path.sep)
     file_path = fs_path[:last_sep_index] + ".py"
     if path_exists_case_sensitive(Path(file_path)):
         member_name = fs_path[last_sep_index + 1 :]
         return file_path, member_name
 
-    init_file_path = fs_path[:last_sep_index] + "/__init__.py"
+    # mod_path may refer to a member within a package
+    init_file_path = fs_path[:last_sep_index] + os.path.sep + "__init__.py"
     if path_exists_case_sensitive(Path(init_file_path)):
         member_name = fs_path[last_sep_index + 1 :]
         return init_file_path, member_name
 
     raise errors.TachParseError(
         f"Failed to translate module path {mod_path} into file path"
     )
```

### Comparing `tach-0.1.9/tach/init.py` & `tach-0.2.0/tests/test_parsing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,104 @@
 import os
-from dataclasses import field, dataclass
-from typing import Optional
 
+import pytest
+from pydantic import ValidationError
 
-from tach import errors
-from tach import filesystem as fs
 from tach.check import check
-from tach.colors import BCOLORS
-from tach.constants import PACKAGE_FILE_NAME, CONFIG_FILE_NAME
-from tach.core import ProjectConfig
-from tach.parsing import dump_project_config_to_yaml
-
-__package_yml_template = """tags: ['{dir_name}']\n"""
-
-
-@dataclass
-class PackageInitResult:
-    package_paths: list[str] = field(default_factory=list)
-    warnings: list[str] = field(default_factory=list)
-
-
-def init_packages(
-    root: str, depth: int, exclude_paths: Optional[list[str]] = None
-) -> PackageInitResult:
-    package_paths: list[str] = []
-    warnings: list[str] = []
-    for dir_path in fs.walk_pypackages(root, depth=depth, exclude_paths=exclude_paths):
-        package_yml_path = os.path.join(dir_path, f"{PACKAGE_FILE_NAME}.yml")
-        package_paths.append(dir_path)
-        if os.path.exists(package_yml_path):
-            warnings.append(
-                f"{BCOLORS.OKCYAN}Package file '{package_yml_path}' already exists.{BCOLORS.ENDC}"
-            )
-            continue
-        package_yml_content = __package_yml_template.format(
-            dir_name=dir_path.replace(os.path.sep, ".")
+from tach.core.config import PackageConfig, TagDependencyRules, ProjectConfig
+from tach.parsing.config import parse_project_config, parse_package_config
+from tach.filesystem import file_to_module_path
+from tach import filesystem as fs
+
+
+def test_file_to_mod_path():
+    assert file_to_module_path("__init__.py") == ""
+    assert file_to_module_path("domain_one/__init__.py") == "domain_one"
+    assert file_to_module_path("domain_one/interface.py") == "domain_one.interface"
+
+
+def test_parse_valid_project_config():
+    result = parse_project_config("example/valid/")
+    assert result == ProjectConfig(
+        constraints=[
+            TagDependencyRules(tag="one", depends_on=["two"]),
+            TagDependencyRules(tag="two", depends_on=["one"]),
+            TagDependencyRules(tag="three", depends_on=[]),
+        ],
+        exclude=["domain_thr.*"],
+        exclude_hidden_paths=True,
+    )
+
+
+def test_run_valid_project_config():
+    current_dir = os.getcwd()
+    try:
+        project = "./example/valid/"
+        fs.chdir(project)
+        project_config = parse_project_config()
+        results = check(
+            ".",
+            project_config,
+            exclude_paths=project_config.exclude,
+            exclude_hidden_paths=project_config.exclude_hidden_paths,
         )
-        fs.write_file(package_yml_path, package_yml_content)
+        assert results == []
+    finally:
+        # Make sure not to dirty the test directory state
+        fs.chdir(current_dir)
 
-    return PackageInitResult(package_paths=package_paths, warnings=warnings)
 
+def test_parse_valid_strict_package_config():
+    result = parse_package_config("example/valid/domain_one")
+    assert result == PackageConfig(strict=True, tags=["one"])
 
-@dataclass
-class InitRootResult:
-    warnings: list[str] = field(default_factory=list)
 
+def test_parse_valid_multi_tag_package_config():
+    result = parse_package_config("example/valid/domain_two")
+    assert result == PackageConfig(strict=False, tags=["two", "shared"])
 
-def init_root(root: str, exclude_paths: Optional[list[str]] = None) -> InitRootResult:
-    project_config_path = fs.get_project_config_path(root)
-    if project_config_path:
-        return InitRootResult(
-            warnings=[
-                f"{BCOLORS.OKCYAN}Project already contains {CONFIG_FILE_NAME}.yml{BCOLORS.ENDC}"
-            ]
-        )
 
-    project_config = ProjectConfig()
-    check_errors = check(
-        root, project_config=project_config, exclude_paths=exclude_paths
-    )
-    for error in check_errors:
-        if error.is_tag_error:
-            project_config.add_dependencies_to_tag(error.source_tag, error.invalid_tags)
-
-    tach_yml_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
-    tach_yml_content = dump_project_config_to_yaml(project_config)
-    fs.write_file(tach_yml_path, tach_yml_content)
+def test_package_with_no_config():
+    result = parse_package_config("example/")
+    assert result is None
 
-    check_errors = check(
-        root, project_config=project_config, exclude_paths=exclude_paths
-    )
-    if check_errors:
-        return InitRootResult(
-            warnings=[
-                "Could not auto-detect all dependencies, use 'tach check' to finish initialization manually."
-            ]
-        )
 
-    return InitRootResult(warnings=[])
+def test_invalid_project_config():
+    with pytest.raises(ValidationError):
+        parse_project_config("example/invalid/")
 
 
-def init_project(
-    root: str, depth: Optional[int] = None, exclude_paths: Optional[list[str]] = None
-) -> list[str]:
-    if not os.path.isdir(root):
-        raise errors.TachSetupError(f"The path {root} is not a directory.")
-
-    if exclude_paths is None:
-        exclude_paths = ["tests/", "docs/"]
-
-    warnings: list[str] = []
-
-    if depth is None:
-        package_init_result = init_packages(root, depth=1, exclude_paths=exclude_paths)
-        warnings.extend(package_init_result.warnings)
-        if len(package_init_result.package_paths) == 1:
-            result = init_packages(
-                package_init_result.package_paths[0],
-                depth=1,
-                exclude_paths=exclude_paths,
-            )
-            warnings.extend(result.warnings)
-    else:
-        package_init_result = init_packages(
-            root, depth=depth, exclude_paths=exclude_paths
-        )
-        warnings.extend(package_init_result.warnings)
+def test_empty_project_config():
+    with pytest.raises(ValueError):
+        parse_project_config("example/invalid/empty")
+
+
+def test_invalid_package_config():
+    with pytest.raises(ValidationError):
+        parse_package_config("example/invalid")
 
-    init_root_result = init_root(root, exclude_paths=exclude_paths)
-    warnings.extend(init_root_result.warnings)
 
-    return warnings
+def test_empty_package_config():
+    with pytest.raises(ValueError):
+        parse_package_config("example/invalid")
+
+
+def test_exclude_hidden_paths_fails():
+    current_dir = os.getcwd()
+    hidden_project = "./example/invalid/hidden/"
+    fs.chdir(hidden_project)
+    try:
+        project_config = parse_project_config()
+        assert project_config.exclude_hidden_paths is False
+        results = check(
+            ".",
+            project_config,
+            exclude_hidden_paths=project_config.exclude_hidden_paths,
+        )
+        assert len(results) == 1
+        assert "strict mode" in results[0].error_info.exception_message
+
+        project_config.exclude_hidden_paths = True
+        assert check(".", project_config, exclude_hidden_paths=True) == []
+    finally:
+        # Make sure not to dirty the test directory state
+        fs.chdir(current_dir)
```

### Comparing `tach-0.1.9/tach/loading.py` & `tach-0.2.0/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/tach/parsing/config.py` & `tach-0.2.0/tach/parsing/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     # Using sort_keys=False here and depending on config.model_dump maintaining 'insertion order'
     # so that 'tag' appears before 'depends_on'
     # Instead, should provide custom yaml.Dumper & yaml.Representer or just write our own
     # Sort only constraints and dependencies alphabetically for now
     config.constraints.sort(key=lambda constr: constr.tag)
     for constr in config.constraints:
         constr.depends_on.sort()
+    config.exclude = list(set(config.exclude)) if config.exclude else []
     return yaml.dump(config.model_dump(), sort_keys=False)
 
 
 def parse_project_config(root: str = ".") -> ProjectConfig:
     file_path = fs.validate_project_config_path(root)
     with open(file_path, "r") as f:
         result = yaml.safe_load(f)
```

### Comparing `tach-0.1.9/tach/parsing/imports.py` & `tach-0.2.0/tach/parsing/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import os
 import re
 from typing import Optional
 from dataclasses import dataclass, field
 
 from tach import filesystem as fs
 
 
@@ -28,28 +29,34 @@
                     lineno=lineno + 1, modules=ignored_modules.split()
                 )
             else:
                 ignores[normal_lineno] = IgnoreDirective(lineno=lineno + 1)
     return ignores
 
 
+@dataclass
+class ProjectImport:
+    mod_path: str
+    line_number: int
+
+
 class ImportVisitor(ast.NodeVisitor):
     def __init__(
         self,
         project_root: str,
         current_mod_path: str,
         is_package: bool = False,
         ignore_directives: Optional[dict[int, IgnoreDirective]] = None,
         ignore_type_checking_imports: bool = False,
     ):
         self.project_root = project_root
         self.current_mod_path = current_mod_path
         self.is_package = is_package
         self.ignored_imports = ignore_directives or {}
-        self.imports: list[str] = []
+        self.imports: list[ProjectImport] = []
         self.ignore_type_checking_imports = ignore_type_checking_imports
 
     def _get_ignored_modules(self, lineno: int) -> Optional[list[str]]:
         # Check for ignore directive at the previous line or on the current line
         directive = self.ignored_imports.get(lineno - 1) or self.ignored_imports.get(
             lineno
         )
@@ -88,40 +95,53 @@
                 # This import is ignored by a tach-ignore directive
                 continue
 
             global_mod_path = (
                 f"{base_mod_path}.{name_node.name}" if node.module else name_node.name
             )
             if fs.is_project_import(self.project_root, global_mod_path):
-                self.imports.append(global_mod_path)
+                self.imports.append(
+                    ProjectImport(
+                        mod_path=global_mod_path,
+                        line_number=node.lineno,
+                    )
+                )
 
     def visit_Import(self, node: ast.Import):
         ignored_modules = self._get_ignored_modules(node.lineno)
         if ignored_modules is not None and len(ignored_modules) == 0:
             # Empty ignore list signifies blanket ignore of following import
             return
 
         ignored_modules = ignored_modules or []
         for alias in node.names:
             if alias.name in ignored_modules or not fs.is_project_import(
                 self.project_root, alias.name
             ):
                 continue
-            self.imports.append(alias.name)
+            self.imports.append(
+                ProjectImport(
+                    mod_path=alias.name,
+                    line_number=node.lineno,
+                )
+            )
 
 
 def get_project_imports(
     project_root: str, file_path: str, ignore_type_checking_imports: bool = False
-) -> list[str]:
+) -> list[ProjectImport]:
     file_content = fs.read_file(file_path)
     parsed_ast = fs.parse_ast(file_path)
     ignore_directives = get_ignore_directives(file_content)
     mod_path = fs.file_to_module_path(file_path)
+    is_package = (
+        file_path.endswith(os.path.sep + "__init__.py") or file_path == "__init__.py"
+    )
     import_visitor = ImportVisitor(
         project_root=project_root,
-        is_package=file_path.endswith("__init__.py"),
+        is_package=is_package,
         current_mod_path=mod_path,
         ignore_directives=ignore_directives,
         ignore_type_checking_imports=ignore_type_checking_imports,
     )
     import_visitor.visit(parsed_ast)
     return import_visitor.imports
```

### Comparing `tach-0.1.9/tach/parsing/interface.py` & `tach-0.2.0/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/tach/parsing/packages.py` & `tach-0.2.0/tach/parsing/packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def build_package_trie(
     root: str,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
 ) -> PackageTrie:
     package_trie = PackageTrie()
 
-    for dir_path in fs.walk_configured_packages(
+    for dir_path, _ in fs.walk_configured_packages(
         root,
         exclude_paths=exclude_paths,
         exclude_hidden_paths=exclude_hidden_paths,
     ):
         package_config = parse_package_config(dir_path)
         if package_config is None:
             raise ValueError(f"Could not parse package config for {dir_path}")
```

### Comparing `tach-0.1.9/tach.egg-info/PKG-INFO` & `tach-0.2.0/tach.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,31 +22,35 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: pydantic==2.7.1
 Requires-Dist: stdlib-list==0.10.0
+Requires-Dist: rich==13.7.1
+Requires-Dist: prompt-toolkit==3.0.43
 
 [![image](https://img.shields.io/pypi/v/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/l/tach.svg)](https://pypi.Python.org/pypi/tach)
 [![image](https://img.shields.io/pypi/pyversions/tach.svg)](https://pypi.Python.org/pypi/tach)
-[![image](https://github.com/Never-Over/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/Never-Over/tach/actions/workflows/ci.yml)
+[![image](https://github.com/gauge-sh/tach/actions/workflows/ci.yml/badge.svg)](https://github.com/gauge-sh/tach/actions/workflows/ci.yml)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # tach
 a Python tool to enforce modular design
 
 
-[Docs](https://never-over.github.io/tach/)
+[Docs](https://gauge-sh.github.io/tach/)
 
-[Discord](https://discord.gg/7crTTJwDv9) - come say hi!
+[Discord](https://discord.gg/DKVksRtuqS) - come say hi!
 
 
- <video loop src="https://github.com/Never-Over/tach/assets/10570340/a9d8d4df-d262-4b2b-b69a-adbc30d069aa">Tach Demo</video> 
+
+https://github.com/gauge-sh/tach/assets/10570340/2f5ed866-124e-4322-afe6-15207727ca38
+
 
 
 ## What is tach?
 `tach` allows you to define boundaries and control dependencies between your Python packages. Each package can also define its public interface.
 
 This enforces a decoupled, modular architecture, and prevents tight coupling.
 If a package tries to import from another package that is not listed as a dependency, tach will report an error.
@@ -56,30 +60,47 @@
 
 ## Installation
 ```bash
 pip install tach
 ```
 
 ## Quickstart
-`tach` comes bundled with a command to set up and define your initial boundaries.
+`tach` comes bundled with a command to interactively define your package boundaries.
+Run the following in the root of your Python project to enter the editor:
+```bash
+tach pkg
+```
+
+The interactive editor allows you to mark which directories should be treated as package boundaries.
+You can navigate with the arrow keys, mark individual packages with `Enter`, and mark all sibling directories
+as packages with `Ctrl + a`.
+
+After identifying your packages, press `Ctrl + s` to initialize the boundaries.
+Each package will receive a `package.yml` with a single tag based on the folder name,
+and a default `tach.yml` file will be created in the current working directory.
+
+If you want to sync your `tach.yml` with the actual dependencies found in your project, you can use `tach sync`:
 ```bash
-tach init
+tach sync [--prune]
 ```
-By running `tach init` from the root of your Python project, `tach` will initialize each top-level Python package. Each package will receive a `package.yml` with a single tag based on the folder name. 
-The tool will take into consideration the usages between packages, and write a matching set of dependencies to `tach.yml` in the project root.
 
-If you'd like to incrementally or individually add new packages to your `tach.yml`, you can use:
+Any dependency errors will be automatically resolved by
+adding the corresponding dependencies to your `tach.yml` file. If you supply `--prune`,
+any dependency constraints in your `tach.yml` which are not necessary will also be removed.
+
+In case you want to start over, `tach clean` lets you delete all `tach` configuration files so that you can re-initialize or configure your packages manually.
 ```bash
-tach add [file_or_path]
+tach clean
 ```
-This will create a boundary around the given file or directory, and update your `tach.yml` with the correct set of dependencies.
 
 
 ## Defining Packages
-To define a package, add a `package.yml` to the corresponding Python package. Add at least one 'tag' to identify the package:
+To define a package, add a `package.yml` to the corresponding Python package. Add at least one 'tag' to identify the package.
+
+Examples:
 ```python
 # core/package.yml
 tags: ["core"]
 ```
 ```python
 # db/package.yml
 tags: ["db"]
@@ -104,17 +125,19 @@
 ```
 With these rules in place, packages with tag `core` can import from packages with tag `db` or `utils`. Packages tagged with `db` can only import from `utils`, and packages tagged with `utils` cannot import from any other packages in the project. 
 
 `tach` will now flag any violation of these boundaries.
 ```bash
 # From the root of your Python project (in this example, `project/`)
 > tach check
-❌ ./utils/helpers.py: Import "core.PublicAPI" is blocked by boundary "core". Tag(s) ["utils"] do not have access to ["core"].
+❌ utils/helpers.py[L10]: Cannot import 'core.PublicAPI'. Tags ['utils'] cannot depend on ['core'].
 ```
 
+NOTE: If your terminal supports hyperlinks, you can click on the failing file path to go directly to the error.
+
 ## Defining Interfaces
 If you want to define a public interface for the package, import and reference each object you want exposed in the package's `__init__.py` and add its name to `__all__`:
 ```python
 # db/__init__.py
 from db.service import PublicAPI
 
 __all__ = ["PublicAPI"]
@@ -127,15 +150,15 @@
 ```
 ```python
 # The only valid import from "db"
 from db import PublicAPI 
 ```
 
 ### Pre-Commit Hook
-`tach` can be installed as a pre-commit hook. See the [docs](https://never-over.github.io/tach/usage/#tach-install) for installation instructions.
+`tach` can be installed as a pre-commit hook. See the [docs](https://gauge-sh.github.io/tach/usage/#tach-install) for installation instructions.
 
 
 ## Advanced
 `tach` supports specific exceptions. You can mark an import with the `tach-ignore` comment:
 ```python
 # tach-ignore
 from db.main import PrivateAPI
```

### Comparing `tach-0.1.9/tach.egg-info/SOURCES.txt` & `tach-0.2.0/tach.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 docs/tach-ignore.md
 docs/tach_demo.mp4
 docs/usage.md
 docs/why-tach.md
 tach/__init__.py
 tach/add.py
 tach/check.py
+tach/clean.py
 tach/cli.py
-tach/init.py
 tach/loading.py
 tach/package.yml
+tach/pkg.py
+tach/sync.py
 tach.egg-info/PKG-INFO
 tach.egg-info/SOURCES.txt
 tach.egg-info/dependency_links.txt
 tach.egg-info/entry_points.txt
 tach.egg-info/requires.txt
 tach.egg-info/top_level.txt
 tach/colors/__init__.py
@@ -45,27 +47,30 @@
 tach/filesystem/__init__.py
 tach/filesystem/install.py
 tach/filesystem/package.py
 tach/filesystem/package.yml
 tach/filesystem/project.py
 tach/filesystem/service.py
 tach/hooks/pre-commit
+tach/interactive/__init__.py
+tach/interactive/package.yml
+tach/interactive/packages.py
 tach/parsing/__init__.py
 tach/parsing/ast_visitor.py
 tach/parsing/config.py
 tach/parsing/imports.py
 tach/parsing/interface.py
 tach/parsing/package.yml
 tach/parsing/packages.py
 tests/__init__.py
 tests/test_add.py
 tests/test_check.py
 tests/test_cli.py
 tests/test_init.py
-tests/test_module_trie.py
+tests/test_package_trie.py
 tests/test_parsing.py
 tests/test_show.py
 tests/example/__init__.py
 tests/example/domain_one/__init__.py
 tests/example/domain_one/package.yml
 tests/example/domain_one/subdomain/__init__.py
 tests/example/domain_one/subdomain/package.yml
```

### Comparing `tach-0.1.9/tests/test_add.py` & `tach-0.2.0/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.9/tests/test_check.py` & `tach-0.2.0/tests/test_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         ("domain_two", "domain_two.subdomain", False),
         ("external", "domain_three", False),
     ],
 )
 def test_check_import(
     project_config, package_trie, file_mod_path, import_mod_path, expected_result
 ):
-    result = check_import(
+    check_error = check_import(
         project_config=project_config,
         package_trie=package_trie,
         file_mod_path=file_mod_path,
         import_mod_path=import_mod_path,
     )
-    assert result.ok == expected_result
+    result = check_error is None
+    assert result == expected_result
```

### Comparing `tach-0.1.9/tests/test_cli.py` & `tach-0.2.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest.mock import Mock
 import pytest
 
 from tach import cli
-from tach.check import ErrorInfo
+from tach.check import ErrorInfo, BoundaryError
 from tach.constants import CONFIG_FILE_NAME
 from tach.core import ProjectConfig, TagDependencyRules
 
 
 @pytest.fixture
 def mock_check(mocker) -> Mock:
     mock = Mock(return_value=[])  # default to a return with no errors
@@ -61,16 +61,21 @@
 
 
 def test_execute_with_error(capfd, mock_path_exists, mock_check, mock_project_config):
     # Mock an error returned from check
     location = "valid_dir/file.py"
     message = "Import valid_dir in valid_dir/file.py is blocked by boundary"
     mock_check.return_value = [
-        ErrorInfo(
-            exception_message="Import valid_dir in valid_dir/file.py is blocked by boundary",
+        BoundaryError(
+            file_path=location,
+            line_number=0,
+            import_mod_path="valid_dir",
+            error_info=ErrorInfo(
+                exception_message="Import valid_dir in valid_dir/file.py is blocked by boundary",
+            ),
         )
     ]
     with pytest.raises(SystemExit) as sys_exit:
         cli.tach_check()
     captured = capfd.readouterr()
     assert sys_exit.value.code == 1
     assert location in captured.err
```

### Comparing `tach-0.1.9/tests/test_module_trie.py` & `tach-0.2.0/tests/test_package_trie.py`

 * *Files identical despite different names*

