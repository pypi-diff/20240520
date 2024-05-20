# Comparing `tmp/TheengsGateway-1.4.0.tar.gz` & `tmp/theengsgateway-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheengsGateway-1.4.0.tar", last modified: Sun Feb 11 16:37:01 2024, max compression
+gzip compressed data, was "theengsgateway-1.5.0.tar", last modified: Mon May 20 14:24:36 2024, max compression
```

## Comparing `TheengsGateway-1.4.0.tar` & `theengsgateway-1.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.056053 TheengsGateway-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.056053 TheengsGateway-1.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.056053 TheengsGateway-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/workflows/manual_test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/.vale.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.060053 TheengsGateway-1.4.0/TheengsGateway/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25082 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/ble_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/decryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/TheengsGateway/privacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/TheengsGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-02-11 16:37:01.000000 TheengsGateway-1.4.0/TheengsGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-02-11 16:37:01.000000 TheengsGateway-1.4.0/TheengsGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 16:37:01.000000 TheengsGateway-1.4.0/TheengsGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-11 16:37:01.000000 TheengsGateway-1.4.0/TheengsGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-11 16:37:01.000000 TheengsGateway-1.4.0/TheengsGateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.060053 TheengsGateway-1.4.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/bin/TheengsGateway
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.060053 TheengsGateway-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.060053 TheengsGateway-1.4.0/docs/.vuepress/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/.vuepress/config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.060053 TheengsGateway-1.4.0/docs/.vuepress/public/
--rw-r--r--   0 runner    (1001) docker     (127)    13946 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/.vuepress/public/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/.vuepress/public/favicon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/.vuepress/public/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/.vuepress/public/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.060053 TheengsGateway-1.4.0/docs/.vuepress/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/.vuepress/styles/index.styl
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)   144050 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/img/Theengs-IRK-extraction.png
--rw-r--r--   0 runner    (1001) docker     (127)   142127 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/img/TheengsGateway_controllers.png
--rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/img/TheengsGateway_mqtt_explorer.png
--rw-r--r--   0 runner    (1001) docker     (127)    50272 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/img/logo-Theengs.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/docs/install/
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/install/install.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/docs/participate/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/participate/adding-decoders.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/participate/development.md
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/participate/support.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/docs/prerequisites/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/prerequisites/broker.md
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/prerequisites/controller.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/prerequisites/hardware.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/docs/use/
--rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/docs/use/use.md
--rw-r--r--   0 runner    (1001) docker     (127)   463115 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.052053 TheengsGateway-1.4.0/vale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.052053 TheengsGateway-1.4.0/vale/styles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.052053 TheengsGateway-1.4.0/vale/styles/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.052053 TheengsGateway-1.4.0/vale/styles/config/vocabularies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:37:01.064053 TheengsGateway-1.4.0/vale/styles/config/vocabularies/Theengs/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-11 16:36:48.000000 TheengsGateway-1.4.0/vale/styles/config/vocabularies/Theengs/accept.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.194663 theengsgateway-1.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.194663 theengsgateway-1.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.194663 theengsgateway-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/workflows/manual_test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/.vale.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.198663 theengsgateway-1.5.0/TheengsGateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/ble_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/decryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/TheengsGateway/privacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/TheengsGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-20 14:24:36.000000 theengsgateway-1.5.0/TheengsGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-20 14:24:36.000000 theengsgateway-1.5.0/TheengsGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:24:36.000000 theengsgateway-1.5.0/TheengsGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-20 14:24:36.000000 theengsgateway-1.5.0/TheengsGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 14:24:36.000000 theengsgateway-1.5.0/TheengsGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.198663 theengsgateway-1.5.0/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/bin/TheengsGateway
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.198663 theengsgateway-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.198663 theengsgateway-1.5.0/docs/.vuepress/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/.vuepress/config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.198663 theengsgateway-1.5.0/docs/.vuepress/public/
+-rw-r--r--   0 runner    (1001) docker     (127)    13946 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/.vuepress/public/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/.vuepress/public/favicon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/.vuepress/public/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/.vuepress/public/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.198663 theengsgateway-1.5.0/docs/.vuepress/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/.vuepress/styles/index.styl
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   144050 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/img/Theengs-IRK-extraction.png
+-rw-r--r--   0 runner    (1001) docker     (127)   142127 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/img/TheengsGateway_controllers.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13048 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/img/TheengsGateway_mqtt_explorer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50272 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/img/logo-Theengs.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/docs/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/install/install.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/docs/participate/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/participate/adding-decoders.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/participate/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/participate/support.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/docs/prerequisites/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/prerequisites/broker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/prerequisites/controller.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/prerequisites/hardware.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/docs/use/
+-rw-r--r--   0 runner    (1001) docker     (127)    17790 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/docs/use/use.md
+-rw-r--r--   0 runner    (1001) docker     (127)   463115 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.190663 theengsgateway-1.5.0/vale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.190663 theengsgateway-1.5.0/vale/styles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.190663 theengsgateway-1.5.0/vale/styles/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.190663 theengsgateway-1.5.0/vale/styles/config/vocabularies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:24:36.202663 theengsgateway-1.5.0/vale/styles/config/vocabularies/Theengs/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-20 14:24:26.000000 theengsgateway-1.5.0/vale/styles/config/vocabularies/Theengs/accept.txt
```

### Comparing `TheengsGateway-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `theengsgateway-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `theengsgateway-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.github/workflows/manual_test-pypi.yml` & `theengsgateway-1.5.0/.github/workflows/manual_test-pypi.yml`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.github/workflows/publish_docs.yml` & `theengsgateway-1.5.0/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.github/workflows/release.yml` & `theengsgateway-1.5.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.github/workflows/test.yml` & `theengsgateway-1.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.gitignore` & `theengsgateway-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/.pre-commit-config.yaml` & `theengsgateway-1.5.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     additional_dependencies:
     - bleak>=0.19.0
     - bluetooth-adapters>=0.15.3; python_version>="3.9"
     - bluetooth-clocks<1.0
     - bluetooth-numbers>=1.0,<2.0
     - importlib-metadata
     - paho-mqtt>=2.0.0,<3.0.0
-    - TheengsDecoder>=1.7.0
+    - TheengsDecoder>=1.7.8
```

### Comparing `TheengsGateway-1.4.0/CODE_OF_CONDUCT.md` & `theengsgateway-1.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/LICENSE` & `theengsgateway-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/PKG-INFO` & `theengsgateway-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: TheengsGateway
-Version: 1.4.0
+Version: 1.5.0
 Home-page: https://github.com/theengs/gateway
 Author: Theengs
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleak>=0.19.0
 Requires-Dist: bluetooth-adapters>=0.15.3; python_version >= "3.9"
 Requires-Dist: bluetooth-clocks<1.0
 Requires-Dist: bluetooth-numbers<2.0,>=1.0
 Requires-Dist: importlib-metadata
 Requires-Dist: paho-mqtt<3.0.0,>=2.0.0
 Requires-Dist: pycryptodomex>=3.18.0
-Requires-Dist: TheengsDecoder>=1.7.0
+Requires-Dist: TheengsDecoder>=1.7.8
 
 **Theengs Gateway** is a multi-platform, multi devices Bluetooth Low Energy (BLE) to MQTT gateway that leverages the [Theengs Decoder library](https://github.com/theengs/decoder).
 It retrieves data from a wide range of [BLE sensors](https://decoder.theengs.io/devices/devices.html), including the LYWSD03MMC, CGD1, CGP1W, H5072, H5075, H5102, TH1, TH2, CGH1, CGDK2, CGPR1, RuuviTag, WS02, WS08, TPMS, MiScale, LYWSD02, LYWSDCGQ, and MiFlora, and translates this information into a readable JSON format and pushes those to an MQTT broker.
 
 Enabling integration to Internet of Things (IoT) platforms or home automation controllers like [NodeRED](https://nodered.org/), [AWS IoT](https://aws.amazon.com/iot/), [Home Assistant](https://www.home-assistant.io/), [OpenHAB](https://www.openhab.org/), [FHEM](https://fhem.de/), [ioBroker](https://www.iobroker.net/) or [Domoticz](https://domoticz.com/).
 
 The gateway uses the Bluetooth Low Energy adapter of your Raspberry Pi, Windows, Apple desktop, laptop, or server by leveraging Python and multi-platform libraries.
```

### Comparing `TheengsGateway-1.4.0/README.md` & `theengsgateway-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/TheengsGateway/ble_gateway.py` & `theengsgateway-1.5.0/TheengsGateway/ble_gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import json
 import logging
 import platform
 import ssl
 import struct
 import sys
 from contextlib import suppress
+from dataclasses import dataclass
 from datetime import datetime
 from random import randrange
 from threading import Thread
 from time import time
 from typing import TYPE_CHECKING, Dict, Union
 
 from bleak import BleakError, BleakScanner
@@ -81,14 +82,26 @@
 }
 
 logger = logging.getLogger("BLEGateway")
 
 DataJSONType = Dict[str, Union[str, int, float, bool]]
 
 
+@dataclass
+class TnM:
+    """Keep track of a timestamp and model_id for a tracker."""
+
+    time: int
+    model_id: str
+
+    def __str__(self) -> str:
+        """Show time and model_id."""
+        return f"({self.time}, {self.model_id})"
+
+
 def get_address(data: DataJSONType) -> str:
     """Return the device address from a data JSON."""
     try:
         return data["mac"]  # type: ignore[return-value]
     except KeyError:
         return data["id"]  # type: ignore[return-value]
 
@@ -113,15 +126,15 @@
         self,
         configuration: dict,
     ) -> None:
         self.configuration = configuration
         self.stopped = False
         self.clock_updates: dict[str, float] = {}
         self.published_messages = 0
-        self.discovered_trackers: dict[str, int] = {}
+        self.discovered_trackers: dict[str, TnM] = {}
 
     def connect_mqtt(self) -> None:
         """Connect to MQTT broker."""
 
         def on_connect(
             client,  # noqa: ANN001
             userdata,  # noqa: ANN001,ARG001
@@ -136,15 +149,15 @@
                     "online",
                     qos=0,
                     retain=True,
                 )
                 self.subscribe(self.configuration["subscribe_topic"])
             else:
                 logger.error(
-                    "Failed to connect to MQTT broker %s:%d reason code: %d",
+                    "Failed to connect to MQTT broker %s:%d reason code: %s",
                     self.configuration["host"],
                     self.configuration["port"],
                     reason_code,
                 )
                 self.client.connect(
                     self.configuration["host"],
                     self.configuration["port"],
@@ -157,29 +170,31 @@
             reason_code,  # noqa: ANN001
             properties,  # noqa: ANN001,ARG001
         ) -> None:
             if reason_code == 0:
                 logger.info("Disconnected from MQTT broker")
             else:
                 logger.error(
-                    "Disconnected from MQTT broker with reason code = %d", reason_code
+                    "Disconnected from MQTT broker with reason code = %s", reason_code
                 )
 
         if self.configuration["enable_websocket"]:
             self.client = mqtt_client.Client(
                 mqtt_client.CallbackAPIVersion.VERSION2, transport="websockets"
             )
         else:
             self.client = mqtt_client.Client(mqtt_client.CallbackAPIVersion.VERSION2)
 
         if self.configuration["enable_tls"]:
             self.client.tls_set(
                 cert_reqs=ssl.CERT_REQUIRED,
                 tls_version=ssl.PROTOCOL_TLS,
             )
+            if self.configuration["tls_insecure"]:
+                self.client.tls_insecure_set(value=True)
 
         self.client.username_pw_set(
             self.configuration["user"],
             self.configuration["pass"],
         )
         self.client.will_set(
             self.configuration["lwt_topic"],
@@ -346,32 +361,42 @@
                     ).strftime("%Y-%m-%d %H:%M:%S"),
                 )
 
     def check_tracker_timeout(self) -> None:
         """Check if tracker timeout is over timeout limit."""
         # If the timestamp is later than current time minus tracker_timeout
         # Publish offline message
-        for address, timestamp in self.discovered_trackers.copy().items():
+        for address, time_model in self.discovered_trackers.copy().items():
             if (
-                round(time()) - timestamp >= self.configuration["tracker_timeout"]
-                and timestamp != 0
+                round(time()) - time_model.time >= self.configuration["tracker_timeout"]
+                and time_model.time != 0
                 and (
                     self.configuration["discovery"]
                     or self.configuration["general_presence"]
                 )
             ):
-                message = json.dumps({"id": address, "presence": "absent"})
+                if (
+                    time_model.model_id in ("APPLEWATCH", "APPLEDEVICE")
+                    and not self.configuration["discovery"]
+                ):
+                    message = json.dumps(
+                        {"id": address, "presence": "absent", "unlocked": False}
+                    )
+                else:
+                    message = json.dumps({"id": address, "presence": "absent"})
 
                 self.publish(
                     message,
                     self.configuration["publish_topic"]
                     + "/"
                     + address.replace(":", ""),
                 )
-                self.discovered_trackers[address] = 0
+                time_model.time = 0
+                self.discovered_trackers[address] = time_model
+                logger.debug("Discovered Trackers: %s", self.discovered_trackers)
 
     async def ble_scan_loop(self) -> None:
         """Scan for BLE devices."""
         scanner_kwargs = {"scanning_mode": self.configuration["scanning_mode"]}
 
         if platform.system() == "Linux":
             if self.configuration["scanning_mode"] == "passive":
@@ -432,14 +457,23 @@
     ) -> None:
         """Detect device in received advertisement data."""
         logger.debug("%s:%s", device.address, advertisement_data)
 
         # Try to resolve private addresses with known IRKs
         address = self.rpa2id(device.address)
 
+        if (
+            address not in self.configuration["whitelist"]
+            and self.configuration["whitelist"] != []
+        ) or (
+            address in self.configuration["blacklist"]
+            and address not in self.configuration["whitelist"]
+        ):
+            return
+
         # Try to add the device to dictionary of clocks to synchronize time.
         self.add_clock(address)
 
         data_json: DataJSONType = {}
 
         if advertisement_data.manufacturer_data:
             # Only look at the first manufacturer data in the advertisement
@@ -562,25 +596,28 @@
         """Publish JSON data to MQTT."""
         # publish general presence "present" if tracker and general_presence true
         if "track" in data_json:
             if (
                 data_json["id"] not in self.discovered_trackers
                 or (
                     data_json["id"] in self.discovered_trackers
-                    and self.discovered_trackers[str(data_json["id"])] == 0
+                    and self.discovered_trackers[str(data_json["id"])].time == 0
                 )
             ) and self.configuration["general_presence"]:
                 message = json.dumps({"id": data_json["id"], "presence": "present"})
                 self.publish(
                     message,
                     self.configuration["publish_topic"]
                     + "/"
                     + get_address(data_json).replace(":", ""),
                 )
-            self.discovered_trackers[str(data_json["id"])] = round(time())
+            self.discovered_trackers[str(data_json["id"])] = TnM(
+                round(time()),
+                str(data_json["model_id"]),
+            )
             logger.debug("Discovered Trackers: %s", self.discovered_trackers)
 
         # Remove "track" if PUBLISH_ADVDATA is 0
         if not self.configuration["publish_advdata"] and "track" in data_json:
             data_json.pop("track", None)
 
         message = json.dumps(data_json)
```

### Comparing `TheengsGateway-1.4.0/TheengsGateway/config.py` & `theengsgateway-1.5.0/TheengsGateway/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,21 @@
     "adapter": "",
     "scanning_mode": "active",
     "time_sync": [],
     "time_format": 0,
     "publish_advdata": 0,
     "bindkeys": {},
     "enable_tls": 0,
+    "tls_insecure": 0,
     "enable_websocket": 0,
     "identities": {},
     "tracker_timeout": 120,
     "ble": 1,
+    "whitelist": [],
+    "blacklist": [],
 }
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command-line arguments and return them."""
     parser = argparse.ArgumentParser(
         description=f"TheengsGateway {version('TheengsGateway')}",
@@ -72,14 +75,20 @@
         "-bk",
         "--bindkeys",
         nargs="+",
         metavar=("ADDRESS", "BINDKEY"),
         help="Device addresses and their bindkeys: ADDR1 KEY1 ADDR2 KEY2",
     )
     parser.add_argument(
+        "-bl",
+        "--blacklist",
+        nargs="+",
+        help="Addresses of Bluetooth devices to ignore, all other devices are allowed",
+    )
+    parser.add_argument(
         "-c",
         "--config",
         type=str,
         default=str(Path("~/theengsgw.conf").expanduser()),
         help="Path to the configuration file (default: ~/theengsgw.conf)",
     )
     parser.add_argument(
@@ -98,21 +107,21 @@
         "-Dh",
         "--hass_discovery",
         type=int,
         help="Enable(1) or disable(0) Home Assistant MQTT discovery (default: 1)",
     )
     parser.add_argument(
         "-Dn",
-        "--discovery_name",
+        "--discovery_device_name",
         type=str,
         help="Device name for Home Assistant",
     )
     parser.add_argument(
         "-Dt",
-        "--discovery-topic",
+        "--discovery_topic",
         type=str,
         help="MQTT Discovery topic",
     )
     parser.add_argument(
         "-Gp",
         "--general_presence",
         type=int,
@@ -178,50 +187,56 @@
         "-prt",
         "--presence_topic",
         type=str,
         help="MQTT presence topic",
     )
     parser.add_argument(
         "-pt",
-        "--pub_topic",
+        "--publish_topic",
         type=str,
         help="MQTT publish topic",
     )
     parser.add_argument(
         "-s",
         "--scanning_mode",
         type=str,
         choices=("active", "passive"),
         help="Scanning mode (default: active)",
     )
     parser.add_argument(
         "-sd",
-        "--scan_duration",
+        "--ble_scan_time",
         type=int,
         help="BLE scan duration (seconds)",
     )
     parser.add_argument(
         "-st",
-        "--sub_topic",
+        "--subscribe_topic",
         type=str,
         help="MQTT subscribe topic",
     )
     parser.add_argument(
         "-tb",
-        "--time_between",
-        type=int,
+        "--ble_time_between_scans",
+        type=float,
         help="Seconds to wait between scans",
     )
     parser.add_argument(
         "-tf",
         "--time_format",
         type=int,
         help="Use 12-hour (1) or 24-hour (0) time format for clocks (default: 0)",
     )
     parser.add_argument(
+        "-ti",
+        "--tls_insecure",
+        type=int,
+        help="Allow (1) or disallow (0: default) insecure TLS (no hostname check)",
+    )
+    parser.add_argument(
         "-tls",
         "--enable_tls",
         type=int,
         help="Enable (1) or disable (0) TLS (default: 0)",
     )
     parser.add_argument(
         "-to",
@@ -238,14 +253,20 @@
     parser.add_argument(
         "-u",
         "--user",
         type=str,
         help="MQTT username",
     )
     parser.add_argument(
+        "-wl",
+        "--whitelist",
+        nargs="+",
+        help="Addresses of Bluetooth devices to allow, all other devices are ignored",
+    )
+    parser.add_argument(
         "-ws",
         "--enable_websocket",
         type=int,
         help="Enable (1) or disable (0) WebSocket (default: 0)",
     )
     return parser.parse_args()
```

### Comparing `TheengsGateway-1.4.0/TheengsGateway/decryption.py` & `theengsgateway-1.5.0/TheengsGateway/decryption.py`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/TheengsGateway/diagnose.py` & `theengsgateway-1.5.0/TheengsGateway/diagnose.py`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/TheengsGateway/discovery.py` & `theengsgateway-1.5.0/TheengsGateway/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import json
 import re
 from time import time
 
 from TheengsDecoder import getProperties
 
-from .ble_gateway import DataJSONType, Gateway, logger
+from .ble_gateway import DataJSONType, Gateway, TnM, logger
 
 ha_dev_classes = [
     "battery",
     "carbon_dioxide",
     "carbon_monoxide",
     "current",
     "data_size",
@@ -43,27 +43,32 @@
     "gas",
     "humidity",
     "illuminance",
     "irradiance",
     "lock",
     "motion",
     "moving",
+    "pm1",
     "pm10",
     "pm25",
     "power",
     "power_factor",
+    "precipitation",
+    "precipitation_intensity",
     "pressure",
     "problem",
     "restart",
     "signal_strength",
+    "sound_pressure",
     "temperature",
     "timestamp",
     "voltage",
     "water",
     "weight",
+    "wind_speed",
     "window",
 ]
 
 ha_dev_units = [
     "W",
     "kW",
     "V",
@@ -260,15 +265,17 @@
 
             self.publish(json.dumps(tracker), config_topic, retain=True)
 
     def copy_pub_device(self, device: dict) -> dict:
         """Copy pub_device and remove "track" if publish_advdata is false."""
         # Update tracker last received time
         if "track" in device:
-            self.discovered_trackers[device["id"]] = round(time())
+            self.discovered_trackers[device["id"]] = TnM(
+                round(time()), device["model_id"]
+            )
             logger.debug("Discovered Trackers: %s", self.discovered_trackers)
 
         pub_device_copy = device.copy()
         # Remove "track" if PUBLISH_ADVDATA is 0
         if not self.configuration["publish_advdata"] and "track" in pub_device_copy:
             pub_device_copy.pop("track", None)
```

### Comparing `TheengsGateway-1.4.0/TheengsGateway/privacy.py` & `theengsgateway-1.5.0/TheengsGateway/privacy.py`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/TheengsGateway.egg-info/PKG-INFO` & `theengsgateway-1.5.0/TheengsGateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: TheengsGateway
-Version: 1.4.0
+Version: 1.5.0
 Home-page: https://github.com/theengs/gateway
 Author: Theengs
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleak>=0.19.0
 Requires-Dist: bluetooth-adapters>=0.15.3; python_version >= "3.9"
 Requires-Dist: bluetooth-clocks<1.0
 Requires-Dist: bluetooth-numbers<2.0,>=1.0
 Requires-Dist: importlib-metadata
 Requires-Dist: paho-mqtt<3.0.0,>=2.0.0
 Requires-Dist: pycryptodomex>=3.18.0
-Requires-Dist: TheengsDecoder>=1.7.0
+Requires-Dist: TheengsDecoder>=1.7.8
 
 **Theengs Gateway** is a multi-platform, multi devices Bluetooth Low Energy (BLE) to MQTT gateway that leverages the [Theengs Decoder library](https://github.com/theengs/decoder).
 It retrieves data from a wide range of [BLE sensors](https://decoder.theengs.io/devices/devices.html), including the LYWSD03MMC, CGD1, CGP1W, H5072, H5075, H5102, TH1, TH2, CGH1, CGDK2, CGPR1, RuuviTag, WS02, WS08, TPMS, MiScale, LYWSD02, LYWSDCGQ, and MiFlora, and translates this information into a readable JSON format and pushes those to an MQTT broker.
 
 Enabling integration to Internet of Things (IoT) platforms or home automation controllers like [NodeRED](https://nodered.org/), [AWS IoT](https://aws.amazon.com/iot/), [Home Assistant](https://www.home-assistant.io/), [OpenHAB](https://www.openhab.org/), [FHEM](https://fhem.de/), [ioBroker](https://www.iobroker.net/) or [Domoticz](https://domoticz.com/).
 
 The gateway uses the Bluetooth Low Energy adapter of your Raspberry Pi, Windows, Apple desktop, laptop, or server by leveraging Python and multi-platform libraries.
```

### Comparing `TheengsGateway-1.4.0/TheengsGateway.egg-info/SOURCES.txt` & `theengsgateway-1.5.0/TheengsGateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/.vuepress/config.js` & `theengsgateway-1.5.0/docs/.vuepress/config.js`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/.vuepress/public/apple-touch-icon.png` & `theengsgateway-1.5.0/docs/.vuepress/public/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/.vuepress/public/favicon-144x144.png` & `theengsgateway-1.5.0/docs/.vuepress/public/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/.vuepress/public/favicon-16x16.png` & `theengsgateway-1.5.0/docs/.vuepress/public/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/.vuepress/public/favicon-32x32.png` & `theengsgateway-1.5.0/docs/.vuepress/public/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/README.md` & `theengsgateway-1.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/img/Theengs-IRK-extraction.png` & `theengsgateway-1.5.0/docs/img/Theengs-IRK-extraction.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/img/TheengsGateway_controllers.png` & `theengsgateway-1.5.0/docs/img/TheengsGateway_controllers.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/img/TheengsGateway_mqtt_explorer.png` & `theengsgateway-1.5.0/docs/img/TheengsGateway_mqtt_explorer.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/img/logo-Theengs.png` & `theengsgateway-1.5.0/docs/img/logo-Theengs.png`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/install/install.md` & `theengsgateway-1.5.0/docs/install/install.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/participate/development.md` & `theengsgateway-1.5.0/docs/participate/development.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/participate/support.md` & `theengsgateway-1.5.0/docs/participate/support.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/prerequisites/broker.md` & `theengsgateway-1.5.0/docs/prerequisites/broker.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/prerequisites/controller.md` & `theengsgateway-1.5.0/docs/prerequisites/controller.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/prerequisites/hardware.md` & `theengsgateway-1.5.0/docs/prerequisites/hardware.md`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/docs/use/use.md` & `theengsgateway-1.5.0/docs/use/use.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,46 +89,50 @@
 
 ## Details options
 ### For a regular installation
 
 ```shell
 C:\Users\1technophile>python -m TheengsGateway -h
 usage: TheengsGateway [-h] [-a ADAPTER] [-b BLE] [-bk ADDRESS [BINDKEY ...]]
+                      [-bl ADDRESS [ADDRESS ...]]
                       [-c CONFIG] [-D DISCOVERY]
                       [-Df DISCOVERY_FILTER [DISCOVERY_FILTER ...]]
-                      [-Dh HASS_DISCOVERY] [-Dn DISCOVERY_NAME]
+                      [-Dh HASS_DISCOVERY] [-Dn DISCOVERY_DEVICE_NAME]
                       [-Dt DISCOVERY_TOPIC] [-Gp GENERAL_PRESENCE] [-H HOST] 
                       [-id ADDRESS [IRK ...]]
                       [-Lt LWT_TOPIC] [-ll {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
                       [-P PORT] [-p PASS] [-pa PUBLISH_ALL] [-padv PUBLISH_ADVDATA]
-                      [-pr PRESENCE] [-prt PRESENCE_TOPIC] [-pt PUB_TOPIC]
-                      [-s {active,passive}] [-sd SCAN_DURATION] [-st SUB_TOPIC]
-                      [-tb TIME_BETWEEN] [-tf TIME_FORMAT] [-tls ENABLE_TLS]
-                      [-ts TIME_SYNC [TIME_SYNC ...]] [-u USER]
+                      [-pr PRESENCE] [-prt PRESENCE_TOPIC] [-pt PUBLISH_TOPIC]
+                      [-s {active,passive}] [-sd BLE_SCAN_TIME] [-st SUBSCRIBE_TOPIC]
+                      [-tb BLE_TIME_BETWEEN_SCANS] [-tf TIME_FORMAT] [-ti TLS_INSECURE]
+                      [-tls ENABLE_TLS] [-ts TIME_SYNC [TIME_SYNC ...]] [-u USER]
+                      [-wl ADDRESS [ADDRESS ...]]
                       [-ws ENABLE_WEBSOCKET]
 
 options:
   -h, --help            show this help message and exit
   -a ADAPTER, --adapter ADAPTER
                         Bluetooth adapter (e.g. hci1 on Linux)
   -b BLE, --ble BLE     Enable (1) or disable (0) BLE (default: 1)
   -bk ADDRESS [BINDKEY ...], --bindkeys ADDRESS [BINDKEY ...]
                         Device addresses and their bindkeys: ADDR1 KEY1 ADDR2 KEY2
+  -bl ADDRESS [ADDRESS ...], --blacklist ADDRESS [ADDRESS ...]
+                        Addresses of Bluetooth devices to ignore, all other devices are allowed
   -c CONFIG, --config CONFIG
                         Path to the configuration file (default: ~/theengsgw.conf)
   -D DISCOVERY, --discovery DISCOVERY
                         Enable(1) or disable(0) MQTT discovery
   -Df DISCOVERY_FILTER [DISCOVERY_FILTER ...], --discovery_filter DISCOVERY_FILTER [DISCOVERY_FILTER ...]
                         Device discovery filter list for Home Assistant
   -Dh HASS_DISCOVERY, --hass_discovery HASS_DISCOVERY
                         Enable(1) or disable(0) Home Assistant MQTT discovery
                         (default: 1)
-  -Dn DISCOVERY_NAME, --discovery_name DISCOVERY_NAME
+  -Dn DISCOVERY_DEVICE_NAME, --discovery_device_name DISCOVERY_DEVICE_NAME
                         Device name for Home Assistant
-  -Dt DISCOVERY_TOPIC, --discovery-topic DISCOVERY_TOPIC
+  -Dt DISCOVERY_TOPIC, --discovery_topic DISCOVERY_TOPIC
                         MQTT Discovery topic
   -Gp GENERAL_PRESENCE, --general_presence GENERAL_PRESENCE
                         Enable (1) or disable (0) general present/absent presence when --discovery: 0
   -H HOST, --host HOST  MQTT host address
   -id ADDRESS [IRK ...], --identities ADDRESS [IRK ...]
                         Identity addresses and their IRKs: ADDR1 IRK1 ADDR2 IRK2
   -Lt LWT_TOPIC, --lwt_topic LWT_TOPIC
@@ -143,51 +147,55 @@
   -padv PUBLISH_ADVDATA, --publish_advdata PUBLISH_ADVDATA
                         Publish advertising and advanced data (1) or not (0)
                         (default: 0)
   -pr PRESENCE, --presence PRESENCE
                         Enable (1) or disable (0) presence publication (default: 1)
   -prt PRESENCE_TOPIC, --presence_topic PRESENCE_TOPIC
                         MQTT presence topic
-  -pt PUB_TOPIC, --pub_topic PUB_TOPIC
+  -pt PUBLISH_TOPIC, --publish_topic PUBLISH_TOPIC
                         MQTT publish topic
   -s {active,passive}, --scanning_mode {active,passive}
                         Scanning mode (default: active)
-  -sd SCAN_DURATION, --scan_duration SCAN_DURATION
+  -sd BLE_SCAN_TIME, --ble_scan_time BLE_SCAN_TIME
                         BLE scan duration (seconds)
-  -st SUB_TOPIC, --sub_topic SUB_TOPIC
+  -st SUBSCRIBE_TOPIC, --subscribe_topic SUBSCRIBE_TOPIC
                         MQTT subscribe topic
-  -tb TIME_BETWEEN, --time_between TIME_BETWEEN
+  -tb BLE_TIME_BETWEEN_SCANS, --ble_time_between_scans BLE_TIME_BETWEEN_SCANS
                         Seconds to wait between scans
   -tf TIME_FORMAT, --time_format TIME_FORMAT
                         Use 12-hour (1) or 24-hour (0) time format for clocks
                         (default: 0)
+  -ti TLS_INSECURE, --tls_insecure TLS_INSECURE
+                        Allow (1) or disallow (0: default) insecure TLS (no hostname check)
   -tls ENABLE_TLS, --enable_tls ENABLE_TLS
                         Enable (1) or disable (0) TLS (default: 0)
   -ts TIME_SYNC [TIME_SYNC ...], --time_sync TIME_SYNC [TIME_SYNC ...]
                         Addresses of Bluetooth devices to synchronize the time
   -to TIME_UNTIL, --tracker_timeout TIME_UNTIL
                         Seconds after which a discovered device tracker not being received is published as offline/away
                         (default: 120)
   -u USER, --user USER  MQTT username
+  -wl ADDRESS [ADDRESS ...], --whitelist ADDRESS [ADDRESS ...]
+                        Addresses of Bluetooth devices to allow, all other devices are ignored
   -ws ENABLE_WEBSOCKET, --enable_websocket ENABLE_WEBSOCKET
                         Enable (1) or disable (0) WebSocket (default: 0)
 ```
 
 ### For a Docker container
 
 ```shell
 docker run --rm \
     --network host \
     -e MQTT_HOST=<host_ip> \
     -e MQTT_USERNAME=<username> \
     -e MQTT_PASSWORD=<password> \
-    -e MQTT_PUB_TOPIC=home/TheengsGateway/BTtoMQTT \
-    -e MQTT_SUB_TOPIC=home/+/BTtoMQTT/undecoded \
+    -e MQTT_PUBLISH_TOPIC=home/TheengsGateway/BTtoMQTT \
+    -e MQTT_SUBSCRIBE_TOPIC=home/+/BTtoMQTT/undecoded \
     -e PUBLISH_ALL=true \
-    -e TIME_BETWEEN=60 \
+    -e BLE_TIME_BETWEEN_SCANS=60 \
     -e SCAN_TIME=60 \
     -e LOG_LEVEL=INFO \
     -e HAAS_DISCOVERY=true \
     -e GENERAL_PRESENCE=false \
     -e DISCOVERY=true \
     -e DISCOVERY_TOPIC=homeassistant \
     -e DISCOVERY_DEVICE_NAME=TheengsGateway \
@@ -242,30 +250,30 @@
 :::
 
 ## Home Assistant auto discovery
 If enabled (default), decoded devices publish their configuration to Home Assistant so the latter can discover them.
 - You can enable/disable this with the `-D` or `--discovery` command line argument with a value of 1 (enable) or 0 (disable).
 - If you want to use Home Assistant discovery with other home automation gateways such as openHAB, set `-Dh` or `--hass_discovery` to 0 (disable).
 - You can set the discovery topic with the `-Dt` or `--discovery_topic` command line argument.
-- You can set the discovery name with the `-Dn` or `--discovery_name` command line argument.
+- You can set the discovery name with the `-Dn` or `--discovery_device_name` command line argument.
 - You can filter devices from discovery with the `-Df` or `--discovery_filter` argument which takes a list of device model ID to filter.
 
 <!-- vale Google.Acronyms = NO -->
 
 The `IBEACON` and random MAC devices (`APPLE`*, `MS-CDP` and `GAEN`) aren't discovered as their addresses (IDs) change over time resulting in multiple discoveries.
 
 :::tip * INFO
 Home Assistant discovers an Apple Watch, iPhone, or iPad if you've configured their Identity MAC address and IRK.
 :::
 
 <!-- vale Google.Acronyms = YES -->
 
 ## Discovered device tracker timeout
 :::tip  NOTE
-`-to TIME_UNTIL, --tracker_timeout` needs to be at least longer than TIME_BETWEEN + SCAN_DURATION to avoid any unwanted temporary offline status messages for discovered trackers.
+`-to TIME_UNTIL, --tracker_timeout` needs to be at least longer than BLE_TIME_BETWEEN_SCANS + BLE_SCAN_TIME to avoid any unwanted temporary offline status messages for discovered trackers.
 :::
 
 ## Passive scanning
 Passive scanning (`-s passive` or `--scanning_mode passive`) only works on Windows or Linux kernel >= 5.10 and BlueZ >= 5.56 with experimental features enabled.
 
 To enable experimental features in BlueZ on a Linux distribution that uses `systemd`, run the following command:
```

### Comparing `TheengsGateway-1.4.0/package-lock.json` & `theengsgateway-1.5.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `TheengsGateway-1.4.0/setup.py` & `theengsgateway-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,12 @@
         "bleak>=0.19.0",
         'bluetooth-adapters>=0.15.3; python_version>="3.9"',
         "bluetooth-clocks<1.0",
         "bluetooth-numbers>=1.0,<2.0",
         "importlib-metadata",
         "paho-mqtt>=2.0.0,<3.0.0",
         "pycryptodomex>=3.18.0",
-        "TheengsDecoder>=1.7.0",
+        "TheengsDecoder>=1.7.8",
     ],
     use_scm_version={"version_scheme": "no-guess-dev"},
     setup_requires=["setuptools_scm"],
 )
```

