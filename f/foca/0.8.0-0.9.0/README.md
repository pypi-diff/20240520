# Comparing `tmp/foca-0.8.0.tar.gz` & `tmp/foca-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foca-0.8.0.tar", last modified: Wed Apr  6 15:13:02 2022, max compression
+gzip compressed data, was "dist/foca-0.9.0.tar", last modified: Sat Jun 25 16:21:38 2022, max compression
```

## Comparing `foca-0.8.0.tar` & `foca-0.9.0.tar`

### file list

```diff
@@ -1,118 +1,122 @@
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    11348 2021-04-21 07:42:32.000000 foca-0.8.0/LICENSE
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      226 2021-04-21 07:42:32.000000 foca-0.8.0/MANIFEST.in
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    25525 2022-04-06 15:13:02.000000 foca-0.8.0/PKG-INFO
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1095 2021-04-21 07:42:32.000000 foca-0.8.0/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    19796 2022-04-06 15:10:41.000000 foca-0.8.0/README.md
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/docker/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1382 2021-08-24 15:04:28.000000 foca-0.8.0/docker/Dockerfile_py3.6
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1382 2021-08-24 15:04:28.000000 foca-0.8.0/docker/Dockerfile_py3.7
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1381 2021-08-24 15:04:28.000000 foca-0.8.0/docker/Dockerfile_py3.8
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1381 2021-08-24 15:04:28.000000 foca-0.8.0/docker/Dockerfile_py3.9
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/docs/
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/docs/api/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2459 2021-04-21 07:42:32.000000 foca-0.8.0/docs/api/conf.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      420 2021-04-21 07:42:32.000000 foca-0.8.0/docs/api/index.rst
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/examples/
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/examples/petstore/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      551 2021-08-24 15:04:28.000000 foca-0.8.0/examples/petstore/Dockerfile
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     5304 2021-08-24 15:04:28.000000 foca-0.8.0/examples/petstore/README.md
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      122 2021-08-24 15:04:28.000000 foca-0.8.0/examples/petstore/app.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      950 2021-08-24 15:04:28.000000 foca-0.8.0/examples/petstore/config.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2471 2021-08-24 15:04:28.000000 foca-0.8.0/examples/petstore/controllers.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      397 2021-08-24 15:04:28.000000 foca-0.8.0/examples/petstore/docker-compose.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3925 2021-04-21 07:42:32.000000 foca-0.8.0/examples/petstore/petstore.yaml
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       48 2022-04-06 15:10:41.000000 foca-0.8.0/foca/__init__.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/api/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/api/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4090 2021-08-24 15:04:28.000000 foca-0.8.0/foca/api/register_openapi.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/config/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/config/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3113 2021-08-24 15:04:28.000000 foca-0.8.0/foca/config/config_parser.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/database/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/database/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3429 2021-08-24 15:04:28.000000 foca-0.8.0/foca/database/register_mongodb.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/errors/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/errors/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     6648 2021-08-24 15:04:28.000000 foca-0.8.0/foca/errors/exceptions.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/factories/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/factories/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1500 2021-08-24 15:04:28.000000 foca-0.8.0/foca/factories/celery_app.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1896 2021-08-24 15:04:28.000000 foca-0.8.0/foca/factories/connexion_app.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2407 2022-04-06 15:10:41.000000 foca-0.8.0/foca/foca.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/models/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/models/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    49147 2021-08-24 15:04:28.000000 foca-0.8.0/foca/models/config.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/security/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.8.0/foca/security/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    11598 2021-08-24 15:04:28.000000 foca-0.8.0/foca/security/auth.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      436 2021-08-24 15:04:28.000000 foca-0.8.0/foca/security/cors.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca/utils/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-08-24 15:04:28.000000 foca-0.8.0/foca/utils/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1143 2021-08-24 15:04:28.000000 foca-0.8.0/foca/utils/db.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2152 2021-08-24 15:04:28.000000 foca-0.8.0/foca/utils/logging.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1313 2021-08-24 15:04:28.000000 foca-0.8.0/foca/utils/misc.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/foca.egg-info/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    25525 2022-04-06 15:13:02.000000 foca-0.8.0/foca.egg-info/PKG-INFO
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2527 2022-04-06 15:13:02.000000 foca-0.8.0/foca.egg-info/SOURCES.txt
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        1 2022-04-06 15:13:02.000000 foca-0.8.0/foca.egg-info/dependency_links.txt
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      263 2022-04-06 15:13:02.000000 foca-0.8.0/foca.egg-info/requires.txt
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        5 2022-04-06 15:13:02.000000 foca-0.8.0/foca.egg-info/top_level.txt
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/images/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     9410 2021-08-24 15:04:28.000000 foca-0.8.0/images/hint.svg
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     9469 2021-08-24 15:04:28.000000 foca-0.8.0/images/hint.svg.2021_02_16_09_54_34.0.svg
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     7549 2021-08-24 15:04:28.000000 foca-0.8.0/images/logo-banner.svg
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      263 2022-04-06 15:10:41.000000 foca-0.8.0/requirements.txt
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      108 2022-04-06 15:10:41.000000 foca-0.8.0/requirements_dev.txt
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      409 2022-04-06 15:13:02.000000 foca-0.8.0/setup.cfg
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2210 2022-04-06 15:10:41.000000 foca-0.8.0/setup.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/templates/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2823 2021-08-24 15:04:28.000000 foca-0.8.0/templates/config.yaml
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/api/
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/api/controllers/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      203 2021-08-24 15:04:28.000000 foca-0.8.0/tests/api/controllers/__init__.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     7296 2021-08-24 15:04:28.000000 foca-0.8.0/tests/api/test_register_openapi.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/config/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1831 2021-08-24 15:04:28.000000 foca-0.8.0/tests/config/test_config_parser.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/database/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3188 2021-08-24 15:04:28.000000 foca-0.8.0/tests/database/test_register_mongodb.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/errors/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4435 2021-08-24 15:04:28.000000 foca-0.8.0/tests/errors/test_errors.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/factories/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      532 2021-04-21 07:42:32.000000 foca-0.8.0/tests/factories/test_celery_app.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1051 2021-04-21 07:42:32.000000 foca-0.8.0/tests/factories/test_connexion_app.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1305 2021-08-24 15:04:28.000000 foca-0.8.0/tests/integration_tests.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/models/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    11274 2021-08-24 15:04:28.000000 foca-0.8.0/tests/models/test_config.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/security/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    15396 2021-08-24 15:04:28.000000 foca-0.8.0/tests/security/test_auth.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      366 2021-04-21 07:42:32.000000 foca-0.8.0/tests/security/test_cors.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/test_files/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      571 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_api.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      145 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_db.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      101 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_invalid_jobs.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1537 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_invalid_log_level.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       96 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_jobs.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      438 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_log.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      435 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/conf_log_invalid.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1451 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/conf_valid.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      329 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/conf_valid_cors_disabled.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      328 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/conf_valid_cors_enabled.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      427 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/empty_conf.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3144 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/invalid.json
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      667 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/invalid.openapi.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      427 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/invalid_conf.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       63 2021-04-21 07:42:32.000000 foca-0.8.0/tests/test_files/invalid_conf_db.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      699 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/openapi_2_petstore.addition.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2280 2022-04-05 14:24:24.000000 foca-0.8.0/tests/test_files/openapi_2_petstore.modified.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1739 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/openapi_2_petstore.original.json
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2416 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/openapi_2_petstore.original.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2666 2022-04-05 14:24:24.000000 foca-0.8.0/tests/test_files/openapi_3_petstore.modified.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2781 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_files/openapi_3_petstore.original.yaml
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3719 2021-08-24 15:04:28.000000 foca-0.8.0/tests/test_foca.py
-drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-04-06 15:13:02.000000 foca-0.8.0/tests/utils/
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1341 2021-08-24 15:04:28.000000 foca-0.8.0/tests/utils/test_db.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1818 2021-08-24 15:04:28.000000 foca-0.8.0/tests/utils/test_logging.py
--rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2279 2021-08-24 15:04:28.000000 foca-0.8.0/tests/utils/test_misc.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    11348 2021-04-21 07:42:32.000000 foca-0.9.0/LICENSE
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      226 2021-04-21 07:42:32.000000 foca-0.9.0/MANIFEST.in
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    27634 2022-06-25 16:21:38.000000 foca-0.9.0/PKG-INFO
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1182 2022-06-25 14:07:03.000000 foca-0.9.0/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    21496 2022-06-25 14:07:03.000000 foca-0.9.0/README.md
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/docker/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1405 2022-06-25 10:22:14.000000 foca-0.9.0/docker/Dockerfile
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/docs/
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/docs/api/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2481 2022-06-25 16:19:50.000000 foca-0.9.0/docs/api/conf.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      420 2021-04-21 07:42:32.000000 foca-0.9.0/docs/api/index.rst
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/examples/
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/examples/petstore/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      553 2022-06-25 15:54:40.000000 foca-0.9.0/examples/petstore/Dockerfile
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     5996 2022-06-25 15:54:40.000000 foca-0.9.0/examples/petstore/README.md
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      194 2022-06-25 12:06:20.000000 foca-0.9.0/examples/petstore/app.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1074 2022-06-25 15:54:40.000000 foca-0.9.0/examples/petstore/config.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1842 2022-06-25 15:54:40.000000 foca-0.9.0/examples/petstore/controllers.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      397 2022-06-25 15:54:40.000000 foca-0.9.0/examples/petstore/docker-compose.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      580 2022-06-25 15:54:40.000000 foca-0.9.0/examples/petstore/exceptions.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3925 2021-04-21 07:42:32.000000 foca-0.9.0/examples/petstore/petstore.yaml
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       90 2022-06-25 16:19:50.000000 foca-0.9.0/foca/__init__.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/api/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/api/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4090 2022-06-25 15:03:33.000000 foca-0.9.0/foca/api/register_openapi.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/config/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/config/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     6839 2022-06-25 16:19:50.000000 foca-0.9.0/foca/config/config_parser.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/database/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/database/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3429 2022-06-25 14:48:14.000000 foca-0.9.0/foca/database/register_mongodb.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/errors/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/errors/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     6645 2022-06-25 10:47:12.000000 foca-0.9.0/foca/errors/exceptions.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/factories/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/factories/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1502 2022-06-25 10:47:12.000000 foca-0.9.0/foca/factories/celery_app.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1904 2022-06-25 10:47:12.000000 foca-0.9.0/foca/factories/connexion_app.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     5036 2022-06-25 16:19:50.000000 foca-0.9.0/foca/foca.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/models/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/models/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    49188 2022-06-25 16:19:50.000000 foca-0.9.0/foca/models/config.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/security/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-04-21 07:42:32.000000 foca-0.9.0/foca/security/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    11617 2022-06-25 10:47:12.000000 foca-0.9.0/foca/security/auth.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      436 2021-08-24 15:04:28.000000 foca-0.9.0/foca/security/cors.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca/utils/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2021-08-24 15:04:28.000000 foca-0.9.0/foca/utils/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1143 2021-08-24 15:04:28.000000 foca-0.9.0/foca/utils/db.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2152 2021-08-24 15:04:28.000000 foca-0.9.0/foca/utils/logging.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1313 2021-08-24 15:04:28.000000 foca-0.9.0/foca/utils/misc.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/foca.egg-info/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    27634 2022-06-25 16:21:37.000000 foca-0.9.0/foca.egg-info/PKG-INFO
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2678 2022-06-25 16:21:37.000000 foca-0.9.0/foca.egg-info/SOURCES.txt
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        1 2022-06-25 16:21:37.000000 foca-0.9.0/foca.egg-info/dependency_links.txt
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      263 2022-06-25 16:21:37.000000 foca-0.9.0/foca.egg-info/requires.txt
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       11 2022-06-25 16:21:37.000000 foca-0.9.0/foca.egg-info/top_level.txt
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/images/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     9410 2021-08-24 15:04:28.000000 foca-0.9.0/images/hint.svg
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     9469 2021-08-24 15:04:28.000000 foca-0.9.0/images/hint.svg.2021_02_16_09_54_34.0.svg
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     7549 2021-08-24 15:04:28.000000 foca-0.9.0/images/logo-banner.svg
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      263 2022-06-21 12:40:22.000000 foca-0.9.0/requirements.txt
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      108 2022-06-21 12:40:12.000000 foca-0.9.0/requirements_dev.txt
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      454 2022-06-25 16:21:38.000000 foca-0.9.0/setup.cfg
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2091 2022-06-25 16:19:50.000000 foca-0.9.0/setup.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/templates/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3059 2022-06-25 12:06:20.000000 foca-0.9.0/templates/config.yaml
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-23 08:30:30.000000 foca-0.9.0/tests/__init__.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/api/
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/api/controllers/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      203 2021-08-24 15:04:28.000000 foca-0.9.0/tests/api/controllers/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     7259 2022-06-25 16:19:50.000000 foca-0.9.0/tests/api/test_register_openapi.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/config/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4391 2022-06-23 08:30:30.000000 foca-0.9.0/tests/config/test_config_parser.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/database/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3188 2021-08-24 15:04:28.000000 foca-0.9.0/tests/database/test_register_mongodb.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/errors/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4455 2022-06-25 10:47:12.000000 foca-0.9.0/tests/errors/test_errors.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/factories/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      529 2022-06-25 10:47:12.000000 foca-0.9.0/tests/factories/test_celery_app.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1048 2022-06-25 10:47:12.000000 foca-0.9.0/tests/factories/test_connexion_app.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4548 2022-06-25 15:54:40.000000 foca-0.9.0/tests/integration_tests.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/models/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    11289 2022-06-25 16:19:50.000000 foca-0.9.0/tests/models/test_config.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/security/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)    15459 2022-06-25 10:47:12.000000 foca-0.9.0/tests/security/test_auth.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      366 2021-04-21 07:42:32.000000 foca-0.9.0/tests/security/test_cors.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/test_files/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-23 08:30:30.000000 foca-0.9.0/tests/test_files/__init__.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      571 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_api.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      145 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_db.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      101 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_invalid_jobs.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1537 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_invalid_log_level.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       96 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_jobs.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      438 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_log.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      435 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/conf_log_invalid.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       10 2022-06-23 08:30:30.000000 foca-0.9.0/tests/test_files/conf_no_yaml.txt
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1451 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/conf_valid.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      329 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/conf_valid_cors_disabled.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      328 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/conf_valid_cors_enabled.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1467 2022-06-23 08:30:30.000000 foca-0.9.0/tests/test_files/conf_valid_custom_invalid.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      427 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/empty_conf.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     3144 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/invalid.json
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      667 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/invalid.openapi.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      427 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/invalid_conf.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)       63 2021-04-21 07:42:32.000000 foca-0.9.0/tests/test_files/invalid_conf_db.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      185 2022-06-23 08:30:30.000000 foca-0.9.0/tests/test_files/model_valid.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      919 2022-06-25 15:54:40.000000 foca-0.9.0/tests/test_files/models_petstore.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)      699 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/openapi_2_petstore.addition.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2280 2022-06-25 15:51:49.000000 foca-0.9.0/tests/test_files/openapi_2_petstore.modified.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1739 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/openapi_2_petstore.original.json
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2416 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/openapi_2_petstore.original.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2666 2022-06-25 15:51:49.000000 foca-0.9.0/tests/test_files/openapi_3_petstore.modified.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2781 2021-08-24 15:04:28.000000 foca-0.9.0/tests/test_files/openapi_3_petstore.original.yaml
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     4222 2022-06-25 16:19:50.000000 foca-0.9.0/tests/test_foca.py
+drwxrwxr-x   0 uniqueg   (1000) uniqueg   (1000)        0 2022-06-25 16:21:38.000000 foca-0.9.0/tests/utils/
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1341 2021-08-24 15:04:28.000000 foca-0.9.0/tests/utils/test_db.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     1818 2021-08-24 15:04:28.000000 foca-0.9.0/tests/utils/test_logging.py
+-rw-rw-r--   0 uniqueg   (1000) uniqueg   (1000)     2279 2021-08-24 15:04:28.000000 foca-0.9.0/tests/utils/test_misc.py
```

### Comparing `foca-0.8.0/LICENSE` & `foca-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/PKG-INFO` & `foca-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foca
-Version: 0.8.0
+Version: 0.9.0
 Summary: Archetype for OpenAPI microservices based on Flask and Connexion
 Home-page: https://github.com/elixir-cloud-aai/foca
 Author: ELIXIR Cloud & AAI
 Author-email: alexander.kanitz@alumni.ethz.ch
 Maintainer: Alexander Kanitz
 Maintainer-email: alexander.kanitz@alumnni.ethz.ch
 License: UNKNOWN
@@ -76,20 +76,21 @@
         
         ```bash
         pip install foca
         ```
         
         (2) Create a [configuration file](#configuration-file).
         
-        (3) Import the FOCA main function `foca()` and pass your config:
+        (3) Import the FOCA class and pass your config file:
         
         ```python
-        from foca import foca
+        from foca import Foca
         
-        app = foca("path/to/my/app/config.yaml")  # returns a Connexion app instance
+        app = Foca(config_file="path/to/my/app/config.yaml")
+        app = foca.create_app()  # returns a Connexion app instance
         ```
         
         (4) Start your [Flask][res-flask] app as usual.
         
         ![Hint][img-hint] _**Check out the [Petstore example application][example]
         shipped with this repository to see FOCA in action!**_
         
@@ -127,15 +128,15 @@
         the specifications as well as a [Swagger][res-swagger]-based user interface to
         explore the API. FOCA supports multiple specification files (versions
         Swagger/OpenAPI 2.x, OpenAPI 3.x and mixed) and multiple fragments thereof, and
         it adds additional features that allow easy modification of specifications on
         the fly. In particular, links to routers and security definitions can be added
         to each specified endpoint.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         api:
           specs:
             - path:
                 - path/to/openapi/specs.yaml
                 - path/to/openapi/additions.yaml
@@ -176,15 +177,15 @@
         ### Configuring MongoDB
         
         FOCA can register one or more [MongoDB][res-mongo-db] databases and/or
         collections for you. To use that functionality, simply include the top-level
         `db` keyword section in your configuration file and tune its behavior through
         the available parameters.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         db:
           host: mongodb
           port: 27017
           dbs:
             myDb:
@@ -208,28 +209,28 @@
         ```
         
         > In this example, two databases (`myDb` and `myOtherDb`) are configured, the
         > former with two and the latter with one collection (`myCollection`,
         > `mySecondCollection` and `myThirdCollection`, respectively). FOCA will
         > automatically register and initialize these databases and collections for you
         > and add convenient clients to the app instance (accessible as children of
-        > `current_app.config['FOCA']` in an [application
+        > `current_app.config.foca` in an [application
         > context][res-flask-app-context]). The collections would be indexed by keys
         > `id`, `other_id` and `third_id`, respectively. Out of these, only `id`
         > will be required to be unique.  
         >  
         > Cf. the [API model][docs-models-db] for further options and details.
         
         ### Configuring exceptions
         
         FOCA provides a convenient, configurable exception handler and a simple way
         of adding new exceptions to be used with that handler. To use it, specify a
         top-level `exceptions` section in the app configuration file.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         exceptions:
           required_members: [['msg'], ['status']]
           status_member: ['status']
           exceptions: my_app.exceptions.exceptions
           logging: one_line
@@ -251,15 +252,15 @@
         
         ### Configuring asynchronous tasks
         
         FOCA offers limited support for running asynchronous tasks via the
         [RabbitMQ][res-rabbitmq] broker and [Celery][res-celery]. To make use of it,
         include the `jobs` top-level section in the app configuration file.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         jobs:
           host: rabbitmq
           port: 5672
           backend: 'rpc://'
           include:
@@ -279,15 +280,15 @@
         ### Configuring logging
         
         FOCA allows you to specify a YAML-based logging configuration to control your
         application's logging behavior in an effort to provide a single configuration
         file for every application. To use it, simply add a `log` top-level section in
         your app configuration file.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         log:
           version: 1
           disable_existing_loggers: False
           formatters:
             standard:
@@ -359,23 +360,71 @@
         > environment at `0.0.0.0:8080`, Flask's debugger switched on, and its reloader
         > off.
         >  
         > Cf. the [API model][docs-models-server] for further options and details.
         
         ### Custom configuration
         
+        If you would like FOCA to validate your custom app configuration (e.g.,
+        parameters required for individual controllers, you can provide a path, in
+        dot notation, to a [`pydantic`][res-pydantic] `BaseModel`-derived model. FOCA
+        then tries to instantiate the model class with any custom parameters listed
+        under keyword section `custom`.
+        
+        Suppose you have a model like the following defined in module
+        `my_app.custom_config`:
+        
+        ```py
+        from pydantic import BaseModel
+        
+        
+        class CustomConfig(BaseModel):
+            my_param: int = 5
+        ```
+        
+        And you have, in your app configuration file `my_app/config.yaml`, the
+        following section:
+        
+        ```console
+        custom:
+          my_param: 10
+        ```
+        
+        You can then have FOCA validate your custom configuration against the
+        `CustomConfig` class by including it in the `Foca()` call like so:
+        
+        ```py
+        from foca import Foca
+        
+        foca = Foca(
+          config="my_app/config.yaml",
+          custom_config_model="my_app.custom_config.CustomConfig",
+        )
+        my_app = foca.create_app()
+        ```
+        
+        We recommend that, when defining your `pydantic` model, that you supply
+        default values wherever possible. In this way, the custom configuration
+        parameters will always be available, even if not explicitly listed in the app
+        configuration (like with the FOCA-specific parameters).
+        
+        > Note that there is tooling available to automatically generate `pydantic`
+        > models from different file formats like JSON Schema etc. See here for the
+        > [datamodel-code-generator][res-datamodel-code-generator] project.
+        
         Apart from the reserved keyword sections listed above, you are free to include
         any other sections and parameters in your app configuration file. FOCA will
         simply attach these to your application instance as described
         [above](#configuration-file) and shown
         [below](#accessing-configuration-parameters). Note, however, that any
-        such parameters need to be **MANUALLY VALIDATED**, as unfortunately (or
-        fortunately!) we can't read your mind just yet.
+        such parameters need to be _manually_ validated. The same is true if you
+        include a `custom` section but do _not_ provide a validation model class via
+        the `custom_config_model` parameter when instantiating `Foca`.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         my_custom_param: 'some_value'
         
         my_custom_param_section:
           another_custom_param: 3
           my_custom_list_param:
@@ -384,33 +433,33 @@
             - 3
         ```
         
         ### Accessing configuration parameters
         
         Once the application is created using `foca()`, one can easily access any
         configuration parameters from within the [application
-        context][res-flask-app-context] through `current_app.config['FOCA'] like so:
+        context][res-flask-app-context] through `current_app.config.foca like so:
         
         ```python
         from flask import current_app
         
-        app_config = current_app.config['FOCA']
+        app_config = current_app.config.foca
         
         db = app_config.db
         api = app_config.api
         server = app_config.server
         exceptions = app_config.exceptions
         security = app_config.security
         jobs = app_config.jobs
         log = app_config.log
         app_specific_param = current_app.config['app_specific_param']
         ```
         
         _Outside of the application context_, configuration parameters are available
-        via `app.config['FOCA']` in a similar way.
+        via `app.config.foca` in a similar way.
         
         ### More examples
         
         Apart from the [annotated template][config-template], you can also check
         out the [configuration file][config-petstore] of the [Petstore app][example]
         for another example.
         
@@ -527,25 +576,27 @@
         [img-hint]: images/hint.svg
         [img-logo-banner]: images/logo-banner.svg
         [license]: LICENSE
         [license-apache]: <https://www.apache.org/licenses/LICENSE-2.0>
         [org-elixir-cloud]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai>
         [res-celery]: <http://docs.celeryproject.org/>
         [res-connexion]: <https://github.com/zalando/connexion>
+        [res-datamodel-code-generator]: <https://github.com/koxudaxi/datamodel-code-generator/>
         [res-cors]: <https://flask-cors.readthedocs.io/en/latest/>
         [res-elixir-cloud-coc]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/CODE_OF_CONDUCT.md>
         [res-elixir-cloud-contributing]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/CONTRIBUTING.md>
         [res-flask]: <http://flask.pocoo.org/>
         [res-flask-app-context]: <https://flask.palletsprojects.com/en/1.1.x/appcontext/>
         [res-foca]: <https://pypi.org/project/foca/>
         [res-jwt]: <https://jwt.io>
         [res-mongo-db]: <https://www.mongodb.com/>
         [res-python-logging]: <https://docs.python.org/3/library/logging.html>
         [res-python-logging-how-to]: <https://docs.python.org/3/howto/logging.html?highlight=yaml#configuring-logging>
         [res-openapi]: <https://www.openapis.org/>
+        [res-pydantic]: <https://pydantic-docs.helpmanual.io/>
         [res-rabbitmq]: <https://www.rabbitmq.com/>
         [res-semver]: <https://semver.org/>
         [res-swagger]: <https://swagger.io/tools/swagger-ui/>
         [res-using-foca]: <https://github.com/elixir-cloud-aai/foca/network/dependents>
         [res-yaml]: <https://yaml.org/>
         
 Keywords: rest api app openapi python microservice
@@ -555,16 +606,16 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
```

### Comparing `foca-0.8.0/PULL_REQUEST_TEMPLATE.md` & `foca-0.9.0/PULL_REQUEST_TEMPLATE.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,11 +14,13 @@
 - [ ] Documentation update
 
 ## Checklist:
 
 - [ ] My code follows the [style guidelines](https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/resources/contributing_guidelines.md#language-specific-guidelines) of this project
 - [ ] I have performed a self-review of my own code
 - [ ] I have commented my code, particularly in hard-to-understand areas
+- [ ] I have updated the documentation (or documentation does not need to be updated)
 - [ ] My changes generate no new warnings
 - [ ] I have added tests that prove my fix is effective or that my feature works
 - [ ] New and existing unit tests pass locally with my changes
 - [ ] I have not reduced the existing code coverage
+
```

### Comparing `foca-0.8.0/README.md` & `foca-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,20 +63,21 @@
 
 ```bash
 pip install foca
 ```
 
 (2) Create a [configuration file](#configuration-file).
 
-(3) Import the FOCA main function `foca()` and pass your config:
+(3) Import the FOCA class and pass your config file:
 
 ```python
-from foca import foca
+from foca import Foca
 
-app = foca("path/to/my/app/config.yaml")  # returns a Connexion app instance
+app = Foca(config_file="path/to/my/app/config.yaml")
+app = foca.create_app()  # returns a Connexion app instance
 ```
 
 (4) Start your [Flask][res-flask] app as usual.
 
 ![Hint][img-hint] _**Check out the [Petstore example application][example]
 shipped with this repository to see FOCA in action!**_
 
@@ -114,15 +115,15 @@
 the specifications as well as a [Swagger][res-swagger]-based user interface to
 explore the API. FOCA supports multiple specification files (versions
 Swagger/OpenAPI 2.x, OpenAPI 3.x and mixed) and multiple fragments thereof, and
 it adds additional features that allow easy modification of specifications on
 the fly. In particular, links to routers and security definitions can be added
 to each specified endpoint.
 
-*Example:*
+_Example:_
 
 ```yaml
 api:
   specs:
     - path:
         - path/to/openapi/specs.yaml
         - path/to/openapi/additions.yaml
@@ -163,15 +164,15 @@
 ### Configuring MongoDB
 
 FOCA can register one or more [MongoDB][res-mongo-db] databases and/or
 collections for you. To use that functionality, simply include the top-level
 `db` keyword section in your configuration file and tune its behavior through
 the available parameters.
 
-*Example:*
+_Example:_
 
 ```yaml
 db:
   host: mongodb
   port: 27017
   dbs:
     myDb:
@@ -195,28 +196,28 @@
 ```
 
 > In this example, two databases (`myDb` and `myOtherDb`) are configured, the
 > former with two and the latter with one collection (`myCollection`,
 > `mySecondCollection` and `myThirdCollection`, respectively). FOCA will
 > automatically register and initialize these databases and collections for you
 > and add convenient clients to the app instance (accessible as children of
-> `current_app.config['FOCA']` in an [application
+> `current_app.config.foca` in an [application
 > context][res-flask-app-context]). The collections would be indexed by keys
 > `id`, `other_id` and `third_id`, respectively. Out of these, only `id`
 > will be required to be unique.  
 >  
 > Cf. the [API model][docs-models-db] for further options and details.
 
 ### Configuring exceptions
 
 FOCA provides a convenient, configurable exception handler and a simple way
 of adding new exceptions to be used with that handler. To use it, specify a
 top-level `exceptions` section in the app configuration file.
 
-*Example:*
+_Example:_
 
 ```yaml
 exceptions:
   required_members: [['msg'], ['status']]
   status_member: ['status']
   exceptions: my_app.exceptions.exceptions
   logging: one_line
@@ -238,15 +239,15 @@
 
 ### Configuring asynchronous tasks
 
 FOCA offers limited support for running asynchronous tasks via the
 [RabbitMQ][res-rabbitmq] broker and [Celery][res-celery]. To make use of it,
 include the `jobs` top-level section in the app configuration file.
 
-*Example:*
+_Example:_
 
 ```yaml
 jobs:
   host: rabbitmq
   port: 5672
   backend: 'rpc://'
   include:
@@ -266,15 +267,15 @@
 ### Configuring logging
 
 FOCA allows you to specify a YAML-based logging configuration to control your
 application's logging behavior in an effort to provide a single configuration
 file for every application. To use it, simply add a `log` top-level section in
 your app configuration file.
 
-*Example:*
+_Example:_
 
 ```yaml
 log:
   version: 1
   disable_existing_loggers: False
   formatters:
     standard:
@@ -346,23 +347,71 @@
 > environment at `0.0.0.0:8080`, Flask's debugger switched on, and its reloader
 > off.
 >  
 > Cf. the [API model][docs-models-server] for further options and details.
 
 ### Custom configuration
 
+If you would like FOCA to validate your custom app configuration (e.g.,
+parameters required for individual controllers, you can provide a path, in
+dot notation, to a [`pydantic`][res-pydantic] `BaseModel`-derived model. FOCA
+then tries to instantiate the model class with any custom parameters listed
+under keyword section `custom`.
+
+Suppose you have a model like the following defined in module
+`my_app.custom_config`:
+
+```py
+from pydantic import BaseModel
+
+
+class CustomConfig(BaseModel):
+    my_param: int = 5
+```
+
+And you have, in your app configuration file `my_app/config.yaml`, the
+following section:
+
+```console
+custom:
+  my_param: 10
+```
+
+You can then have FOCA validate your custom configuration against the
+`CustomConfig` class by including it in the `Foca()` call like so:
+
+```py
+from foca import Foca
+
+foca = Foca(
+  config="my_app/config.yaml",
+  custom_config_model="my_app.custom_config.CustomConfig",
+)
+my_app = foca.create_app()
+```
+
+We recommend that, when defining your `pydantic` model, that you supply
+default values wherever possible. In this way, the custom configuration
+parameters will always be available, even if not explicitly listed in the app
+configuration (like with the FOCA-specific parameters).
+
+> Note that there is tooling available to automatically generate `pydantic`
+> models from different file formats like JSON Schema etc. See here for the
+> [datamodel-code-generator][res-datamodel-code-generator] project.
+
 Apart from the reserved keyword sections listed above, you are free to include
 any other sections and parameters in your app configuration file. FOCA will
 simply attach these to your application instance as described
 [above](#configuration-file) and shown
 [below](#accessing-configuration-parameters). Note, however, that any
-such parameters need to be **MANUALLY VALIDATED**, as unfortunately (or
-fortunately!) we can't read your mind just yet.
+such parameters need to be _manually_ validated. The same is true if you
+include a `custom` section but do _not_ provide a validation model class via
+the `custom_config_model` parameter when instantiating `Foca`.
 
-*Example:*
+_Example:_
 
 ```yaml
 my_custom_param: 'some_value'
 
 my_custom_param_section:
   another_custom_param: 3
   my_custom_list_param:
@@ -371,33 +420,33 @@
     - 3
 ```
 
 ### Accessing configuration parameters
 
 Once the application is created using `foca()`, one can easily access any
 configuration parameters from within the [application
-context][res-flask-app-context] through `current_app.config['FOCA'] like so:
+context][res-flask-app-context] through `current_app.config.foca like so:
 
 ```python
 from flask import current_app
 
-app_config = current_app.config['FOCA']
+app_config = current_app.config.foca
 
 db = app_config.db
 api = app_config.api
 server = app_config.server
 exceptions = app_config.exceptions
 security = app_config.security
 jobs = app_config.jobs
 log = app_config.log
 app_specific_param = current_app.config['app_specific_param']
 ```
 
 _Outside of the application context_, configuration parameters are available
-via `app.config['FOCA']` in a similar way.
+via `app.config.foca` in a similar way.
 
 ### More examples
 
 Apart from the [annotated template][config-template], you can also check
 out the [configuration file][config-petstore] of the [Petstore app][example]
 for another example.
 
@@ -514,23 +563,25 @@
 [img-hint]: images/hint.svg
 [img-logo-banner]: images/logo-banner.svg
 [license]: LICENSE
 [license-apache]: <https://www.apache.org/licenses/LICENSE-2.0>
 [org-elixir-cloud]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai>
 [res-celery]: <http://docs.celeryproject.org/>
 [res-connexion]: <https://github.com/zalando/connexion>
+[res-datamodel-code-generator]: <https://github.com/koxudaxi/datamodel-code-generator/>
 [res-cors]: <https://flask-cors.readthedocs.io/en/latest/>
 [res-elixir-cloud-coc]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/CODE_OF_CONDUCT.md>
 [res-elixir-cloud-contributing]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/CONTRIBUTING.md>
 [res-flask]: <http://flask.pocoo.org/>
 [res-flask-app-context]: <https://flask.palletsprojects.com/en/1.1.x/appcontext/>
 [res-foca]: <https://pypi.org/project/foca/>
 [res-jwt]: <https://jwt.io>
 [res-mongo-db]: <https://www.mongodb.com/>
 [res-python-logging]: <https://docs.python.org/3/library/logging.html>
 [res-python-logging-how-to]: <https://docs.python.org/3/howto/logging.html?highlight=yaml#configuring-logging>
 [res-openapi]: <https://www.openapis.org/>
+[res-pydantic]: <https://pydantic-docs.helpmanual.io/>
 [res-rabbitmq]: <https://www.rabbitmq.com/>
 [res-semver]: <https://semver.org/>
 [res-swagger]: <https://swagger.io/tools/swagger-ui/>
 [res-using-foca]: <https://github.com/elixir-cloud-aai/foca/network/dependents>
 [res-yaml]: <https://yaml.org/>
```

### Comparing `foca-0.8.0/docker/Dockerfile_py3.6` & `foca-0.9.0/docker/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-FROM python:3.6-slim-stretch as base
+ARG PY_IMAGE=3.10-slim-buster
+FROM python:$PY_IMAGE as base
 
 # Metadata
 LABEL software="FOCA"
 LABEL software.description="Kickstart OpenAPI-based microservice development with Flask & Connexion"
 LABEL software.website="https://github.com/elixir-cloud-aai/foca"
 LABEL software.license="https://spdx.org/licenses/Apache-2.0"
 LABEL maintainer="alexander.kanitz@alumni.ethz.ch"
```

### Comparing `foca-0.8.0/docs/api/conf.py` & `foca-0.9.0/docs/api/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-import os
+from pathlib import Path
 import sys
 
 from sphinx.ext import apidoc
 
-sys.path.insert(0, os.path.abspath('../..'))
+sys.path.insert(0, Path.cwd().resolve().parents[1])
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'FOCA'
 copyright = '2020, ELIXIR Cloud & AAI'
 author = 'ELIXIR Cloud & AAI'
```

### Comparing `foca-0.8.0/examples/petstore/Dockerfile` & `foca-0.9.0/examples/petstore/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ### BASE IMAGE ###
-FROM elixircloud/foca:latest
+FROM elixircloud/foca:petstore
 
 # Metadata
 LABEL software="Petstore application"
 LABEL software.description="Example application for FOCA microservice archetype"
 LABEL software.website="https://github.com/elixir-cloud-aai/foca"
 LABEL software.documentation="https://github.com/elixir-cloud-aai/foca"
 LABEL software.license="https://spdx.org/licenses/Apache-2.0"
```

### Comparing `foca-0.8.0/examples/petstore/README.md` & `foca-0.9.0/examples/petstore/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
 FOCA makes sure that
 
 * the returned app instance contains all [configuration parameters][app-config]
 * FOCA configuration parameters are validated
 * requests and responses sent to/from the API endpoints configured in the
   [Petstore][app-specs] [OpenAPI][res-openapi] specification are validated
-* a [MongoDB][res-mongo-db] collection to store pets in is registered with The
+* a [MongoDB][res-mongo-db] collection to store pets in is registered with the
   app
 * [CORS][res-cors] is enabled
-* handles exceptions (here only returns `500 / Internal Server Error` for all
-  problems)
+* exceptions are handled according to the definitions in the `exceptions`
+  dictionary in module [`exceptions`][app-exceptions]
 
 Apart from writing the configuration file, all that was left for us to do to
 set up this example app was to write a _very_ simple app [entry point
-module][app-entry-point], implement the [endpoint controller
+module][app-entrypoint], implement the [endpoint controller
 logic][app-controllers] and prepare the [`Dockerfile`][app-dockerfile] and
 [Docker Compose][res-docker-compose] [configuration][app-docker-compose] for
 easy shipping/installation!
 
 ![Hint][img-hint] _**Check the [FOCA documentation][docs] for further
 details.**_
 
@@ -49,18 +49,43 @@
 
 Clone repository:
 
 ```bash
 git clone https://github.com/elixir-cloud-aai/foca.git
 ```
 
+Traverse to the repository root directory:
+
+```bash
+cd foca
+```
+
+Locally build the FOCA base image based on the current state of FOCA and based
+on one of the supported Python versions (here: `3.9`):
+
+```bash
+docker build \
+  -t elixircloud/foca:petstore \
+  -f docker/Dockerfile \
+  .
+```
+
+> If you wish to modify FOCA code itself and then have those code changes
+> reflected in the example app, don't forget to rebuild the FOCA base image
+> before re-starting services via `docker-compose` in the next steps!  
+>  
+> You can also optionally build FOCA with another supported version of Python.
+> In that case, add `--build-arg PY_IMAGE="PYTHON_IMAGE_TAG"` to the `docker
+> build` command above, where `PYTHON_IMAGE_TAG` is the tag of the official
+> Python image you would like to use.
+
 Traverse to example app directory:
 
 ```bash
-cd foca/examples/petstore
+cd examples/petstore
 ```
 
 Build and run services in detached/daemonized mode:
 
 ```bash
 docker-compose up -d --build
 ```
@@ -68,25 +93,26 @@
 > In case Docker complains about port conflicts or if any of the used ports are
 > blocked by a firewall, you will need to re-map the conflicting port(s) in the
 > [Docker Compose config][app-docker-compose]. In particular, for each of the
 > services that failed to start because of a port conflict, you will need to
 > change the **first** of the two numbers listed below the corresponding
 > `ports` keyword to some unused/open port. Note that if you change the mapped
 > port for the `app` service you will need to manually append it to `localhost`
-> when you access the API (or the Swagger UI) in subsequent steps, like, e.g.,
-> so: `http://localhost:8080/`.
+> when you access the API (or the Swagger UI) in subsequent steps. For example,
+> assuming you would like to run the app on port `8080` instead of the default
+> of `80`, then the app will be availabe via : `http://localhost:8080/`.
 
 That's it, you can now visit the application's [Swagger UI][res-swagger-ui] in
 your browser, e.g.,:
 
 ```bash
 firefox http://localhost/ui  # or use your browser of choice
 ```
 
-> Mac users may need to replace `localhost` with `0.0.0.0`.
+> Note that Mac users may need to replace `localhost` with `0.0.0.0`.
 
 ## Explore app
 
 In the [Swagger UI][res-swagger-ui], you may use the `GET`/`POST` endpoints by
 providing the required/desired values based on the indicated descriptions, then
 hit the `Try it out!` button!
 
@@ -112,57 +138,43 @@
   ```
 
 * To **retrieve information on a specific pet**:
 
   ```console
   curl -X GET \
       --header 'Accept: application/json' \
-      'http://localhost/pets/0' 
+      'http://localhost/pets/0'  # replace 0 with the the pet ID of choice
   ```
 
 * To **delete a pet**:  :-(
 
   ```console
   curl -X DELETE \
       --header 'Accept: application/json' \
-      'http://localhost/pets/0' 
+      'http://localhost/pets/0'  # replace 0 with the the pet ID of choice
   ```
 
 ## Modify app
 
 You can make use of this example to create your own app. Just modify any or all
 of the following:
 
 * [FOCA configuration file][app-config]
+* [Main application module][app-entrypoint]
 * [API specification][app-specs]
 * [Endpoint controller module][app-controllers]
-* [Main application module][app-entrypoint]
-* [Dockerfile][app-dockerfile]
-* [Docker Compose configuration][app-docker-compose]
-
-### Modifying FOCA
-
-In case you want to change FOCA itself and want the code changes to be
-reflected in the Petstore app, you will need to manually rebuild the FOCA
-container image like so:
-
-```bash
-docker build -t elixircloud/foca:latest .  # execute in the FOCA root directory
-```
-
-Then re-build and start the Petstore app as described before:
-
-```bash
-docker-compose up --build -d  # execute in _this_ directory
-```
+* [Registered exceptions][app-exceptions]
+* [`Dockerfile`][app-dockerfile]
+* [`docker-compose` configuration][app-docker-compose]
 
 [app-config]: config.yaml
 [app-controllers]: controllers.py
 [app-dockerfile]: Dockerfile
 [app-docker-compose]: docker-compose.yaml
+[app-exceptions]: exceptions.py
 [app-entrypoint]: app.py
 [app-specs]: petstore.yaml
 [docs]: <https://foca.readthedocs.io/en/latest/>
 [docs-config-file]: ../../README.md#configuration-file
 [img-hint]: ../../images/hint.svg
 [res-cors]: <https://flask-cors.readthedocs.io/en/latest/>
 [res-curl]: <https://curl.se/>
```

### Comparing `foca-0.8.0/examples/petstore/config.yaml` & `foca-0.9.0/examples/petstore/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -38,7 +38,12 @@
     host: mongodb
     port: 27017
     dbs:
         petstore:
             collections:
                 pets:
                     indexes: null
+
+exceptions:
+    required_members: [['message'], ['code']]
+    status_member: ['code']
+    exceptions: exceptions.exceptions
```

### Comparing `foca-0.8.0/examples/petstore/controllers.py` & `foca-0.9.0/examples/petstore/controllers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,77 @@
+"""Petstore controllers."""
+
 import logging
 
 from flask import (current_app, make_response)
-from werkzeug.exceptions import NotFound
+from pymongo.collection import Collection
 
-logger = logging.getLogger(__name__)
+from exceptions import NotFound
 
-error_response = {
-    'code': 500,
-    'message': 'Something went wrong.',
-}
+logger = logging.getLogger(__name__)
 
 
 def findPets(limit=None, tags=None):
-    try:
-        db_collection = (
-            current_app.config['FOCA'].db.dbs['petstore']
-            .collections['pets'].client
-        )
-        filter_dict = {} if tags is None else {'tag': {'$in': tags}}
-        if not limit:
-            limit = 0
-        records = db_collection.find(
-            filter_dict,
-            {'_id': False}
-        ).sort([('$natural', -1)]).limit(limit)
-        return list(records)
-    except Exception as e:
-        logger.error(f"{type(e).__name__}: {e}")
-        return error_response
+    db_collection: Collection = (
+        current_app.config.foca.db.dbs['petstore']
+        .collections['pets'].client
+    )
+    filter_dict = {} if tags is None else {'tag': {'$in': tags}}
+    if not limit:
+        limit = 0
+    records = db_collection.find(
+        filter_dict,
+        {'_id': False}
+    ).sort([('$natural', -1)]).limit(limit)
+    return list(records)
 
 
 def addPet(pet):
-    try:
-        db_collection = (
-            current_app.config['FOCA'].db.dbs['petstore']
-            .collections['pets'].client
-        )
-        counter = 0
-        ctr = db_collection.find({}).sort([('$natural', -1)])
-        if not ctr.count() == 0:
-            counter = ctr[0].get('id') + 1
-        record = {
-            "id": counter,
-            "name": pet['name'],
-            "tag": pet['tag']
-        }
-        db_collection.insert_one(record)
-        del record['_id']
-        return record
-    except Exception as e:
-        logger.error(f"{type(e).__name__}: {e}")
-        return error_response
+    db_collection: Collection = (
+        current_app.config.foca.db.dbs['petstore']
+        .collections['pets'].client
+    )
+    counter = 0
+    ctr = db_collection.find({}).sort([('$natural', -1)])
+    if not ctr.count() == 0:
+        counter = ctr[0].get('id') + 1
+    record = {
+        "id": counter,
+        "name": pet['name'],
+        "tag": pet['tag']
+    }
+    db_collection.insert_one(record)
+    del record['_id']
+    return record
 
 
 def findPetById(id):
-    try:
-        db_collection = (
-            current_app.config['FOCA'].db.dbs['petstore']
-            .collections['pets'].client
-        )
-        record = db_collection.find_one(
-            {"id": id},
-            {'_id': False},
-        )
-        if not record:
-            raise NotFound
-        return record
-    except Exception as e:
-        logger.error(f"{type(e).__name__}: {e}")
-        return error_response
+    db_collection: Collection = (
+        current_app.config.foca.db.dbs['petstore']
+        .collections['pets'].client
+    )
+    record = db_collection.find_one(
+        {"id": id},
+        {'_id': False},
+    )
+    if record is None:
+        raise NotFound
+    return record
 
 
 def deletePet(id):
-    try:
-        db_collection = (
-            current_app.config['FOCA'].db.dbs['petstore']
-            .collections['pets'].client
-        )
-        record = db_collection.find_one(
-            {"id": id},
-            {'_id': False},
-        )
-        if not record:
-            raise NotFound
-        db_collection.delete_one({"id": id})
-        response = make_response('', 204)
-        response.mimetype = current_app.config['JSONIFY_MIMETYPE']
-        return response
-    except Exception as e:
-        logger.error(f"{type(e).__name__}: {e}")
-        return error_response
+    db_collection: Collection = (
+        current_app.config.foca.db.dbs['petstore']
+        .collections['pets'].client
+    )
+    record = db_collection.find_one(
+        {"id": id},
+        {'_id': False},
+    )
+    if record is None:
+        raise NotFound
+    db_collection.delete_one(
+        {"id": id},
+    )
+    response = make_response('', 204)
+    response.mimetype = current_app.config['JSONIFY_MIMETYPE']
+    return response
```

### Comparing `foca-0.8.0/examples/petstore/petstore.yaml` & `foca-0.9.0/examples/petstore/petstore.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/foca/api/register_openapi.py` & `foca-0.9.0/foca/api/register_openapi.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/foca/database/register_mongodb.py` & `foca-0.9.0/foca/database/register_mongodb.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/foca/errors/exceptions.py` & `foca-0.9.0/foca/errors/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     Args:
         exception: Raised exception.
 
     Returns:
         JSON-formatted error response.
     """
     # Look up exception & get status code
-    conf = current_app.config['FOCA'].exceptions
+    conf = current_app.config.foca.exceptions
     exc = type(exception)
     if exc not in conf.mapping:
         exc = Exception
     try:
         status = int(_get_by_path(
             obj=conf.mapping[exc],
             key_sequence=conf.status_member,
```

### Comparing `foca-0.8.0/foca/factories/celery_app.py` & `foca-0.9.0/foca/factories/celery_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
     Args:
         app: Flask application instance.
 
     Returns:
         Celery application instance.
     """
-    conf = app.config['FOCA'].jobs
+    conf = app.config.foca.jobs
 
     # Instantiate Celery app
     celery = Celery(
         app=__name__,
         broker=f"pyamqp://{conf.host}:{conf.port}//",
         backend=conf.backend,
         include=conf.include,
     )
     calling_module = ':'.join([stack()[1].filename, stack()[1].function])
     logger.debug(f"Celery app created from '{calling_module}'.")
 
     # Update Celery app configuration with Flask app configuration
-    celery.conf['FOCA'] = app.config['FOCA']
+    setattr(celery.conf, 'foca', app.config.foca)
     logger.debug('Celery app configured.')
 
     class ContextTask(celery.Task):  # type: ignore
         # https://github.com/python/mypy/issues/4284)
         """Create subclass of task that wraps task execution in application
         context.
         """
```

### Comparing `foca-0.8.0/foca/factories/connexion_app.py` & `foca-0.9.0/foca/factories/connexion_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,11 +67,11 @@
     app.app.config['TESTING'] = conf.testing
 
     logger.debug('Flask app settings:')
     for (key, value) in app.app.config.items():
         logger.debug('* {}: {}'.format(key, value))
 
     # Add user configuration to Flask app config
-    app.app.config['FOCA'] = config
+    setattr(app.app.config, 'foca', config)
 
     logger.debug('Connexion app configured.')
     return app
```

### Comparing `foca-0.8.0/foca/models/config.py` & `foca-0.9.0/foca/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from copy import deepcopy
 from enum import Enum
 from functools import reduce
 import importlib
 import operator
 from pathlib import Path
-import os
 from typing import (Any, Dict, List, Optional, Union)
 
 from pydantic import (BaseModel, Field, validator)  # pylint: disable=E0611
 import pymongo
 
 
 def _validate_log_level_choices(level: int) -> int:
@@ -208,15 +207,15 @@
             specified as a sequence of keys, are excluded. Set to ``None`` to
             disable filtering. Note that only one of `public_members` and
             `private_members` filters can be active.
         exceptions: Path to dictionary containing the actual exception classes
             as keys and a dictionary of JSON members (as per `required_members`
             and `extension_members`) as values. Path should be a dot-separated
             path to the module containing the dictionary (which needs to also
-            contain imports for all listed expcetions), followed by the name of
+            contain imports for all listed exceptions), followed by the name of
             the dictionary itself. For example, for ``myapp.errors.exc_dict``,
             the dictionary ``exc_dict`` would be attempted to be imported from
             module ``myapp.errors`` (must be available in the Pythonpath). To
             ensure that all exceptions arising during the app context are
             handled, it is strongly advised to add the catch-all exception
             ``Exception``. If missing, any exceptions not listed will only
             provoke an empty JSON response.
@@ -249,15 +248,15 @@
             specified as a sequence of keys, are excluded. Set to ``None`` to
             disable filtering. Note that only one of `public_members` and
             `private_members` filters can be active.
         exceptions: Path to dictionary containing the actual exception classes
             as keys and a dictionary of JSON members (as per `required_members`
             and `extension_members`) as values. Path should be a dot-separated
             path to the module containing the dictionary (which needs to also
-            contain imports for all listed expcetions), followed by the name of
+            contain imports for all listed exceptions), followed by the name of
             the dictionary itself. For example, for ``myapp.errors.exc_dict``,
             the dictionary ``exc_dict`` would be attempted to be imported from
             module ``myapp.errors`` (must be available in the Pythonpath). To
             ensure that all exceptions arising during the app context are
             handled, it is strongly advised to add the catch-all exception
             ``Exception``. If missing, any exceptions not listed will only
             provoke an empty JSON response.
@@ -528,17 +527,17 @@
     Raises:
         pydantic.ValidationError: The class was instantianted with an illegal
             data type.
 
     Example:
 
         >>> SpecConfig(path="/my/path.yaml")
-        SpecConfig(path=['/my/path.yaml'], path_out='/my/path.modified.yaml', \
-append=None, add_operation_fields=None, add_security_fields=None, disable_auth\
-=False, connexion=None)
+        SpecConfig(path=[PosixPath('/my/path.yaml')], path_out=PosixPath('/my/\
+path.modified.yaml'), append=None, add_operation_fields=None, add_security_fie\
+lds=None, disable_auth=False, connexion=None)
 
         >>> SpecConfig(
         ...     path=["/path/to/specs.yaml", "/path/to/add_specs.yaml"],
         ...     path_out="/path/to/specs.modified.yaml",
         ...     append=[
         ...         {
         ...             "security": {
@@ -559,64 +558,62 @@
         ...     },
         ...     add_security_fields = {
         ...         "x-apikeyInfoFunc": "security.auth.validate_token",
         ...         "x-some-other-custom-field": "some_value",
         ...     },
         ...     disable_auth = False
         ... )
-        SpecConfig(path=['/path/to/specs.yaml', '/path/to/add_specs.yaml'], pa\
-th_out='/path/to/specs.modified.yaml', append=[{'security': {'jwt': {'type': '\
-apiKey', 'name': 'Authorization', 'in': 'header'}}}, {'my_other_root_field': '\
-some_value'}], add_operation_fields={'x-swagger-router-controller': 'controlle\
-rs.my_specs', 'x-some-other-custom-field': 'some_value'}, add_security_fields=\
-{'x-apikeyInfoFunc': 'security.auth.validate_token', 'x-some-other-custom-fiel\
-d': 'some_value'}, disable_auth=False, connexion=None)
+        SpecConfig(path=[PosixPath('/path/to/specs.yaml'), PosixPath('/path/to\
+/add_specs.yaml')], path_out=PosixPath('/path/to/specs.modified.yaml'), append\
+=[{'security': {'jwt': {'type': 'apiKey', 'name': 'Authorization', 'in': 'head\
+er'}}}, {'my_other_root_field': 'some_value'}], add_operation_fields={'x-swagg\
+er-router-controller': 'controllers.my_specs', 'x-some-other-custom-field': 's\
+ome_value'}, add_security_fields={'x-apikeyInfoFunc': 'security.auth.validate_\
+token', 'x-some-other-custom-field': 'some_value'}, disable_auth=False, connex\
+ion=None)
     """
-    path: Union[str, List[str]]
-    path_out: Optional[str] = None
+    path: Union[Path, List[Path]]
+    path_out: Optional[Path] = None
     append: Optional[List[Dict]] = None
     add_operation_fields: Optional[Dict] = None
     add_security_fields: Optional[Dict] = None
     disable_auth: bool = False
     connexion: Optional[Dict] = None
 
     # resolve relative path
     @validator('path', always=True, allow_reuse=True)
     def set_abs_path(cls, v):  # pylint: disable=E0213
         """Resolve path relative to caller's current working directory if no
         absolute path provided.
         """
-        # if path is a str, convert it to list
-        if(isinstance(v, str)):
-            if not Path(v).is_absolute():
-                return [str(Path.cwd() / v)]
+        # if path is not a list, convert it to single-item list
+        if(isinstance(v, Path)):
+            if not v.is_absolute():
+                return [Path.cwd() / v]
             return [v]
         else:
-            # modify each relaive part of the list
+            # make each path absolute
             v = [
-                str(Path.cwd() / path)
-                if not Path(path).is_absolute()
+                Path.cwd() / path
+                if not path.is_absolute()
                 else path
                 for path in v
             ]
         return v
 
     # set default if no output file path provided
     @validator('path_out', always=True, allow_reuse=True)
     def set_default_out_path(cls, v, *, values):  # pylint: disable=E0213
-        """Set default output path for spec file if not supplied by user.
-        """
+        """Set default output path for spec file if not supplied by user."""
         if 'path' in values and values['path'] is not None:
             if not v:
-                return '.'.join([
-                    os.path.splitext(values['path'][0])[0],
-                    "modified.yaml"
-                ])
-            if not Path(v).is_absolute():
-                return str(Path.cwd() / v)
+                path = values['path'][0]
+                return path.parent / f"{path.stem}.modified.yaml"
+            if not v.is_absolute():
+                return Path.cwd() / v
         return v
 
 
 class APIConfig(FOCABaseConfig):
     """Model for a list of configuration parameters for OpenAPI 2.x or 3.x
     specifications to be attached to a Connexion app.
 
@@ -632,17 +629,17 @@
         pydantic.ValidationError: The class was instantianted with an illegal
             data type.
 
     Example:
         >>> APIConfig(
         ...     specs=[SpecConfig(path='/path/to/specs.yaml')],
         ... )
-        APIConfig(specs=[SpecConfig(path='/path/to/specs.yaml', path_out='/pat\
-h/to/specs.modified.yaml', append=None, add_operation_fields=None, connexion=N\
-one)])
+        APIConfig(specs=[SpecConfig(path=[PosixPath('/path/to/specs.yaml')], p\
+ath_out=PosixPath('/path/to/specs.modified.yaml'), append=None, add_operation_\
+fields=None, add_security_fields=None, disable_auth=False, connexion=None)])
     """
     specs: List[SpecConfig] = []
 
 
 class AuthConfig(FOCABaseConfig):
     """Model for parameters used to configure JSON Web Token (JWT)-based
     authorization for the app.
```

### Comparing `foca-0.8.0/foca/security/auth.py` & `foca-0.9.0/foca/security/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # Set parameters defined by OpenID Connect specification
     # Cf. https://openid.net/specs/openid-connect-discovery-1_0.html
     oidc_suffix_config: str = ".well-known/openid-configuration"
     oidc_config_claim_userinfo: str = 'userinfo_endpoint'
     oidc_config_claim_public_keys: str = 'jwks_uri'
 
     # Fetch security parameters
-    conf = current_app.config['FOCA'].security.auth
+    conf = current_app.config.foca.security.auth
     add_key_to_claims: bool = conf.add_key_to_claims
     allow_expired: bool = conf.allow_expired
     audience: Optional[Iterable[str]] = conf.audience
     claim_identity: str = conf.claim_identity
     claim_issuer: str = conf.claim_issuer
     algorithms: Iterable[str] = conf.algorithms
     validation_methods: List[str] = [e.value for e in conf.validation_methods]
@@ -52,16 +52,16 @@
             "configured"
         )
 
     # Decode JWT
     try:
         claims = jwt.decode(
             jwt=token,
-            verify=False,
             algorithms=algorithms,
+            options={"verify_signature": False}
         )
     except Exception as e:
         raise Unauthorized("JWT could not be decoded") from e
     logger.debug(f"Decoded claims: {claims}")
 
     # Verify existence of issuer claim
     if claim_issuer not in claims:
```

### Comparing `foca-0.8.0/foca/utils/db.py` & `foca-0.9.0/foca/utils/db.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/foca/utils/logging.py` & `foca-0.9.0/foca/utils/logging.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/foca/utils/misc.py` & `foca-0.9.0/foca/utils/misc.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/foca.egg-info/PKG-INFO` & `foca-0.9.0/foca.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foca
-Version: 0.8.0
+Version: 0.9.0
 Summary: Archetype for OpenAPI microservices based on Flask and Connexion
 Home-page: https://github.com/elixir-cloud-aai/foca
 Author: ELIXIR Cloud & AAI
 Author-email: alexander.kanitz@alumni.ethz.ch
 Maintainer: Alexander Kanitz
 Maintainer-email: alexander.kanitz@alumnni.ethz.ch
 License: UNKNOWN
@@ -76,20 +76,21 @@
         
         ```bash
         pip install foca
         ```
         
         (2) Create a [configuration file](#configuration-file).
         
-        (3) Import the FOCA main function `foca()` and pass your config:
+        (3) Import the FOCA class and pass your config file:
         
         ```python
-        from foca import foca
+        from foca import Foca
         
-        app = foca("path/to/my/app/config.yaml")  # returns a Connexion app instance
+        app = Foca(config_file="path/to/my/app/config.yaml")
+        app = foca.create_app()  # returns a Connexion app instance
         ```
         
         (4) Start your [Flask][res-flask] app as usual.
         
         ![Hint][img-hint] _**Check out the [Petstore example application][example]
         shipped with this repository to see FOCA in action!**_
         
@@ -127,15 +128,15 @@
         the specifications as well as a [Swagger][res-swagger]-based user interface to
         explore the API. FOCA supports multiple specification files (versions
         Swagger/OpenAPI 2.x, OpenAPI 3.x and mixed) and multiple fragments thereof, and
         it adds additional features that allow easy modification of specifications on
         the fly. In particular, links to routers and security definitions can be added
         to each specified endpoint.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         api:
           specs:
             - path:
                 - path/to/openapi/specs.yaml
                 - path/to/openapi/additions.yaml
@@ -176,15 +177,15 @@
         ### Configuring MongoDB
         
         FOCA can register one or more [MongoDB][res-mongo-db] databases and/or
         collections for you. To use that functionality, simply include the top-level
         `db` keyword section in your configuration file and tune its behavior through
         the available parameters.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         db:
           host: mongodb
           port: 27017
           dbs:
             myDb:
@@ -208,28 +209,28 @@
         ```
         
         > In this example, two databases (`myDb` and `myOtherDb`) are configured, the
         > former with two and the latter with one collection (`myCollection`,
         > `mySecondCollection` and `myThirdCollection`, respectively). FOCA will
         > automatically register and initialize these databases and collections for you
         > and add convenient clients to the app instance (accessible as children of
-        > `current_app.config['FOCA']` in an [application
+        > `current_app.config.foca` in an [application
         > context][res-flask-app-context]). The collections would be indexed by keys
         > `id`, `other_id` and `third_id`, respectively. Out of these, only `id`
         > will be required to be unique.  
         >  
         > Cf. the [API model][docs-models-db] for further options and details.
         
         ### Configuring exceptions
         
         FOCA provides a convenient, configurable exception handler and a simple way
         of adding new exceptions to be used with that handler. To use it, specify a
         top-level `exceptions` section in the app configuration file.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         exceptions:
           required_members: [['msg'], ['status']]
           status_member: ['status']
           exceptions: my_app.exceptions.exceptions
           logging: one_line
@@ -251,15 +252,15 @@
         
         ### Configuring asynchronous tasks
         
         FOCA offers limited support for running asynchronous tasks via the
         [RabbitMQ][res-rabbitmq] broker and [Celery][res-celery]. To make use of it,
         include the `jobs` top-level section in the app configuration file.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         jobs:
           host: rabbitmq
           port: 5672
           backend: 'rpc://'
           include:
@@ -279,15 +280,15 @@
         ### Configuring logging
         
         FOCA allows you to specify a YAML-based logging configuration to control your
         application's logging behavior in an effort to provide a single configuration
         file for every application. To use it, simply add a `log` top-level section in
         your app configuration file.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         log:
           version: 1
           disable_existing_loggers: False
           formatters:
             standard:
@@ -359,23 +360,71 @@
         > environment at `0.0.0.0:8080`, Flask's debugger switched on, and its reloader
         > off.
         >  
         > Cf. the [API model][docs-models-server] for further options and details.
         
         ### Custom configuration
         
+        If you would like FOCA to validate your custom app configuration (e.g.,
+        parameters required for individual controllers, you can provide a path, in
+        dot notation, to a [`pydantic`][res-pydantic] `BaseModel`-derived model. FOCA
+        then tries to instantiate the model class with any custom parameters listed
+        under keyword section `custom`.
+        
+        Suppose you have a model like the following defined in module
+        `my_app.custom_config`:
+        
+        ```py
+        from pydantic import BaseModel
+        
+        
+        class CustomConfig(BaseModel):
+            my_param: int = 5
+        ```
+        
+        And you have, in your app configuration file `my_app/config.yaml`, the
+        following section:
+        
+        ```console
+        custom:
+          my_param: 10
+        ```
+        
+        You can then have FOCA validate your custom configuration against the
+        `CustomConfig` class by including it in the `Foca()` call like so:
+        
+        ```py
+        from foca import Foca
+        
+        foca = Foca(
+          config="my_app/config.yaml",
+          custom_config_model="my_app.custom_config.CustomConfig",
+        )
+        my_app = foca.create_app()
+        ```
+        
+        We recommend that, when defining your `pydantic` model, that you supply
+        default values wherever possible. In this way, the custom configuration
+        parameters will always be available, even if not explicitly listed in the app
+        configuration (like with the FOCA-specific parameters).
+        
+        > Note that there is tooling available to automatically generate `pydantic`
+        > models from different file formats like JSON Schema etc. See here for the
+        > [datamodel-code-generator][res-datamodel-code-generator] project.
+        
         Apart from the reserved keyword sections listed above, you are free to include
         any other sections and parameters in your app configuration file. FOCA will
         simply attach these to your application instance as described
         [above](#configuration-file) and shown
         [below](#accessing-configuration-parameters). Note, however, that any
-        such parameters need to be **MANUALLY VALIDATED**, as unfortunately (or
-        fortunately!) we can't read your mind just yet.
+        such parameters need to be _manually_ validated. The same is true if you
+        include a `custom` section but do _not_ provide a validation model class via
+        the `custom_config_model` parameter when instantiating `Foca`.
         
-        *Example:*
+        _Example:_
         
         ```yaml
         my_custom_param: 'some_value'
         
         my_custom_param_section:
           another_custom_param: 3
           my_custom_list_param:
@@ -384,33 +433,33 @@
             - 3
         ```
         
         ### Accessing configuration parameters
         
         Once the application is created using `foca()`, one can easily access any
         configuration parameters from within the [application
-        context][res-flask-app-context] through `current_app.config['FOCA'] like so:
+        context][res-flask-app-context] through `current_app.config.foca like so:
         
         ```python
         from flask import current_app
         
-        app_config = current_app.config['FOCA']
+        app_config = current_app.config.foca
         
         db = app_config.db
         api = app_config.api
         server = app_config.server
         exceptions = app_config.exceptions
         security = app_config.security
         jobs = app_config.jobs
         log = app_config.log
         app_specific_param = current_app.config['app_specific_param']
         ```
         
         _Outside of the application context_, configuration parameters are available
-        via `app.config['FOCA']` in a similar way.
+        via `app.config.foca` in a similar way.
         
         ### More examples
         
         Apart from the [annotated template][config-template], you can also check
         out the [configuration file][config-petstore] of the [Petstore app][example]
         for another example.
         
@@ -527,25 +576,27 @@
         [img-hint]: images/hint.svg
         [img-logo-banner]: images/logo-banner.svg
         [license]: LICENSE
         [license-apache]: <https://www.apache.org/licenses/LICENSE-2.0>
         [org-elixir-cloud]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai>
         [res-celery]: <http://docs.celeryproject.org/>
         [res-connexion]: <https://github.com/zalando/connexion>
+        [res-datamodel-code-generator]: <https://github.com/koxudaxi/datamodel-code-generator/>
         [res-cors]: <https://flask-cors.readthedocs.io/en/latest/>
         [res-elixir-cloud-coc]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/CODE_OF_CONDUCT.md>
         [res-elixir-cloud-contributing]: <https://github.com/elixir-cloud-aai/elixir-cloud-aai/blob/dev/CONTRIBUTING.md>
         [res-flask]: <http://flask.pocoo.org/>
         [res-flask-app-context]: <https://flask.palletsprojects.com/en/1.1.x/appcontext/>
         [res-foca]: <https://pypi.org/project/foca/>
         [res-jwt]: <https://jwt.io>
         [res-mongo-db]: <https://www.mongodb.com/>
         [res-python-logging]: <https://docs.python.org/3/library/logging.html>
         [res-python-logging-how-to]: <https://docs.python.org/3/howto/logging.html?highlight=yaml#configuring-logging>
         [res-openapi]: <https://www.openapis.org/>
+        [res-pydantic]: <https://pydantic-docs.helpmanual.io/>
         [res-rabbitmq]: <https://www.rabbitmq.com/>
         [res-semver]: <https://semver.org/>
         [res-swagger]: <https://swagger.io/tools/swagger-ui/>
         [res-using-foca]: <https://github.com/elixir-cloud-aai/foca/network/dependents>
         [res-yaml]: <https://yaml.org/>
         
 Keywords: rest api app openapi python microservice
@@ -555,16 +606,16 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
```

### Comparing `foca-0.8.0/foca.egg-info/SOURCES.txt` & `foca-0.9.0/foca.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 MANIFEST.in
 PULL_REQUEST_TEMPLATE.md
 README.md
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
-docker/Dockerfile_py3.6
-docker/Dockerfile_py3.7
-docker/Dockerfile_py3.8
-docker/Dockerfile_py3.9
+docker/Dockerfile
 docs/api/conf.py
 docs/api/index.rst
 examples/petstore/Dockerfile
 examples/petstore/README.md
 examples/petstore/app.py
 examples/petstore/config.yaml
 examples/petstore/controllers.py
 examples/petstore/docker-compose.yaml
+examples/petstore/exceptions.py
 examples/petstore/petstore.yaml
 foca/__init__.py
 foca/foca.py
 foca.egg-info/PKG-INFO
 foca.egg-info/SOURCES.txt
 foca.egg-info/dependency_links.txt
 foca.egg-info/requires.txt
@@ -46,41 +44,47 @@
 foca/utils/db.py
 foca/utils/logging.py
 foca/utils/misc.py
 images/hint.svg
 images/hint.svg.2021_02_16_09_54_34.0.svg
 images/logo-banner.svg
 templates/config.yaml
+tests/__init__.py
 tests/integration_tests.py
 tests/test_foca.py
 tests/api/test_register_openapi.py
 tests/api/controllers/__init__.py
 tests/config/test_config_parser.py
 tests/database/test_register_mongodb.py
 tests/errors/test_errors.py
 tests/factories/test_celery_app.py
 tests/factories/test_connexion_app.py
 tests/models/test_config.py
 tests/security/test_auth.py
 tests/security/test_cors.py
+tests/test_files/__init__.py
 tests/test_files/conf_api.yaml
 tests/test_files/conf_db.yaml
 tests/test_files/conf_invalid_jobs.yaml
 tests/test_files/conf_invalid_log_level.yaml
 tests/test_files/conf_jobs.yaml
 tests/test_files/conf_log.yaml
 tests/test_files/conf_log_invalid.yaml
+tests/test_files/conf_no_yaml.txt
 tests/test_files/conf_valid.yaml
 tests/test_files/conf_valid_cors_disabled.yaml
 tests/test_files/conf_valid_cors_enabled.yaml
+tests/test_files/conf_valid_custom_invalid.yaml
 tests/test_files/empty_conf.yaml
 tests/test_files/invalid.json
 tests/test_files/invalid.openapi.yaml
 tests/test_files/invalid_conf.yaml
 tests/test_files/invalid_conf_db.yaml
+tests/test_files/model_valid.py
+tests/test_files/models_petstore.py
 tests/test_files/openapi_2_petstore.addition.yaml
 tests/test_files/openapi_2_petstore.modified.yaml
 tests/test_files/openapi_2_petstore.original.json
 tests/test_files/openapi_2_petstore.original.yaml
 tests/test_files/openapi_3_petstore.modified.yaml
 tests/test_files/openapi_3_petstore.original.yaml
 tests/utils/test_db.py
```

### Comparing `foca-0.8.0/images/hint.svg` & `foca-0.9.0/images/hint.svg`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/images/hint.svg.2021_02_16_09_54_34.0.svg` & `foca-0.9.0/images/hint.svg.2021_02_16_09_54_34.0.svg`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/images/logo-banner.svg` & `foca-0.9.0/images/logo-banner.svg`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/templates/config.yaml` & `foca-0.9.0/templates/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # FOCA CONFIGURATION
 
-# Available in app context as attributes of `current_app.config['FOCA']`
+# Available in app context as attributes of `current_app.config.foca`
 # Automatically validated via FOCA
 # Cf. https://foca.readthedocs.io/en/latest/modules/foca.models.html
 
 # SERVER CONFIGURATION
 # Cf. https://foca.readthedocs.io/en/latest/modules/foca.models.html#foca.models.config.ServerConfig
 server:
   host: '0.0.0.0'
@@ -96,11 +96,18 @@
       stream: ext://sys.stderr
   root:
     level: 10
     handlers: [console]
 
 
 # CUSTOM APP CONFIGURATION
+# Available in app context as attributes of `current_app.config.foca`
 
-# Available in app context as attributes of `current_app.config['FOCA']`
-# NOT VALIDATED VIA FOCA; if desired, validate parameters in app
-my_custom_param: 'some_value'
+# Can be validated by FOCA by passing a Pydantic model class to the
+# `custom_config_model` parameter in the `foca.Foca()` constructor
+custom:
+  my_param: 'some_value'
+
+# Any other sections/parameters are *not* validated by FOCA; if desired,
+# validate parameters in app
+custom_params_not_validated:
+  my_other_param: 'some_other_value'
```

### Comparing `foca-0.8.0/tests/api/test_register_openapi.py` & `foca-0.9.0/tests/api/test_register_openapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 import pytest
 from yaml import YAMLError
 
 from foca.api.register_openapi import register_openapi
 from foca.models.config import SpecConfig
 
 # Define mock data
-DIR = Path(__file__).parent.parent / "test_files"
-PATH_SPECS_2_YAML_ORIGINAL = str(DIR / "openapi_2_petstore.original.yaml")
-PATH_SPECS_2_YAML_MODIFIED = str(DIR / "openapi_2_petstore.modified.yaml")
-PATH_SPECS_2_JSON_ORIGINAL = str(DIR / "openapi_2_petstore.original.json")
-PATH_SPECS_2_YAML_ADDITION = str(DIR / "openapi_2_petstore.addition.yaml")
-PATH_SPECS_3_YAML_ORIGINAL = str(DIR / "openapi_3_petstore.original.yaml")
-PATH_SPECS_3_YAML_MODIFIED = str(DIR / "openapi_3_petstore.modified.yaml")
-PATH_SPECS_INVALID_JSON = str(DIR / "invalid.json")
-PATH_SPECS_INVALID_YAML = str(DIR / "invalid.openapi.yaml")
-PATH_NOT_FOUND = str(DIR / "does/not/exist.yaml")
+DIR = Path(__file__).parents[1].resolve() / "test_files"
+PATH_SPECS_2_YAML_ORIGINAL = DIR / "openapi_2_petstore.original.yaml"
+PATH_SPECS_2_YAML_MODIFIED = DIR / "openapi_2_petstore.modified.yaml"
+PATH_SPECS_2_JSON_ORIGINAL = DIR / "openapi_2_petstore.original.json"
+PATH_SPECS_2_YAML_ADDITION = DIR / "openapi_2_petstore.addition.yaml"
+PATH_SPECS_3_YAML_ORIGINAL = DIR / "openapi_3_petstore.original.yaml"
+PATH_SPECS_3_YAML_MODIFIED = DIR / "openapi_3_petstore.modified.yaml"
+PATH_SPECS_INVALID_JSON = DIR / "invalid.json"
+PATH_SPECS_INVALID_YAML = DIR / "invalid.openapi.yaml"
+PATH_NOT_FOUND = DIR / "does/not/exist.yaml"
 OPERATION_FIELDS_2 = {"x-swagger-router-controller": "controllers"}
 OPERATION_FIELDS_2_NO_RESOLVE = {"x-swagger-router-controller": YAMLError}
 OPERATION_FIELDS_3 = {"x-openapi-router-controller": "controllers"}
 SECURITY_FIELDS_2 = {"x-apikeyInfoFunc": "controllers.validate_token"}
 SECURITY_FIELDS_3 = {"x-bearerInfoFunc": "controllers.validate_token"}
 APPEND = {
     "info": {
@@ -118,15 +118,15 @@
         with pytest.raises(InvalidSpecification):
             register_openapi(app=app, specs=spec_configs)
 
     def test_openapi_2_json_invalid(self):
         """Registration failing because of invalid JSON spec file."""
         app = App(__name__)
         spec_configs = [SpecConfig(path=PATH_SPECS_INVALID_JSON)]
-        with pytest.raises(YAMLError):
+        with pytest.raises(ValueError):
             register_openapi(app=app, specs=spec_configs)
 
     def test_openapi_not_found(self):
         """Registration failing because spec file is unavailable."""
         app = App(__name__)
         spec_configs = [SpecConfig(path=PATH_NOT_FOUND)]
         with pytest.raises(OSError):
```

### Comparing `foca-0.8.0/tests/database/test_register_mongodb.py` & `foca-0.9.0/tests/database/test_register_mongodb.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/errors/test_errors.py` & `foca-0.9.0/tests/errors/test_errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,54 +99,54 @@
     )
     assert res == EXPECTED_EXCLUDE_RESULT
 
 
 def test__problem_handler_json():
     """Test problem handler with instance of custom, unlisted error."""
     app = Flask(__name__)
-    app.config['FOCA'] = Config()
-    EXPECTED_RESPONSE = app.config['FOCA'].exceptions.mapping[Exception]
+    setattr(app.config, 'foca', Config())
+    EXPECTED_RESPONSE = app.config.foca.exceptions.mapping[Exception]
     with app.app_context():
         res = _problem_handler_json(UnknownException())
         assert isinstance(res, Response)
         assert res.status == '500 INTERNAL SERVER ERROR'
         assert res.mimetype == "application/problem+json"
         response = json.loads(res.data.decode('utf-8'))
         assert response == EXPECTED_RESPONSE
 
 
 def test__problem_handler_json_no_fallback_exception():
     """Test problem handler; unlisted error without fallback."""
     app = Flask(__name__)
-    app.config['FOCA'] = Config()
-    del app.config['FOCA'].exceptions.mapping[Exception]
+    setattr(app.config, 'foca', Config())
+    del app.config.foca.exceptions.mapping[Exception]
     with app.app_context():
         res = _problem_handler_json(UnknownException())
         assert isinstance(res, Response)
         assert res.status == '500 INTERNAL SERVER ERROR'
         assert res.mimetype == "application/problem+json"
         response = res.data.decode("utf-8")
         assert response == ""
 
 
 def test__problem_handler_json_with_public_members():
     """Test problem handler with public members."""
     app = Flask(__name__)
-    app.config['FOCA'] = Config()
-    app.config['FOCA'].exceptions.public_members = PUBLIC_MEMBERS
+    setattr(app.config, 'foca', Config())
+    app.config.foca.exceptions.public_members = PUBLIC_MEMBERS
     with app.app_context():
         res = _problem_handler_json(UnknownException())
         assert isinstance(res, Response)
         assert res.status == '500 INTERNAL SERVER ERROR'
         assert res.mimetype == "application/problem+json"
 
 
 def test__problem_handler_json_with_private_members():
     """Test problem handler with private members."""
     app = Flask(__name__)
-    app.config['FOCA'] = Config()
-    app.config['FOCA'].exceptions.private_members = PRIVATE_MEMBERS
+    setattr(app.config, 'foca', Config())
+    app.config.foca.exceptions.private_members = PRIVATE_MEMBERS
     with app.app_context():
         res = _problem_handler_json(UnknownException())
         assert isinstance(res, Response)
         assert res.status == '500 INTERNAL SERVER ERROR'
         assert res.mimetype == "application/problem+json"
```

### Comparing `foca-0.8.0/tests/factories/test_celery_app.py` & `foca-0.9.0/tests/factories/test_celery_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 
 def test_create_celery_app():
     """Test Connexion app creation."""
     cnx_app = create_connexion_app(CONFIG)
     cel_app = create_celery_app(cnx_app.app)
     assert isinstance(cel_app, Celery)
-    assert cel_app.conf['FOCA'] == CONFIG
+    assert cel_app.conf.foca == CONFIG
```

### Comparing `foca-0.8.0/tests/factories/test_connexion_app.py` & `foca-0.9.0/tests/factories/test_connexion_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def test_add_config_to_connexion_app():
     """Test if app config is updated."""
     cnx_app = App(__name__)
     cnx_app = __add_config_to_connexion_app(cnx_app, CONFIG)
     assert isinstance(cnx_app, App)
-    assert cnx_app.app.config['FOCA'] == CONFIG
+    assert cnx_app.app.config.foca == CONFIG
 
 
 def test_create_connexion_app_without_config():
     """Test Connexion app creation without config."""
     cnx_app = create_connexion_app()
     assert isinstance(cnx_app, App)
```

### Comparing `foca-0.8.0/tests/models/test_config.py` & `foca-0.9.0/tests/models/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,26 +362,26 @@
     assert res.path_out is not None
     assert Path(res.path_out).is_absolute()
 
 
 def test_SpecConfig_full():
     """Test SpecConfig instantiation; full example"""
     res = SpecConfig(**SPEC_CONFIG)
-    assert res.path_out == SPEC_CONFIG['path_out']
+    assert str(res.path_out) == SPEC_CONFIG['path_out']
 
 
 def test_SpecConfig_minimal():
     """Test SpecConfig instantiation; minimal example"""
     res = SpecConfig(path=PATH)
-    assert res.path_out == PATH_MODIFIED
+    assert str(res.path_out) == PATH_MODIFIED
 
 
 def test_SpecConfig_merge():
     """Test SpecConfig instantiation; multiple config files"""
     res = SpecConfig(path=[PATH, PATH_ADDITION])
-    assert res.path_out == PATH_MODIFIED
+    assert str(res.path_out) == PATH_MODIFIED
 
 
 def test_SpecConfig_extra_arg():
     """Test SpecConfig instantiation; extra argument."""
     with pytest.raises(ValidationError):
         SpecConfig(non_existing=PATH)
```

### Comparing `foca-0.8.0/tests/security/test_auth.py` & `foca-0.9.0/tests/security/test_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 class TestValidateToken:
     """Tests for `validate_token()`."""
 
     def test_success_all_validation_checks(self, monkeypatch):
         """Test for validating token successfully via all methods."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
+        setattr(app.config, 'foca', Config())
         request = MagicMock(name='requests')
         request.status_code = 200
         request.return_value.json.return_value = {
             'userinfo_endpoint': MOCK_URL,
             'jwks_uri': MOCK_URL,
         }
         monkeypatch.setattr('requests.get', request)
@@ -146,16 +146,16 @@
         with app.app_context():
             res = validate_token(token=MOCK_TOKEN_HEADER_KID)
             assert res['user_id'] == MOCK_USER_ID
 
     def test_success_any_validation_check(self, monkeypatch):
         """Test for validating token successfully via any method."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
-        app.config['FOCA'].security.auth.\
+        setattr(app.config, 'foca', Config())
+        app.config.foca.security.auth.\
             validation_checks = ValidationChecksEnum.any
         request = MagicMock(name='requests')
         request.status_code = 200
         request.return_value.json.return_value = {
             'userinfo_endpoint': MOCK_URL,
             'jwks_uri': MOCK_URL,
         }
@@ -167,56 +167,56 @@
         with app.app_context():
             res = validate_token(token=MOCK_TOKEN_HEADER_KID)
             assert res['user_id'] == MOCK_USER_ID
 
     def test_no_validation_methods(self):
         """Test for failed validation due to missing validation methods."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
-        app.config['FOCA'].security.auth.validation_methods = []
+        setattr(app.config, 'foca', Config())
+        app.config.foca.security.auth.validation_methods = []
         with app.app_context():
             with pytest.raises(Unauthorized):
                 validate_token(token=MOCK_TOKEN)
 
     def test_invalid_token(self):
         """Test for failed validation due to invalid token."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
+        setattr(app.config, 'foca', Config())
         with app.app_context():
             with pytest.raises(Unauthorized):
                 validate_token(token=MOCK_TOKEN_INVALID)
 
     def test_no_claims(self, monkeypatch):
         """Test for token with no issuer claim."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
+        setattr(app.config, 'foca', Config())
         monkeypatch.setattr(
             'jwt.decode',
             lambda *args, **kwargs: {},
         )
         with app.app_context():
             with pytest.raises(Unauthorized):
                 validate_token(token=MOCK_TOKEN_INVALID)
 
     def test_oidc_config_unavailable(self, monkeypatch):
         """Test for mocking an unavailable OIDC configuration server."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
+        setattr(app.config, 'foca', Config())
         monkeypatch.setattr(
             'requests.get',
             lambda **kwargs: _raise(ConnectionError)
         )
         with app.app_context():
             with pytest.raises(Unauthorized):
                 validate_token(token=MOCK_TOKEN_HEADER_KID)
 
     def test_success_no_subject_claim(self, monkeypatch):
         """Test for validating token without subject claim."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
+        setattr(app.config, 'foca', Config())
         monkeypatch.setattr(
             'jwt.decode',
             lambda *args, **kwargs: MOCK_CLAIMS_NO_SUB,
         )
         request = MagicMock(name='requests')
         request.status_code = 200
         request.return_value.json.return_value = {
@@ -236,15 +236,15 @@
             with pytest.raises(Unauthorized):
                 validate_token(token=MOCK_TOKEN_HEADER_KID)
 
     def test_fail_all_validation_checks_all_required(self, monkeypatch):
         """Test for all token validation methods failing when all methods
         are required to pass."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
+        setattr(app.config, 'foca', Config())
         request = MagicMock(name='requests')
         request.status_code = 200
         request.return_value.json.return_value = {
             'userinfo_endpoint': MOCK_URL,
             'jwks_uri': MOCK_URL,
         }
         monkeypatch.setattr('requests.get', request)
@@ -260,16 +260,16 @@
             with pytest.raises(Unauthorized):
                 validate_token(token=MOCK_TOKEN_HEADER_KID)
 
     def test_fail_all_validation_checks_any_required(self, monkeypatch):
         """Test for all token validation methods failing when any method
         is required to pass."""
         app = Flask(__name__)
-        app.config['FOCA'] = Config()
-        app.config['FOCA'].security.auth.\
+        setattr(app.config, 'foca', Config())
+        app.config.foca.security.auth.\
             validation_checks = ValidationChecksEnum.any
         request = MagicMock(name='requests')
         request.status_code = 200
         request.return_value.json.return_value = {
             'userinfo_endpoint': MOCK_URL,
             'jwks_uri': MOCK_URL,
         }
```

### Comparing `foca-0.8.0/tests/test_files/conf_api.yaml` & `foca-0.9.0/tests/test_files/conf_api.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/conf_invalid_log_level.yaml` & `foca-0.9.0/tests/test_files/conf_invalid_log_level.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/conf_valid.yaml` & `foca-0.9.0/tests/test_files/conf_valid.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/invalid.json` & `foca-0.9.0/tests/test_files/invalid.json`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/invalid.openapi.yaml` & `foca-0.9.0/tests/test_files/invalid.openapi.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/openapi_2_petstore.addition.yaml` & `foca-0.9.0/tests/test_files/openapi_2_petstore.addition.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/openapi_2_petstore.modified.yaml` & `foca-0.9.0/tests/test_files/openapi_2_petstore.modified.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/openapi_2_petstore.original.json` & `foca-0.9.0/tests/test_files/openapi_2_petstore.original.json`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/openapi_2_petstore.original.yaml` & `foca-0.9.0/tests/test_files/openapi_2_petstore.original.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/openapi_3_petstore.modified.yaml` & `foca-0.9.0/tests/test_files/openapi_3_petstore.modified.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_files/openapi_3_petstore.original.yaml` & `foca-0.9.0/tests/test_files/openapi_3_petstore.original.yaml`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/test_foca.py` & `foca-0.9.0/tests/test_foca.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,134 @@
 """Tests for `foca.py` module."""
 
-import pathlib
+from pathlib import Path
 import pytest
 import shutil
-import os
 
 from connexion import App
 from pydantic import ValidationError
 from pymongo.collection import Collection
 from pymongo.database import Database
-from yaml import safe_load, safe_dump, YAMLError
+from yaml import (
+    safe_load,
+    safe_dump,
+)
 
-from foca.foca import foca
+from foca import Foca
 
-DIR = pathlib.Path(__file__).parent / "test_files"
+DIR = Path(__file__).parent / "test_files"
 PATH_SPECS_2_YAML_ORIGINAL = str(DIR / "openapi_2_petstore.original.yaml")
 PATH_SPECS_2_YAML_MODIFIED = str(DIR / "openapi_2_petstore.modified.yaml")
 PATH_SPECS_INVALID_OPENAPI = str(DIR / "invalid_openapi_2.yaml")
 EMPTY_CONF = str(DIR / "empty_conf.yaml")
 INVALID_CONF = str(DIR / "invalid_conf.yaml")
 VALID_CONF = str(DIR / "conf_valid.yaml")
 VALID_DB_CONF = str(DIR / "conf_db.yaml")
 INVALID_DB_CONF = str(DIR / "invalid_conf_db.yaml")
 INVALID_LOG_CONF = str(DIR / "conf_invalid_log_level.yaml")
 JOBS_CONF = str(DIR / "conf_jobs.yaml")
 INVALID_JOBS_CONF = str(DIR / "conf_invalid_jobs.yaml")
 API_CONF = str(DIR / "conf_api.yaml")
-VALID_CORS_DIS_CONF = str(DIR / "conf_valid_cors_disabled.yaml")
-VALID_CORS_ENA_CONF = str(DIR / "conf_valid_cors_enabled.yaml")
+VALID_CORS_CONF_DISABLED = str(DIR / "conf_valid_cors_disabled.yaml")
+VALID_CORS_CONF_ENABLED = str(DIR / "conf_valid_cors_enabled.yaml")
 
 
-def create_temporary_copy(path, CONF):
+def create_modified_api_conf(path, temp_dir, api_specs_in, api_specs_out):
     """Create a copy of a configuration YAML file"""
-    temp_path = os.path.join(DIR, 'temp_test.yaml')
+    temp_path = Path(temp_dir) / 'temp_test.yaml'
     shutil.copy2(path, temp_path)
     with open(temp_path, 'r+') as conf_file:
         conf = safe_load(conf_file)
-        conf["api"]["specs"][0]["path"] = CONF
-        conf["api"]["specs"][0]["path_out"] = PATH_SPECS_2_YAML_MODIFIED
+        conf["api"]["specs"][0]["path"] = api_specs_in
+        conf["api"]["specs"][0]["path_out"] = api_specs_out
         conf_file.seek(0)
         safe_dump(conf, conf_file)
         conf_file.truncate()
     return temp_path
 
 
 def test_foca_output_defaults():
     """Ensure foca() returns a Connexion app instance; defaults only."""
-    app = foca()
+    foca = Foca()
+    app = foca.create_app()
     assert isinstance(app, App)
 
 
 def test_foca_empty_conf():
     """Ensure foca() require non-empty configuration parameters (if a field is
     present)"""
+    foca = Foca(config_file=EMPTY_CONF)
     with pytest.raises(ValidationError):
-        foca(EMPTY_CONF)
+        foca.create_app()
 
 
 def test_foca_invalid_structure():
     """Test foca(); invalid configuration file structure."""
-    with pytest.raises(YAMLError):
-        foca(INVALID_CONF)
+    foca = Foca(config_file=INVALID_CONF)
+    with pytest.raises(ValueError):
+        foca.create_app()
 
 
 def test_foca_invalid_log():
     """Test foca(); invalid log field"""
+    foca = Foca(config_file=INVALID_LOG_CONF)
     with pytest.raises(ValidationError):
-        foca(INVALID_LOG_CONF)
+        foca.create_app()
 
 
 def test_foca_jobs():
     """Ensure foca() returns a Connexion app instance; valid jobs field"""
-    app = foca(JOBS_CONF)
+    foca = Foca(config_file=JOBS_CONF)
+    app = foca.create_app()
     assert isinstance(app, App)
 
 
 def test_foca_invalid_jobs():
     """Test foca(); invalid jobs field"""
+    foca = Foca(config_file=INVALID_JOBS_CONF)
     with pytest.raises(ValidationError):
-        foca(INVALID_JOBS_CONF)
+        foca.create_app()
 
 
-def test_foca_api():
+def test_foca_api(tmpdir):
     """Ensure foca() returns a Connexion app instance; valid api field"""
-    temp_file = create_temporary_copy(
+    temp_file = create_modified_api_conf(
         API_CONF,
+        tmpdir,
         PATH_SPECS_2_YAML_ORIGINAL,
+        PATH_SPECS_2_YAML_MODIFIED,
     )
-    app = foca(temp_file)
+    foca = Foca(config_file=temp_file)
+    app = foca.create_app()
     assert isinstance(app, App)
-    os.remove(temp_file)
 
 
 def test_foca_db():
     """Ensure foca() returns a Connexion app instance; valid db field"""
-    app = foca(VALID_DB_CONF)
-    my_db = app.app.config['FOCA'].db.dbs['my-db']
+    foca = Foca(config_file=VALID_DB_CONF)
+    app = foca.create_app()
+    my_db = app.app.config.foca.db.dbs['my-db']
     my_coll = my_db.collections['my-col-1']
     assert isinstance(my_db.client, Database)
     assert isinstance(my_coll.client, Collection)
     assert isinstance(app, App)
 
 
 def test_foca_invalid_db():
     """Test foca(); invalid db field"""
+    foca = Foca(config_file=INVALID_DB_CONF)
     with pytest.raises(ValidationError):
-        foca(INVALID_DB_CONF)
+        foca.create_app()
 
 
 def test_foca_CORS_enabled():
     """Ensures CORS is enabled for Microservice"""
-    app = foca(VALID_CORS_ENA_CONF)
-    assert app.app.config['FOCA'].security.cors.enabled is True
+    foca = Foca(config_file=VALID_CORS_CONF_ENABLED)
+    app = foca.create_app()
+    assert app.app.config.foca.security.cors.enabled is True
 
 
 def test_foca_CORS_disabled():
     """Ensures CORS is disabled if user explicitly mentions"""
-    app = foca(VALID_CORS_DIS_CONF)
-    assert app.app.config['FOCA'].security.cors.enabled is False
+    foca = Foca(config_file=VALID_CORS_CONF_DISABLED)
+    app = foca.create_app()
+    assert app.app.config.foca.security.cors.enabled is False
```

### Comparing `foca-0.8.0/tests/utils/test_db.py` & `foca-0.9.0/tests/utils/test_db.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/utils/test_logging.py` & `foca-0.9.0/tests/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `foca-0.8.0/tests/utils/test_misc.py` & `foca-0.9.0/tests/utils/test_misc.py`

 * *Files identical despite different names*

