# Comparing `tmp/ansibleguy_webui-0.0.20.tar.gz` & `tmp/ansibleguy_webui-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansibleguy_webui-0.0.20.tar", last modified: Mon May 13 20:10:02 2024, max compression
+gzip compressed data, was "ansibleguy_webui-0.0.21.tar", last modified: Mon May 20 16:18:42 2024, max compression
```

## Comparing `ansibleguy_webui-0.0.20.tar` & `ansibleguy_webui-0.0.21.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43936 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 20:10:00.000000 ansibleguy_webui-0.0.20/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.428903 ansibleguy_webui-0.0.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.432903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.432903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.436903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21503 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    18404 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.436903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/form_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/hardcoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.440903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/features.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.440903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.440903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    40135 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
--rw-r--r--   0 runner    (1001) docker     (127)    14987 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.428903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw.css
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw_mobile.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/img/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.444903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    17643 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw.js
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw_nav.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/credentials.js
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/edit.js
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/logs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/manage.js
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/repository.js
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/login.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/alert.js
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/api_key.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/environment.js
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/permission.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/body.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.448903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/autoRefresh.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/add.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/add_dir.html
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/add_git.html
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/copy.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/delete.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/download.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/expand.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/return.html
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/run.html
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/sort.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/icon/stop.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/button/refresh.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/alert.html
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/alert.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/403.html
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/error/js_disabled.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/fallback.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.452903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/job.html
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/snippet.html
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/snippet_test.html
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/head.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials.html
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/manage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository.html
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/remember_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/saml.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/rest_framework/api.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/alert.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/alert_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/api_key.html
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/permission.html
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/permission_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/environment.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.456903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/form_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.460903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/subps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util_no_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.460903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/handle_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/web_serve_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-13 20:08:53.000000 ansibleguy_webui-0.0.20/src/ansibleguy-webui/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:10:02.464903 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43936 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 20:10:02.000000 ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.680671 ansibleguy_webui-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)    33252 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43936 2024-05-20 16:18:42.680671 ansibleguy_webui-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 16:18:40.000000 ansibleguy_webui-0.0.21/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:18:42.680671 ansibleguy_webui-0.0.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.648671 ansibleguy_webui-0.0.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.652671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.652671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.656671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22138 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15453 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20317 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/job_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.656671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/form_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/hardcoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.656671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/db_sqlite_patched/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.660671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.660671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/play_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/play_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.660671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    40135 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0004_v0_0_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0005_v0_0_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14987 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/job_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.648671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/css/aw.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/css/aw_mobile.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14912 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/img/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    18339 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/aw.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/aw_nav.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/credentials.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/edit.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/logs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/manage.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/repository.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/login.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/alert.js
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/api_key.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/environment.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/permission.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/body.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.664671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/autoRefresh.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.668671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/add.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/add_dir.html
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/add_git.html
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/copy.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/download.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/expand.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/return.html
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/run.html
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/sort.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/icon/stop.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/button/refresh.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.668671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/django_saml2_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/django_saml2_auth/denied.html
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/django_saml2_auth/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/django_saml2_auth/signout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.668671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/email/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/email/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/email/alert.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.668671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/error/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/error/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/error/js_disabled.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/fallback.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.668671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/job.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/snippet.html
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/snippet_test.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/head.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.672671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/credentials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/manage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/repository.html
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.672671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/password_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/remember_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/saml.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.672671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/rest_framework/api.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.672671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/alert_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/api_key.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/permission.html
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/permission_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.672671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/system/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/system/environment.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.672671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templatetags/form_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templatetags/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.676671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/subps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/util_no_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.676671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.676671 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/handle_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/web_serve_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-20 16:17:32.000000 ansibleguy_webui-0.0.21/src/ansibleguy-webui/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:18:42.676671 ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43936 2024-05-20 16:18:42.000000 ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-20 16:18:42.000000 ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:18:42.000000 ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 16:18:42.000000 ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-20 16:18:42.000000 ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/top_level.txt
```

### Comparing `ansibleguy_webui-0.0.20/LICENSE.txt` & `ansibleguy_webui-0.0.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/PKG-INFO` & `ansibleguy_webui-0.0.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansibleguy-webui
-Version: 0.0.20
+Version: 0.0.21
 Summary: Basic WebUI for using Ansible
 Author-email: AnsibleGuy <contact@ansibleguy.net>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -765,15 +765,15 @@
 
   - [x] Execute Ansible using [ansible-runner](https://ansible.readthedocs.io/projects/runner/en/latest/python_interface/)
 
     - [x] Scheduled execution (Cron-Format)
 
     - [x] Manual/immediate execution
 
-    - [ ] Custom Execution-Forms
+    - [x] Custom Execution-Forms
 
     - [ ] Support for [ad-hoc commands](https://docs.ansible.com/ansible/latest/command_guide/intro_adhoc.html)
 
     - [ ] Support for [Process-Isolation](https://ansible.readthedocs.io/projects/runner/en/stable/standalone/#running-with-process-isolation)
 
   - [x] Job Logging
```

### Comparing `ansibleguy_webui-0.0.20/README.md` & `ansibleguy_webui-0.0.21/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
   - [x] Execute Ansible using [ansible-runner](https://ansible.readthedocs.io/projects/runner/en/latest/python_interface/)
 
     - [x] Scheduled execution (Cron-Format)
 
     - [x] Manual/immediate execution
 
-    - [ ] Custom Execution-Forms
+    - [x] Custom Execution-Forms
 
     - [ ] Support for [ad-hoc commands](https://docs.ansible.com/ansible/latest/command_guide/intro_adhoc.html)
 
     - [ ] Support for [Process-Isolation](https://ansible.readthedocs.io/projects/runner/en/stable/standalone/#running-with-process-isolation)
 
   - [x] Job Logging
```

#### html2text {}

```diff
@@ -31,15 +31,15 @@
 _l_a_t_e_s_t_/_C_O_N_T_R_I_B_U_T_E_._m_d_)_ _-_-_-_-_ _#_#_ _R_o_a_d_m_a_p_ _-_ _[_x_]_ _A_n_s_i_b_l_e_ _C_o_n_f_i_g_ _-_ _[_x_]_ _S_t_a_t_i_c
 _P_l_a_y_b_o_o_k_-_D_i_r_e_c_t_o_r_y_ _-_ _[_x_]_ _G_i_t_ _R_e_p_o_s_i_t_o_r_y_ _s_u_p_p_o_r_t_ _-_ _[_ _]_ _U_s_e_r_s_ _-_ _[_x_]_ _M_a_n_a_g_e_m_e_n_t
 _i_n_t_e_r_f_a_c_e_ _(_D_j_a_n_g_o_ _b_u_i_l_t_-_i_n_)_ _-_ _[_x_]_ _G_r_o_u_p_s_ _&_ _J_o_b_ _P_e_r_m_i_s_s_i_o_n_s_ _-_ _[_ _]_ _[_L_D_A_P
 _i_n_t_e_g_r_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_j_a_n_g_o_-_a_u_t_h_-_l_d_a_p_/_d_j_a_n_g_o_-_a_u_t_h_-_l_d_a_p_)_ _-_ _[_x_]_ _[_S_A_M_L
 _S_S_O_ _i_n_t_e_g_r_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_g_r_a_f_a_n_a_/_d_j_a_n_g_o_-_s_a_m_l_2_-_a_u_t_h_)_ _-_ _[_ _]_ _J_o_b_s_ _-_ _[_x_]
 _E_x_e_c_u_t_e_ _A_n_s_i_b_l_e_ _u_s_i_n_g_ _[_a_n_s_i_b_l_e_-_r_u_n_n_e_r_]_(_h_t_t_p_s_:_/_/_a_n_s_i_b_l_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_p_r_o_j_e_c_t_s_/
 _r_u_n_n_e_r_/_e_n_/_l_a_t_e_s_t_/_p_y_t_h_o_n___i_n_t_e_r_f_a_c_e_/_)_ _-_ _[_x_]_ _S_c_h_e_d_u_l_e_d_ _e_x_e_c_u_t_i_o_n_ _(_C_r_o_n_-_F_o_r_m_a_t_)_ _-_ 
-_[_x_]_ _M_a_n_u_a_l_/_i_m_m_e_d_i_a_t_e_ _e_x_e_c_u_t_i_o_n_ _-_ _[_ _]_ _C_u_s_t_o_m_ _E_x_e_c_u_t_i_o_n_-_F_o_r_m_s_ _-_ _[_ _]_ _S_u_p_p_o_r_t_ _f_o_r_ 
+_[_x_]_ _M_a_n_u_a_l_/_i_m_m_e_d_i_a_t_e_ _e_x_e_c_u_t_i_o_n_ _-_ _[_x_]_ _C_u_s_t_o_m_ _E_x_e_c_u_t_i_o_n_-_F_o_r_m_s_ _-_ _[_ _]_ _S_u_p_p_o_r_t_ _f_o_r_ 
 _[_a_d_-_h_o_c_ _c_o_m_m_a_n_d_s_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_n_s_i_b_l_e_._c_o_m_/_a_n_s_i_b_l_e_/_l_a_t_e_s_t_/_c_o_m_m_a_n_d___g_u_i_d_e_/
 _i_n_t_r_o___a_d_h_o_c_._h_t_m_l_)_ _-_ _[_ _]_ _S_u_p_p_o_r_t_ _f_o_r_ _[_P_r_o_c_e_s_s_-_I_s_o_l_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
 _a_n_s_i_b_l_e_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_p_r_o_j_e_c_t_s_/_r_u_n_n_e_r_/_e_n_/_s_t_a_b_l_e_/_s_t_a_n_d_a_l_o_n_e_/_#_r_u_n_n_i_n_g_-_w_i_t_h_-
 _p_r_o_c_e_s_s_-_i_s_o_l_a_t_i_o_n_)_ _-_ _[_x_]_ _J_o_b_ _L_o_g_g_i_n_g_ _-_ _[_x_]_ _W_r_i_t_e_ _j_o_b_ _m_e_t_a_d_a_t_a_ _t_o_ _d_a_t_a_b_a_s_e_ _-_ _[_x_]
 _W_r_i_t_e_ _f_u_l_l_ _j_o_b_-_l_o_g_s_ _t_o_ _F_i_l_e_s_y_s_t_e_m_ _-_ _[_x_]_ _S_e_c_r_e_t_ _h_a_n_d_l_i_n_g_ _(_C_o_n_n_e_c_t_,_ _B_e_c_o_m_e_,
 _V_a_u_l_t_)_ _-_ _[_x_]_ _U_s_e_r_-_s_p_e_c_i_f_i_c_ _j_o_b_ _c_r_e_d_e_n_t_i_a_l_s_ _-_ _[_x_]_ _A_l_e_r_t_i_n_g_ _o_n_ _F_a_i_l_u_r_e_ _-_ _[_x_]_ _E_-
 _M_a_i_l_ _-_ _[_x_]_ _S_u_p_p_o_r_t_ _f_o_r_ _e_x_t_e_r_n_a_l_ _P_l_u_g_i_n_s_ _(_*_s_i_m_p_l_e_ _I_n_t_e_r_f_a_c_e_ _f_o_r_ _S_c_r_i_p_t_s_*_)_ _-_ _[_ _]
```

### Comparing `ansibleguy_webui-0.0.20/pyproject.toml` & `ansibleguy_webui-0.0.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/__main__.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/__main__.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/admin.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/admin.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/alert.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/alert.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rest_framework.generics import GenericAPIView
 from rest_framework import serializers
 from rest_framework.response import Response
 from drf_spectacular.utils import extend_schema, OpenApiResponse
 
 from aw.model.job import Job
 from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user, api_docs_put, api_docs_delete, \
-    api_docs_post
+    api_docs_post, validate_no_xss
 from aw.utils.permission import has_manager_privileges
 from aw.model.alert import BaseAlert, AlertPlugin, AlertGlobal, AlertGroup, AlertUser
 
 
 def update_jobs(alert: BaseAlert, job_ids: list):
     jobs = []
     for job_id in job_ids:
@@ -193,14 +193,21 @@
 
 
 class AlertUserWriteRequest(BaseAlertWriteRequest):
     class Meta:
         model = AlertUser
         fields = AlertUser.api_fields_write
 
+    def validate(self, attrs: dict):
+        for field in AlertUser.api_fields_write:
+            if field in attrs:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
 
 class APIAlertUser(GenericAPIView):
     http_method_names = ['get', 'post']
     serializer_class = AlertUserReadResponse
     permission_classes = API_PERMISSION
 
     @staticmethod
@@ -348,14 +355,21 @@
 
 
 class AlertGlobalWriteRequest(BaseAlertWriteRequest):
     class Meta:
         model = AlertGlobal
         fields = AlertGlobal.api_fields_write
 
+    def validate(self, attrs: dict):
+        for field in AlertGlobal.api_fields_write:
+            if field in attrs:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
 
 class APIAlertGlobal(GenericAPIView):
     http_method_names = ['get', 'post']
     serializer_class = AlertGlobalReadResponse
     permission_classes = API_PERMISSION
 
     @staticmethod
@@ -509,14 +523,21 @@
 
 
 class AlertGroupWriteRequest(BaseAlertWriteRequest):
     class Meta:
         model = AlertGroup
         fields = AlertGroup.api_fields_write
 
+    def validate(self, attrs: dict):
+        for field in AlertGroup.api_fields_write:
+            if field in attrs:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
 
 class APIAlertGroup(GenericAPIView):
     http_method_names = ['get', 'post']
     serializer_class = AlertGroupReadResponse
     permission_classes = API_PERMISSION
 
     @staticmethod
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/base.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ObjectDoesNotExist
 from django.http import JsonResponse
+from django.utils.html import escape as escape_html
 from rest_framework import serializers
+from rest_framework.exceptions import ValidationError
 from rest_framework.permissions import IsAuthenticated
 from rest_framework_api_key.permissions import BaseHasAPIKey
 from drf_spectacular.utils import OpenApiResponse
 
 from aw.model.api import AwAPIKey
 from aw.base import USERS, GROUPS
+from aw.utils.util import is_set
 
 
 class HasAwAPIKey(BaseHasAPIKey):
     model = AwAPIKey
 
 
 API_PERMISSION = [IsAuthenticated | HasAwAPIKey]
@@ -84,7 +87,12 @@
         403: OpenApiResponse(response=GenericResponse, description=f'Not privileged to create {item}'),
     }
 
 
 def not_implemented(*args, **kwargs):
     del args, kwargs
     return JsonResponse({'error': 'Not yet implemented'}, status=404)
+
+
+def validate_no_xss(value: str, field: str):
+    if is_set(value) and isinstance(value, str) and value != escape_html(value):
+        raise ValidationError(f"Found illegal characters in field '{field}'")
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/credentials.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rest_framework.response import Response
 from drf_spectacular.utils import extend_schema, OpenApiResponse, OpenApiParameter
 
 from aw.model.job import Job, JobExecution
 from aw.model.job_credential import BaseJobCredentials, JobUserCredentials, JobGlobalCredentials
 from aw.model.permission import CHOICE_PERMISSION_READ, CHOICE_PERMISSION_WRITE, CHOICE_PERMISSION_DELETE
 from aw.api_endpoints.base import API_PERMISSION, get_api_user, GenericResponse, BaseResponse, api_docs_delete, \
-    api_docs_put, api_docs_post
+    api_docs_put, api_docs_post, validate_no_xss
 from aw.utils.permission import has_credentials_permission, has_manager_privileges
 from aw.config.hardcoded import SECRET_HIDDEN
 from aw.utils.util import is_null
 from aw.base import USERS
 
 
 class JobGlobalCredentialsReadResponse(serializers.ModelSerializer):
@@ -46,20 +46,34 @@
 
     name = serializers.CharField(validators=[])  # uc on update
     vault_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
     become_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
     connect_pass = serializers.CharField(max_length=100, required=False, default=None, allow_blank=True)
     ssh_key = serializers.CharField(max_length=5000, required=False, default=None, allow_blank=True)
 
+    def validate(self, attrs: dict):
+        for field in JobGlobalCredentials.api_fields_write:
+            if field in attrs and field not in BaseJobCredentials.SECRET_ATTRS:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
 
 class JobUserCredentialsWriteRequest(JobGlobalCredentialsWriteRequest):
     class Meta:
         model = JobUserCredentials
         fields = JobUserCredentials.api_fields_write
 
+    def validate(self, attrs: dict):
+        for field in JobUserCredentials.api_fields_write:
+            if field in attrs and field not in BaseJobCredentials.SECRET_ATTRS:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
 
 def are_global_credentials(request) -> bool:
     if 'global' in request.GET and request.GET['global'] != 'true':
         return False
 
     return True
 
@@ -364,15 +378,15 @@
                 status=400,
             )
 
         try:
             # not working with password properties: 'Job.objects.filter(id=job_id).update(**serializer.data)'
             for field, value in serializer.validated_data.items():
                 if field in BaseJobCredentials.SECRET_ATTRS:
-                    if is_null(value) or value == SECRET_HIDDEN:
+                    if (field not in BaseJobCredentials.EMPTY_ATTRS and is_null(value)) or value == SECRET_HIDDEN:
                         value = getattr(credentials, field)
 
                     elif field == 'ssh_key':
                         value = _validate_and_fix_ssh_key(value)
                         if value is None:
                             return Response(
                                 data={'msg': f"Provided {_log_global_user(are_global)} ssh-key is not valid'"},
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/filesystem.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/filesystem.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from re import match as regex_match
+
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.utils import IntegrityError
 from rest_framework.views import APIView
 from rest_framework import serializers
 from rest_framework.response import Response
+from rest_framework.exceptions import ValidationError
 from drf_spectacular.utils import extend_schema, OpenApiResponse, OpenApiParameter
 
 from aw.config.hardcoded import JOB_EXECUTION_LIMIT
 from aw.model.job import Job, JobExecution
 from aw.model.permission import CHOICE_PERMISSION_READ, CHOICE_PERMISSION_EXECUTE, \
     CHOICE_PERMISSION_WRITE, CHOICE_PERMISSION_DELETE
 from aw.model.job_credential import JobGlobalCredentials
 from aw.api_endpoints.base import API_PERMISSION, get_api_user, BaseResponse, GenericResponse, \
-    LogDownloadResponse, api_docs_put, api_docs_delete, api_docs_post
+    LogDownloadResponse, api_docs_put, api_docs_delete, api_docs_post, validate_no_xss
 from aw.api_endpoints.job_util import get_viewable_jobs_serialized, JobReadResponse, get_job_executions_serialized, \
     JobExecutionReadResponse, get_viewable_jobs, get_job_execution_serialized, get_log_file_content
 from aw.utils.permission import has_job_permission, has_credentials_permission, has_manager_privileges
 from aw.execute.queue import queue_add
 from aw.execute.util import update_status, is_execution_status
 from aw.utils.util import is_set, ansible_log_html, ansible_log_text
 from aw.base import USERS
@@ -24,14 +27,42 @@
 class JobWriteRequest(serializers.ModelSerializer):
     class Meta:
         model = Job
         fields = Job.api_fields_write
 
     name = serializers.CharField(validators=[])  # uc on update
 
+    def validate(self, attrs: dict):
+        for field in Job.api_fields_write:
+            if field in attrs:
+                validate_no_xss(value=attrs[field], field=field)
+
+        for prompt_field in ['execution_prompts_required', 'execution_prompts_optional']:
+            if prompt_field in attrs and is_set(attrs[prompt_field]):
+                if regex_match(Job.execution_prompts_regex, attrs[prompt_field]) is None:
+                    raise ValidationError('Invalid execution prompt pattern')
+
+                translated = []
+                for field in attrs[prompt_field].split(','):
+                    if field in Job.execution_prompt_aliases:
+                        translated.append(Job.execution_prompt_aliases[field])
+
+                    else:
+                        translated.append(field)
+
+                attrs[prompt_field] = ','.join(translated)
+
+        return attrs
+
+
+class JobExecutionRequest(serializers.ModelSerializer):
+    class Meta:
+        model = JobExecution
+        fields = JobExecution.api_fields_exec
+
 
 def _find_job(job_id: int) -> (Job, None):
     try:
         return Job.objects.get(id=job_id)
 
     except ObjectDoesNotExist:
         return None
@@ -274,14 +305,15 @@
 
         return Response(data={'msg': f"Job with ID {job_id} does not exist"}, status=404)
 
     @extend_schema(
         request=None,
         responses={
             200: OpenApiResponse(JobReadResponse, description='Job execution queued'),
+            400: OpenApiResponse(JobReadResponse, description='Bad parameters provided'),
             403: OpenApiResponse(JobReadResponse, description='Not privileged to execute the job'),
             404: OpenApiResponse(JobReadResponse, description='Job does not exist'),
         },
         summary='Execute a job.',
         operation_id='job_execute'
     )
     def post(self, request, job_id: int):
@@ -289,15 +321,31 @@
         try:
             job = _find_job(job_id)
 
             if job is not None:
                 if not has_job_permission(user=user, job=job, permission_needed=CHOICE_PERMISSION_EXECUTE):
                     return Response(data={'msg': f"Not privileged to execute the job '{job.name}'"}, status=403)
 
-                queue_add(job=job, user=user)
+                if len(request.data) > 0:
+                    serializer = JobExecutionRequest(data=request.data)
+                    if not serializer.is_valid():
+                        return Response(
+                            data={'msg': f"Provided job-execution data is not valid: '{serializer.errors}'"},
+                            status=400,
+                        )
+
+                    execution = JobExecution(
+                        user=user, job=job, **serializer.validated_data,
+                    )
+
+                else:
+                    execution = JobExecution(user=user, job=job, comment='Triggered')
+
+                execution.save()
+                queue_add(execution=execution)
                 return Response(data={'msg': f"Job '{job.name}' execution queued"}, status=200)
 
         except ObjectDoesNotExist:
             pass
 
         return Response(data={'msg': f"Job with ID '{job_id}' does not exist"}, status=404)
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/job_util.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/job_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 class JobExecutionReadResponse(serializers.ModelSerializer):
     class Meta:
         model = JobExecution
         fields = JobExecution.api_fields_read
 
     job_name = serializers.CharField(required=False)
     job_comment = serializers.CharField(required=False)
+    comment = serializers.CharField(required=False)
     user_name = serializers.CharField(required=False)
     status_name = serializers.CharField(required=False)
     failed = serializers.BooleanField(required=False)
     error_s = serializers.CharField(required=False)
     error_m = serializers.CharField(required=False)
     time_start = serializers.CharField(required=False)
     time_fin = serializers.CharField(required=False)
@@ -44,14 +45,15 @@
 
 
 def get_job_execution_serialized(execution: JobExecution) -> dict:
     serialized = JobExecutionReadResponse(instance=execution).data
     serialized['job'] = execution.job.id
     serialized['job_name'] = execution.job.name
     serialized['job_comment'] = execution.job.comment
+    serialized['comment'] = execution.comment
     serialized['user'] = execution.user.id if execution.user is not None else None
     serialized['user_name'] = execution.user_name
     serialized['time_start'] = execution.time_created_str
     serialized['time_fin'] = None
     serialized['failed'] = None
     serialized['error_s'] = None
     serialized['error_m'] = None
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/key.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/key.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/permission.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from drf_spectacular.utils import extend_schema
 
 from aw.model.job import Job
 from aw.model.job_credential import JobGlobalCredentials
 from aw.model.permission import JobPermission, JobPermissionMapping, JobPermissionMemberUser, \
     JobPermissionMemberGroup, JobCredentialsPermissionMapping, JobRepositoryPermissionMapping
 from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user, api_docs_put, api_docs_delete, \
-    api_docs_post
+    api_docs_post, validate_no_xss
 from aw.utils.permission import has_manager_privileges
 from aw.utils.util import is_set
 from aw.base import USERS, GROUPS
 from aw.model.repository import Repository
 
 
 class PermissionReadResponse(serializers.ModelSerializer):
@@ -56,14 +56,21 @@
         )
         self.fields['repositories'] = serializers.MultipleChoiceField(
             choices=[repo.id for repo in Repository.objects.all()]
         )
         self.fields['users'] = serializers.MultipleChoiceField(choices=[user.id for user in USERS.objects.all()])
         self.fields['groups'] = serializers.MultipleChoiceField(choices=[group.id for group in GROUPS.objects.all()])
 
+    def validate(self, attrs: dict):
+        for field in JobPermission.api_fields_write:
+            if field in attrs:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
     @staticmethod
     def create_or_update(validated_data: dict, perm: JobPermission = None):
         # pylint: disable=R0912,R0915
         if 'permission' in validated_data:
             permission = validated_data['permission']
         else:
             permission = JobPermission.permission_default
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/repository.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rest_framework.generics import GenericAPIView
 from rest_framework import serializers
 from rest_framework.response import Response
 from drf_spectacular.utils import extend_schema, OpenApiResponse, OpenApiParameter
 
 from aw.model.repository import Repository
 from aw.api_endpoints.base import API_PERMISSION, GenericResponse, get_api_user, LogDownloadResponse, api_docs_put, \
-    api_docs_delete, api_docs_post
+    api_docs_delete, api_docs_post, validate_no_xss
 from aw.utils.permission import has_manager_privileges, has_repository_permission, get_viewable_repositories
 from aw.model.job import Job
 from aw.utils.util import unset_or_null, is_set
 from aw.model.permission import CHOICE_PERMISSION_READ, CHOICE_PERMISSION_WRITE, CHOICE_PERMISSION_DELETE, \
     CHOICE_PERMISSION_EXECUTE
 from aw.execute.repository import api_update_repository
 from aw.api_endpoints.job_util import get_log_file_content
@@ -23,14 +23,21 @@
 class RepositoryWriteRequest(serializers.ModelSerializer):
     class Meta:
         model = Repository
         fields = Repository.api_fields_write
 
     name = serializers.CharField(validators=[])  # uc on update
 
+    def validate(self, attrs: dict):
+        for field in Repository.api_fields_write:
+            if field in attrs:
+                validate_no_xss(value=attrs[field], field=field)
+
+        return attrs
+
 
 class RepositoryReadResponse(RepositoryWriteRequest):
     class Meta:
         model = Repository
         fields = Repository.api_fields_read
 
     rtype_name = serializers.CharField()
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/api_endpoints/system.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/api_endpoints/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,18 +100,18 @@
             )
 
         config_db = get_config_from_db()
         try:
             changed = False
             for setting, value in serializer.validated_data.items():
                 if setting in SystemConfig.SECRET_ATTRS:
-                    if is_null(value) or value == SECRET_HIDDEN:
+                    if (setting not in SystemConfig.EMPTY_ATTRS and is_null(value)) or value == SECRET_HIDDEN:
                         value = getattr(config_db, setting)
 
-                if is_set(value) and str(config[setting]) != str(value):
+                if (setting in SystemConfig.EMPTY_ATTRS or is_set(value)) and str(config[setting]) != str(value):
                     setattr(config_db, setting, value)
                     changed = True
 
             if changed:
                 log(msg='System config changed - updating', level=5)
                 config_db.save()
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/apps.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/apps.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/defaults.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/environment.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/environment.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/form_metadata.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/form_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,16 @@
             'mode_check': 'Check Mode (Try Run)',
             'cmd_args': 'Commandline Arguments',
             'enabled': 'Schedule Enabled',
             'tags_skip': 'Skip Tags',
             'credentials_needed': 'Needs Credentials',
             'credentials_default': 'Default Job Credentials',
             'credentials_category': 'Credentials Category',
-            'form': 'Execution Form',
+            'execution_prompts_required': 'Execution Prompts - Required',
+            'execution_prompts_optional': 'Execution Prompts - Optional',
         },
         'credentials': {
             'connect_user': 'Connect User',
             'connect_pass': 'Connect Password',
             'become_user': 'Become User',
             'become_pass': 'Become Password',
             'vault_file': 'Vault Password File',
@@ -37,26 +38,14 @@
             'git_playbook_base': 'Git Playbook Base-Directory',
             'git_isolate': 'Git Isolate Directory',
             'git_hook_pre': 'Git Pre-Hook',
             'git_hook_post': 'Git Post-Hook',
             'git_override_initialize': 'Git Override Initialize-Command',
             'git_override_update': 'Git Override Update-Command',
         },
-        'execution_form_field': {
-            'help': 'Help Text',
-            'var': 'Variable',
-            'var_type': 'Variable Type',
-            'field_type': 'Field Type',
-            'multiple': 'Multiple Choices',
-            'separator': 'Multiple-Choice Separator',
-            'validate_error': 'Validation Error-Message',
-            'validate_regex': 'Validation Regex',
-            'validate_max': 'Maximum Value',
-            'validate_min': 'Minimum Value',
-        },
     },
     'settings': {
         'permissions': {
             'jobs_all': 'All jobs',
             'credentials_all': 'All credentials',
             'repositories_all': 'All repositories',
         },
@@ -137,15 +126,18 @@
             'credentials_needed': 'If the job requires credentials to be specified '
                                   '(either as default or at execution-time; '
                                   'fallback are the user-credentials of the executing user)',
             'credentials_default': 'Specify job-level default credentials to use',
             'credentials_category': 'The credential category can be used for dynamic matching of '
                                     'user credentials at execution time',
             'enabled': 'En- or disable the schedule. Can be ignored if no schedule was set',
-            'form': 'Select a Job-Execution form to display on ad-hoc executions',
+            'execution_prompts_required': 'Required job attributes and/or variables to prompt at custom execution. '
+                                          'Comma-separated list of key-value pairs.<br>'
+                                          "Variables can be supplied like so: 'var={VAR-NAME}#{DISPLAY-NAME}'<br>"
+                                          "Example: 'limit,check,var=add_user#User to add' ",
         },
         'credentials': {
             'vault_file': 'Path to the file containing your vault-password',
             'vault_id': 'For details see: '
                         '<a href="https://docs.ansible.com/ansible/latest/vault_guide/'
                         'vault_managing_passwords.html">'
                         'Ansible Docs - Managing Passwords</a>',
@@ -169,26 +161,14 @@
             'git_hook_post': 'Commands to execute after initializing/updating the repository. '
                              'Comma-separated list of shell-commands',
             'git_override_initialize': 'Advanced usage! Completely override the command used to initialize '
                                        '(clone) the repository',
             'git_override_update': 'Advanced usage! Completely override the command used to update '
                                    '(pull) the repository',
         },
-        'execution_form_field': {
-            'var_type': '<b>WARNING</b>: Choose env-var for secret values! Commandline arguments are viewable and '
-                        'will be logged',
-            'multiple': 'If multiple the form should support multiple user-choices',
-            'separator': 'If multiple choices are used - they will be joined on serialization before they get passed '
-                         'to the Ansible Execution. This separator will be used on that join operation',
-            'validate_error': 'Error-Message to display on validation error',
-            'validate_regex': 'Regex to validate the value. Test it here: '
-                              '<a href="https://regex101.com/">regex101.com</a>. (flavor needs to be JavaScript)',
-            'validate_max': 'Field-type integer: maximum integer; Field-type string: maximum length',
-            'validate_min': 'Field-type integer: minimum integer; Field-type string: minimum length',
-        },
     },
     'settings': {
         'permissions': {
             'jobs_all': 'Match permission to all existing jobs (present and future)',
             'credentials_all': 'Match permission to all existing credentials (present and future)',
             'repositories_all': 'Match permission to all existing repositories (present and future)',
         },
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/hardcoded.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/hardcoded.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/main.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/config/navigation.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/config/navigation.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         _tmpl_text = _tmpl_base / 'alert.txt'
         if _tmpl_html.is_file():
             tmpl_html = str(_tmpl_html)
 
         if _tmpl_text.is_file():
             tmpl_text = str(_tmpl_text)
 
-    tmpl_ctx = {'execution': execution, 'stats': stats, 'web_addr': get_main_web_address(), 'error_msgs': error_msgs}
+    tmpl_ctx = {'execution': execution, 'stats': stats, 'url': get_main_web_address(), 'error_msgs': error_msgs}
     text_content = get_template(tmpl_text).render(tmpl_ctx)
     html_content = get_template(tmpl_html).render(tmpl_ctx)
     html_content = html_transform_styles(html=html_content, pretty_print=True, allow_network=False)
 
     msg.attach(MIMEText(text_content, 'plain'))
     msg.attach(MIMEText(html_content, 'html'))
 
@@ -71,15 +71,14 @@
 
         else:
             ssl_context.check_hostname = False
             ssl_context.verify_mode = ssl.CERT_NONE
 
         if config['mail_transport'] == MAIL_TRANSPORT_TYPE_SSL:
             with SMTP_SSL(server, port, context=ssl_context) as server:
-                server.login(config['mail_user'], config['mail_pass'])
                 _email_send(server=server, user=user, stats=stats, execution=execution, error_msgs=error_msgs)
 
         else:
             with SMTP(server, port) as server:
                 if config['mail_transport'] == MAIL_TRANSPORT_TYPE_STARTTLS:
                     server.starttls(context=ssl_context)
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/alert_plugin/plugin_wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     if not Path(alert.plugin.executable).is_file():
         log(
             msg=f"Alert plugin has an invalid executable configured: {alert.name} ({alert.plugin.executable})",
             level=3,
         )
         return
 
+    url = get_main_web_address()
+
     data = {
         'alert': {
             'type': 'global',
             'condition': alert.condition_name.lower(),
         },
         'user': {
             'name': user.username,
@@ -44,23 +46,26 @@
             'last_login': int(unix_timestamp(datetime_from_db(user.last_login).timetuple())),
             'groups': [group.name for group in user.groups.all()],
         },
         'execution': {
             'failed': failed,
             'status': execution.status_name,
             'job_name': execution.job.name,
+            'job_id': execution.job.id,
+            'execution_id': execution.id,
             'user_name': execution.user_name,
             'time_start': int(unix_timestamp(execution.time_created_dt.timetuple())),
             'time_start_pretty': execution.time_created_str,
             'time_fin': None,
             'time_fin_pretty': None,
             'time_duration': None,
             'time_duration_pretty': None,
             'error_short': None,
             'error_med': None,
+            'log_url': f"{url}/ui/jobs/log?job={execution.job.id}",
         },
         'errors': error_msgs,
         'stats': stats,
     }
 
     try:
         user_extended = UserExtended.objects.get(user=user)
@@ -87,15 +92,15 @@
             data['execution']['error_med'] = execution.result.error.med
 
     for log_attr in JobExecution.log_file_fields:
         url_attr = f'{log_attr}_url'
         file = getattr(execution, log_attr)
         if Path(file).is_file():
             data['execution'][log_attr] = file
-            data['execution'][url_attr] = f"{get_main_web_address()}{getattr(execution, url_attr)}"
+            data['execution'][url_attr] = f"{url}{getattr(execution, url_attr)}"
 
         else:
             data['execution'][log_attr] = None
             data['execution'][url_attr] = None
 
     tmp_file = f"{config['path_run']}/.aw_alert_{time()}.json"
     write_file_0600(
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/play.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_credentials.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/play_credentials.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/play_util.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/play_util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/repository.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/scheduler.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,30 +74,31 @@
 
                 except ThreadError as err:
                     log(msg=f'Got thread error: {err}', level=2)
 
         except Exception as err:
             log(msg=f'Got unexpected error: {err}', level=1)
             self.stop()
-            return
 
     def status(self):
         log(msg=f"Running job-threads: {self.thread_manager.list_pretty()}", level=4)
 
     def check(self):
         log('Checking for queued jobs', level=7)
         while True:
-            queue_item = queue_get()
-            if queue_item is None:
+            execution = queue_get()
+            if execution is None:
                 break
 
-            job, user = queue_item
-
-            log(f"Adding job-thread for queued job: '{job.name}' (triggered by user '{user.username}')", level=4)
-            self._add_thread(job=job, execution=JobExecution(user=user, job=job, comment='Triggered'), once=True)
+            log(
+                f"Adding job-thread for queued job: '{execution.job.name}' "
+                f"(triggered by user '{execution.user.username}')",
+                level=4,
+            )
+            self._add_thread(job=execution.job, execution=execution, once=True)
 
     def reload(self, signum=None):
         if not self.reloading and not self.stopping:
             self.reloading = True
 
             if signum is not None:
                 log('Reloading..', level=3)
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/threader.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/threader.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/execute/util.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/execute/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0001_v0_0_12.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0002_v0_0_13.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0003_v0_0_14.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/migrations/0006_v0_0_19.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/alert.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/alert.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/base.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/base.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
 
 class Job(BaseJob):
     CHANGE_FIELDS = [
         'name', 'playbook_file', 'inventory_file', 'repository', 'schedule', 'enabled', 'limit', 'verbosity',
         'mode_diff', 'mode_check', 'tags', 'tags_skip', 'verbosity', 'comment', 'environment_vars', 'cmd_args',
         'credentials_default', 'credentials_needed', 'credentials_category',
+        'execution_prompts_required', 'execution_prompts_optional',
     ]
     form_fields_primary = ['name', 'playbook_file', 'inventory_file', 'repository']
     form_fields = CHANGE_FIELDS
     api_fields_read = ['id']
     api_fields_read.extend(CHANGE_FIELDS)
     api_fields_write = api_fields_read.copy()
     api_fields_read.append('next_run')
@@ -100,14 +101,26 @@
     credentials_needed = models.BooleanField(choices=CHOICES_BOOL, default=False)
     credentials_default = models.ForeignKey(
         JobGlobalCredentials, on_delete=models.SET_NULL, related_name='job_fk_creddflt', null=True, blank=True,
     )
     credentials_category = models.CharField(max_length=100, **DEFAULT_NONE)
     repository = models.ForeignKey(Repository, on_delete=models.SET_NULL, related_name='job_fk_repo', **DEFAULT_NONE)
 
+    execution_prompts_max_len = 2000
+    execution_prompts_regex = (r'^(limit|verbosity|comment|mode_diff|diff|mode_check|check|environment_vars|env_vars|'
+                               r'tags|tags_skip|skip_tags|cmd_args|var=[^,#]*?|var=[^#]*?#[^,]*?|[,$])+$')
+    execution_prompt_aliases = {
+        'check': 'mode_check',
+        'diff': 'mode_diff',
+        'env_vars': 'environment_vars',
+        'skip_tags': 'tags_skip',
+    }
+    execution_prompts_required = models.CharField(max_length=execution_prompts_max_len, **DEFAULT_NONE)
+    execution_prompts_optional = models.CharField(max_length=execution_prompts_max_len, **DEFAULT_NONE)
+
     def __str__(self) -> str:
         limit = '' if self.limit is None else f' [{self.limit}]'
         return f"Job '{self.name}' ({self.playbook_file} => {self.inventory_file}{limit})"
 
     class Meta:
         constraints = [
             models.UniqueConstraint(fields=['name'], name='job_name_unique')
@@ -190,17 +203,21 @@
         return f"Job execution {self.created} of host '{self.hostname}': {result}"
 
 
 class JobExecution(BaseJob):
     api_fields_read = [
         'id', 'job', 'job_name', 'user', 'user_name', 'result', 'status', 'status_name', 'time_start', 'time_fin',
         'failed', 'error_s', 'error_m', 'log_stdout', 'log_stdout_url', 'log_stderr', 'log_stderr_url', 'job_comment',
-        'credential_global', 'credential_user', 'command', 'log_stdout_repo', 'log_stderr_repo',
+        'comment', 'credential_global', 'credential_user', 'command', 'log_stdout_repo', 'log_stderr_repo',
         'log_stdout_repo_url', 'log_stderr_repo_url',
     ]
+    api_fields_exec = [
+        'comment', 'limit', 'verbosity', 'mode_diff', 'mode_check', 'environment_vars', 'tags', 'tags_skip',
+        'cmd_args',
+    ]
     log_file_fields = ['log_stdout', 'log_stderr', 'log_stdout_repo', 'log_stderr_repo']
 
     # NOTE: scheduled execution will have no user
     user = models.ForeignKey(
         USERS, on_delete=models.SET_NULL, null=True,
         related_name='jobexec_fk_user', editable=False,
     )
@@ -271,12 +288,10 @@
 
     @property
     def user_name(self) -> str:
         return self.user.username if self.user is not None else 'Scheduled'
 
 
 class JobQueue(BareModel):
-    job = models.ForeignKey(Job, on_delete=models.CASCADE, related_name='jobqueue_fk_job')
-    user = models.ForeignKey(
-        USERS, on_delete=models.SET_NULL, null=True,
-        related_name='jobqueue_fk_user',
+    execution = models.ForeignKey(
+        JobExecution, on_delete=models.CASCADE, related_name='jobqueue_fk_jobexec', **DEFAULT_NONE,
     )
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/job_credential.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/job_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     }
     PUBLIC_ATTRS_ARGS = {
         'connect_user': '--user',
         'become_user': '--become-user',
         'vault_file': '--vault-password-file',
         'vault_id': '--vault-id',
     }
+    EMPTY_ATTRS = [
+        'connect_user', 'vault_file', 'vault_id', 'vault_pass', 'become_pass', 'connect_pass', 'ssh_key',
+    ]
 
     name = models.CharField(max_length=100, null=False, blank=False)
     connect_user = models.CharField(max_length=100, **DEFAULT_NONE)
     become_user = models.CharField(max_length=100, default='root', null=True, blank=True)
     # default become_user according to ansible-playbook docs
     vault_file = models.CharField(max_length=300, **DEFAULT_NONE)
     vault_id = models.CharField(max_length=50, **DEFAULT_NONE)
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/permission.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/repository.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/repository.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/model/system.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/model/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     (MAIL_TRANSPORT_TYPE_STARTTLS, 'StartTLS'),
 ]
 
 
 # NOTE: add default-values to config.defaults.CONFIG_DEFAULTS
 class SystemConfig(BaseModel):
     SECRET_ATTRS = ['mail_pass']
+    EMPTY_ATTRS = [
+        'path_ansible_config', 'path_ssh_known_hosts', 'logo_url', 'ara_server', 'global_environment_vars',
+        'mail_server', 'mail_sender', 'mail_user', 'mail_pass',
+    ]
     api_fields_read = [
         'path_run', 'path_play', 'path_log', 'path_template', 'timezone', 'run_timeout', 'session_timeout',
         'path_ansible_config', 'path_ssh_known_hosts', 'debug', 'logo_url', 'ara_server', 'global_environment_vars',
         'mail_server', 'mail_transport', 'mail_ssl_verify', 'mail_sender', 'mail_user',
     ]
 
     # NOTE: 'AW_DB' is needed to get this config from DB and 'AW_SECRET' cannot be saved because of security breach
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/settings.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/settings.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw.css` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/css/aw.css`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,18 @@
     width: 20vw;
 }
 
 input:invalid {
 	border-color: red;
 }
 
+.aw-exec-form {
+    overflow: hidden;
+}
+
 .mb-3 {
     margin-bottom: 0.1rem !important;
 }
 
 .aw-fs-choices {
     background-color: var(--tableRow1);
     width: 20vw;
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/css/aw_mobile.css` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/css/aw_mobile.css`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     }
 
     .aw-form-inline-right {
         float: none;
     }
 
     form .form-control, .aw-fs-choices {
-        width: 35vw;
+        width: 45vw;
     }
 
     .aw-responsive-lg {
         display: none;
     }
 }
 
@@ -46,15 +46,15 @@
         align-items: center;
         justify-content: center;
         border-top: 2px solid rgba(255, 255, 255, 0.6);
         margin-top: 10px;
     }
 
     form .form-control, .aw-fs-choices {
-        width: 50vw;
+        width: 60vw;
     }
 
     .aw-responsive-lg {
         display: none;
     }
 
     .aw-responsive-med {
@@ -74,15 +74,15 @@
 
     .aw-file-content-line {
         text-indent: -5vw;
         padding-left: 5vw;
     }
 
     form .form-control, .aw-login, .aw-login-fields, .aw-fs-choices {
-        width: 70vw;
+        width: 90vw;
     }
 
     .aw-btn-action-icon {
         font-size: 20px !important;
     }
 
     .aw-btn-action {
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/img/logo.svg` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/aw.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -202,21 +202,44 @@
         if (shouldSwitch) {
             rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
             switching = true;
         }
     }
 }
 
+function escapeRegExp(string) {
+    return string.replace(/[.*+?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
+}
+
+function replaceAll(str, search, replace) {
+    return str.replace(new RegExp(escapeRegExp(search), 'g'), replace);
+}
+
+// see: https://docs.djangoproject.com/en/5.0/ref/templates/language/#automatic-html-escaping
+function escapeHTML(data) {
+    if (!is_set(data)) {
+        return data;
+    }
+    data = data.replaceAll('<', '&lt;');
+    data = data.replaceAll('>', '&gt;');
+    data = data.replaceAll('&', '&amp;');
+    return data;
+}
+
+function capitalizeFirstLetter(string) {
+    return string.charAt(0).toUpperCase() + string.slice(1);
+}
+
 // API CALLS
 const CSRF_TOKEN = getCookie('csrftoken');
 
 function apiActionSuccess(result) {
     resultDiv = document.getElementById('aw-api-result');
     if (result.msg) {
-        resultDiv.innerHTML = 'Success: ' + result.msg;
+        resultDiv.innerHTML = 'Success: ' + escapeHTML(result.msg);
     } else {
         resultDiv.innerHTML = 'Success';
     }
     apiActionErrorClear();
     $('html, body').animate({
         scrollTop: 0
     }, 'fast');
@@ -232,15 +255,15 @@
     errorFullIframe.write('<h1><b>FULL ERROR:</b></h1><br>' + result.responseText);
     errorFullIframe.close();
 
     // inform user about the error and allow to toggle/show the full/verbose error message
     errorDiv = document.getElementById('aw-api-error');
     let errorHTML = "Got error: " + result.statusText + ' (' + result.status + ')';
     if (is_set(result.responseJSON.msg)) {
-        errorHTML += ' - ' + result.responseJSON.msg;
+        errorHTML += ' - ' + escapeHTML(result.responseJSON.msg);
     } else {
         errorHTML += '<br><button class="btn btn-warning aw-btn-action" title="Full error" onclick="apiActionFullError()">Show full error</button><br>';
     }
     errorDiv.innerHTML = errorHTML;
 
     apiActionSuccessClear();
     $('html, body').animate({
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/aw_nav.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/aw_nav.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/credentials.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/credentials.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/edit.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/edit.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/logs.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/logs.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,7 @@
-function escapeRegExp(string) {
-    return string.replace(/[.*+?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
-}
-
-function replaceAll(str, search, replace) {
-    return str.replace(new RegExp(escapeRegExp(search), 'g'), replace);
-}
-
 function addLogLines($this) {
     let logParentElement = $this.attr("aw-expand");
     let logElement = $this.attr("aw-log");
     let logElementEnd = document.getElementById($this.attr("aw-log-end"));
     let job_id = $this.attr("aw-job");
     let exec_id = $this.attr("aw-exec");
     let hidden = document.getElementById(logParentElement).getAttribute("hidden");
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/jobs/repository.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/jobs/repository.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/login.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/login.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/alert.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/alert.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/api_key.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/api_key.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/static/js/settings/permission.js` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/static/js/settings/permission.js`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/body.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/body.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/email/alert.txt` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/email/alert.txt`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/job.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/job.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/forms/snippet.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/forms/snippet.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/head.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/head.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/credentials.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/credentials_edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/edit.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/logs.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/logs.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/repository.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/jobs/repository_edit.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/nav.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/nav.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/login.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_done.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/password_change_form.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/registration/saml.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/registration/saml.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/rest_framework/api.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/alert.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/alert.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/api_key.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/api_key.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/settings/permission.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/settings/permission.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/config.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/system/config.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templates/system/environment.html` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templates/system/environment.html`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/form_util.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templatetags/form_util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/templatetags/util.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/templatetags/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/urls.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/urls.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/crypto.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/debug.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/debug.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/deployment.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/deployment.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/http.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/http.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/permission.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/permission.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/subps.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/subps.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/util.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/util.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/utils/version.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/utils/version.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/base.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/base.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/auth.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/auth.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/job.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,34 @@
                   r'((((\d+,)+\d+|(\d+(\/|-|#)\d+)|\d+L?|\*(\/\d+)?|L(-\d+)?|\?|[A-Z]{3}(-[A-Z]{3})?) ?){5,7})$',
             message='The provided schedule is not in a valid cron format',
         )],
         required=False,
         help_text=Meta.help_texts['schedule'],
     )
 
+    execution_prompts_required = forms.CharField(
+        max_length=Job.execution_prompts_max_len,
+        validators=[RegexValidator(
+            regex=Job.execution_prompts_regex,
+            message='The provided expression is not in a valid format',
+        )],
+        required=False,
+        label=Meta.labels['execution_prompts_required'],
+        help_text=Meta.help_texts['execution_prompts_required'],
+    )
+    execution_prompts_optional = forms.CharField(
+        max_length=Job.execution_prompts_max_len,
+        validators=[RegexValidator(
+            regex=Job.execution_prompts_regex,
+            message='The provided expression is not in a valid format',
+        )],
+        required=False,
+        label=Meta.labels['execution_prompts_optional'],
+    )
+
 
 @login_required
 @ui_endpoint_wrapper_kwargs
 def job_edit(request, job_id: int = None, clone: bool = False) -> HttpResponse:
     job_form = JobForm()
     form_method = 'post'
     form_api = 'job'
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/settings.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/settings.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/forms/system.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/forms/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/job.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/job.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/main.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/settings.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/settings.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/aw/views/system.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/aw/views/system.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/cli.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/cli_init.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/cli_init.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/db.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/db.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/handle_signals.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/handle_signals.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/main.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/main.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/manage.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/manage.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/web_serve_static.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/web_serve_static.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy-webui/webserver.py` & `ansibleguy_webui-0.0.21/src/ansibleguy-webui/webserver.py`

 * *Files identical despite different names*

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/PKG-INFO` & `ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansibleguy-webui
-Version: 0.0.20
+Version: 0.0.21
 Summary: Basic WebUI for using Ansible
 Author-email: AnsibleGuy <contact@ansibleguy.net>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -765,15 +765,15 @@
 
   - [x] Execute Ansible using [ansible-runner](https://ansible.readthedocs.io/projects/runner/en/latest/python_interface/)
 
     - [x] Scheduled execution (Cron-Format)
 
     - [x] Manual/immediate execution
 
-    - [ ] Custom Execution-Forms
+    - [x] Custom Execution-Forms
 
     - [ ] Support for [ad-hoc commands](https://docs.ansible.com/ansible/latest/command_guide/intro_adhoc.html)
 
     - [ ] Support for [Process-Isolation](https://ansible.readthedocs.io/projects/runner/en/stable/standalone/#running-with-process-isolation)
 
   - [x] Job Logging
```

### Comparing `ansibleguy_webui-0.0.20/src/ansibleguy_webui.egg-info/SOURCES.txt` & `ansibleguy_webui-0.0.21/src/ansibleguy_webui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

