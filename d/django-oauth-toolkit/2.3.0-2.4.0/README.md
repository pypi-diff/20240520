# Comparing `tmp/django-oauth-toolkit-2.3.0.tar.gz` & `tmp/django_oauth_toolkit-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oauth-toolkit-2.3.0.tar", last modified: Wed May 31 21:01:09 2023, max compression
+gzip compressed data, was "django_oauth_toolkit-2.4.0.tar", last modified: Mon May 20 13:53:25 2024, max compression
```

## Comparing `django-oauth-toolkit-2.3.0.tar` & `django_oauth_toolkit-2.4.0.tar`

### file list

```diff
@@ -1,103 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.933997 django-oauth-toolkit-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-31 21:01:09.933997 django-oauth-toolkit-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.921996 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 21:01:09.000000 django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.925996 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/cleartokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/createapplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.929997 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0002_auto_20190406_1805.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0003_auto_20201211_1314.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0004_auto_20200902_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0005_auto_20211222_2352.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0006_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0007_application_post_logout_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.921996 django-oauth-toolkit-2.3.0/oauth2_provider/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.929997 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_registration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorize.html
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorized-token-delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/logout_confirm.html
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.929997 django-oauth-toolkit-2.3.0/oauth2_provider/views/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/oauth2_provider/views/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-31 21:01:09.937997 django-oauth-toolkit-2.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:01:09.933997 django-oauth-toolkit-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_application_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    73185 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_authorization_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    57835 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_introspection_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_introspection_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_oauth2_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_oauth2_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_oidc_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_scopes_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_token_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_token_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-31 21:00:56.000000 django-oauth-toolkit-2.3.0/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.310014 django_oauth_toolkit-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-20 13:53:25.310014 django_oauth_toolkit-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.310014 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-20 13:53:25.000000 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-20 13:53:25.000000 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:53:25.000000 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:53:25.000000 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 13:53:25.000000 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 13:53:25.000000 django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.298014 django_oauth_toolkit-2.4.0/oauth2_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.298014 django_oauth_toolkit-2.4.0/oauth2_provider/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.298014 django_oauth_toolkit-2.4.0/oauth2_provider/contrib/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/contrib/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/contrib/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/contrib/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.298014 django_oauth_toolkit-2.4.0/oauth2_provider/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.298014 django_oauth_toolkit-2.4.0/oauth2_provider/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/management/commands/cleartokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/management/commands/createapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.302014 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0002_auto_20190406_1805.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0003_auto_20201211_1314.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0004_auto_20200902_2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0005_auto_20211222_2352.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0006_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0007_application_post_logout_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0008_alter_accesstoken_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0009_add_hash_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0010_application_allowed_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28783 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/oauth2_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39872 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/oauth2_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.290014 django_oauth_toolkit-2.4.0/oauth2_provider/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.302014 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_registration_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/authorize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/authorized-token-delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/logout_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.306014 django_oauth_toolkit-2.4.0/oauth2_provider/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13089 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20946 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/oauth2_provider/views/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-20 13:53:25.310014 django_oauth_toolkit-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:53:25.310014 django_oauth_toolkit-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_application_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76562 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_authorization_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57755 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_introspection_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_introspection_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24195 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_oauth2_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23695 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_oauth2_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33193 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_oidc_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16867 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_scopes_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_token_endpoint_cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_token_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_token_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-20 13:53:16.000000 django_oauth_toolkit-2.4.0/tests/test_validators.py
```

### Comparing `django-oauth-toolkit-2.3.0/AUTHORS` & `django_oauth_toolkit-2.4.0/AUTHORS`

 * *Files 24% similar despite different names*

```diff
@@ -5,34 +5,41 @@
 Federico Frenguelli
 
 Contributors
 ------------
 
 Abhishek Patel
 Adam Johnson
+Adam Zahradník
 Adheeth P Praveen
 Alan Crosswell
+Alan Rominger
 Alejandro Mantecon Guillen
 Aleksander Vaskevich
 Alessandro De Angelis
+Alex Manning
 Alex Szabó
+Aliaksei Kanstantsinau
 Allisson Azevedo
 Andrea Greco
 Andrej Zbín
 Andrew Chen Wang
+Andrew Zickler
 Antoine Laurent
 Anvesh Agarwal
 Aristóbulo Meneses
 Aryan Iyappan
+Asaf Klibansky
 Ash Christopher
 Asif Saif Uddin
 Bart Merenda
 Bas van Oostveen
 Brian Helba
 Carl Schwan
+Daniel Golding
 Daniel 'Vector' Kerr
 Darrel O'Pry
 Dave Burkholder
 David Fischer
 David Hill
 David Smith
 Dawid Wolski
@@ -41,47 +48,56 @@
 Dulmandakh Sukhbaatar
 Dylan Giesler
 Dylan Tack
 Eduardo Oliveira
 Egor Poderiagin
 Emanuele Palazzetti
 Federico Dolce
+Florian Demmer
 Frederico Vieira
+Gaël Utard
+Glauco Junior
 Hasan Ramezani
 Hiroki Kiyohara
 Hossein Shakiba
 Islam Kamel
+Ivan Lukyanets
 Jadiel Teófilo
 Jens Timmerman
 Jerome Leclanche
 Jesse Gibbs
 Jim Graham
+John Byrne
 Jonas Nygaard Pedersen
 Jonathan Steffan
 Jordi Sanchez
 Joseph Abrahams
 Josh Thomas
 Jozef Knaperek
 Julian Mundhahs
 Julien Palard
 Jun Zhou
 Kaleb Porter
 Kristian Rune Larsen
+Lazaros Toumanidis
 Ludwig Hähne
+Łukasz Skarżyński
 Marcus Sonestedt
 Matias Seniquiel
 Michael Howitz
 Owen Gong
 Patrick Palacin
 Paul Dekkers
 Paul Oswald
 Pavel Tvrdík
 Peter Carnesciali
 Peter Karman
+Peter McDonald
 Petr Dlouhý
+pySilver
 Rodney Richardson
 Rustem Saiargaliev
 Rustem Saiargaliev
 Sandro Rodrigues
 Shaheed Haque
 Shaun Stanworth
 Silvano Cerza
@@ -90,7 +106,10 @@
 Stéphane Raimbault
 Tom Evans
 Vinay Karanam
 Víðir Valberg Guðmundsson
 Will Beaufoy
 pySilver
 Łukasz Skarżyński
+Wouter Klein Heerenbrink
+Yaroslav Halchenko
+Yuri Savin
```

### Comparing `django-oauth-toolkit-2.3.0/LICENSE` & `django_oauth_toolkit-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/PKG-INFO` & `django_oauth_toolkit-2.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: django-oauth-toolkit
-Version: 2.3.0
+Version: 2.4.0
 Summary: OAuth2 Provider for Django
 Home-page: https://github.com/jazzband/django-oauth-toolkit
 Author: Federico Frenguelli, Massimiliano Pippi
 Author-email: synasius@gmail.com
 Keywords: django,oauth,oauth2,oauthlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: django!=4.0.0,>=3.2
+Requires-Dist: requests>=2.13.0
+Requires-Dist: oauthlib>=3.1.0
+Requires-Dist: jwcrypto>=0.8.0
+Requires-Dist: pytz>=2024.1
 
 Django OAuth Toolkit
 ====================
 
 .. image:: https://jazzband.co/static/img/badge.svg
    :target: https://jazzband.co/
    :alt: Jazzband
@@ -59,26 +65,26 @@
 If you are facing one or more of the following:
  * Your Django app exposes a web API you want to protect with OAuth2 authentication,
  * You need to implement an OAuth2 authorization server to provide tokens management for your infrastructure,
 
 Django OAuth Toolkit can help you providing out of the box all the endpoints, data and logic needed to add OAuth2
 capabilities to your Django projects. Django OAuth Toolkit makes extensive use of the excellent
 `OAuthLib <https://github.com/idan/oauthlib>`_, so that everything is
-`rfc-compliant <http://tools.ietf.org/html/rfc6749>`_.
+`rfc-compliant <https://rfc-editor.org/rfc/rfc6749.html>`_.
 
 Reporting security issues
 -------------------------
 
 Please report any security issues to the JazzBand security team at <security@jazzband.co>. Do not file an issue on the tracker.
 
 Requirements
 ------------
 
-* Python 3.7+
-* Django 2.2, 3.2, 4.0 (4.0.1+ due to a regression), 4.1, or 4.2
+* Python 3.8+
+* Django 3.2, 4.0 (4.0.1+ due to a regression), 4.1, 4.2, or 5.0
 * oauthlib 3.1+
 
 Installation
 ------------
 
 Install with pip::
```

### Comparing `django-oauth-toolkit-2.3.0/README.rst` & `django_oauth_toolkit-2.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -29,26 +29,26 @@
 If you are facing one or more of the following:
  * Your Django app exposes a web API you want to protect with OAuth2 authentication,
  * You need to implement an OAuth2 authorization server to provide tokens management for your infrastructure,
 
 Django OAuth Toolkit can help you providing out of the box all the endpoints, data and logic needed to add OAuth2
 capabilities to your Django projects. Django OAuth Toolkit makes extensive use of the excellent
 `OAuthLib <https://github.com/idan/oauthlib>`_, so that everything is
-`rfc-compliant <http://tools.ietf.org/html/rfc6749>`_.
+`rfc-compliant <https://rfc-editor.org/rfc/rfc6749.html>`_.
 
 Reporting security issues
 -------------------------
 
 Please report any security issues to the JazzBand security team at <security@jazzband.co>. Do not file an issue on the tracker.
 
 Requirements
 ------------
 
-* Python 3.7+
-* Django 2.2, 3.2, 4.0 (4.0.1+ due to a regression), 4.1, or 4.2
+* Python 3.8+
+* Django 3.2, 4.0 (4.0.1+ due to a regression), 4.1, 4.2, or 5.0
 * oauthlib 3.1+
 
 Installation
 ------------
 
 Install with pip::
```

### Comparing `django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/PKG-INFO` & `django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: django-oauth-toolkit
-Version: 2.3.0
+Version: 2.4.0
 Summary: OAuth2 Provider for Django
 Home-page: https://github.com/jazzband/django-oauth-toolkit
 Author: Federico Frenguelli, Massimiliano Pippi
 Author-email: synasius@gmail.com
 Keywords: django,oauth,oauth2,oauthlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: django!=4.0.0,>=3.2
+Requires-Dist: requests>=2.13.0
+Requires-Dist: oauthlib>=3.1.0
+Requires-Dist: jwcrypto>=0.8.0
+Requires-Dist: pytz>=2024.1
 
 Django OAuth Toolkit
 ====================
 
 .. image:: https://jazzband.co/static/img/badge.svg
    :target: https://jazzband.co/
    :alt: Jazzband
@@ -59,26 +65,26 @@
 If you are facing one or more of the following:
  * Your Django app exposes a web API you want to protect with OAuth2 authentication,
  * You need to implement an OAuth2 authorization server to provide tokens management for your infrastructure,
 
 Django OAuth Toolkit can help you providing out of the box all the endpoints, data and logic needed to add OAuth2
 capabilities to your Django projects. Django OAuth Toolkit makes extensive use of the excellent
 `OAuthLib <https://github.com/idan/oauthlib>`_, so that everything is
-`rfc-compliant <http://tools.ietf.org/html/rfc6749>`_.
+`rfc-compliant <https://rfc-editor.org/rfc/rfc6749.html>`_.
 
 Reporting security issues
 -------------------------
 
 Please report any security issues to the JazzBand security team at <security@jazzband.co>. Do not file an issue on the tracker.
 
 Requirements
 ------------
 
-* Python 3.7+
-* Django 2.2, 3.2, 4.0 (4.0.1+ due to a regression), 4.1, or 4.2
+* Python 3.8+
+* Django 3.2, 4.0 (4.0.1+ due to a regression), 4.1, 4.2, or 5.0
 * oauthlib 3.1+
 
 Installation
 ------------
 
 Install with pip::
```

### Comparing `django-oauth-toolkit-2.3.0/django_oauth_toolkit.egg-info/SOURCES.txt` & `django_oauth_toolkit-2.4.0/django_oauth_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 oauth2_provider/models.py
 oauth2_provider/oauth2_backends.py
 oauth2_provider/oauth2_validators.py
 oauth2_provider/scopes.py
 oauth2_provider/settings.py
 oauth2_provider/signals.py
 oauth2_provider/urls.py
+oauth2_provider/utils.py
 oauth2_provider/validators.py
 oauth2_provider/contrib/__init__.py
 oauth2_provider/contrib/rest_framework/__init__.py
 oauth2_provider/contrib/rest_framework/authentication.py
 oauth2_provider/contrib/rest_framework/permissions.py
 oauth2_provider/management/__init__.py
 oauth2_provider/management/commands/__init__.py
@@ -41,14 +42,17 @@
 oauth2_provider/migrations/0001_initial.py
 oauth2_provider/migrations/0002_auto_20190406_1805.py
 oauth2_provider/migrations/0003_auto_20201211_1314.py
 oauth2_provider/migrations/0004_auto_20200902_2022.py
 oauth2_provider/migrations/0005_auto_20211222_2352.py
 oauth2_provider/migrations/0006_alter_application_client_secret.py
 oauth2_provider/migrations/0007_application_post_logout_redirect_uris.py
+oauth2_provider/migrations/0008_alter_accesstoken_token.py
+oauth2_provider/migrations/0009_add_hash_client_secret.py
+oauth2_provider/migrations/0010_application_allowed_origins.py
 oauth2_provider/migrations/__init__.py
 oauth2_provider/templates/oauth2_provider/application_confirm_delete.html
 oauth2_provider/templates/oauth2_provider/application_detail.html
 oauth2_provider/templates/oauth2_provider/application_form.html
 oauth2_provider/templates/oauth2_provider/application_list.html
 oauth2_provider/templates/oauth2_provider/application_registration_form.html
 oauth2_provider/templates/oauth2_provider/authorize.html
@@ -81,10 +85,12 @@
 tests/test_oauth2_validators.py
 tests/test_oidc_views.py
 tests/test_password.py
 tests/test_rest_framework.py
 tests/test_scopes.py
 tests/test_scopes_backend.py
 tests/test_settings.py
+tests/test_token_endpoint_cors.py
 tests/test_token_revocation.py
 tests/test_token_view.py
+tests/test_utils.py
 tests/test_validators.py
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/admin.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/admin.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/backends.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/backends.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/authentication.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/contrib/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/contrib/rest_framework/permissions.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/contrib/rest_framework/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 class IsAuthenticatedOrTokenHasScope(BasePermission):
     """
     The user is authenticated using some backend or the token has the right scope
     This only returns True if the user is authenticated, but not using a token
     or using a token, and the token has the correct scope.
 
-    This is usefull when combined with the DjangoModelPermissions to allow people browse
+    This is useful when combined with the DjangoModelPermissions to allow people browse
     the browsable api's if they log in using the a non token bassed middleware,
     and let them access the api's using a rest client with a token
     """
 
     def has_permission(self, request, view):
         is_authenticated = IsAuthenticated().has_permission(request, view)
         oauth2authenticated = False
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/decorators.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/decorators.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/exceptions.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/forms.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/forms.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/generators.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         raise NotImplementedError()
 
 
 class ClientIdGenerator(BaseHashGenerator):
     def hash(self):
         """
         Generate a client_id for Basic Authentication scheme without colon char
-        as in http://tools.ietf.org/html/rfc2617#section-2
+        as in https://rfc-editor.org/rfc/rfc2617.html#section-2
         """
         return oauthlib_generate_client_id(length=40, chars=UNICODE_ASCII_CHARACTER_SET)
 
 
 class ClientSecretGenerator(BaseHashGenerator):
     def hash(self):
         length = oauth2_settings.CLIENT_SECRET_GENERATOR_LENGTH
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/http.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/http.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/management/commands/createapplication.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/management/commands/createapplication.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,21 @@
         )
         parser.add_argument(
             "--client-secret",
             type=str,
             help="The secret for this application",
         )
         parser.add_argument(
+            "--no-hash-client-secret",
+            dest="hash_client_secret",
+            action="store_false",
+            help="Don't hash the client secret",
+        )
+        parser.set_defaults(hash_client_secret=True)
+        parser.add_argument(
             "--name",
             type=str,
             help="The name this application",
         )
         parser.add_argument(
             "--skip-authorization",
             action="store_true",
@@ -70,15 +77,15 @@
         # and also with custom application models.
         application_fields = [field.name for field in Application._meta.fields]
         application_data = {}
         for key, value in options.items():
             # Data in options must be cleaned because there are unneeded key-value like
             # verbosity and others. Also do not pass any None to the Application
             # instance so default values will be generated for those fields
-            if key in application_fields and value:
+            if key in application_fields and (isinstance(value, bool) or value):
                 if key == "user":
                     application_data.update({"user_id": value})
                 else:
                     application_data.update({key: value})
 
         new_application = Application(**application_data)
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/middleware.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+import logging
+
 from django.contrib.auth import authenticate
 from django.utils.cache import patch_vary_headers
 
+from oauth2_provider.models import get_access_token_model
+
+
+log = logging.getLogger(__name__)
+
 
 class OAuth2TokenMiddleware:
     """
     Middleware for OAuth2 user authentication
 
     This middleware is able to work along with AuthenticationMiddleware and its behaviour depends
     on the order it's processed with.
@@ -32,7 +39,25 @@
                 user = authenticate(request=request)
                 if user:
                     request.user = request._cached_user = user
 
         response = self.get_response(request)
         patch_vary_headers(response, ("Authorization",))
         return response
+
+
+class OAuth2ExtraTokenMiddleware:
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        authheader = request.META.get("HTTP_AUTHORIZATION", "")
+        if authheader.startswith("Bearer"):
+            tokenstring = authheader.split()[1]
+            AccessToken = get_access_token_model()
+            try:
+                token = AccessToken.objects.get(token=tokenstring)
+                request.access_token = token
+            except AccessToken.DoesNotExist as e:
+                log.exception(e)
+        response = self.get_response(request)
+        return response
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0001_initial.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0002_auto_20190406_1805.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0002_auto_20190406_1805.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0004_auto_20200902_2022.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0004_auto_20200902_2022.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/migrations/0005_auto_20211222_2352.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/migrations/0005_auto_20211222_2352.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/models.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,28 @@
 from jwcrypto import jwk
 from jwcrypto.common import base64url_encode
 from oauthlib.oauth2.rfc6749 import errors
 
 from .generators import generate_client_id, generate_client_secret
 from .scopes import get_scopes_backend
 from .settings import oauth2_settings
-from .validators import RedirectURIValidator, WildcardSet
+from .utils import jwk_from_pem
+from .validators import AllowedURIValidator
 
 
 logger = logging.getLogger(__name__)
 
 
 class ClientSecretField(models.CharField):
     def pre_save(self, model_instance, add):
         secret = getattr(model_instance, self.attname)
+        should_be_hashed = getattr(model_instance, "hash_client_secret", True)
+        if not should_be_hashed:
+            return super().pre_save(model_instance, add)
+
         try:
             hasher = identify_hasher(secret)
             logger.debug(f"{model_instance}: {self.attname} is already hashed with {hasher}.")
         except ValueError:
             logger.debug(f"{model_instance}: {self.attname} is not hashed; hashing it now.")
             hashed_secret = make_password(secret)
             setattr(model_instance, self.attname, hashed_secret)
@@ -105,30 +110,37 @@
     redirect_uris = models.TextField(
         blank=True,
         help_text=_("Allowed URIs list, space separated"),
     )
     post_logout_redirect_uris = models.TextField(
         blank=True,
         help_text=_("Allowed Post Logout URIs list, space separated"),
+        default="",
     )
     client_type = models.CharField(max_length=32, choices=CLIENT_TYPES)
     authorization_grant_type = models.CharField(max_length=32, choices=GRANT_TYPES)
     client_secret = ClientSecretField(
         max_length=255,
         blank=True,
         default=generate_client_secret,
         db_index=True,
         help_text=_("Hashed on Save. Copy it now if this is a new secret."),
     )
+    hash_client_secret = models.BooleanField(default=True)
     name = models.CharField(max_length=255, blank=True)
     skip_authorization = models.BooleanField(default=False)
 
     created = models.DateTimeField(auto_now_add=True)
     updated = models.DateTimeField(auto_now=True)
     algorithm = models.CharField(max_length=5, choices=ALGORITHM_TYPES, default=NO_ALGORITHM, blank=True)
+    allowed_origins = models.TextField(
+        blank=True,
+        help_text=_("Allowed origins list to enable CORS, space separated"),
+        default="",
+    )
 
     class Meta:
         abstract = True
 
     def __str__(self):
         return self.name or self.client_id
 
@@ -161,14 +173,22 @@
         """
         Checks if given URI is one of the items in :attr:`post_logout_redirect_uris` string
 
         :param uri: URI to check
         """
         return redirect_to_uri_allowed(uri, self.post_logout_redirect_uris.split())
 
+    def origin_allowed(self, origin):
+        """
+        Checks if given origin is one of the items in :attr:`allowed_origins` string
+
+        :param origin: Origin to check
+        """
+        return self.allowed_origins and is_origin_allowed(origin, self.allowed_origins.split())
+
     def clean(self):
         from django.core.exceptions import ValidationError
 
         grant_types = (
             AbstractApplication.GRANT_AUTHORIZATION_CODE,
             AbstractApplication.GRANT_IMPLICIT,
             AbstractApplication.GRANT_OPENID_HYBRID,
@@ -178,27 +198,33 @@
             AbstractApplication.GRANT_OPENID_HYBRID,
         )
 
         redirect_uris = self.redirect_uris.strip().split()
         allowed_schemes = set(s.lower() for s in self.get_allowed_schemes())
 
         if redirect_uris:
-            validator = RedirectURIValidator(WildcardSet())
+            validator = AllowedURIValidator(
+                allowed_schemes, name="redirect uri", allow_path=True, allow_query=True
+            )
             for uri in redirect_uris:
                 validator(uri)
-                scheme = urlparse(uri).scheme
-                if scheme not in allowed_schemes:
-                    raise ValidationError(_("Unauthorized redirect scheme: {scheme}").format(scheme=scheme))
 
         elif self.authorization_grant_type in grant_types:
             raise ValidationError(
                 _("redirect_uris cannot be empty with grant_type {grant_type}").format(
                     grant_type=self.authorization_grant_type
                 )
             )
+        allowed_origins = self.allowed_origins.strip().split()
+        if allowed_origins:
+            # oauthlib allows only https scheme for CORS
+            validator = AllowedURIValidator(oauth2_settings.ALLOWED_SCHEMES, "allowed origin")
+            for uri in allowed_origins:
+                validator(uri)
+
         if self.algorithm == AbstractApplication.RS256_ALGORITHM:
             if not oauth2_settings.OIDC_RSA_PRIVATE_KEY:
                 raise ValidationError(_("You must set OIDC_RSA_PRIVATE_KEY to use RSA algorithm"))
 
         if self.algorithm == AbstractApplication.HS256_ALGORITHM:
             if any(
                 (
@@ -230,15 +256,15 @@
         return True
 
     @property
     def jwk_key(self):
         if self.algorithm == AbstractApplication.RS256_ALGORITHM:
             if not oauth2_settings.OIDC_RSA_PRIVATE_KEY:
                 raise ImproperlyConfigured("You must set OIDC_RSA_PRIVATE_KEY to use RSA algorithm")
-            return jwk.JWK.from_pem(oauth2_settings.OIDC_RSA_PRIVATE_KEY.encode("utf8"))
+            return jwk_from_pem(oauth2_settings.OIDC_RSA_PRIVATE_KEY)
         elif self.algorithm == AbstractApplication.HS256_ALGORITHM:
             return jwk.JWK(kty="oct", k=base64url_encode(self.client_secret))
         raise ImproperlyConfigured("This application does not support signed tokens")
 
 
 class ApplicationManager(models.Manager):
     def get_by_natural_key(self, client_id):
@@ -352,14 +378,15 @@
         blank=True,
         null=True,
         related_name="refreshed_access_token",
     )
     token = models.CharField(
         max_length=255,
         unique=True,
+        db_index=True,
     )
     id_token = models.OneToOneField(
         oauth2_settings.ID_TOKEN_MODEL,
         on_delete=models.CASCADE,
         blank=True,
         null=True,
         related_name="access_token",
@@ -765,7 +792,30 @@
             and parsed_allowed_uri.path == parsed_uri.path
         ):
             aqs_set = set(parse_qsl(parsed_allowed_uri.query))
             if aqs_set.issubset(uqs_set):
                 return True
 
     return False
+
+
+def is_origin_allowed(origin, allowed_origins):
+    """
+    Checks if a given origin uri is allowed based on the provided allowed_origins configuration.
+
+    :param origin: Origin URI to check
+    :param allowed_origins: A list of Origin URIs that are allowed
+    """
+
+    parsed_origin = urlparse(origin)
+
+    if parsed_origin.scheme not in oauth2_settings.ALLOWED_SCHEMES:
+        return False
+
+    for allowed_origin in allowed_origins:
+        parsed_allowed_origin = urlparse(allowed_origin)
+        if (
+            parsed_allowed_origin.scheme == parsed_origin.scheme
+            and parsed_allowed_origin.netloc == parsed_origin.netloc
+        ):
+            return True
+    return False
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_backends.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/oauth2_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,19 @@
         headers = request.META.copy()
         if "wsgi.input" in headers:
             del headers["wsgi.input"]
         if "wsgi.errors" in headers:
             del headers["wsgi.errors"]
         if "HTTP_AUTHORIZATION" in headers:
             headers["Authorization"] = headers["HTTP_AUTHORIZATION"]
+        # Add Access-Control-Allow-Origin header to the token endpoint response for authentication code grant,
+        # if the origin is allowed by RequestValidator.is_origin_allowed.
+        # https://github.com/oauthlib/oauthlib/pull/791
+        if "HTTP_ORIGIN" in headers:
+            headers["Origin"] = headers["HTTP_ORIGIN"]
         if request.is_secure():
             headers["X_DJANGO_OAUTH_TOOLKIT_SECURE"] = "1"
         elif "X_DJANGO_OAUTH_TOOLKIT_SECURE" in headers:
             del headers["X_DJANGO_OAUTH_TOOLKIT_SECURE"]
 
         return headers
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/oauth2_validators.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/oauth2_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from collections import OrderedDict
 from datetime import datetime, timedelta
 from urllib.parse import unquote_plus
 
 import requests
 from django.conf import settings
 from django.contrib.auth import authenticate, get_user_model
-from django.contrib.auth.hashers import check_password
+from django.contrib.auth.hashers import check_password, identify_hasher
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import transaction
 from django.db.models import Q
 from django.http import HttpRequest
 from django.utils import dateformat, timezone
+from django.utils.crypto import constant_time_compare
 from django.utils.timezone import make_aware
 from django.utils.translation import gettext_lazy as _
 from jwcrypto import jws, jwt
 from jwcrypto.common import JWException
 from jwcrypto.jwt import JWTExpired
 from oauthlib.oauth2.rfc6749 import utils
 from oauthlib.openid import RequestValidator
@@ -33,14 +34,15 @@
     get_application_model,
     get_grant_model,
     get_id_token_model,
     get_refresh_token_model,
 )
 from .scopes import get_scopes_backend
 from .settings import oauth2_settings
+from .utils import get_timezone
 
 
 log = logging.getLogger("oauth2_provider")
 
 GRANT_TYPE_MAPPING = {
     "authorization_code": (
         AbstractApplication.GRANT_AUTHORIZATION_CODE,
@@ -98,24 +100,36 @@
         Return authentication string if request contains basic auth credentials,
         otherwise return None
         """
         auth = request.headers.get("HTTP_AUTHORIZATION", None)
         if not auth:
             return None
 
-        splitted = auth.split(" ", 1)
-        if len(splitted) != 2:
+        split = auth.split(" ", 1)
+        if len(split) != 2:
             return None
-        auth_type, auth_string = splitted
+        auth_type, auth_string = split
 
         if auth_type != "Basic":
             return None
 
         return auth_string
 
+    def _check_secret(self, provided_secret, stored_secret):
+        """
+        Checks whether the provided client secret is valid.
+
+        Supports both hashed and unhashed secrets.
+        """
+        try:
+            identify_hasher(stored_secret)
+            return check_password(provided_secret, stored_secret)
+        except ValueError:  # Raised if the stored_secret is not hashed.
+            return constant_time_compare(provided_secret, stored_secret)
+
     def _authenticate_basic_auth(self, request):
         """
         Authenticates with HTTP Basic Auth.
 
         Note: as stated in rfc:`2.3.1`, client_id and client_secret must be encoded with
         "application/x-www-form-urlencoded" encoding algorithm.
         """
@@ -148,15 +162,15 @@
 
         if self._load_application(client_id, request) is None:
             log.debug("Failed basic auth: Application %s does not exist" % client_id)
             return False
         elif request.client.client_id != client_id:
             log.debug("Failed basic auth: wrong client id %s" % client_id)
             return False
-        elif not check_password(client_secret, request.client.client_secret):
+        elif not self._check_secret(client_secret, request.client.client_secret):
             log.debug("Failed basic auth: wrong client secret %s" % client_secret)
             return False
         else:
             return True
 
     def _authenticate_request_body(self, request):
         """
@@ -166,22 +180,22 @@
         Remember that this method is NOT RECOMMENDED and SHOULD be limited to
         clients unable to directly utilize the HTTP Basic authentication scheme.
         See rfc:`2.3.1` for more details.
         """
         # TODO: check if oauthlib has already unquoted client_id and client_secret
         try:
             client_id = request.client_id
-            client_secret = getattr(request, "client_secret", "")
+            client_secret = getattr(request, "client_secret", "") or ""
         except AttributeError:
             return False
 
         if self._load_application(client_id, request) is None:
             log.debug("Failed body auth: Application %s does not exists" % client_id)
             return False
-        elif not check_password(client_secret, request.client.client_secret):
+        elif not self._check_secret(client_secret, request.client.client_secret):
             log.debug("Failed body auth: wrong client secret %s" % client_secret)
             return False
         else:
             return True
 
     def _load_application(self, client_id, request):
         """
@@ -288,15 +302,14 @@
 
     def authenticate_client_id(self, client_id, request, *args, **kwargs):
         """
         If we are here, the client did not authenticate itself as in rfc:`3.2.1` and we can
         proceed only if the client exists and is not of type "Confidential".
         """
         if self._load_application(client_id, request) is not None:
-            log.debug("Application %r has type %r" % (client_id, request.client.client_type))
             return request.client.client_type != AbstractApplication.CLIENT_CONFIDENTIAL
         return False
 
     def confirm_redirect_uri(self, client_id, code, redirect_uri, client, *args, **kwargs):
         """
         Ensure the redirect_uri is listed in the Application instance redirect_uris field
         """
@@ -316,14 +329,26 @@
         If it exists, it's assigned to request.client.
         """
         return self._load_application(client_id, request) is not None
 
     def get_default_redirect_uri(self, client_id, request, *args, **kwargs):
         return request.client.default_redirect_uri
 
+    def get_or_create_user_from_content(self, content):
+        """
+        An optional layer to define where to store the profile in `UserModel` or a separate model.
+        For example `UserOAuth`, where `user = models.OneToOneField(UserModel)` .
+
+        The function is called after checking that username is in the content.
+
+        Returns an UserModel instance;
+        """
+        user, _ = UserModel.objects.get_or_create(**{UserModel.USERNAME_FIELD: content["username"]})
+        return user
+
     def _get_token_from_authentication_server(
         self, token, introspection_url, introspection_token, introspection_credentials
     ):
         """Use external introspection endpoint to "crack open" the token.
         :param introspection_url: introspection endpoint URL
         :param introspection_token: Bearer token
         :param introspection_credentials: Basic Auth credentials (id,secret)
@@ -366,17 +391,15 @@
             content = response.json()
         except ValueError:
             log.exception("Introspection: Failed to parse response as json")
             return None
 
         if "active" in content and content["active"] is True:
             if "username" in content:
-                user, _created = UserModel.objects.get_or_create(
-                    **{UserModel.USERNAME_FIELD: content["username"]}
-                )
+                user = self.get_or_create_user_from_content(content)
             else:
                 user = None
 
             max_caching_time = datetime.now() + timedelta(
                 seconds=oauth2_settings.RESOURCE_SERVER_TOKEN_CACHING_SECONDS
             )
 
@@ -384,15 +407,19 @@
                 expires = datetime.utcfromtimestamp(content["exp"])
                 if expires > max_caching_time:
                     expires = max_caching_time
             else:
                 expires = max_caching_time
 
             scope = content.get("scope", "")
-            expires = make_aware(expires) if settings.USE_TZ else expires
+
+            if settings.USE_TZ:
+                expires = make_aware(
+                    expires, timezone=get_timezone(oauth2_settings.AUTHENTICATION_SERVER_EXP_TIME_ZONE)
+                )
 
             access_token, _created = AccessToken.objects.update_or_create(
                 token=token,
                 defaults={
                     "user": user,
                     "application": None,
                     "scope": scope,
@@ -532,15 +559,15 @@
 
     @transaction.atomic
     def save_bearer_token(self, token, request, *args, **kwargs):
         """
         Save access and refresh token, If refresh token is issued, remove or
         reuse old refresh token as in rfc:`6`
 
-        @see: https://tools.ietf.org/html/draft-ietf-oauth-v2-31#page-43
+        @see: https://rfc-editor.org/rfc/rfc6749.html#section-6
         """
 
         if "scope" not in token:
             raise FatalClientError("Failed to renew access token: missing scope")
 
         # expires_in is passed to Server on initialization
         # custom server class can have logic to override this
@@ -709,16 +736,18 @@
         return False
 
     def get_original_scopes(self, refresh_token, request, *args, **kwargs):
         # Avoid second query for RefreshToken since this method is invoked *after*
         # validate_refresh_token.
         rt = request.refresh_token_instance
         if not rt.access_token_id:
-            return AccessToken.objects.get(source_refresh_token_id=rt.id).scope
-
+            try:
+                return AccessToken.objects.get(source_refresh_token_id=rt.id).scope
+            except AccessToken.DoesNotExist:
+                return []
         return rt.access_token.scope
 
     def validate_refresh_token(self, refresh_token, client, request, *args, **kwargs):
         """
         Check refresh_token exists and refers to the right client.
         Also attach User instance to the request object
         """
@@ -904,15 +933,15 @@
         This function is separate to allow further customization.
         """
         if isinstance(audience, str):
             audience = [audience]
         return Application.objects.filter(client_id__in=audience).first()
 
     def validate_user_match(self, id_token_hint, scopes, claims, request):
-        # TODO: Fix to validate when necessary acording
+        # TODO: Fix to validate when necessary according
         # https://github.com/idan/oauthlib/blob/master/oauthlib/oauth2/rfc6749/request_validator.py#L556
         # http://openid.net/specs/openid-connect-core-1_0.html#AuthRequest id_token_hint section
         return True
 
     def get_authorization_code_nonce(self, client_id, code, redirect_uri, request):
         """Extracts nonce from saved authorization code.
         If present in the Authentication Request, Authorization
@@ -941,7 +970,17 @@
         current user's claims.
 
         """
         return self.get_oidc_claims(request.access_token, None, request)
 
     def get_additional_claims(self, request):
         return {}
+
+    def is_origin_allowed(self, client_id, origin, request, *args, **kwargs):
+        """Indicate if the given origin is allowed to access the token endpoint
+        via Cross-Origin Resource Sharing (CORS).  CORS is used by browser-based
+        clients, such as Single-Page Applications, to perform the Authorization
+        Code Grant.
+
+        Verifies if request's origin is within Application's allowed origins list.
+        """
+        return request.client.origin_allowed(origin)
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/scopes.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/scopes.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/settings.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 This module provides the `oauth2_settings` object, that is used to access
 OAuth2 Provider settings, checking for user settings first, then falling
 back to the defaults.
 """
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
+from django.core.signals import setting_changed
 from django.http import HttpRequest
-from django.test.signals import setting_changed
 from django.urls import reverse
 from django.utils.module_loading import import_string
 from oauthlib.common import Request
 
 
 USER_SETTINGS = getattr(settings, "OAUTH2_PROVIDER", None)
 
@@ -64,14 +64,15 @@
     "APPLICATION_ADMIN_CLASS": "oauth2_provider.admin.ApplicationAdmin",
     "ACCESS_TOKEN_ADMIN_CLASS": "oauth2_provider.admin.AccessTokenAdmin",
     "GRANT_ADMIN_CLASS": "oauth2_provider.admin.GrantAdmin",
     "ID_TOKEN_ADMIN_CLASS": "oauth2_provider.admin.IDTokenAdmin",
     "REFRESH_TOKEN_ADMIN_CLASS": "oauth2_provider.admin.RefreshTokenAdmin",
     "REQUEST_APPROVAL_PROMPT": "force",
     "ALLOWED_REDIRECT_URI_SCHEMES": ["http", "https"],
+    "ALLOWED_SCHEMES": ["https"],
     "OIDC_ENABLED": False,
     "OIDC_ISS_ENDPOINT": "",
     "OIDC_USERINFO_ENDPOINT": "",
     "OIDC_RSA_PRIVATE_KEY": "",
     "OIDC_RSA_PRIVATE_KEYS_INACTIVE": [],
     "OIDC_JWKS_MAX_AGE_SECONDS": 3600,
     "OIDC_RESPONSE_TYPES_SUPPORTED": [
@@ -97,14 +98,16 @@
     "_SCOPES": [],
     "_DEFAULT_SCOPES": [],
     # Resource Server with Token Introspection
     "RESOURCE_SERVER_INTROSPECTION_URL": None,
     "RESOURCE_SERVER_AUTH_TOKEN": None,
     "RESOURCE_SERVER_INTROSPECTION_CREDENTIALS": None,
     "RESOURCE_SERVER_TOKEN_CACHING_SECONDS": 36000,
+    # Authentication Server Exp Timezone: the time zone use dby Auth Server for generate EXP
+    "AUTHENTICATION_SERVER_EXP_TIME_ZONE": "UTC",
     # Whether or not PKCE is required
     "PKCE_REQUIRED": True,
     # Whether to re-create OAuthlibCore on every request.
     # Should only be required in testing.
     "ALWAYS_RELOAD_OAUTHLIB_CORE": False,
     "CLEAR_EXPIRED_TOKENS_BATCH_SIZE": 10000,
     "CLEAR_EXPIRED_TOKENS_BATCH_INTERVAL": 0,
@@ -290,15 +293,15 @@
             django_request = _PhonyHttpRequest()
             django_request.META = request.headers
             if request.headers.get("X_DJANGO_OAUTH_TOOLKIT_SECURE", False):
                 django_request._scheme = "https"
         else:
             raise TypeError("request must be a django or oauthlib request: got %r" % request)
         abs_url = django_request.build_absolute_uri(reverse("oauth2_provider:oidc-connect-discovery-info"))
-        return abs_url[: -len("/.well-known/openid-configuration/")]
+        return abs_url[: -len("/.well-known/openid-configuration")]
 
 
 oauth2_settings = OAuth2ProviderSettings(USER_SETTINGS, DEFAULTS, IMPORT_STRINGS, MANDATORY)
 
 
 def reload_oauth2_settings(*args, **kwargs):
     setting = kwargs["setting"]
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_detail.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_detail.html`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,42 @@
 
             <li>
                 <p><b>{% trans "Client secret" %}</b></p>
                 <input class="input-block-level" type="text" value="{{ application.client_secret }}" readonly>
             </li>
 
             <li>
+                <p><b>{% trans "Hash client secret" %}</b></p>
+                <p>{{ application.hash_client_secret|yesno:_("yes,no") }}</p>
+            </li>
+
+            <li>
                 <p><b>{% trans "Client type" %}</b></p>
                 <p>{{ application.client_type }}</p>
             </li>
 
             <li>
                 <p><b>{% trans "Authorization Grant Type" %}</b></p>
                 <p>{{ application.authorization_grant_type }}</p>
             </li>
 
             <li>
                 <p><b>{% trans "Redirect Uris" %}</b></p>
                 <textarea class="input-block-level" readonly>{{ application.redirect_uris }}</textarea>
             </li>
+
+            <li>
+                <p><b>{% trans "Post Logout Redirect Uris" %}</b></p>
+                <textarea class="input-block-level" readonly>{{ application.post_logout_redirect_uris }}</textarea>
+            </li>
+
+            <li>
+                <p><b>{% trans "Allowed Origins" %}</b></p>
+                <textarea class="input-block-level" readonly>{{ application.allowed_origins }}</textarea>
+            </li>
         </ul>
 
         <div class="btn-toolbar">
             <a class="btn" href="{% url "oauth2_provider:list" %}">{% trans "Go Back" %}</a>
             <a class="btn btn-primary" href="{% url "oauth2_provider:update" application.id %}">{% trans "Edit" %}</a>
             <a class="btn btn-danger" href="{% url "oauth2_provider:delete" application.id %}">{% trans "Delete" %}</a>
         </div>
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_form.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_form.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/application_list.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/application_list.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorize.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/authorized-tokens.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/base.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/base.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/templates/oauth2_provider/logout_confirm.html` & `django_oauth_toolkit-2.4.0/oauth2_provider/templates/oauth2_provider/logout_confirm.html`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/urls.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,16 +27,20 @@
         r"^authorized_tokens/(?P<pk>[\w-]+)/delete/$",
         views.AuthorizedTokenDeleteView.as_view(),
         name="authorized-token-delete",
     ),
 ]
 
 oidc_urlpatterns = [
+    # .well-known/openid-configuration/ is deprecated
+    # https://openid.net/specs/openid-connect-discovery-1_0.html#ProviderConfig
+    # does not specify a trailing slash
+    # Support for trailing slash shall be removed in a future release.
     re_path(
-        r"^\.well-known/openid-configuration/$",
+        r"^\.well-known/openid-configuration/?$",
         views.ConnectDiscoveryInfoView.as_view(),
         name="oidc-connect-discovery-info",
     ),
     re_path(r"^\.well-known/jwks.json$", views.JwksInfoView.as_view(), name="jwks-info"),
     re_path(r"^userinfo/$", views.UserInfoView.as_view(), name="user-info"),
     re_path(r"^logout/$", views.RPInitiatedLogoutView.as_view(), name="rp-initiated-logout"),
 ]
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/__init__.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/application.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,20 @@
         """
         return modelform_factory(
             get_application_model(),
             fields=(
                 "name",
                 "client_id",
                 "client_secret",
+                "hash_client_secret",
                 "client_type",
                 "authorization_grant_type",
                 "redirect_uris",
+                "post_logout_redirect_uris",
+                "allowed_origins",
                 "algorithm",
             ),
         )
 
     def form_valid(self, form):
         form.instance.user = self.request.user
         return super().form_valid(form)
@@ -88,13 +91,16 @@
         """
         return modelform_factory(
             get_application_model(),
             fields=(
                 "name",
                 "client_id",
                 "client_secret",
+                "hash_client_secret",
                 "client_type",
                 "authorization_grant_type",
                 "redirect_uris",
+                "post_logout_redirect_uris",
+                "allowed_origins",
                 "algorithm",
             ),
         )
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/base.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,18 +73,18 @@
     This endpoint is reached two times during the authorization process:
     * first receive a ``GET`` request from user asking authorization for a certain client
     application, a form is served possibly showing some useful info and prompting for
     *authorize/do not authorize*.
 
     * then receive a ``POST`` request possibly after user authorized the access
 
-    Some informations contained in the ``GET`` request and needed to create a Grant token during
+    Some information contained in the ``GET`` request and needed to create a Grant token during
     the ``POST`` request would be lost between the two steps above, so they are temporarily stored in
     hidden fields on the form.
-    A possible alternative could be keeping such informations in the session.
+    A possible alternative could be keeping such information in the session.
 
     The endpoint is used in the following flows:
     * Authorization code
     * Implicit grant
     """
 
     template_name = "oauth2_provider/authorize.html"
@@ -240,14 +240,41 @@
 
         return redirect_to_login(
             parsed.geturl(),
             resolved_login_url,
             self.get_redirect_field_name(),
         )
 
+    def handle_no_permission(self):
+        """
+        Generate response for unauthorized users.
+
+        If prompt is set to none, then we redirect with an error code
+        as defined by OIDC 3.1.2.6
+
+        Some code copied from OAuthLibMixin.error_response, but that is designed
+        to operated on OAuth1Error from oauthlib wrapped in a OAuthToolkitError
+        """
+        prompt = self.request.GET.get("prompt")
+        redirect_uri = self.request.GET.get("redirect_uri")
+        if prompt == "none" and redirect_uri:
+            response_parameters = {"error": "login_required"}
+
+            # REQUIRED if the Authorization Request included the state parameter.
+            # Set to the value received from the Client
+            state = self.request.GET.get("state")
+            if state:
+                response_parameters["state"] = state
+
+            separator = "&" if "?" in redirect_uri else "?"
+            redirect_to = redirect_uri + separator + urlencode(response_parameters)
+            return self.redirect(redirect_to, application=None)
+        else:
+            return super().handle_no_permission()
+
 
 @method_decorator(csrf_exempt, name="dispatch")
 class TokenView(OAuthLibMixin, View):
     """
     Implements an endpoint to provide access tokens
 
     The endpoint is used in the following flows:
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/generic.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/generic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from django.views.generic import View
 
 from .mixins import (
     ClientProtectedResourceMixin,
-    OAuthLibMixin,
     ProtectedResourceMixin,
     ReadWriteScopedResourceMixin,
     ScopedResourceMixin,
 )
 
 
-class ProtectedResourceView(ProtectedResourceMixin, OAuthLibMixin, View):
+class ProtectedResourceView(ProtectedResourceMixin, View):
     """
     Generic view protecting resources by providing OAuth2 authentication out of the box
     """
 
     pass
 
 
@@ -31,21 +30,19 @@
     Generic view protecting resources with OAuth2 authentication and read/write scopes.
     GET, HEAD, OPTIONS http methods require "read" scope. Otherwise "write" scope is required.
     """
 
     pass
 
 
-class ClientProtectedResourceView(ClientProtectedResourceMixin, OAuthLibMixin, View):
-
+class ClientProtectedResourceView(ClientProtectedResourceMixin, View):
     """View for protecting a resource with client-credentials method.
     This involves allowing access tokens, Basic Auth and plain credentials in request body.
     """
 
     pass
 
 
 class ClientProtectedScopedResourceView(ScopedResourceMixin, ClientProtectedResourceView):
-
     """Impose scope restrictions if client protection fallsback to access token."""
 
     pass
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/introspect.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/introspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from oauth2_provider.views.generic import ClientProtectedScopedResourceView
 
 
 @method_decorator(csrf_exempt, name="dispatch")
 class IntrospectTokenView(ClientProtectedScopedResourceView):
     """
     Implements an endpoint for token introspection based
-    on RFC 7662 https://tools.ietf.org/html/rfc7662
+    on RFC 7662 https://rfc-editor.org/rfc/rfc7662.html
 
     To access this view the request must pass a OAuth2 Bearer Token
     which is allowed to access the scope `introspection`.
     """
 
     required_scopes = ["introspection"]
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/mixins.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,14 @@
         scopes = super().get_scopes(*args, **kwargs)
 
         # this returns a copy so that self.required_scopes is not modified
         return scopes + [self.read_write_scope]
 
 
 class ClientProtectedResourceMixin(OAuthLibMixin):
-
     """Mixin for protecting resources with client authentication as mentioned in rfc:`3.2.1`
     This involves authenticating with any of: HTTP Basic Auth, Client Credentials and
     Access token in that order. Breaks off after first validation.
     """
 
     def dispatch(self, request, *args, **kwargs):
         # let preflight OPTIONS requests pass
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/oidc.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/oidc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
+import warnings
 from urllib.parse import urlparse
 
 from django.contrib.auth import logout
+from django.contrib.auth.models import AnonymousUser
 from django.http import HttpResponse, JsonResponse
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.views.decorators.csrf import csrf_exempt
 from django.views.generic import FormView, View
-from jwcrypto import jwk, jwt
+from jwcrypto import jwt
 from jwcrypto.common import JWException
 from jwcrypto.jws import InvalidJWSObject
 from jwcrypto.jwt import JWTExpired
 from oauthlib.common import add_params_to_uri
 
 from ..exceptions import (
     ClientIdMissmatch,
@@ -20,20 +22,22 @@
     InvalidOIDCRedirectURIError,
     LogoutDenied,
     OIDCError,
 )
 from ..forms import ConfirmLogoutForm
 from ..http import OAuth2ResponseRedirect
 from ..models import (
+    AbstractGrant,
     get_access_token_model,
     get_application_model,
     get_id_token_model,
     get_refresh_token_model,
 )
 from ..settings import oauth2_settings
+from ..utils import jwk_from_pem
 from .mixins import OAuthLibMixin, OIDCLogoutOnlyMixin, OIDCOnlyMixin
 
 
 Application = get_application_model()
 
 
 class ConnectDiscoveryInfoView(OIDCOnlyMixin, View):
@@ -89,14 +93,15 @@
             "scopes_supported": scopes_supported,
             "response_types_supported": oauth2_settings.OIDC_RESPONSE_TYPES_SUPPORTED,
             "subject_types_supported": oauth2_settings.OIDC_SUBJECT_TYPES_SUPPORTED,
             "id_token_signing_alg_values_supported": signing_algorithms,
             "token_endpoint_auth_methods_supported": (
                 oauth2_settings.OIDC_TOKEN_ENDPOINT_AUTH_METHODS_SUPPORTED
             ),
+            "code_challenge_methods_supported": [key for key, _ in AbstractGrant.CODE_CHALLENGE_METHODS],
             "claims_supported": oidc_claims,
         }
         if oauth2_settings.OIDC_RP_INITIATED_LOGOUT_ENABLED:
             data["end_session_endpoint"] = end_session_endpoint
         response = JsonResponse(data)
         response["Access-Control-Allow-Origin"] = "*"
         return response
@@ -110,15 +115,15 @@
     def get(self, request, *args, **kwargs):
         keys = []
         if oauth2_settings.OIDC_RSA_PRIVATE_KEY:
             for pem in [
                 oauth2_settings.OIDC_RSA_PRIVATE_KEY,
                 *oauth2_settings.OIDC_RSA_PRIVATE_KEYS_INACTIVE,
             ]:
-                key = jwk.JWK.from_pem(pem.encode("utf8"))
+                key = jwk_from_pem(pem)
                 data = {"alg": "RS256", "use": "sig", "kid": key.thumbprint()}
                 data.update(json.loads(key.export_public()))
                 keys.append(data)
         response = JsonResponse({"keys": keys})
         response["Access-Control-Allow-Origin"] = "*"
         response["Cache-Control"] = (
             "Cache-Control: public, "
@@ -219,14 +224,16 @@
     be set to the Application that is requesting the logout. `token_user` is the id_token user, which will
     used to revoke the tokens if found.
 
     The `id_token_hint` will be validated if given. If both `client_id` and `id_token_hint` are given they
     will be validated against each other.
     """
 
+    warnings.warn("This method is deprecated and will be removed in version 2.5.0.", DeprecationWarning)
+
     id_token = None
     must_prompt_logout = True
     token_user = None
     if id_token_hint:
         # Only basic validation has been done on the IDToken at this point.
         id_token, claims = _load_id_token(id_token_hint)
 
@@ -309,25 +316,24 @@
     def get(self, request, *args, **kwargs):
         id_token_hint = request.GET.get("id_token_hint")
         client_id = request.GET.get("client_id")
         post_logout_redirect_uri = request.GET.get("post_logout_redirect_uri")
         state = request.GET.get("state")
 
         try:
-            prompt, (redirect_uri, application), token_user = validate_logout_request(
-                request=request,
+            application, token_user = self.validate_logout_request(
                 id_token_hint=id_token_hint,
                 client_id=client_id,
                 post_logout_redirect_uri=post_logout_redirect_uri,
             )
         except OIDCError as error:
             return self.error_response(error)
 
-        if not prompt:
-            return self.do_logout(application, redirect_uri, state, token_user)
+        if not self.must_prompt(token_user):
+            return self.do_logout(application, post_logout_redirect_uri, state, token_user)
 
         self.oidc_data = {
             "id_token_hint": id_token_hint,
             "client_id": client_id,
             "post_logout_redirect_uri": post_logout_redirect_uri,
             "state": state,
         }
@@ -341,36 +347,116 @@
     def form_valid(self, form):
         id_token_hint = form.cleaned_data.get("id_token_hint")
         client_id = form.cleaned_data.get("client_id")
         post_logout_redirect_uri = form.cleaned_data.get("post_logout_redirect_uri")
         state = form.cleaned_data.get("state")
 
         try:
-            prompt, (redirect_uri, application), token_user = validate_logout_request(
-                request=self.request,
+            application, token_user = self.validate_logout_request(
                 id_token_hint=id_token_hint,
                 client_id=client_id,
                 post_logout_redirect_uri=post_logout_redirect_uri,
             )
 
-            if not prompt or form.cleaned_data.get("allow"):
-                return self.do_logout(application, redirect_uri, state, token_user)
+            if not self.must_prompt(token_user) or form.cleaned_data.get("allow"):
+                return self.do_logout(application, post_logout_redirect_uri, state, token_user)
             else:
                 raise LogoutDenied()
 
         except OIDCError as error:
             return self.error_response(error)
 
+    def validate_post_logout_redirect_uri(self, application, post_logout_redirect_uri):
+        """
+        Validate the OIDC RP-Initiated Logout Request post_logout_redirect_uri parameter
+        """
+
+        if not post_logout_redirect_uri:
+            return
+
+        if not application:
+            raise InvalidOIDCClientError()
+        scheme = urlparse(post_logout_redirect_uri)[0]
+        if not scheme:
+            raise InvalidOIDCRedirectURIError("A Scheme is required for the redirect URI.")
+        if oauth2_settings.OIDC_RP_INITIATED_LOGOUT_STRICT_REDIRECT_URIS and (
+            scheme == "http" and application.client_type != "confidential"
+        ):
+            raise InvalidOIDCRedirectURIError("http is only allowed with confidential clients.")
+        if scheme not in application.get_allowed_schemes():
+            raise InvalidOIDCRedirectURIError(f'Redirect to scheme "{scheme}" is not permitted.')
+        if not application.post_logout_redirect_uri_allowed(post_logout_redirect_uri):
+            raise InvalidOIDCRedirectURIError("This client does not have this redirect uri registered.")
+
+    def validate_logout_request_user(self, id_token_hint, client_id):
+        """
+        Validate the an OIDC RP-Initiated Logout Request user
+        """
+
+        if not id_token_hint:
+            return
+
+        # Only basic validation has been done on the IDToken at this point.
+        id_token, claims = _load_id_token(id_token_hint)
+
+        if not id_token or not _validate_claims(self.request, claims):
+            raise InvalidIDTokenError()
+
+        # If both id_token_hint and client_id are given it must be verified that they match.
+        if client_id:
+            if id_token.application.client_id != client_id:
+                raise ClientIdMissmatch()
+
+        return id_token
+
+    def get_request_application(self, id_token, client_id):
+        if client_id:
+            return get_application_model().objects.get(client_id=client_id)
+        if id_token:
+            return id_token.application
+
+    def validate_logout_request(self, id_token_hint, client_id, post_logout_redirect_uri):
+        """
+        Validate an OIDC RP-Initiated Logout Request.
+        `(application, token_user)` is returned.
+
+        If it is set, `application` is the Application that is requesting the logout.
+        `token_user` is the id_token user, which will used to revoke the tokens if found.
+
+        The `id_token_hint` will be validated if given. If both `client_id` and `id_token_hint` are given they
+        will be validated against each other.
+        """
+
+        id_token = self.validate_logout_request_user(id_token_hint, client_id)
+        application = self.get_request_application(id_token, client_id)
+        self.validate_post_logout_redirect_uri(application, post_logout_redirect_uri)
+
+        return application, id_token.user if id_token else None
+
+    def must_prompt(self, token_user):
+        """Indicate whether the logout has to be confirmed by the user. This happens if the
+        specifications force a confirmation, or it is enabled by `OIDC_RP_INITIATED_LOGOUT_ALWAYS_PROMPT`.
+
+        A logout without user interaction (i.e. no prompt) is only allowed
+        if an ID Token is provided that matches the current user.
+        """
+        return (
+            oauth2_settings.OIDC_RP_INITIATED_LOGOUT_ALWAYS_PROMPT
+            or token_user is None
+            or token_user != self.request.user
+        )
+
     def do_logout(self, application=None, post_logout_redirect_uri=None, state=None, token_user=None):
-        # Delete Access Tokens
-        if oauth2_settings.OIDC_RP_INITIATED_LOGOUT_DELETE_TOKENS:
+        user = token_user or self.request.user
+        # Delete Access Tokens if a user was found
+        if oauth2_settings.OIDC_RP_INITIATED_LOGOUT_DELETE_TOKENS and not isinstance(user, AnonymousUser):
             AccessToken = get_access_token_model()
             RefreshToken = get_refresh_token_model()
             access_tokens_to_delete = AccessToken.objects.filter(
-                user=token_user or self.request.user,
+                user=user,
                 application__client_type__in=self.token_deletion_client_types,
                 application__authorization_grant_type__in=self.token_deletion_grant_types,
             )
             # This queryset has to be evaluated eagerly. The queryset would be empty with lazy evaluation
             # because `access_tokens_to_delete` represents an empty queryset once `refresh_tokens_to_delete`
             # is evaluated as all AccessTokens have been deleted.
             refresh_tokens_to_delete = list(
```

### Comparing `django-oauth-toolkit-2.3.0/oauth2_provider/views/token.py` & `django_oauth_toolkit-2.4.0/oauth2_provider/views/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     context_object_name = "authorized_tokens"
     template_name = "oauth2_provider/authorized-tokens.html"
     model = get_access_token_model()
 
     def get_queryset(self):
         """
-        Show only user"s tokens
+        Show only user's tokens
         """
         return super().get_queryset().select_related("application").filter(user=self.request.user)
 
 
 class AuthorizedTokenDeleteView(LoginRequiredMixin, DeleteView):
     """
     View for revoking a specific token
```

### Comparing `django-oauth-toolkit-2.3.0/setup.cfg` & `django_oauth_toolkit-2.4.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -8,39 +8,41 @@
 author_email = synasius@gmail.com
 url = https://github.com/jazzband/django-oauth-toolkit
 keywords = django, oauth, oauth2, oauthlib
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 2.2
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
+python_requires = >=3.8
 install_requires = 
-	django >= 2.2, != 4.0.0
+	django >= 3.2, != 4.0.0
 	requests >= 2.13.0
 	oauthlib >= 3.1.0
 	jwcrypto >= 0.8.0
+	pytz >= 2024.1
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [egg_info]
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_auth_backends.py` & `django_oauth_toolkit-2.4.0/tests/test_auth_backends.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,45 +6,42 @@
 from django.core.exceptions import SuspiciousOperation
 from django.http import HttpResponse
 from django.test import RequestFactory, TestCase
 from django.test.utils import modify_settings, override_settings
 from django.utils.timezone import now, timedelta
 
 from oauth2_provider.backends import OAuth2Backend
-from oauth2_provider.middleware import OAuth2TokenMiddleware
+from oauth2_provider.middleware import OAuth2ExtraTokenMiddleware, OAuth2TokenMiddleware
 from oauth2_provider.models import get_access_token_model, get_application_model
 
 
 UserModel = get_user_model()
 ApplicationModel = get_application_model()
 AccessTokenModel = get_access_token_model()
 
 
 class BaseTest(TestCase):
     """
     Base class for cases in this module
     """
 
-    def setUp(self):
-        self.user = UserModel.objects.create_user("user", "test@example.com", "123456")
-        self.app = ApplicationModel.objects.create(
+    factory = RequestFactory()
+
+    @classmethod
+    def setUpTestData(cls):
+        cls.user = UserModel.objects.create_user("user", "test@example.com", "123456")
+        cls.app = ApplicationModel.objects.create(
             name="app",
             client_type=ApplicationModel.CLIENT_CONFIDENTIAL,
             authorization_grant_type=ApplicationModel.GRANT_CLIENT_CREDENTIALS,
-            user=self.user,
+            user=cls.user,
         )
-        self.token = AccessTokenModel.objects.create(
-            user=self.user, token="tokstr", application=self.app, expires=now() + timedelta(days=365)
+        cls.token = AccessTokenModel.objects.create(
+            user=cls.user, token="tokstr", application=cls.app, expires=now() + timedelta(days=365)
         )
-        self.factory = RequestFactory()
-
-    def tearDown(self):
-        self.user.delete()
-        self.app.delete()
-        self.token.delete()
 
 
 class TestOAuth2Backend(BaseTest):
     def test_authenticate(self):
         auth_headers = {
             "HTTP_AUTHORIZATION": "Bearer " + "tokstr",
         }
@@ -99,18 +96,14 @@
 )
 @modify_settings(
     MIDDLEWARE={
         "append": "oauth2_provider.middleware.OAuth2TokenMiddleware",
     }
 )
 class TestOAuth2Middleware(BaseTest):
-    def setUp(self):
-        super().setUp()
-        self.anon_user = AnonymousUser()
-
     def dummy_get_response(self, request):
         return HttpResponse()
 
     def test_middleware_wrong_headers(self):
         m = OAuth2TokenMiddleware(self.dummy_get_response)
         request = self.factory.get("/a-resource")
         m(request)
@@ -127,15 +120,15 @@
         auth_headers = {
             "HTTP_AUTHORIZATION": "Bearer " + "tokstr",
         }
         request = self.factory.get("/a-resource", **auth_headers)
         request.user = self.user
         m(request)
         self.assertIs(request.user, self.user)
-        request.user = self.anon_user
+        request.user = AnonymousUser()
         m(request)
         self.assertEqual(request.user.pk, self.user.pk)
 
     def test_middleware_success(self):
         m = OAuth2TokenMiddleware(self.dummy_get_response)
         auth_headers = {
             "HTTP_AUTHORIZATION": "Bearer " + "tokstr",
@@ -158,7 +151,62 @@
         auth_headers = {
             "HTTP_AUTHORIZATION": "Bearer " + "tokstr",
         }
         request = self.factory.get("/a-resource", **auth_headers)
         response = m(request)
         self.assertIn("Vary", response)
         self.assertIn("Authorization", response["Vary"])
+
+
+@override_settings(
+    AUTHENTICATION_BACKENDS=(
+        "oauth2_provider.backends.OAuth2Backend",
+        "django.contrib.auth.backends.ModelBackend",
+    ),
+)
+@modify_settings(
+    MIDDLEWARE={
+        "append": "oauth2_provider.middleware.OAuth2TokenMiddleware",
+    }
+)
+class TestOAuth2ExtraTokenMiddleware(BaseTest):
+    def dummy_get_response(self, request):
+        return HttpResponse()
+
+    def test_middleware_wrong_headers(self):
+        m = OAuth2ExtraTokenMiddleware(self.dummy_get_response)
+        request = self.factory.get("/a-resource")
+        m(request)
+        self.assertFalse(hasattr(request, "access_token"))
+        auth_headers = {
+            "HTTP_AUTHORIZATION": "Beerer " + "badstring",  # a Beer token for you!
+        }
+        request = self.factory.get("/a-resource", **auth_headers)
+        m(request)
+        self.assertFalse(hasattr(request, "access_token"))
+
+    def test_middleware_token_does_not_exist(self):
+        m = OAuth2ExtraTokenMiddleware(self.dummy_get_response)
+        auth_headers = {
+            "HTTP_AUTHORIZATION": "Bearer " + "badtokstr",
+        }
+        request = self.factory.get("/a-resource", **auth_headers)
+        m(request)
+        self.assertFalse(hasattr(request, "access_token"))
+
+    def test_middleware_success(self):
+        m = OAuth2ExtraTokenMiddleware(self.dummy_get_response)
+        auth_headers = {
+            "HTTP_AUTHORIZATION": "Bearer " + "tokstr",
+        }
+        request = self.factory.get("/a-resource", **auth_headers)
+        m(request)
+        self.assertEqual(request.access_token, self.token)
+
+    def test_middleware_response(self):
+        m = OAuth2ExtraTokenMiddleware(self.dummy_get_response)
+        auth_headers = {
+            "HTTP_AUTHORIZATION": "Bearer " + "tokstr",
+        }
+        request = self.factory.get("/a-resource", **auth_headers)
+        response = m(request)
+        self.assertIsInstance(response, HttpResponse)
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_authorization_code.py` & `django_oauth_toolkit-2.4.0/tests/test_authorization_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,37 +39,35 @@
 class ResourceView(ProtectedResourceView):
     def get(self, request, *args, **kwargs):
         return "This is a protected resource"
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    factory = RequestFactory()
 
-        self.oauth2_settings.ALLOWED_REDIRECT_URI_SCHEMES = ["http", "custom-scheme"]
-        self.oauth2_settings.PKCE_REQUIRED = False
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
 
-        self.application = Application.objects.create(
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris=(
                 "http://localhost http://example.com http://example.org custom-scheme://example.com"
             ),
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
             client_secret=CLEARTEXT_SECRET,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        self.test_user.delete()
-        self.dev_user.delete()
+    def setUp(self):
+        self.oauth2_settings.ALLOWED_REDIRECT_URI_SCHEMES = ["http", "custom-scheme"]
+        self.oauth2_settings.PKCE_REQUIRED = False
 
 
 class TestRegressionIssue315(BaseTest):
     """
     Test to avoid regression for the issue 315: request object
     was being reassigned when getting AuthorizationView
     """
@@ -479,15 +477,15 @@
         self.assertIn("error=access_denied", response["Location"])
         self.assertIn("state=random_state_string", response["Location"])
 
     def test_code_post_auth_redirection_uri_with_querystring(self):
         """
         Tests that a redirection uri with query string is allowed
         and query string is retained on redirection.
-        See http://tools.ietf.org/html/rfc6749#section-3.1.2
+        See https://rfc-editor.org/rfc/rfc6749.html#section-3.1.2
         """
         self.client.login(username="test_user", password="123456")
 
         form_data = {
             "client_id": self.application.client_id,
             "state": "random_state_string",
             "scope": "read write",
@@ -543,14 +541,41 @@
 
         response = self.client.post(reverse("oauth2_provider:authorize"), data=form_data)
         self.assertEqual(response.status_code, 400)
 
 
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestOIDCAuthorizationCodeView(BaseTest):
+    def test_login(self):
+        """
+        Test login page is rendered if user is not authenticated
+        """
+        self.oauth2_settings.PKCE_REQUIRED = False
+
+        query_data = {
+            "client_id": self.application.client_id,
+            "response_type": "code",
+            "state": "random_state_string",
+            "scope": "openid",
+            "redirect_uri": "http://example.org",
+        }
+        path = reverse("oauth2_provider:authorize")
+        response = self.client.get(path, data=query_data)
+        # The authorization view redirects to the login page with the
+        self.assertEqual(response.status_code, 302)
+        scheme, netloc, path, params, query, fragment = urlparse(response["Location"])
+        self.assertEqual(path, settings.LOGIN_URL)
+        parsed_query = parse_qs(query)
+        next = parsed_query["next"][0]
+        self.assertIn(f"client_id={self.application.client_id}", next)
+        self.assertIn("response_type=code", next)
+        self.assertIn("state=random_state_string", next)
+        self.assertIn("scope=openid", next)
+        self.assertIn("redirect_uri=http%3A%2F%2Fexample.org", next)
+
     def test_id_token_skip_authorization_completely(self):
         """
         If application.skip_authorization = True, should skip the authorization page.
         """
         self.client.login(username="test_user", password="123456")
         self.application.skip_authorization = True
         self.application.save()
@@ -643,14 +668,41 @@
         self.assertIn("redirect_uri=http%3A%2F%2Fexample.org", next)
         self.assertIn("state=random_state_string", next)
         self.assertIn("scope=read+write", next)
         self.assertIn(f"client_id={self.application.client_id}", next)
 
         self.assertNotIn("prompt=login", next)
 
+    def test_prompt_none_unauthorized(self):
+        """
+        Test response for redirect when supplied with prompt: none
+
+        Should redirect to redirect_uri with an error of login_required
+        """
+        self.oauth2_settings.PKCE_REQUIRED = False
+
+        query_data = {
+            "client_id": self.application.client_id,
+            "response_type": "code",
+            "state": "random_state_string",
+            "scope": "read write",
+            "redirect_uri": "http://example.org",
+            "prompt": "none",
+        }
+
+        response = self.client.get(reverse("oauth2_provider:authorize"), data=query_data)
+
+        self.assertEqual(response.status_code, 302)
+
+        scheme, netloc, path, params, query, fragment = urlparse(response["Location"])
+        parsed_query = parse_qs(query)
+
+        self.assertIn("login_required", parsed_query["error"])
+        self.assertIn("random_state_string", parsed_query["state"])
+
 
 class BaseAuthorizationCodeTokenView(BaseTest):
     def get_auth(self, scope="read write"):
         """
         Helper method to retrieve a valid authorization code
         """
         authcode_data = {
@@ -998,14 +1050,47 @@
         self.oauth2_settings.ROTATE_REFRESH_TOKEN = False
 
         response = self.client.post(reverse("oauth2_provider:token"), data=token_request_data, **auth_headers)
         self.assertEqual(response.status_code, 200)
         response = self.client.post(reverse("oauth2_provider:token"), data=token_request_data, **auth_headers)
         self.assertEqual(response.status_code, 200)
 
+    def test_refresh_with_deleted_token(self):
+        """
+        Ensure that using a deleted refresh token returns 400
+        """
+        self.client.login(username="test_user", password="123456")
+        authorization_code = self.get_auth()
+
+        token_request_data = {
+            "grant_type": "authorization_code",
+            "scope": "read write",
+            "code": authorization_code,
+            "redirect_uri": "http://example.org",
+        }
+        auth_headers = get_basic_auth_header(self.application.client_id, CLEARTEXT_SECRET)
+
+        # get a refresh token
+        response = self.client.post(reverse("oauth2_provider:token"), data=token_request_data, **auth_headers)
+
+        content = json.loads(response.content.decode("utf-8"))
+        rt = content["refresh_token"]
+
+        token_request_data = {
+            "grant_type": "refresh_token",
+            "refresh_token": rt,
+            "scope": "read write",
+        }
+
+        # delete the access token
+        AccessToken.objects.filter(token=content["access_token"]).delete()
+
+        response = self.client.post(reverse("oauth2_provider:token"), data=token_request_data, **auth_headers)
+        self.assertEqual(response.status_code, 400)
+
     def test_basic_auth_bad_authcode(self):
         """
         Request an access token using a bad authorization code
         """
         self.client.login(username="test_user", password="123456")
 
         token_request_data = {
@@ -1555,18 +1640,19 @@
         self.assertEqual(content["token_type"], "Bearer")
         self.assertEqual(content["scope"], "read write")
         self.assertEqual(content["expires_in"], self.oauth2_settings.ACCESS_TOKEN_EXPIRE_SECONDS)
 
 
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestOIDCAuthorizationCodeTokenView(BaseAuthorizationCodeTokenView):
-    def setUp(self):
-        super().setUp()
-        self.application.algorithm = Application.RS256_ALGORITHM
-        self.application.save()
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.application.algorithm = Application.RS256_ALGORITHM
+        cls.application.save()
 
     def test_id_token_public(self):
         """
         Request an access token using client_type: public
         """
         self.client.login(username="test_user", password="123456")
 
@@ -1632,19 +1718,23 @@
         self.assertIn("access_token", content)
         self.assertIn("id_token", content)
         self.assertEqual(content["expires_in"], self.oauth2_settings.ACCESS_TOKEN_EXPIRE_SECONDS)
 
 
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestOIDCAuthorizationCodeHSAlgorithm(BaseAuthorizationCodeTokenView):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.application.algorithm = Application.HS256_ALGORITHM
+        cls.application.save()
+
     def setUp(self):
         super().setUp()
         self.oauth2_settings.OIDC_RSA_PRIVATE_KEY = None
-        self.application.algorithm = Application.HS256_ALGORITHM
-        self.application.save()
 
     def test_id_token(self):
         """
         Request an access token using an HS256 application
         """
         self.client.login(username="test_user", password="123456")
 
@@ -1728,18 +1818,19 @@
         view = ResourceView.as_view()
         response = view(request)
         self.assertEqual(response.status_code, 403)
 
 
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestOIDCAuthorizationCodeProtectedResource(BaseTest):
-    def setUp(self):
-        super().setUp()
-        self.application.algorithm = Application.RS256_ALGORITHM
-        self.application.save()
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.application.algorithm = Application.RS256_ALGORITHM
+        cls.application.save()
 
     def test_id_token_resource_access_allowed(self):
         self.client.login(username="test_user", password="123456")
 
         # retrieve a valid authorization code
         authcode_data = {
             "client_id": self.application.client_id,
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_client_credential.py` & `django_oauth_toolkit-2.4.0/tests/test_client_credential.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,32 +31,29 @@
     def get(self, request, *args, **kwargs):
         return "This is a protected resource"
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 @pytest.mark.oauth2_settings(presets.DEFAULT_SCOPES_RW)
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    factory = RequestFactory()
 
-        self.application = Application.objects.create(
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+
+        cls.application = Application.objects.create(
             name="test_client_credentials_app",
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_PUBLIC,
             authorization_grant_type=Application.GRANT_CLIENT_CREDENTIALS,
             client_secret=CLEARTEXT_SECRET,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        self.test_user.delete()
-        self.dev_user.delete()
-
 
 class TestClientCredential(BaseTest):
     def test_client_credential_access_allowed(self):
         """
         Request an access token using Client Credential Flow with hashed secrets
         """
         self.assertNotEqual(self.application.client_secret, CLEARTEXT_SECRET)
@@ -94,15 +91,15 @@
         self.assertEqual(response.status_code, 200)
 
         content = json.loads(response.content.decode("utf-8"))
         access_token = AccessToken.objects.get(token=content["access_token"])
         self.assertIsNone(access_token.user)
 
 
-class TestView(OAuthLibMixin, View):
+class ExampleView(OAuthLibMixin, View):
     server_class = BackendApplicationServer
     validator_class = OAuth2Validator
     oauthlib_backend_class = OAuthLibCore
 
     def get_scopes(self):
         return ["read", "write"]
 
@@ -128,37 +125,37 @@
         auth_headers = {
             "HTTP_AUTHORIZATION": "Bearer " + access_token,
         }
 
         request = self.request_factory.get("/fake-req", **auth_headers)
         request.user = "fake"
 
-        test_view = TestView()
+        test_view = ExampleView()
         self.assertIsInstance(test_view.get_server(), BackendApplicationServer)
 
         valid, r = test_view.verify_request(request)
         self.assertTrue(valid)
         self.assertIsNone(r.user)
         self.assertEqual(r.client, self.application)
         self.assertEqual(r.scopes, ["read", "write"])
 
     def test_raises_error_with_invalid_hex_in_query_params(self):
         request = self.request_factory.get("/fake-req?auth_token=%%7A")
 
         with pytest.raises(SuspiciousOperation):
-            TestView().verify_request(request)
+            ExampleView().verify_request(request)
 
     @patch("oauth2_provider.views.mixins.OAuthLibMixin.get_oauthlib_core")
     def test_reraises_value_errors_as_is(self, patched_core):
         patched_core.return_value.verify_request.side_effect = ValueError("Generic error")
 
         request = self.request_factory.get("/fake-req")
 
         with pytest.raises(ValueError):
-            TestView().verify_request(request)
+            ExampleView().verify_request(request)
 
 
 class TestClientResourcePasswordBased(BaseTest):
     def test_client_resource_password_based(self):
         """
         Request an access token using Resource Owner Password Based flow
         """
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_commands.py` & `django_oauth_toolkit-2.4.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/tests/test_decorators.py` & `django_oauth_toolkit-2.4.0/tests/test_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,32 @@
 
 Application = get_application_model()
 AccessToken = get_access_token_model()
 UserModel = get_user_model()
 
 
 class TestProtectedResourceDecorator(TestCase):
+    request_factory = RequestFactory()
+
     @classmethod
-    def setUpClass(cls):
-        cls.request_factory = RequestFactory()
-        super().setUpClass()
-
-    def setUp(self):
-        self.user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.application = Application.objects.create(
+    def setUpTestData(cls):
+        cls.user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.application = Application.objects.create(
             name="test_client_credentials_app",
-            user=self.user,
+            user=cls.user,
             client_type=Application.CLIENT_PUBLIC,
             authorization_grant_type=Application.GRANT_CLIENT_CREDENTIALS,
         )
 
-        self.access_token = AccessToken.objects.create(
-            user=self.user,
+        cls.access_token = AccessToken.objects.create(
+            user=cls.user,
             scope="read write",
             expires=timezone.now() + timedelta(seconds=300),
             token="secret-access-token-key",
-            application=self.application,
+            application=cls.application,
         )
 
     def test_access_denied(self):
         @protected_resource()
         def view(request, *args, **kwargs):
             return "protected contents"
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_generator.py` & `django_oauth_toolkit-2.4.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/tests/test_hybrid.py` & `django_oauth_toolkit-2.4.0/tests/test_hybrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,38 +44,37 @@
 
     def get(self, request, *args, **kwargs):
         return "This is a protected resource"
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.hy_test_user = UserModel.objects.create_user("hy_test_user", "test_hy@example.com", "123456")
-        self.hy_dev_user = UserModel.objects.create_user("hy_dev_user", "dev_hy@example.com", "123456")
-        self.oauth2_settings.PKCE_REQUIRED = False
-        self.oauth2_settings.ALLOWED_REDIRECT_URI_SCHEMES = ["http", "custom-scheme"]
+    factory = RequestFactory()
+
+    @classmethod
+    def setUpTestData(cls):
+        cls.hy_test_user = UserModel.objects.create_user("hy_test_user", "test_hy@example.com", "123456")
+        cls.hy_dev_user = UserModel.objects.create_user("hy_dev_user", "dev_hy@example.com", "123456")
 
-        self.application = Application(
+        cls.application = Application(
             name="Hybrid Test Application",
             redirect_uris=(
                 "http://localhost http://example.com http://example.org custom-scheme://example.com"
             ),
-            user=self.hy_dev_user,
+            user=cls.hy_dev_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_OPENID_HYBRID,
             algorithm=Application.RS256_ALGORITHM,
             client_secret=CLEARTEXT_SECRET,
         )
-        self.application.save()
+        cls.application.save()
 
-    def tearDown(self):
-        self.application.delete()
-        self.hy_test_user.delete()
-        self.hy_dev_user.delete()
+    def setUp(self):
+        self.oauth2_settings.PKCE_REQUIRED = False
+        self.oauth2_settings.ALLOWED_REDIRECT_URI_SCHEMES = ["http", "custom-scheme"]
 
 
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestRegressionIssue315Hybrid(BaseTest):
     """
     Test to avoid regression for the issue 315: request object
     was being reassigned when getting AuthorizationView
@@ -686,15 +685,15 @@
         self.assertIn("custom-scheme://example.com?", response["Location"])
         self.assertIn("error=access_denied", response["Location"])
 
     def test_code_post_auth_redirection_uri_with_querystring_code_token(self):
         """
         Tests that a redirection uri with query string is allowed
         and query string is retained on redirection.
-        See http://tools.ietf.org/html/rfc6749#section-3.1.2
+        See https://rfc-editor.org/rfc/rfc6749.html#section-3.1.2
         """
         self.client.login(username="hy_test_user", password="123456")
 
         form_data = {
             "client_id": self.application.client_id,
             "state": "random_state_string",
             "scope": "openid read write",
@@ -709,15 +708,15 @@
         self.assertIn("code=", response["Location"])
         self.assertIn("access_token=", response["Location"])
 
     def test_code_post_auth_redirection_uri_with_querystring_code_id_token(self):
         """
         Tests that a redirection uri with query string is allowed
         and query string is retained on redirection.
-        See http://tools.ietf.org/html/rfc6749#section-3.1.2
+        See https://rfc-editor.org/rfc/rfc6749.html#section-3.1.2
         """
         self.client.login(username="hy_test_user", password="123456")
 
         form_data = {
             "client_id": self.application.client_id,
             "state": "random_state_string",
             "scope": "openid read write",
@@ -733,15 +732,15 @@
         self.assertIn("code=", response["Location"])
         self.assertIn("id_token=", response["Location"])
 
     def test_code_post_auth_redirection_uri_with_querystring_code_id_token_token(self):
         """
         Tests that a redirection uri with query string is allowed
         and query string is retained on redirection.
-        See http://tools.ietf.org/html/rfc6749#section-3.1.2
+        See https://rfc-editor.org/rfc/rfc6749.html#section-3.1.2
         """
         self.client.login(username="hy_test_user", password="123456")
 
         form_data = {
             "client_id": self.application.client_id,
             "state": "random_state_string",
             "scope": "openid read write",
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_implicit.py` & `django_oauth_toolkit-2.4.0/tests/test_implicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,29 @@
 class ResourceView(ProtectedResourceView):
     def get(self, request, *args, **kwargs):
         return "This is a protected resource"
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    factory = RequestFactory()
 
-        self.application = Application.objects.create(
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+
+        cls.application = Application.objects.create(
             name="Test Implicit Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_PUBLIC,
             authorization_grant_type=Application.GRANT_IMPLICIT,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        self.test_user.delete()
-        self.dev_user.delete()
-
 
 @pytest.mark.oauth2_settings(presets.DEFAULT_SCOPES_RO)
 class TestImplicitAuthorizationCodeView(BaseTest):
     def test_pre_auth_valid_client_default_scopes(self):
         """
         Test response for a valid client_id with response_type: token and default_scopes
         """
@@ -201,15 +198,15 @@
         self.assertEqual(response.status_code, 302)
         self.assertIn("error=access_denied", response["Location"])
 
     def test_implicit_redirection_uri_with_querystring(self):
         """
         Tests that a redirection uri with query string is allowed
         and query string is retained on redirection.
-        See http://tools.ietf.org/html/rfc6749#section-3.1.2
+        See https://rfc-editor.org/rfc/rfc6749.html#section-3.1.2
         """
         self.client.login(username="test_user", password="123456")
 
         form_data = {
             "client_id": self.application.client_id,
             "state": "random_state_string",
             "scope": "read write",
@@ -272,18 +269,19 @@
         response = view(request)
         self.assertEqual(response, "This is a protected resource")
 
 
 @pytest.mark.usefixtures("oidc_key")
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestOpenIDConnectImplicitFlow(BaseTest):
-    def setUp(self):
-        super().setUp()
-        self.application.algorithm = Application.RS256_ALGORITHM
-        self.application.save()
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.application.algorithm = Application.RS256_ALGORITHM
+        cls.application.save()
 
     def test_id_token_post_auth_allow(self):
         """
         Test authorization code is given for an allowed request with response_type: id_token
         """
         self.client.login(username="test_user", password="123456")
 
@@ -359,15 +357,15 @@
             "scope": "openid",
             "redirect_uri": "http://example.org",
         }
 
         response = self.client.get(reverse("oauth2_provider:authorize"), data=query_data)
         self.assertEqual(response.status_code, 302)
         self.assertIn("error=invalid_request", response["Location"])
-        self.assertIn("error_description=Request+is+missing+mandatory+nonce+paramete", response["Location"])
+        self.assertIn("error_description=Request+is+missing+mandatory+nonce+parameter", response["Location"])
 
     def test_id_token_post_auth_deny(self):
         """
         Test error when resource owner deny access
         """
         self.client.login(username="test_user", password="123456")
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_introspection_auth.py` & `django_oauth_toolkit-2.4.0/tests/test_introspection_auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,113 +25,125 @@
     import mock
 
 
 Application = get_application_model()
 AccessToken = get_access_token_model()
 UserModel = get_user_model()
 
-exp = datetime.datetime.now() + datetime.timedelta(days=1)
+default_exp = datetime.datetime.now() + datetime.timedelta(days=1)
 
 
 class ScopeResourceView(ScopedProtectedResourceView):
     required_scopes = ["dolphin"]
 
     def get(self, request, *args, **kwargs):
         return HttpResponse("This is a protected resource", 200)
 
     def post(self, request, *args, **kwargs):
         return HttpResponse("This is a protected resource", 200)
 
 
+class MockResponse:
+    def __init__(self, json_data, status_code):
+        self.json_data = json_data
+        self.status_code = status_code
+
+    def json(self):
+        return self.json_data
+
+
 def mocked_requests_post(url, data, *args, **kwargs):
     """
     Mock the response from the authentication server
     """
 
-    class MockResponse:
-        def __init__(self, json_data, status_code):
-            self.json_data = json_data
-            self.status_code = status_code
-
-        def json(self):
-            return self.json_data
-
     if "token" in data and data["token"] and data["token"] != "12345678900":
         return MockResponse(
             {
                 "active": True,
                 "scope": "read write dolphin",
                 "client_id": "client_id_{}".format(data["token"]),
                 "username": "{}_user".format(data["token"]),
-                "exp": int(calendar.timegm(exp.timetuple())),
+                "exp": int(calendar.timegm(default_exp.timetuple())),
             },
             200,
         )
 
     return MockResponse(
         {
             "active": False,
         },
         200,
     )
 
 
+def mocked_introspect_request_short_living_token(url, data, *args, **kwargs):
+    exp = datetime.datetime.now() + datetime.timedelta(minutes=30)
+
+    return MockResponse(
+        {
+            "active": True,
+            "scope": "read write dolphin",
+            "client_id": "client_id_{}".format(data["token"]),
+            "username": "{}_user".format(data["token"]),
+            "exp": int(calendar.timegm(exp.timetuple())),
+        },
+        200,
+    )
+
+
 urlpatterns = [
     path("oauth2/", include("oauth2_provider.urls")),
     path("oauth2-test-resource/", ScopeResourceView.as_view()),
 ]
 
 
 @override_settings(ROOT_URLCONF=__name__)
 @pytest.mark.usefixtures("oauth2_settings")
 @pytest.mark.oauth2_settings(presets.INTROSPECTION_SETTINGS)
 class TestTokenIntrospectionAuth(TestCase):
     """
     Tests for Authorization through token introspection
     """
 
-    def setUp(self):
-        self.validator = OAuth2Validator()
-        self.request = mock.MagicMock(wraps=Request)
-        self.resource_server_user = UserModel.objects.create_user(
+    @classmethod
+    def setUpTestData(cls):
+        cls.validator = OAuth2Validator()
+        cls.request = mock.MagicMock(wraps=Request)
+        cls.resource_server_user = UserModel.objects.create_user(
             "resource_server", "test@example.com", "123456"
         )
 
-        self.application = Application.objects.create(
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.resource_server_user,
+            user=cls.resource_server_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
         )
 
-        self.resource_server_token = AccessToken.objects.create(
-            user=self.resource_server_user,
+        cls.resource_server_token = AccessToken.objects.create(
+            user=cls.resource_server_user,
             token="12345678900",
-            application=self.application,
+            application=cls.application,
             expires=timezone.now() + datetime.timedelta(days=1),
             scope="introspection",
         )
 
-        self.invalid_token = AccessToken.objects.create(
-            user=self.resource_server_user,
+        cls.invalid_token = AccessToken.objects.create(
+            user=cls.resource_server_user,
             token="12345678901",
-            application=self.application,
+            application=cls.application,
             expires=timezone.now() + datetime.timedelta(days=-1),
             scope="read write dolphin",
         )
 
+    def setUp(self):
         self.oauth2_settings.RESOURCE_SERVER_AUTH_TOKEN = self.resource_server_token.token
 
-    def tearDown(self):
-        self.resource_server_token.delete()
-        self.application.delete()
-        AccessToken.objects.all().delete()
-        UserModel.objects.all().delete()
-
     @mock.patch("requests.post", side_effect=mocked_requests_post)
     def test_get_token_from_authentication_server_not_existing_token(self, mock_get):
         """
         Test method _get_token_from_authentication_server with non existing token
         """
         token = self.validator._get_token_from_authentication_server(
             self.resource_server_token.token,
@@ -152,32 +164,84 @@
             self.oauth2_settings.RESOURCE_SERVER_AUTH_TOKEN,
             self.oauth2_settings.RESOURCE_SERVER_INTROSPECTION_CREDENTIALS,
         )
         self.assertIsInstance(token, AccessToken)
         self.assertEqual(token.user.username, "foo_user")
         self.assertEqual(token.scope, "read write dolphin")
 
-    @mock.patch("requests.post", side_effect=mocked_requests_post)
-    def test_get_token_from_authentication_server_expires_timezone(self, mock_get):
+    @mock.patch("requests.post", side_effect=mocked_introspect_request_short_living_token)
+    def test_get_token_from_authentication_server_expires_no_timezone(self, mock_get):
         """
         Test method _get_token_from_authentication_server for projects with USE_TZ False
         """
         settings_use_tz_backup = settings.USE_TZ
         settings.USE_TZ = False
         try:
-            self.validator._get_token_from_authentication_server(
+            access_token = self.validator._get_token_from_authentication_server(
                 "foo",
                 oauth2_settings.RESOURCE_SERVER_INTROSPECTION_URL,
                 oauth2_settings.RESOURCE_SERVER_AUTH_TOKEN,
                 oauth2_settings.RESOURCE_SERVER_INTROSPECTION_CREDENTIALS,
             )
+
+            self.assertFalse(access_token.is_expired())
+        except ValueError as exception:
+            self.fail(str(exception))
+        finally:
+            settings.USE_TZ = settings_use_tz_backup
+
+    @mock.patch("requests.post", side_effect=mocked_introspect_request_short_living_token)
+    def test_get_token_from_authentication_server_expires_utc_timezone(self, mock_get):
+        """
+        Test method _get_token_from_authentication_server for projects with USE_TZ True and a UTC Timezone
+        """
+        settings_use_tz_backup = settings.USE_TZ
+        settings_time_zone_backup = settings.TIME_ZONE
+        settings.USE_TZ = True
+        settings.TIME_ZONE = "UTC"
+        try:
+            access_token = self.validator._get_token_from_authentication_server(
+                "foo",
+                oauth2_settings.RESOURCE_SERVER_INTROSPECTION_URL,
+                oauth2_settings.RESOURCE_SERVER_AUTH_TOKEN,
+                oauth2_settings.RESOURCE_SERVER_INTROSPECTION_CREDENTIALS,
+            )
+
+            self.assertFalse(access_token.is_expired())
+        except ValueError as exception:
+            self.fail(str(exception))
+        finally:
+            settings.USE_TZ = settings_use_tz_backup
+            settings.TIME_ZONE = settings_time_zone_backup
+
+    @mock.patch("requests.post", side_effect=mocked_introspect_request_short_living_token)
+    def test_get_token_from_authentication_server_expires_non_utc_timezone(self, mock_get):
+        """
+        Test method _get_token_from_authentication_server for projects with USE_TZ True and a non UTC Timezone
+
+        This test is important to check if the UTC Exp. date gets converted correctly
+        """
+        settings_use_tz_backup = settings.USE_TZ
+        settings_time_zone_backup = settings.TIME_ZONE
+        settings.USE_TZ = True
+        settings.TIME_ZONE = "Europe/Amsterdam"
+        try:
+            access_token = self.validator._get_token_from_authentication_server(
+                "foo",
+                oauth2_settings.RESOURCE_SERVER_INTROSPECTION_URL,
+                oauth2_settings.RESOURCE_SERVER_AUTH_TOKEN,
+                oauth2_settings.RESOURCE_SERVER_INTROSPECTION_CREDENTIALS,
+            )
+
+            self.assertFalse(access_token.is_expired())
         except ValueError as exception:
             self.fail(str(exception))
         finally:
             settings.USE_TZ = settings_use_tz_backup
+            settings.TIME_ZONE = settings_time_zone_backup
 
     @mock.patch("requests.post", side_effect=mocked_requests_post)
     def test_validate_bearer_token(self, mock_get):
         """
         Test method validate_bearer_token
         """
         # with token = None
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_introspection_view.py` & `django_oauth_toolkit-2.4.0/tests/test_introspection_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,72 +23,68 @@
 @pytest.mark.usefixtures("oauth2_settings")
 @pytest.mark.oauth2_settings(presets.INTROSPECTION_SETTINGS)
 class TestTokenIntrospectionViews(TestCase):
     """
     Tests for Authorized Token Introspection Views
     """
 
-    def setUp(self):
-        self.resource_server_user = UserModel.objects.create_user("resource_server", "test@example.com")
-        self.test_user = UserModel.objects.create_user("bar_user", "dev@example.com")
+    @classmethod
+    def setUpTestData(cls):
+        cls.resource_server_user = UserModel.objects.create_user("resource_server", "test@example.com")
+        cls.test_user = UserModel.objects.create_user("bar_user", "dev@example.com")
 
-        self.application = Application.objects.create(
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.test_user,
+            user=cls.test_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
             client_secret=CLEARTEXT_SECRET,
         )
 
-        self.resource_server_token = AccessToken.objects.create(
-            user=self.resource_server_user,
+        cls.resource_server_token = AccessToken.objects.create(
+            user=cls.resource_server_user,
             token="12345678900",
-            application=self.application,
+            application=cls.application,
             expires=timezone.now() + datetime.timedelta(days=1),
             scope="introspection",
         )
 
-        self.valid_token = AccessToken.objects.create(
-            user=self.test_user,
+        cls.valid_token = AccessToken.objects.create(
+            user=cls.test_user,
             token="12345678901",
-            application=self.application,
+            application=cls.application,
             expires=timezone.now() + datetime.timedelta(days=1),
             scope="read write dolphin",
         )
 
-        self.invalid_token = AccessToken.objects.create(
-            user=self.test_user,
+        cls.invalid_token = AccessToken.objects.create(
+            user=cls.test_user,
             token="12345678902",
-            application=self.application,
+            application=cls.application,
             expires=timezone.now() + datetime.timedelta(days=-1),
             scope="read write dolphin",
         )
 
-        self.token_without_user = AccessToken.objects.create(
+        cls.token_without_user = AccessToken.objects.create(
             user=None,
             token="12345678903",
-            application=self.application,
+            application=cls.application,
             expires=timezone.now() + datetime.timedelta(days=1),
             scope="read write dolphin",
         )
 
-        self.token_without_app = AccessToken.objects.create(
-            user=self.test_user,
+        cls.token_without_app = AccessToken.objects.create(
+            user=cls.test_user,
             token="12345678904",
             application=None,
             expires=timezone.now() + datetime.timedelta(days=1),
             scope="read write dolphin",
         )
 
-    def tearDown(self):
-        AccessToken.objects.all().delete()
-        Application.objects.all().delete()
-        UserModel.objects.all().delete()
-
     def test_view_forbidden(self):
         """
         Test that the view is restricted for logged-in users.
         """
         response = self.client.get(reverse("oauth2_provider:introspect"))
         self.assertEqual(response.status_code, 403)
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_mixins.py` & `django_oauth_toolkit-2.4.0/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/tests/test_models.py` & `django_oauth_toolkit-2.4.0/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import timedelta
 
 import pytest
 from django.contrib.auth import get_user_model
+from django.contrib.auth.hashers import check_password
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.test import TestCase
 from django.test.utils import override_settings
 from django.utils import timezone
 
 from oauth2_provider.models import (
     clear_expired,
@@ -15,28 +16,28 @@
     get_id_token_model,
     get_refresh_token_model,
 )
 
 from . import presets
 
 
+CLEARTEXT_SECRET = "1234567890abcdefghijklmnopqrstuvwxyz"
+
 Application = get_application_model()
 Grant = get_grant_model()
 AccessToken = get_access_token_model()
 RefreshToken = get_refresh_token_model()
 UserModel = get_user_model()
 IDToken = get_id_token_model()
 
 
 class BaseTestModels(TestCase):
-    def setUp(self):
-        self.user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-
-    def tearDown(self):
-        self.user.delete()
+    @classmethod
+    def setUpTestData(cls):
+        cls.user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
 
 
 class TestModels(BaseTestModels):
     def test_allow_scopes(self):
         self.client.login(username="test_user", password="123456")
         app = Application.objects.create(
             name="test_app",
@@ -50,14 +51,41 @@
 
         self.assertTrue(access_token.allow_scopes(["read", "write"]))
         self.assertTrue(access_token.allow_scopes(["write", "read"]))
         self.assertTrue(access_token.allow_scopes(["write", "read", "read"]))
         self.assertTrue(access_token.allow_scopes([]))
         self.assertFalse(access_token.allow_scopes(["write", "destroy"]))
 
+    def test_hashed_secret(self):
+        app = Application.objects.create(
+            name="test_app",
+            redirect_uris="http://localhost http://example.com http://example.org",
+            user=self.user,
+            client_type=Application.CLIENT_CONFIDENTIAL,
+            authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
+            client_secret=CLEARTEXT_SECRET,
+            hash_client_secret=True,
+        )
+
+        self.assertNotEqual(app.client_secret, CLEARTEXT_SECRET)
+        self.assertTrue(check_password(CLEARTEXT_SECRET, app.client_secret))
+
+    def test_unhashed_secret(self):
+        app = Application.objects.create(
+            name="test_app",
+            redirect_uris="http://localhost http://example.com http://example.org",
+            user=self.user,
+            client_type=Application.CLIENT_CONFIDENTIAL,
+            authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
+            client_secret=CLEARTEXT_SECRET,
+            hash_client_secret=False,
+        )
+
+        self.assertEqual(app.client_secret, CLEARTEXT_SECRET)
+
     def test_grant_authorization_code_redirect_uris(self):
         app = Application(
             name="test_app",
             redirect_uris="",
             user=self.user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
@@ -218,28 +246,25 @@
         # Patch oauth2 settings to use a custom AccessToken model
         self.oauth2_settings.GRANT_MODEL = "tests.GrantNotInstalled"
 
         self.assertRaises(LookupError, get_grant_model)
 
 
 class TestGrantModel(BaseTestModels):
-    def setUp(self):
-        super().setUp()
-        self.application = Application.objects.create(
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="",
-            user=self.user,
+            user=cls.user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        super().tearDown()
-
     def test_str(self):
         grant = Grant(code="test_code")
         self.assertEqual("%s" % grant, grant.code)
 
     def test_expires_can_be_none(self):
         grant = Grant(code="test_code")
         self.assertIsNone(grant.expires)
@@ -290,77 +315,78 @@
     def test_str(self):
         refresh_token = RefreshToken(token="test_token")
         self.assertEqual("%s" % refresh_token, refresh_token.token)
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class TestClearExpired(BaseTestModels):
-    def setUp(self):
-        super().setUp()
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
         # Insert many tokens, both expired and not, and grants.
-        self.num_tokens = 100
-        self.delta_secs = 1000
-        self.now = timezone.now()
-        self.earlier = self.now - timedelta(seconds=self.delta_secs)
-        self.later = self.now + timedelta(seconds=self.delta_secs)
+        cls.num_tokens = 100
+        cls.delta_secs = 1000
+        cls.now = timezone.now()
+        cls.earlier = cls.now - timedelta(seconds=cls.delta_secs)
+        cls.later = cls.now + timedelta(seconds=cls.delta_secs)
 
         app = Application.objects.create(
             name="test_app",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.user,
+            user=cls.user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
         )
         # make 200 access tokens, half current and half expired.
         expired_access_tokens = [
-            AccessToken(token="expired AccessToken {}".format(i), expires=self.earlier)
-            for i in range(self.num_tokens)
+            AccessToken(token="expired AccessToken {}".format(i), expires=cls.earlier)
+            for i in range(cls.num_tokens)
         ]
         for a in expired_access_tokens:
             a.save()
 
         current_access_tokens = [
-            AccessToken(token=f"current AccessToken {i}", expires=self.later) for i in range(self.num_tokens)
+            AccessToken(token=f"current AccessToken {i}", expires=cls.later) for i in range(cls.num_tokens)
         ]
         for a in current_access_tokens:
             a.save()
 
         # Give the first half of the access tokens a refresh token,
         # alternating between current and expired ones.
         for i in range(0, len(expired_access_tokens) // 2, 2):
             RefreshToken(
                 token=f"expired AT's refresh token {i}",
                 application=app,
                 access_token=expired_access_tokens[i],
-                user=self.user,
+                user=cls.user,
             ).save()
 
         for i in range(1, len(current_access_tokens) // 2, 2):
             RefreshToken(
                 token=f"current AT's refresh token {i}",
                 application=app,
                 access_token=current_access_tokens[i],
-                user=self.user,
+                user=cls.user,
             ).save()
 
         # Make some grants, half of which are expired.
-        for i in range(self.num_tokens):
+        for i in range(cls.num_tokens):
             Grant(
-                user=self.user,
+                user=cls.user,
                 code=f"old grant code {i}",
                 application=app,
-                expires=self.earlier,
+                expires=cls.earlier,
                 redirect_uri="https://localhost/redirect",
             ).save()
-        for i in range(self.num_tokens):
+        for i in range(cls.num_tokens):
             Grant(
-                user=self.user,
+                user=cls.user,
                 code=f"new grant code {i}",
                 application=app,
-                expires=self.later,
+                expires=cls.later,
                 redirect_uri="https://localhost/redirect",
             ).save()
 
     def test_clear_expired_tokens_incorect_timetype(self):
         self.oauth2_settings.REFRESH_TOKEN_EXPIRE_SECONDS = "A"
         with pytest.raises(ImproperlyConfigured) as excinfo:
             clear_expired()
@@ -550,7 +576,33 @@
 
     # HS256, hybrid + confidential -> forbidden
     application.client_type = Application.CLIENT_CONFIDENTIAL
     application.authorization_grant_type = Application.GRANT_OPENID_HYBRID
     with pytest.raises(ValidationError) as exc:
         application.clean()
     assert "You cannot use HS256" in str(exc.value)
+
+    application.authorization_grant_type = Application.GRANT_AUTHORIZATION_CODE
+
+    # allowed_origins can be only https://
+    application.allowed_origins = "http://example.com"
+    with pytest.raises(ValidationError) as exc:
+        application.clean()
+    assert "allowed origin URI Validation error. invalid_scheme: http://example.com" in str(exc.value)
+    application.allowed_origins = "https://example.com"
+    application.clean()
+
+
+@pytest.mark.django_db
+@pytest.mark.oauth2_settings(presets.ALLOWED_SCHEMES_DEFAULT)
+def test_application_origin_allowed_default_https(oauth2_settings, cors_application):
+    """Test that http schemes are not allowed because ALLOWED_SCHEMES allows only https"""
+    assert cors_application.origin_allowed("https://example.com")
+    assert not cors_application.origin_allowed("http://example.com")
+
+
+@pytest.mark.django_db
+@pytest.mark.oauth2_settings(presets.ALLOWED_SCHEMES_HTTP)
+def test_application_origin_allowed_http(oauth2_settings, cors_application):
+    """Test that http schemes are allowed because http was added to ALLOWED_SCHEMES"""
+    assert cors_application.origin_allowed("https://example.com")
+    assert cors_application.origin_allowed("http://example.com")
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_oauth2_backends.py` & `django_oauth_toolkit-2.4.0/tests/test_oauth2_backends.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     from unittest import mock
 except ImportError:
     import mock
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class TestOAuthLibCoreBackend(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.oauthlib_core = OAuthLibCore()
+    factory = RequestFactory()
+
+    @classmethod
+    def setUpTestData(cls):
+        cls.oauthlib_core = OAuthLibCore()
 
     def test_swappable_server_class(self):
         self.oauth2_settings.OAUTH2_SERVER_CLASS = mock.MagicMock
         oauthlib_core = OAuthLibCore()
         self.assertTrue(isinstance(oauthlib_core.server, mock.MagicMock))
 
     def test_form_urlencoded_extract_params(self):
@@ -56,31 +58,29 @@
 UserModel = get_user_model()
 ApplicationModel = get_application_model()
 AccessTokenModel = get_access_token_model()
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class TestOAuthLibCoreBackendErrorHandling(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.oauthlib_core = OAuthLibCore()
-        self.user = UserModel.objects.create_user("john", "test@example.com", "123456")
-        self.app = ApplicationModel.objects.create(
+    factory = RequestFactory()
+
+    @classmethod
+    def setUpTestData(cls):
+        cls.oauthlib_core = OAuthLibCore()
+        cls.user = UserModel.objects.create_user("john", "test@example.com", "123456")
+        cls.app = ApplicationModel.objects.create(
             name="app",
             client_id="app_id",
             client_secret="app_secret",
             client_type=ApplicationModel.CLIENT_CONFIDENTIAL,
             authorization_grant_type=ApplicationModel.GRANT_PASSWORD,
-            user=self.user,
+            user=cls.user,
         )
 
-    def tearDown(self):
-        self.user.delete()
-        self.app.delete()
-
     def test_create_token_response_valid(self):
         payload = (
             "grant_type=password&username=john&password=123456&client_id=app_id&client_secret=app_secret"
         )
         request = self.factory.post(
             "/o/token/",
             payload,
@@ -149,16 +149,15 @@
     the OAuthLibCoreBackend core methods.
     """
 
     class MyOAuthLibCore(OAuthLibCore):
         def _get_extra_credentials(self, request):
             return 1
 
-    def setUp(self):
-        self.factory = RequestFactory()
+    factory = RequestFactory()
 
     def test_create_token_response_gets_extra_credentials(self):
         """
         Make sures that extra_credentials parameter is passed to oauthlib
         """
         payload = "grant_type=password&username=john&password=123456"
         request = self.factory.post("/o/token/", payload, content_type="application/x-www-form-urlencoded")
@@ -168,37 +167,35 @@
             create_token_response.return_value = mocked, mocked, mocked
             core = self.MyOAuthLibCore()
             core.create_token_response(request)
             self.assertTrue(create_token_response.call_args[0][4] == 1)
 
 
 class TestJSONOAuthLibCoreBackend(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.oauthlib_core = JSONOAuthLibCore()
+    factory = RequestFactory()
 
     def test_application_json_extract_params(self):
         payload = json.dumps(
             {
                 "grant_type": "password",
                 "username": "john",
                 "password": "123456",
             }
         )
         request = self.factory.post("/o/token/", payload, content_type="application/json")
+        oauthlib_core = JSONOAuthLibCore()
 
-        uri, http_method, body, headers = self.oauthlib_core._extract_params(request)
+        uri, http_method, body, headers = oauthlib_core._extract_params(request)
         self.assertIn("grant_type=password", body)
         self.assertIn("username=john", body)
         self.assertIn("password=123456", body)
 
 
 class TestOAuthLibCore(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
+    factory = RequestFactory()
 
     def test_validate_authorization_request_unsafe_query(self):
         auth_headers = {
             "HTTP_AUTHORIZATION": "Bearer " + "a_casual_token",
         }
         request = self.factory.get("/fake-resource?next=/fake", **auth_headers)
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_oauth2_validators.py` & `django_oauth_toolkit-2.4.0/tests/test_oauth2_validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import contextlib
 import datetime
 import json
 
 import pytest
 from django.contrib.auth import get_user_model
+from django.contrib.auth.hashers import make_password
 from django.test import TestCase, TransactionTestCase
 from django.utils import timezone
 from jwcrypto import jwt
 from oauthlib.common import Request
 
 from oauth2_provider.exceptions import FatalClientError
 from oauth2_provider.models import get_access_token_model, get_application_model, get_refresh_token_model
@@ -95,27 +96,48 @@
 
         self.blank_secret_request.client_secret = CLEARTEXT_BLANK_SECRET
         self.assertTrue(self.validator._authenticate_request_body(self.blank_secret_request))
 
         self.blank_secret_request.client_secret = "wrong_client_secret"
         self.assertFalse(self.validator._authenticate_request_body(self.blank_secret_request))
 
+    def test_authenticate_request_body_unhashed_secret(self):
+        self.application.client_secret = CLEARTEXT_SECRET
+        self.application.hash_client_secret = False
+        self.application.save()
+
+        self.request.client_id = "client_id"
+        self.request.client_secret = CLEARTEXT_SECRET
+        self.assertTrue(self.validator._authenticate_request_body(self.request))
+
+        self.application.hash_client_secret = True
+        self.application.save()
+
     def test_extract_basic_auth(self):
         self.request.headers = {"HTTP_AUTHORIZATION": "Basic 123456"}
         self.assertEqual(self.validator._extract_basic_auth(self.request), "123456")
         self.request.headers = {}
         self.assertIsNone(self.validator._extract_basic_auth(self.request))
         self.request.headers = {"HTTP_AUTHORIZATION": "Dummy 123456"}
         self.assertIsNone(self.validator._extract_basic_auth(self.request))
         self.request.headers = {"HTTP_AUTHORIZATION": "Basic"}
         self.assertIsNone(self.validator._extract_basic_auth(self.request))
         self.request.headers = {"HTTP_AUTHORIZATION": "Basic 123456 789"}
         self.assertEqual(self.validator._extract_basic_auth(self.request), "123456 789")
 
-    def test_authenticate_basic_auth(self):
+    def test_authenticate_basic_auth_hashed_secret(self):
+        self.request.encoding = "utf-8"
+        self.request.headers = get_basic_auth_header("client_id", CLEARTEXT_SECRET)
+        self.assertTrue(self.validator._authenticate_basic_auth(self.request))
+
+    def test_authenticate_basic_auth_unhashed_secret(self):
+        self.application.client_secret = CLEARTEXT_SECRET
+        self.application.hash_client_secret = False
+        self.application.save()
+
         self.request.encoding = "utf-8"
         self.request.headers = get_basic_auth_header("client_id", CLEARTEXT_SECRET)
         self.assertTrue(self.validator._authenticate_basic_auth(self.request))
 
     def test_authenticate_basic_auth_default_encoding(self):
         self.request.encoding = None
         self.request.headers = get_basic_auth_header("client_id", CLEARTEXT_SECRET)
@@ -144,14 +166,21 @@
 
     def test_authenticate_basic_auth_not_utf8(self):
         self.request.encoding = "utf-8"
         # b64decode("test") will become b"\xb5\xeb-", it can"t be decoded as utf-8
         self.request.headers = {"HTTP_AUTHORIZATION": "Basic test"}
         self.assertFalse(self.validator._authenticate_basic_auth(self.request))
 
+    def test_authenticate_check_secret(self):
+        hashed = make_password(CLEARTEXT_SECRET)
+        self.assertTrue(self.validator._check_secret(CLEARTEXT_SECRET, CLEARTEXT_SECRET))
+        self.assertTrue(self.validator._check_secret(CLEARTEXT_SECRET, hashed))
+        self.assertFalse(self.validator._check_secret(hashed, hashed))
+        self.assertFalse(self.validator._check_secret(hashed, CLEARTEXT_SECRET))
+
     def test_authenticate_client_id(self):
         self.assertTrue(self.validator.authenticate_client_id("client_id", self.request))
 
     def test_authenticate_client_id_fail(self):
         self.application.client_type = Application.CLIENT_CONFIDENTIAL
         self.application.save()
         self.assertFalse(self.validator.authenticate_client_id("client_id", self.request))
@@ -302,20 +331,28 @@
         self.validator._create_access_token = create_access_token_mock
 
         self.validator.save_bearer_token(token, self.request)
 
         assert create_access_token_mock.call_count == 1
         assert create_refresh_token_mock.call_count == 1
 
+    def test_get_or_create_user_from_content(self):
+        content = {"username": "test_user"}
+        UserModel.objects.filter(username=content["username"]).delete()
+        user = self.validator.get_or_create_user_from_content(content)
+
+        self.assertIsNotNone(user)
+        self.assertEqual(content["username"], user.username)
+
 
 class TestOAuth2ValidatorProvidesErrorData(TransactionTestCase):
     """These test cases check that the recommended error codes are returned
     when token authentication fails.
 
-    RFC-6750: https://tools.ietf.org/html/rfc6750
+    RFC-6750: https://rfc-editor.org/rfc/rfc6750.html
 
     > If the protected resource request does not include authentication
     > credentials or does not contain an access token that enables access
     > to the protected resource, the resource server MUST include the HTTP
     > "WWW-Authenticate" response header field[.]
     >
     > ...
@@ -327,15 +364,15 @@
     > ...
     >
     > If the protected resource request included an access token and failed
     > authentication, the resource server SHOULD include the "error"
     > attribute to provide the client with the reason why the access
     > request was declined.
 
-    See https://tools.ietf.org/html/rfc6750#section-3.1 for the allowed error
+    See https://rfc-editor.org/rfc/rfc6750.html#section-3.1 for the allowed error
     codes.
     """
 
     def setUp(self):
         self.user = UserModel.objects.create_user(
             "user",
             "test@example.com",
@@ -444,19 +481,20 @@
 
 
 class TestOAuth2ValidatorErrorResourceToken(TestCase):
     """The following tests check logger information when response from oauth2
     is unsuccessful.
     """
 
-    def setUp(self):
-        self.token = "test_token"
-        self.introspection_url = "http://example.com/token/introspection/"
-        self.introspection_token = "test_introspection_token"
-        self.validator = OAuth2Validator()
+    @classmethod
+    def setUpTestData(cls):
+        cls.token = "test_token"
+        cls.introspection_url = "http://example.com/token/introspection/"
+        cls.introspection_token = "test_introspection_token"
+        cls.validator = OAuth2Validator()
 
     def test_response_when_auth_server_response_return_404(self):
         with self.assertLogs(logger="oauth2_provider") as mock_log:
             self.validator._get_token_from_authentication_server(
                 self.token, self.introspection_url, self.introspection_token, None
             )
             self.assertIn(
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_oidc_views.py` & `django_oauth_toolkit-2.4.0/tests/test_oidc_views.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,29 @@
 from django.contrib.auth import get_user
 from django.contrib.auth.models import AnonymousUser
 from django.test import RequestFactory, TestCase
 from django.urls import reverse
 from django.utils import timezone
 from pytest_django.asserts import assertRedirects
 
-from oauth2_provider.exceptions import ClientIdMissmatch, InvalidOIDCClientError, InvalidOIDCRedirectURIError
+from oauth2_provider.exceptions import (
+    ClientIdMissmatch,
+    InvalidIDTokenError,
+    InvalidOIDCClientError,
+    InvalidOIDCRedirectURIError,
+)
 from oauth2_provider.models import get_access_token_model, get_id_token_model, get_refresh_token_model
 from oauth2_provider.oauth2_validators import OAuth2Validator
 from oauth2_provider.settings import oauth2_settings
-from oauth2_provider.views.oidc import _load_id_token, _validate_claims, validate_logout_request
+from oauth2_provider.views.oidc import (
+    RPInitiatedLogoutView,
+    _load_id_token,
+    _validate_claims,
+    validate_logout_request,
+)
 
 from . import presets
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RW)
 class TestConnectDiscoveryInfoView(TestCase):
@@ -34,21 +44,49 @@
                 "code token",
                 "code id_token",
                 "code id_token token",
             ],
             "subject_types_supported": ["public"],
             "id_token_signing_alg_values_supported": ["RS256", "HS256"],
             "token_endpoint_auth_methods_supported": ["client_secret_post", "client_secret_basic"],
+            "code_challenge_methods_supported": ["plain", "S256"],
             "claims_supported": ["sub"],
         }
-        response = self.client.get(reverse("oauth2_provider:oidc-connect-discovery-info"))
+        response = self.client.get("/o/.well-known/openid-configuration")
         self.assertEqual(response.status_code, 200)
         assert response.json() == expected_response
 
-    def expect_json_response_with_rp(self, base):
+    def test_get_connect_discovery_info_deprecated(self):
+        expected_response = {
+            "issuer": "http://localhost/o",
+            "authorization_endpoint": "http://localhost/o/authorize/",
+            "token_endpoint": "http://localhost/o/token/",
+            "userinfo_endpoint": "http://localhost/o/userinfo/",
+            "jwks_uri": "http://localhost/o/.well-known/jwks.json",
+            "scopes_supported": ["read", "write", "openid"],
+            "response_types_supported": [
+                "code",
+                "token",
+                "id_token",
+                "id_token token",
+                "code token",
+                "code id_token",
+                "code id_token token",
+            ],
+            "subject_types_supported": ["public"],
+            "id_token_signing_alg_values_supported": ["RS256", "HS256"],
+            "token_endpoint_auth_methods_supported": ["client_secret_post", "client_secret_basic"],
+            "code_challenge_methods_supported": ["plain", "S256"],
+            "claims_supported": ["sub"],
+        }
+        response = self.client.get("/o/.well-known/openid-configuration/")
+        self.assertEqual(response.status_code, 200)
+        assert response.json() == expected_response
+
+    def expect_json_response_with_rp_logout(self, base):
         expected_response = {
             "issuer": f"{base}",
             "authorization_endpoint": f"{base}/authorize/",
             "token_endpoint": f"{base}/token/",
             "userinfo_endpoint": f"{base}/userinfo/",
             "jwks_uri": f"{base}/.well-known/jwks.json",
             "scopes_supported": ["read", "write", "openid"],
@@ -60,24 +98,25 @@
                 "code token",
                 "code id_token",
                 "code id_token token",
             ],
             "subject_types_supported": ["public"],
             "id_token_signing_alg_values_supported": ["RS256", "HS256"],
             "token_endpoint_auth_methods_supported": ["client_secret_post", "client_secret_basic"],
+            "code_challenge_methods_supported": ["plain", "S256"],
             "claims_supported": ["sub"],
             "end_session_endpoint": f"{base}/logout/",
         }
         response = self.client.get(reverse("oauth2_provider:oidc-connect-discovery-info"))
         self.assertEqual(response.status_code, 200)
         assert response.json() == expected_response
 
     def test_get_connect_discovery_info_with_rp_logout(self):
         self.oauth2_settings.OIDC_RP_INITIATED_LOGOUT_ENABLED = True
-        self.expect_json_response_with_rp(self.oauth2_settings.OIDC_ISS_ENDPOINT)
+        self.expect_json_response_with_rp_logout(self.oauth2_settings.OIDC_ISS_ENDPOINT)
 
     def test_get_connect_discovery_info_without_issuer_url(self):
         self.oauth2_settings.OIDC_ISS_ENDPOINT = None
         self.oauth2_settings.OIDC_USERINFO_ENDPOINT = None
         expected_response = {
             "issuer": "http://testserver/o",
             "authorization_endpoint": "http://testserver/o/authorize/",
@@ -93,25 +132,26 @@
                 "code token",
                 "code id_token",
                 "code id_token token",
             ],
             "subject_types_supported": ["public"],
             "id_token_signing_alg_values_supported": ["RS256", "HS256"],
             "token_endpoint_auth_methods_supported": ["client_secret_post", "client_secret_basic"],
+            "code_challenge_methods_supported": ["plain", "S256"],
             "claims_supported": ["sub"],
         }
         response = self.client.get(reverse("oauth2_provider:oidc-connect-discovery-info"))
         self.assertEqual(response.status_code, 200)
         assert response.json() == expected_response
 
     def test_get_connect_discovery_info_without_issuer_url_with_rp_logout(self):
         self.oauth2_settings.OIDC_RP_INITIATED_LOGOUT_ENABLED = True
         self.oauth2_settings.OIDC_ISS_ENDPOINT = None
         self.oauth2_settings.OIDC_USERINFO_ENDPOINT = None
-        self.expect_json_response_with_rp("http://testserver/o")
+        self.expect_json_response_with_rp_logout("http://testserver/o")
 
     def test_get_connect_discovery_info_without_rsa_key(self):
         self.oauth2_settings.OIDC_RSA_PRIVATE_KEY = None
         response = self.client.get(reverse("oauth2_provider:oidc-connect-discovery-info"))
         self.assertEqual(response.status_code, 200)
         assert response.json()["id_token_signing_alg_values_supported"] == ["HS256"]
 
@@ -183,15 +223,17 @@
     request = RequestFactory().get("")
     request.user = user
     return request
 
 
 @pytest.mark.django_db
 @pytest.mark.parametrize("ALWAYS_PROMPT", [True, False])
-def test_validate_logout_request(oidc_tokens, public_application, other_user, rp_settings, ALWAYS_PROMPT):
+def test_deprecated_validate_logout_request(
+    oidc_tokens, public_application, other_user, rp_settings, ALWAYS_PROMPT
+):
     rp_settings.OIDC_RP_INITIATED_LOGOUT_ALWAYS_PROMPT = ALWAYS_PROMPT
     oidc_tokens = oidc_tokens
     application = oidc_tokens.application
     client_id = application.client_id
     id_token = oidc_tokens.id_token
     assert validate_logout_request(
         request=mock_request_for(oidc_tokens.user),
@@ -225,14 +267,21 @@
     ) == (True, ("http://example.org", application), oidc_tokens.user)
     assert validate_logout_request(
         request=mock_request_for(oidc_tokens.user),
         id_token_hint=id_token,
         client_id=client_id,
         post_logout_redirect_uri="http://example.org",
     ) == (ALWAYS_PROMPT, ("http://example.org", application), oidc_tokens.user)
+    with pytest.raises(InvalidIDTokenError):
+        validate_logout_request(
+            request=mock_request_for(oidc_tokens.user),
+            id_token_hint="111",
+            client_id=public_application.client_id,
+            post_logout_redirect_uri="http://other.org",
+        )
     with pytest.raises(ClientIdMissmatch):
         validate_logout_request(
             request=mock_request_for(oidc_tokens.user),
             id_token_hint=id_token,
             client_id=public_application.client_id,
             post_logout_redirect_uri="http://other.org",
         )
@@ -260,14 +309,113 @@
     with pytest.raises(InvalidOIDCRedirectURIError):
         validate_logout_request(
             request=mock_request_for(oidc_tokens.user),
             id_token_hint=None,
             client_id=client_id,
             post_logout_redirect_uri="http://other.org",
         )
+    with pytest.raises(InvalidOIDCRedirectURIError):
+        rp_settings.OIDC_RP_INITIATED_LOGOUT_STRICT_REDIRECT_URIS = True
+        validate_logout_request(
+            request=mock_request_for(oidc_tokens.user),
+            id_token_hint=None,
+            client_id=public_application.client_id,
+            post_logout_redirect_uri="http://other.org",
+        )
+
+
+@pytest.mark.django_db
+def test_validate_logout_request(oidc_tokens, public_application, rp_settings):
+    oidc_tokens = oidc_tokens
+    application = oidc_tokens.application
+    client_id = application.client_id
+    id_token = oidc_tokens.id_token
+    view = RPInitiatedLogoutView()
+    view.request = mock_request_for(oidc_tokens.user)
+    assert view.validate_logout_request(
+        id_token_hint=None,
+        client_id=None,
+        post_logout_redirect_uri=None,
+    ) == (None, None)
+    assert view.validate_logout_request(
+        id_token_hint=None,
+        client_id=client_id,
+        post_logout_redirect_uri=None,
+    ) == (application, None)
+    assert view.validate_logout_request(
+        id_token_hint=None,
+        client_id=client_id,
+        post_logout_redirect_uri="http://example.org",
+    ) == (application, None)
+    assert view.validate_logout_request(
+        id_token_hint=id_token,
+        client_id=None,
+        post_logout_redirect_uri="http://example.org",
+    ) == (application, oidc_tokens.user)
+    assert view.validate_logout_request(
+        id_token_hint=id_token,
+        client_id=client_id,
+        post_logout_redirect_uri="http://example.org",
+    ) == (application, oidc_tokens.user)
+    with pytest.raises(InvalidIDTokenError):
+        view.validate_logout_request(
+            id_token_hint="111",
+            client_id=public_application.client_id,
+            post_logout_redirect_uri="http://other.org",
+        )
+    with pytest.raises(ClientIdMissmatch):
+        view.validate_logout_request(
+            id_token_hint=id_token,
+            client_id=public_application.client_id,
+            post_logout_redirect_uri="http://other.org",
+        )
+    with pytest.raises(InvalidOIDCClientError):
+        view.validate_logout_request(
+            id_token_hint=None,
+            client_id=None,
+            post_logout_redirect_uri="http://example.org",
+        )
+    with pytest.raises(InvalidOIDCRedirectURIError):
+        view.validate_logout_request(
+            id_token_hint=None,
+            client_id=client_id,
+            post_logout_redirect_uri="example.org",
+        )
+    with pytest.raises(InvalidOIDCRedirectURIError):
+        view.validate_logout_request(
+            id_token_hint=None,
+            client_id=client_id,
+            post_logout_redirect_uri="imap://example.org",
+        )
+    with pytest.raises(InvalidOIDCRedirectURIError):
+        view.validate_logout_request(
+            id_token_hint=None,
+            client_id=client_id,
+            post_logout_redirect_uri="http://other.org",
+        )
+    with pytest.raises(InvalidOIDCRedirectURIError):
+        rp_settings.OIDC_RP_INITIATED_LOGOUT_STRICT_REDIRECT_URIS = True
+        view.validate_logout_request(
+            id_token_hint=None,
+            client_id=public_application.client_id,
+            post_logout_redirect_uri="http://other.org",
+        )
+
+
+@pytest.mark.django_db
+@pytest.mark.parametrize("ALWAYS_PROMPT", [True, False])
+def test_must_prompt(oidc_tokens, other_user, rp_settings, ALWAYS_PROMPT):
+    rp_settings.OIDC_RP_INITIATED_LOGOUT_ALWAYS_PROMPT = ALWAYS_PROMPT
+    oidc_tokens = oidc_tokens
+    assert RPInitiatedLogoutView(request=mock_request_for(oidc_tokens.user)).must_prompt(None) is True
+    assert (
+        RPInitiatedLogoutView(request=mock_request_for(oidc_tokens.user)).must_prompt(oidc_tokens.user)
+        == ALWAYS_PROMPT
+    )
+    assert RPInitiatedLogoutView(request=mock_request_for(other_user)).must_prompt(oidc_tokens.user) is True
 
 
 def test__load_id_token():
     assert _load_id_token("Not a Valid ID Token.") == (None, None)
 
 
 def is_logged_in(client):
@@ -370,15 +518,15 @@
         },
     )
     assert rsp.status_code == 400
     assert is_logged_in(logged_in_client)
 
 
 @pytest.mark.django_db
-def test_rp_initiated_logout_get_id_token_client_id(logged_in_client, oidc_tokens, rp_settings):
+def test_rp_initiated_logout_get_client_id(logged_in_client, oidc_tokens, rp_settings):
     rsp = logged_in_client.get(
         reverse("oauth2_provider:rp-initiated-logout"), data={"client_id": oidc_tokens.application.client_id}
     )
     assert rsp.status_code == 200
     assert is_logged_in(logged_in_client)
 
 
@@ -398,14 +546,23 @@
     rsp = logged_in_client.post(reverse("oauth2_provider:rp-initiated-logout"), form_data)
     assert rsp.status_code == 302
     assert rsp["Location"] == "http://testserver/"
     assert not is_logged_in(logged_in_client)
 
 
 @pytest.mark.django_db
+def test_rp_initiated_logout_post_no_session(client, oidc_tokens, rp_settings):
+    form_data = {"client_id": oidc_tokens.application.client_id, "allow": True}
+    rsp = client.post(reverse("oauth2_provider:rp-initiated-logout"), form_data)
+    assert rsp.status_code == 302
+    assert rsp["Location"] == "http://testserver/"
+    assert not is_logged_in(client)
+
+
+@pytest.mark.django_db
 @pytest.mark.oauth2_settings(presets.OIDC_SETTINGS_RP_LOGOUT)
 def test_rp_initiated_logout_expired_tokens_accept(logged_in_client, application, expired_id_token):
     # Accepting expired (but otherwise valid and signed by us) tokens is enabled. Logout should go through.
     rsp = logged_in_client.get(
         reverse("oauth2_provider:rp-initiated-logout"),
         data={
             "id_token_hint": expired_id_token,
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_password.py` & `django_oauth_toolkit-2.4.0/tests/test_password.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,32 +21,29 @@
 class ResourceView(ProtectedResourceView):
     def get(self, request, *args, **kwargs):
         return "This is a protected resource"
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    factory = RequestFactory()
 
-        self.application = Application.objects.create(
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+
+        cls.application = Application.objects.create(
             name="Test Password Application",
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_PUBLIC,
             authorization_grant_type=Application.GRANT_PASSWORD,
             client_secret=CLEARTEXT_SECRET,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        self.test_user.delete()
-        self.dev_user.delete()
-
 
 class TestPasswordTokenView(BaseTest):
     def test_get_token(self):
         """
         Request an access token using Resource Owner Password Flow
         """
         token_request_data = {
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_rest_framework.py` & `django_oauth_toolkit-2.4.0/tests/test_rest_framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,32 +126,33 @@
 ]
 
 
 @override_settings(ROOT_URLCONF=__name__)
 @pytest.mark.usefixtures("oauth2_settings")
 @pytest.mark.oauth2_settings(presets.REST_FRAMEWORK_SCOPES)
 class TestOAuth2Authentication(TestCase):
-    def setUp(self):
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
 
-        self.application = Application.objects.create(
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
         )
 
-        self.access_token = AccessToken.objects.create(
-            user=self.test_user,
+        cls.access_token = AccessToken.objects.create(
+            user=cls.test_user,
             scope="read write",
             expires=timezone.now() + timedelta(seconds=300),
             token="secret-access-token-key",
-            application=self.application,
+            application=cls.application,
         )
 
     def _create_authorization_header(self, token):
         return "Bearer {0}".format(token)
 
     def test_authentication_allow(self):
         auth = self._create_authorization_header(self.access_token.token)
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_scopes.py` & `django_oauth_toolkit-2.4.0/tests/test_scopes.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,33 +54,30 @@
     },
 }
 
 
 @pytest.mark.usefixtures("oauth2_settings")
 @pytest.mark.oauth2_settings(SCOPE_SETTINGS)
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    factory = RequestFactory()
 
-        self.application = Application.objects.create(
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
             client_secret=CLEARTEXT_SECRET,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        self.test_user.delete()
-        self.dev_user.delete()
-
 
 class TestScopesSave(BaseTest):
     def test_scopes_saved_in_grant(self):
         """
         Test scopes are properly saved in grant
         """
         self.oauth2_settings.PKCE_REQUIRED = False
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_settings.py` & `django_oauth_toolkit-2.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-oauth-toolkit-2.3.0/tests/test_token_revocation.py` & `django_oauth_toolkit-2.4.0/tests/test_token_revocation.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,30 @@
 RefreshToken = get_refresh_token_model()
 UserModel = get_user_model()
 
 CLEARTEXT_SECRET = "1234567890abcdefghijklmnopqrstuvwxyz"
 
 
 class BaseTest(TestCase):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
-        self.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+    factory = RequestFactory()
 
-        self.application = Application.objects.create(
+    @classmethod
+    def setUpTestData(cls):
+        cls.test_user = UserModel.objects.create_user("test_user", "test@example.com", "123456")
+        cls.dev_user = UserModel.objects.create_user("dev_user", "dev@example.com", "123456")
+
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.dev_user,
+            user=cls.dev_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
             client_secret=CLEARTEXT_SECRET,
         )
 
-    def tearDown(self):
-        self.application.delete()
-        self.test_user.delete()
-        self.dev_user.delete()
-
 
 class TestRevocationView(BaseTest):
     def test_revoke_access_token(self):
         tok = AccessToken.objects.create(
             user=self.test_user,
             token="1234567890",
             application=self.application,
```

### Comparing `django-oauth-toolkit-2.3.0/tests/test_token_view.py` & `django_oauth_toolkit-2.4.0/tests/test_token_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,27 @@
 
 
 class TestAuthorizedTokenViews(TestCase):
     """
     TestCase superclass for Authorized Token Views" Test Cases
     """
 
-    def setUp(self):
-        self.foo_user = UserModel.objects.create_user("foo_user", "test@example.com", "123456")
-        self.bar_user = UserModel.objects.create_user("bar_user", "dev@example.com", "123456")
+    @classmethod
+    def setUpTestData(cls):
+        cls.foo_user = UserModel.objects.create_user("foo_user", "test@example.com", "123456")
+        cls.bar_user = UserModel.objects.create_user("bar_user", "dev@example.com", "123456")
 
-        self.application = Application.objects.create(
+        cls.application = Application.objects.create(
             name="Test Application",
             redirect_uris="http://localhost http://example.com http://example.org",
-            user=self.bar_user,
+            user=cls.bar_user,
             client_type=Application.CLIENT_CONFIDENTIAL,
             authorization_grant_type=Application.GRANT_AUTHORIZATION_CODE,
         )
 
-    def tearDown(self):
-        self.foo_user.delete()
-        self.bar_user.delete()
-
 
 class TestAuthorizedTokenListView(TestAuthorizedTokenViews):
     """
     Tests for the Authorized Token ListView
     """
 
     def test_list_view_authorization_required(self):
```

