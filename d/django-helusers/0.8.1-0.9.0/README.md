# Comparing `tmp/django-helusers-0.8.1.tar.gz` & `tmp/django-helusers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-helusers-0.8.1.tar", last modified: Tue Apr  4 13:09:04 2023, max compression
+gzip compressed data, was "django-helusers-0.9.0.tar", last modified: Wed Aug  9 13:56:54 2023, max compression
```

## Comparing `django-helusers-0.8.1.tar` & `django-helusers-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.597259 django-helusers-0.8.1/
--rw-rw-r--   0 akik      (1001) akik      (1001)     1299 2021-12-01 06:38:00.000000 django-helusers-0.8.1/LICENSE
--rw-rw-r--   0 akik      (1001) akik      (1001)      104 2021-12-01 06:38:00.000000 django-helusers-0.8.1/MANIFEST.in
--rw-rw-r--   0 akik      (1001) akik      (1001)    22601 2023-04-04 13:09:04.597259 django-helusers-0.8.1/PKG-INFO
--rw-rw-r--   0 akik      (1001) akik      (1001)    18001 2023-03-30 07:15:05.000000 django-helusers-0.8.1/README.md
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/django_helusers.egg-info/
--rw-rw-r--   0 akik      (1001) akik      (1001)    22601 2023-04-04 13:09:04.000000 django-helusers-0.8.1/django_helusers.egg-info/PKG-INFO
--rw-rw-r--   0 akik      (1001) akik      (1001)     1579 2023-04-04 13:09:04.000000 django-helusers-0.8.1/django_helusers.egg-info/SOURCES.txt
--rw-rw-r--   0 akik      (1001) akik      (1001)        1 2023-04-04 13:09:04.000000 django-helusers-0.8.1/django_helusers.egg-info/dependency_links.txt
--rw-rw-r--   0 akik      (1001) akik      (1001)       66 2023-04-04 13:09:04.000000 django-helusers-0.8.1/django_helusers.egg-info/requires.txt
--rw-rw-r--   0 akik      (1001) akik      (1001)        9 2023-04-04 13:09:04.000000 django-helusers-0.8.1/django_helusers.egg-info/top_level.txt
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/
--rw-rw-r--   0 akik      (1001) akik      (1001)       52 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/__init__.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     3729 2023-03-30 07:22:51.000000 django-helusers-0.8.1/helusers/_oidc_auth_impl.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1479 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/_rest_framework_jwt_impl.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1556 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/adapter.py
--rw-rw-r--   0 akik      (1001) akik      (1001)      583 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/admin.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     3403 2023-03-30 07:15:22.000000 django-helusers-0.8.1/helusers/admin_site.py
--rw-rw-r--   0 akik      (1001) akik      (1001)      382 2022-04-12 11:32:14.000000 django-helusers-0.8.1/helusers/apps.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1663 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/authz.py
--rw-rw-r--   0 akik      (1001) akik      (1001)      196 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/context_processors.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1713 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/defaults.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     3106 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/jwt.py
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/locale/
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/locale/fi/
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/locale/fi/LC_MESSAGES/
--rw-rw-r--   0 akik      (1001) akik      (1001)     1849 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/locale/fi/LC_MESSAGES/django.po
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/management/
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/management/commands/
--rw-rw-r--   0 akik      (1001) akik      (1001)     1935 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/management/commands/sync_helusers.py
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/migrations/
--rw-rw-r--   0 akik      (1001) akik      (1001)     1481 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/migrations/0001_add_ad_groups.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1203 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/migrations/0002_add_oidcbackchannellogoutevent.py
--rw-rw-r--   0 akik      (1001) akik      (1001)        0 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/migrations/__init__.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     5797 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/models.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     4838 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/oidc.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     4860 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/pipeline.py
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/providers/
--rw-rw-r--   0 akik      (1001) akik      (1001)        0 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/__init__.py
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/providers/helsinki/
--rw-rw-r--   0 akik      (1001) akik      (1001)        0 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki/__init__.py
--rw-rw-r--   0 akik      (1001) akik      (1001)       63 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki/admin.py
--rw-rw-r--   0 akik      (1001) akik      (1001)       27 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki/models.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1079 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki/provider.py
--rw-rw-r--   0 akik      (1001) akik      (1001)      168 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki/urls.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1053 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki/views.py
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.597259 django-helusers-0.8.1/helusers/providers/helsinki_oidc/
--rw-rw-r--   0 akik      (1001) akik      (1001)        0 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki_oidc/__init__.py
--rw-rw-r--   0 akik      (1001) akik      (1001)       63 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki_oidc/admin.py
--rw-rw-r--   0 akik      (1001) akik      (1001)       27 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki_oidc/models.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1192 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki_oidc/provider.py
--rw-rw-r--   0 akik      (1001) akik      (1001)      176 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki_oidc/urls.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1013 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/providers/helsinki_oidc/views.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     2312 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/settings.py
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.593259 django-helusers-0.8.1/helusers/templates/
-drwxrwxr-x   0 akik      (1001) akik      (1001)        0 2023-04-04 13:09:04.597259 django-helusers-0.8.1/helusers/templates/admin/
--rw-rw-r--   0 akik      (1001) akik      (1001)       33 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/templates/admin/base_site.html
--rw-rw-r--   0 akik      (1001) akik      (1001)      799 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/templates/admin/base_site_default.html
--rw-rw-r--   0 akik      (1001) akik      (1001)      847 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/templates/admin/base_site_grappelli.html
--rw-rw-r--   0 akik      (1001) akik      (1001)     1503 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/templates/admin/hel_login.html
--rw-rw-r--   0 akik      (1001) akik      (1001)     2371 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/tunnistamo_oidc.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     1223 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/urls.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     5439 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/user_utils.py
--rw-rw-r--   0 akik      (1001) akik      (1001)      912 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/utils.py
--rw-rw-r--   0 akik      (1001) akik      (1001)     5213 2021-12-01 06:38:00.000000 django-helusers-0.8.1/helusers/views.py
--rw-rw-r--   0 akik      (1001) akik      (1001)       38 2023-04-04 13:09:04.597259 django-helusers-0.8.1/setup.cfg
--rw-rw-r--   0 akik      (1001) akik      (1001)     1543 2023-04-04 11:16:05.000000 django-helusers-0.8.1/setup.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.759850 django-helusers-0.9.0/
+-rw-r--r--   0 keso       (501) staff       (20)     1299 2021-02-15 11:35:13.000000 django-helusers-0.9.0/LICENSE
+-rw-r--r--   0 keso       (501) staff       (20)      104 2021-02-15 11:35:13.000000 django-helusers-0.9.0/MANIFEST.in
+-rw-r--r--   0 keso       (501) staff       (20)    18981 2023-08-09 13:56:54.759728 django-helusers-0.9.0/PKG-INFO
+-rw-r--r--   0 keso       (501) staff       (20)    17970 2023-08-08 12:23:58.000000 django-helusers-0.9.0/README.md
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.754776 django-helusers-0.9.0/django_helusers.egg-info/
+-rw-r--r--   0 keso       (501) staff       (20)    18981 2023-08-09 13:56:54.000000 django-helusers-0.9.0/django_helusers.egg-info/PKG-INFO
+-rw-r--r--   0 keso       (501) staff       (20)     1620 2023-08-09 13:56:54.000000 django-helusers-0.9.0/django_helusers.egg-info/SOURCES.txt
+-rw-r--r--   0 keso       (501) staff       (20)        1 2023-08-09 13:56:54.000000 django-helusers-0.9.0/django_helusers.egg-info/dependency_links.txt
+-rw-r--r--   0 keso       (501) staff       (20)       66 2023-08-09 13:56:54.000000 django-helusers-0.9.0/django_helusers.egg-info/requires.txt
+-rw-r--r--   0 keso       (501) staff       (20)        9 2023-08-09 13:56:54.000000 django-helusers-0.9.0/django_helusers.egg-info/top_level.txt
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.757046 django-helusers-0.9.0/helusers/
+-rw-r--r--   0 keso       (501) staff       (20)       52 2023-06-07 08:55:40.000000 django-helusers-0.9.0/helusers/__init__.py
+-rw-r--r--   0 keso       (501) staff       (20)     3387 2023-06-21 12:14:58.000000 django-helusers-0.9.0/helusers/_oidc_auth_impl.py
+-rw-r--r--   0 keso       (501) staff       (20)     1479 2023-06-07 08:55:49.000000 django-helusers-0.9.0/helusers/_rest_framework_jwt_impl.py
+-rw-r--r--   0 keso       (501) staff       (20)     1556 2023-06-07 08:55:54.000000 django-helusers-0.9.0/helusers/adapter.py
+-rw-r--r--   0 keso       (501) staff       (20)      583 2023-06-07 08:55:58.000000 django-helusers-0.9.0/helusers/admin.py
+-rw-r--r--   0 keso       (501) staff       (20)     3403 2023-06-07 08:56:03.000000 django-helusers-0.9.0/helusers/admin_site.py
+-rw-r--r--   0 keso       (501) staff       (20)      382 2023-06-07 08:56:07.000000 django-helusers-0.9.0/helusers/apps.py
+-rw-r--r--   0 keso       (501) staff       (20)     1460 2023-08-08 12:23:58.000000 django-helusers-0.9.0/helusers/authz.py
+-rw-r--r--   0 keso       (501) staff       (20)      196 2023-06-07 08:56:14.000000 django-helusers-0.9.0/helusers/context_processors.py
+-rw-r--r--   0 keso       (501) staff       (20)     1713 2023-06-07 08:56:22.000000 django-helusers-0.9.0/helusers/defaults.py
+-rw-r--r--   0 keso       (501) staff       (20)     4127 2023-08-08 12:23:22.000000 django-helusers-0.9.0/helusers/jwt.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.753239 django-helusers-0.9.0/helusers/locale/
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.753283 django-helusers-0.9.0/helusers/locale/fi/
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.757276 django-helusers-0.9.0/helusers/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 keso       (501) staff       (20)      887 2023-08-09 13:56:27.000000 django-helusers-0.9.0/helusers/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 keso       (501) staff       (20)     1800 2023-08-09 13:56:10.000000 django-helusers-0.9.0/helusers/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.753389 django-helusers-0.9.0/helusers/management/
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.757390 django-helusers-0.9.0/helusers/management/commands/
+-rw-r--r--   0 keso       (501) staff       (20)     1935 2023-06-07 08:56:57.000000 django-helusers-0.9.0/helusers/management/commands/sync_helusers.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.757715 django-helusers-0.9.0/helusers/migrations/
+-rw-r--r--   0 keso       (501) staff       (20)     1481 2023-06-07 08:55:21.000000 django-helusers-0.9.0/helusers/migrations/0001_add_ad_groups.py
+-rw-r--r--   0 keso       (501) staff       (20)     1203 2023-06-07 08:55:36.000000 django-helusers-0.9.0/helusers/migrations/0002_add_oidcbackchannellogoutevent.py
+-rw-r--r--   0 keso       (501) staff       (20)        0 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/migrations/__init__.py
+-rw-r--r--   0 keso       (501) staff       (20)     5797 2023-06-07 08:56:35.000000 django-helusers-0.9.0/helusers/models.py
+-rw-r--r--   0 keso       (501) staff       (20)     4353 2023-06-20 09:44:55.000000 django-helusers-0.9.0/helusers/oidc.py
+-rw-r--r--   0 keso       (501) staff       (20)     4860 2023-06-07 08:56:39.000000 django-helusers-0.9.0/helusers/pipeline.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.757804 django-helusers-0.9.0/helusers/providers/
+-rw-r--r--   0 keso       (501) staff       (20)        0 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/__init__.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.758453 django-helusers-0.9.0/helusers/providers/helsinki/
+-rw-r--r--   0 keso       (501) staff       (20)        0 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki/__init__.py
+-rw-r--r--   0 keso       (501) staff       (20)       63 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki/admin.py
+-rw-r--r--   0 keso       (501) staff       (20)       27 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki/models.py
+-rw-r--r--   0 keso       (501) staff       (20)     1079 2023-06-07 08:56:42.000000 django-helusers-0.9.0/helusers/providers/helsinki/provider.py
+-rw-r--r--   0 keso       (501) staff       (20)      168 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki/urls.py
+-rw-r--r--   0 keso       (501) staff       (20)     1053 2023-06-07 08:58:03.000000 django-helusers-0.9.0/helusers/providers/helsinki/views.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.759095 django-helusers-0.9.0/helusers/providers/helsinki_oidc/
+-rw-r--r--   0 keso       (501) staff       (20)        0 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki_oidc/__init__.py
+-rw-r--r--   0 keso       (501) staff       (20)       63 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki_oidc/admin.py
+-rw-r--r--   0 keso       (501) staff       (20)       27 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki_oidc/models.py
+-rw-r--r--   0 keso       (501) staff       (20)     1192 2023-06-07 08:56:44.000000 django-helusers-0.9.0/helusers/providers/helsinki_oidc/provider.py
+-rw-r--r--   0 keso       (501) staff       (20)      176 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/providers/helsinki_oidc/urls.py
+-rw-r--r--   0 keso       (501) staff       (20)     1013 2023-06-07 08:58:08.000000 django-helusers-0.9.0/helusers/providers/helsinki_oidc/views.py
+-rw-r--r--   0 keso       (501) staff       (20)     1476 2023-08-08 12:23:58.000000 django-helusers-0.9.0/helusers/settings.py
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.753726 django-helusers-0.9.0/helusers/templates/
+drwxr-xr-x   0 keso       (501) staff       (20)        0 2023-08-09 13:56:54.759545 django-helusers-0.9.0/helusers/templates/admin/
+-rw-r--r--   0 keso       (501) staff       (20)       33 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/templates/admin/base_site.html
+-rw-r--r--   0 keso       (501) staff       (20)      799 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/templates/admin/base_site_default.html
+-rw-r--r--   0 keso       (501) staff       (20)      847 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/templates/admin/base_site_grappelli.html
+-rw-r--r--   0 keso       (501) staff       (20)     1503 2021-02-15 11:35:13.000000 django-helusers-0.9.0/helusers/templates/admin/hel_login.html
+-rw-r--r--   0 keso       (501) staff       (20)     2371 2023-06-07 08:57:18.000000 django-helusers-0.9.0/helusers/tunnistamo_oidc.py
+-rw-r--r--   0 keso       (501) staff       (20)     1223 2022-02-18 06:33:17.000000 django-helusers-0.9.0/helusers/urls.py
+-rw-r--r--   0 keso       (501) staff       (20)     5439 2023-06-07 08:57:27.000000 django-helusers-0.9.0/helusers/user_utils.py
+-rw-r--r--   0 keso       (501) staff       (20)     2802 2023-08-08 12:23:22.000000 django-helusers-0.9.0/helusers/utils.py
+-rw-r--r--   0 keso       (501) staff       (20)     5213 2022-02-18 06:33:17.000000 django-helusers-0.9.0/helusers/views.py
+-rw-r--r--   0 keso       (501) staff       (20)       38 2023-08-09 13:56:54.759889 django-helusers-0.9.0/setup.cfg
+-rw-r--r--   0 keso       (501) staff       (20)     1543 2023-08-09 10:14:06.000000 django-helusers-0.9.0/setup.py
```

### Comparing `django-helusers-0.8.1/LICENSE` & `django-helusers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/PKG-INFO` & `django-helusers-0.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,475 +1,448 @@
-Metadata-Version: 2.1
-Name: django-helusers
-Version: 0.8.1
-Summary: Django app for the user infrastructure of the City of Helsinki
-Home-page: https://github.com/City-of-Helsinki/django-helusers
-Author: City of Helsinki
-Author-email: dev@hel.fi
-License: BSD License
-Description: [![Run tests](https://github.com/City-of-Helsinki/django-helusers/actions/workflows/test.yml/badge.svg)](https://github.com/City-of-Helsinki/django-helusers/actions/workflows/test.yml)
-        [![codecov](https://codecov.io/gh/City-of-Helsinki/django-helusers/branch/master/graph/badge.svg?token=bOfnYCJsWW)](https://codecov.io/gh/City-of-Helsinki/django-helusers)
-        
-        # Django app for City of Helsinki user infrastructure
-        
-        Django-helusers is your friendly app for bolting authentication into Django projects for City of Helsinki. Authentication schemes are based on [OAuth2](https://oauth.net/2/) and [OpenID Connect (OIDC)](https://openid.net/connect/).
-        
-        A baseline `User` model is provided that can be used with the various authentication use cases that are supported. The model supports mapping from AD groups to Django groups based on the authentication data.
-        
-        Additionally, there are **optional** functionalities that can be used as needed.
-        
-        Functionalities for server needing (API) access token verification:
-        
-        * For servers using Django REST Framework
-        * For servers not using Django REST Framework
-        
-        Functionalities for server needing to authenticate against OIDC or OAuth2 server:
-        
-        * support Django session login against OIDC or OAuth2 server, including Helsinki Tunnistus service and Azure AD
-        * augmented login template for Django admin, adding OIDC/OAuth2 login button
-        
-        ## Adding django-helusers your Django project
-        
-        Add `django-helusers` in your project's dependencies.
-        
-        Some optional features of `django-helusers` have additional dependencies.
-        These are mentioned in their relevant sections.
-        
-        ### Adding django-helusers Django apps
-        
-        Django-helusers provides two Django apps: `HelusersConfig` provides the
-        models and templates needed for helusers to work and `HelusersAdminConfig`
-        reconfigures Django admin to work with helusers.
-        
-        Before adding the apps, you will need to remove `django.contrib.admin`, as
-        `HelusersAdminConfig` is implementation of same functionality. You will get
-        `django.core.exceptions.ImproperlyConfigured: Application labels aren't unique, duplicates:
-        admin`-error, if you forget this step.
-        
-        Then proceed by adding these apps to your `INSTALLED_APPS` in settings.py:
-        
-        ```python
-        INSTALLED_APPS = (
-            'helusers.apps.HelusersConfig',
-            'helusers.apps.HelusersAdminConfig',
-            ...
-        )
-        ```
-        
-        Us usual with `INSTALLED_APPS`, ordering matters. `HelusersConfig` must come
-        before `HelusersAdminConfig` and anything else providing admin templates.
-        Unless, of course, you wish to override the admin templates provided here.
-        
-        One possible gotcha is, if you've added custom views to admin without
-        forwarding context from `each_context` to the your template.  Helusers
-        templates expect variables from `each_context` and will break if they are
-        missing.
-        
-        ### Adding user model
-        
-        helusers provides a baseline user model adding fields for Helsinki
-        specific information. As per Django [best practice](https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project)
-        you should subclass this model to make future customization easier:
-        
-        ```python
-        
-        # users/models.py
-        
-        from helusers.models import AbstractUser
-        
-        
-        class User(AbstractUser):
-            pass
-        ```
-        
-        and reference it in settings.py:
-        
-        ```python
-        # myproject/settings.py
-        
-        AUTH_USER_MODEL = 'users.User'
-        ```
-        
-        ## Optional features
-        
-        ### Django REST Framework API authentication using JWT
-        
-        If you have a REST API implemented using Django REST Framework and you want to authorize access to your API using JWTs, then this might be useful to you.
-        
-        API token authentication is a stateless authentication method, where every request is
-        authenticated by checking the signature of the included JWT token. It still
-        creates a persistent Django user, which is updated with the information
-        from the token with every request.
-        
-        - Include `drf-oidc-auth` in your project's dependencies.
-        - Configure REST framework to use the `ApiTokenAuthentication` class in `settings.py`:
-        
-        ```python
-        REST_FRAMEWORK = {
-            'DEFAULT_AUTHENTICATION_CLASSES': (
-                'helusers.oidc.ApiTokenAuthentication',
-            ),
+[![Run tests](https://github.com/City-of-Helsinki/django-helusers/actions/workflows/test.yml/badge.svg)](https://github.com/City-of-Helsinki/django-helusers/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/City-of-Helsinki/django-helusers/branch/master/graph/badge.svg?token=bOfnYCJsWW)](https://codecov.io/gh/City-of-Helsinki/django-helusers)
+
+# Django app for City of Helsinki user infrastructure
+
+Django-helusers is your friendly app for bolting authentication into Django projects for City of Helsinki. Authentication schemes are based on [OAuth2](https://oauth.net/2/) and [OpenID Connect (OIDC)](https://openid.net/connect/).
+
+A baseline `User` model is provided that can be used with the various authentication use cases that are supported. The model supports mapping from AD groups to Django groups based on the authentication data.
+
+Additionally, there are **optional** functionalities that can be used as needed.
+
+Functionalities for server needing (API) access token verification:
+
+* For servers using Django REST Framework
+* For servers not using Django REST Framework
+
+Functionalities for server needing to authenticate against OIDC or OAuth2 server:
+
+* support Django session login against OIDC or OAuth2 server, including Helsinki Tunnistus service and Azure AD
+* augmented login template for Django admin, adding OIDC/OAuth2 login button
+
+## Adding django-helusers your Django project
+
+Add `django-helusers` in your project's dependencies.
+
+Some optional features of `django-helusers` have additional dependencies.
+These are mentioned in their relevant sections.
+
+### Adding django-helusers Django apps
+
+Django-helusers provides two Django apps: `HelusersConfig` provides the
+models and templates needed for helusers to work and `HelusersAdminConfig`
+reconfigures Django admin to work with helusers.
+
+Before adding the apps, you will need to remove `django.contrib.admin`, as
+`HelusersAdminConfig` is implementation of same functionality. You will get
+`django.core.exceptions.ImproperlyConfigured: Application labels aren't unique, duplicates:
+admin`-error, if you forget this step.
+
+Then proceed by adding these apps to your `INSTALLED_APPS` in settings.py:
+
+```python
+INSTALLED_APPS = (
+    'helusers.apps.HelusersConfig',
+    'helusers.apps.HelusersAdminConfig',
+    ...
+)
+```
+
+Us usual with `INSTALLED_APPS`, ordering matters. `HelusersConfig` must come
+before `HelusersAdminConfig` and anything else providing admin templates.
+Unless, of course, you wish to override the admin templates provided here.
+
+One possible gotcha is, if you've added custom views to admin without
+forwarding context from `each_context` to the your template.  Helusers
+templates expect variables from `each_context` and will break if they are
+missing.
+
+### Adding user model
+
+helusers provides a baseline user model adding fields for Helsinki
+specific information. As per Django [best practice](https://docs.djangoproject.com/en/3.0/topics/auth/customizing/#using-a-custom-user-model-when-starting-a-project)
+you should subclass this model to make future customization easier:
+
+```python
+
+# users/models.py
+
+from helusers.models import AbstractUser
+
+
+class User(AbstractUser):
+    pass
+```
+
+and reference it in settings.py:
+
+```python
+# myproject/settings.py
+
+AUTH_USER_MODEL = 'users.User'
+```
+
+## Optional features
+
+### Django REST Framework API authentication using JWT
+
+If you have a REST API implemented using Django REST Framework and you want to authorize access to your API using JWTs, then this might be useful to you.
+
+API token authentication is a stateless authentication method, where every request is
+authenticated by checking the signature of the included JWT token. It still
+creates a persistent Django user, which is updated with the information
+from the token with every request.
+
+- Configure REST framework to use the `ApiTokenAuthentication` class in `settings.py`:
+
+```python
+REST_FRAMEWORK = {
+    'DEFAULT_AUTHENTICATION_CLASSES': (
+        'helusers.oidc.ApiTokenAuthentication',
+    ),
+}
+```
+
+- Set your deployment-specific variables in your project settings. See [Token authentication settings](#token-authentication-settings)
+
+### API authentication using JWT in any setup
+
+If you want to authorize access to your API using JWTs, but you are not using Django REST Framework, then this might be useful to you.
+
+API token authentication is a stateless authentication method, where every request is authenticated by checking the signature of the included JWT token.
+It still creates a persistent Django user, which is updated with the information from the token with every request.
+
+Django-helusers contains a `helusers.oidc.RequestJWTAuthentication` class.
+It has a method called `authenticate` that takes a [Django HttpRequest](https://docs.djangoproject.com/en/3.1/ref/request-response/#django.http.HttpRequest) as an argument, looks for a JWT from that request and performs authentication.
+User of this class can use it in any way they need to perform authentication and/or authorization.
+Check the class documentation for more details.
+
+
+### Token authentication settings
+
+Some settings are needed (and some are optional) that affect how the `ApiTokenAuthentication` and `RequestJWTAuthentication` classes work.
+
+```python
+OIDC_API_TOKEN_AUTH = {
+    # Audience that must be present in the token for it to be
+    # accepted. Value must be agreed between your SSO service and your
+    # application instance. Essentially this allows your application to
+    # know that the token is meant to be used with it.
+    # Multiple acceptable audiences are supported,
+    # so this setting can also be a list of strings.
+    # This setting is required.
+    'AUDIENCE': 'https://api.hel.fi/auth/projects',
+
+    # Who we trust to sign the tokens. The library will request the
+    # public signature keys from standard locations below this URL.
+    # Multiple issuers are supported, so this
+    # setting can also be a list of strings.
+    # Default is https://tunnistamo.hel.fi.
+    'ISSUER': 'https://api.hel.fi/sso/openid',
+
+    # The following can be used if you need certain scopes for any
+    # functionality of the API. Usually this is not needed, as checking
+    # the audience is enough. Default is False.
+    'REQUIRE_API_SCOPE_FOR_AUTHENTICATION': True,
+    # The name of the claim that is used to read in the scopes from the JWT.
+    # Supports multiple fields as a list. If the field is deeper in the claims
+    # use dot notation. e.g. "authorization.permissions.scopes"
+    # Default is https://api.hel.fi/auth.
+    'API_AUTHORIZATION_FIELD': 'scope_field',
+    # The request will be denied if scopes don't contain anything starting
+    # with the value provided here. Supports multiple scope prefixes as a list.
+    # Only one scope needs to match if multiple prefixes are provided.
+    'API_SCOPE_PREFIX': 'projects',
+
+    # In order to do the authentication the token authentication classes need
+    # some facts from the authorization server, mainly its public keys for
+    # verifying the JWT's signature. This setting controls the time how long
+    # authorization server configuration and public keys are "remembered".
+    # The value is in seconds. Default is 24 hours.
+    'OIDC_CONFIG_EXPIRATION_TIME': 600,
+}
+```
+
+### OIDC back channel logout endpoint
+
+Django-helusers provides an [OIDC back channel logout](https://openid.net/specs/openid-connect-backchannel-1_0.html) endpoint implementation.
+
+By default the OIDC back channel logout endpoint is disabled. You can enable it in your project's settings:
+
+```python
+# myproject/settings.py
+HELUSERS_BACK_CHANNEL_LOGOUT_ENABLED = True
+
+# These settings specify which authentication server(s) are trusted
+# to send back channel logout requests.
+OIDC_API_TOKEN_AUTH = {
+    # Who we trust to sign the logout tokens. The library will request
+    # the public signature keys from standard locations below this URL.
+    # Multiple issuers are supported, so this setting can also be a list
+    # of strings. Default is https://tunnistamo.hel.fi.
+    'ISSUER': 'https://api.hel.fi/sso/openid',
+
+    # Audience that must be present in the logout token for it to
+    # be accepted. Value must be agreed between your SSO service
+    # and your application instance. Essentially this allows your
+    # application to know that the token is meant to be used with
+    # it. Multiple acceptable audiences are supported, so this
+    # setting can also be a list of strings. This setting is required.
+    'AUDIENCE': 'https://api.hel.fi/auth/projects',
+}
+```
+
+You will also need to add Django-helusers URLs to your URL dispatcher configuration:
+
+```python
+# myproject/urls.py
+urlpatterns = [
+    ...
+    # You can adjust the prefix as you want
+    path('helauth/', include('helusers.urls')),
+    ...
+]
+```
+
+With these settings your project now provides an endpoint at `https://<your-domain>/helauth/logout/oidc/backchannel/` that responds to the OIDC back channel logout requests.
+
+When the endpoint receives a valid request, it stores information about the logout event to the database. This information is used when authentication for other requests is performed. The `helusers.oidc.RequestJWTAuthentication` class that performs authentication based on a JWT bearer token, checks if the token's session has been terminated (by a logout event), and if that's the case, it doesn't authenticate the caller.
+
+#### Logout event callback
+
+The project using the OIDC back channel logout functionality has an option to attach a callback into the logout event handler. This is done by telling Django-helusers where this callback is located. Configure it in your project's settings:
+
+```python
+# myproject/settings.py
+HELUSERS_BACK_CHANNEL_LOGOUT_CALLBACK = "myproject.utils.logout_callback"
+```
+
+When a valid logout event is received, the callback is called. The callback receives two keyword arguments:
+
+* `request`: the [HttpRequest](https://docs.djangoproject.com/en/2.2/ref/request-response/#httprequest-objects) object describing the request to the logout endpoint
+* `jwt`: a `helusers.jwt.JWT` instance of the logout token
+
+The callback can affect the result of the back channel logout event handling by returning an [HttpResponse](https://docs.djangoproject.com/en/2.2/ref/request-response/#httpresponse-objects) instance with a status code between 400 and 599 inclusive. If such a response object is returned by the callback, the logout event handling is terminated and the response is sent to the requester. Any other kind of return value from the callback is ignored.
+
+### Adding Tunnistamo authentication
+
+django-helusers ships with backend for authenticating against Tunnistamo
+using OIDC. Configuring this includes a Tunnistamo login button to the admin login screen.
+
+There is also a deprecated legacy OAuth2 backend using
+allauth framework.
+
+Include `social-auth-app-django` in your project's dependencies.
+
+Add `social_django` into your `INSTALLED_APPS` setting:
+
+```python
+# myproject/settings.py
+INSTALLED_APPS = (
+    ...
+    'social_django',
+    ...
+)
+```
+
+Typically you would want to support authenticating using both OIDC and local
+database tables. Local users are useful for initial django admin login, before
+you've delegated permissions to users coming through OIDC.
+
+Add backend configuration to your `settings.py`:
+
+```python
+AUTHENTICATION_BACKENDS = [
+    'helusers.tunnistamo_oidc.TunnistamoOIDCAuth',
+    'django.contrib.auth.backends.ModelBackend',
+]
+LOGIN_REDIRECT_URL = '/'
+LOGOUT_REDIRECT_URL = '/'
+```
+
+`LOGIN_REDIRECT_URL` is the default landing URL after succesful login, if your
+form did not specify anything else.
+
+`LOGOUT_REDIRECT_URL` is the same for logout. django-helusers requires this
+to be set.
+
+Configure `social_django` [authentication pipeline](https://python-social-auth.readthedocs.io/en/latest/pipeline.html)
+to handle the users. Django-helusers provides a default pipeline that could well
+suit your needs. Use it by importing it into your `settings.py`:
+
+```python
+from helusers.defaults import SOCIAL_AUTH_PIPELINE
+```
+
+If the default pipeline isn't suitable for your needs as is, build your pipeline
+by hand and set the `SOCIAL_AUTH_PIPELINE` setting to it. You can use the default
+pipeline as an inspiration and use the functions from `helusers.pipeline` in your
+own pipeline.
+
+You will also need to add URLs for `social_django` & `helusers` to your URL
+dispatcher configuration (`urls.py`):
+
+```python
+urlpatterns = [
+    ...
+    path('pysocial/', include('social_django.urls', namespace='social')),
+    path('helauth/', include('helusers.urls')),
+    ...
+]
+```
+
+You can change the paths if they conflict with your application.
+
+Finally, you will need to configure your SESSION_SERIALIZER. helusers stores
+the access token expiration time as a datetime which is not serializable
+to JSON, so Django needs to be configured to use the built-in
+PickleSerializer:
+
+```python
+SESSION_SERIALIZER = 'django.contrib.sessions.serializers.PickleSerializer'
+```
+
+#### Django session login
+
+Django session login is the usual login to Django that sets up a session
+and is typically implemented using a browser cookie. This is usually done
+using form with username & password fields. Django-helusers adds another
+path that delegates the login to an OIDC provider. User logs in at the
+provider and, upon successful return, a Django session is created for them.
+For us, the main use case has been allowing logins to Django admin.
+
+To support session login Django-helusers needs three settings that must
+be configured both at Helsinki OIDC provider and your project instance.
+The settings are:
+* client ID
+* client secret
+* Tunnistamo OIDC endpoint
+
+`Client` is OAuth2 / OIDC name for anything wanting to authenticate
+users. Thus your application would be a `client`
+
+Additionally you will need to provide your "callback URL" to the folks
+configuring Tunnistamo. This is implemented by `python-social-auth` and
+will, by default, be `https://app.domain/auth/complete/tunnistamo/`. During
+development on your own laptop your `app.domain` would be `localhost`.
+
+After you've received your client ID, client secret and Tunnistamo OIDC
+endpoint you would configure them as follows:
+```python
+SOCIAL_AUTH_TUNNISTAMO_KEY = 'https://i/am/clientid/in/url/style'
+SOCIAL_AUTH_TUNNISTAMO_SECRET = 'iamyoursecret'
+SOCIAL_AUTH_TUNNISTAMO_OIDC_ENDPOINT = 'https://tunnistamo.example.com/'
+```
+
+Note that `client ID` becomes `KEY` and `client secret` becomes `SECRET`.
+
+#### Active Directory groups
+
+Helusers can sync users AD groups to local Django groups when using an AD 
+login method in Tunnistamo. To enable groups sync you should add "ad_groups" 
+scope to the Tunnistamo OIDC authorize call. It can be done by adding
+the following to the settings:
+
+```python
+SOCIAL_AUTH_TUNNISTAMO_SCOPE = 'ad_groups'
+```
+
+That setting will add "ad_groups" scope to the default social auth scopes
+"openid profile email". If you would like to modify the default social
+auth scopes you can set all of the scopes in the `SOCIAL_AUTH_TUNNISTAMO_SCOPE` 
+setting and set `SOCIAL_AUTH_TUNNISTAMO_IGNORE_DEFAULT_SCOPE` to `True`.
+
+Additionally, the client in Tunnistamo should be configured with AD groups
+enabled.
+
+When the users returns from Tunnistamo with "ad_groups" claim set Helusers will 
+add all of the groups as an instance of `ADGroup` model to the database.
+
+Then, Helusers will add any missing ADGroups to the users' ad_groups-relation
+and remove any ADGroups the user is not a member of anymore.
+
+To use groups in Django permissions, you should use the Django admin view 
+(HELSINKI USERS > AD Group Mappings) to set mappings between ADGroups and 
+Groups. Helusers will then add the user to Django groups that are mapped
+to their AD Groups.
+
+Note that after creating mappings you cannot manually add a user to a mapped
+group if they are not a member of the corresponding AD group because the
+group will be removed the next time the user logs in.
+
+#### Adding tunnistamo URL to template context
+
+If you need to access the Tunnistamo API from your JS code, you can include
+the Tunnistamo base URL in your template context using helusers's context processor:
+
+```python
+TEMPLATES = [
+    {
+        'OPTIONS': {
+            'context_processors': [
+                'helusers.context_processors.settings'
+            ]
         }
-        ```
-        
-        - Set your deployment-specific variables in `local_settings.py`, e.g.:
-        
-        ```python
-        OIDC_API_TOKEN_AUTH = {
-            # Audience that must be present in the token for the request to be
-            # accepted. Value must be agreed between your SSO service and your
-            # application instance. Essentially this allows your application to
-            # know that the token in meant to be used with it.
-            'AUDIENCE': 'https://api.hel.fi/auth/projects',
-            # Who we trust to sign the tokens. The library will request the
-            # public signature keys from standard locations below this URL
-            'ISSUER': 'https://api.hel.fi/sso/openid'
-            # The following can be used if you need certain OAuth2 scopes
-            # for any functionality of the API. The request will be denied
-            # if scopes starting with API_SCOPE_PREFIX are not present
-            # in the token claims. Usually this is not needed, as checking
-            # the audience is enough.
-            'REQUIRE_API_SCOPE_FOR_AUTHENTICATION': True,
-            'API_SCOPE_PREFIX': 'projects',
-        }
-        ```
-        
-        ### API authentication using JWT in any setup
-        
-        If you want to authorize access to your API using JWTs, but you are not using Django REST Framework, then this might be useful to you.
-        
-        API token authentication is a stateless authentication method, where every request is authenticated by checking the signature of the included JWT token.
-        It still creates a persistent Django user, which is updated with the information from the token with every request.
-        
-        Django-helusers contains a `helusers.oidc.RequestJWTAuthentication` class.
-        It has a method called `authenticate` that takes a [Django HttpRequest](https://docs.djangoproject.com/en/3.1/ref/request-response/#django.http.HttpRequest) as an argument, looks for a JWT from that request and performs authentication.
-        User of this class can use it in any way they need to perform authentication and/or authorization.
-        Check the class documentation for more details.
-        
-        Some settings are needed (and some are optional) that affect how the `RequestJWTAuthentication` class works.
-        
-        ```python
-        OIDC_API_TOKEN_AUTH = {
-            # Audience that must be present in the token for it to be
-            # accepted. Value must be agreed between your SSO service and your
-            # application instance. Essentially this allows your application to
-            # know that the token is meant to be used with it.
-            # RequestJWTAuthentication supports multiple acceptable audiences,
-            # so this setting can also be a list of strings.
-            # This setting is required.
-            'AUDIENCE': 'https://api.hel.fi/auth/projects',
-        
-            # Who we trust to sign the tokens. The library will request the
-            # public signature keys from standard locations below this URL.
-            # RequestJWTAuthentication supports multiple issuers, so this
-            # setting can also be a list of strings.
-            # Default is https://tunnistamo.hel.fi.
-            'ISSUER': 'https://api.hel.fi/sso/openid'
-        
-            # The following can be used if you need certain scopes for any
-            # functionality of the API. Usually this is not needed, as checking
-            # the audience is enough. Default is False.
-            'REQUIRE_API_SCOPE_FOR_AUTHENTICATION': True,
-            # The name of the claim that is used to read in the scopes from the JWT.
-            # Default is https://api.hel.fi/auth.
-            'API_AUTHORIZATION_FIELD': 'scope_field',
-            # The request will be denied if scopes don't contain anything starting
-            # with the value provided here.
-            'API_SCOPE_PREFIX': 'projects',
-        
-            # In order to do the authentication RequestJWTAuthentication needs
-            # some facts from the authorization server, mainly its public keys for
-            # verifying the JWT's signature. This setting controls the time how long
-            # authorization server configuration and public keys are "remembered".
-            # The value is in seconds. Default is 24 hours.
-            'OIDC_CONFIG_EXPIRATION_TIME': 600,
-        }
-        ```
-        
-        ### OIDC back channel logout endpoint
-        
-        Django-helusers provides an [OIDC back channel logout](https://openid.net/specs/openid-connect-backchannel-1_0.html) endpoint implementation.
-        
-        By default the OIDC back channel logout endpoint is disabled. You can enable it in your project's settings:
-        
-        ```python
-        # myproject/settings.py
-        HELUSERS_BACK_CHANNEL_LOGOUT_ENABLED = True
-        
-        # These settings specify which authentication server(s) are trusted
-        # to send back channel logout requests.
-        OIDC_API_TOKEN_AUTH = {
-            # Who we trust to sign the logout tokens. The library will request
-            # the public signature keys from standard locations below this URL.
-            # Multiple issuers are supported, so this setting can also be a list
-            # of strings. Default is https://tunnistamo.hel.fi.
-            'ISSUER': 'https://api.hel.fi/sso/openid'
-        
-            # Audience that must be present in the logout token for it to
-            # be accepted. Value must be agreed between your SSO service
-            # and your application instance. Essentially this allows your
-            # application to know that the token is meant to be used with
-            # it. Multiple acceptable audiences are supported, so this
-            # setting can also be a list of strings. This setting is required.
-            'AUDIENCE': 'https://api.hel.fi/auth/projects',
-        }
-        ```
-        
-        You will also need to add Django-helusers URLs to your URL dispatcher configuration:
-        
-        ```python
-        # myproject/urls.py
-        urlpatterns = [
-            ...
-            # You can adjust the prefix as you want
-            path('helauth/', include('helusers.urls')),
-            ...
-        ]
-        ```
-        
-        With these settings your project now provides an endpoint at `https://<your-domain>/helauth/logout/oidc/backchannel/` that responds to the OIDC back channel logout requests.
-        
-        When the endpoint receives a valid request, it stores information about the logout event to the database. This information is used when authentication for other requests is performed. The `helusers.oidc.RequestJWTAuthentication` class that performs authentication based on a JWT bearer token, checks if the token's session has been terminated (by a logout event), and if that's the case, it doesn't authenticate the caller.
-        
-        #### Logout event callback
-        
-        The project using the OIDC back channel logout functionality has an option to attach a callback into the logout event handler. This is done by telling Django-helusers where this callback is located. Configure it in your project's settings:
-        
-        ```python
-        # myproject/settings.py
-        HELUSERS_BACK_CHANNEL_LOGOUT_CALLBACK = "myproject.utils.logout_callback"
-        ```
-        
-        When a valid logout event is received, the callback is called. The callback receives two keyword arguments:
-        
-        * `request`: the [HttpRequest](https://docs.djangoproject.com/en/2.2/ref/request-response/#httprequest-objects) object describing the request to the logout endpoint
-        * `jwt`: a `helusers.jwt.JWT` instance of the logout token
-        
-        The callback can affect the result of the back channel logout event handling by returning an [HttpResponse](https://docs.djangoproject.com/en/2.2/ref/request-response/#httpresponse-objects) instance with a status code between 400 and 599 inclusive. If such a response object is returned by the callback, the logout event handling is terminated and the response is sent to the requester. Any other kind of return value from the callback is ignored.
-        
-        ### Adding Tunnistamo authentication
-        
-        django-helusers ships with backend for authenticating against Tunnistamo
-        using OIDC. Configuring this includes a Tunnistamo login button to the admin login screen.
-        
-        There is also a deprecated legacy OAuth2 backend using
-        allauth framework.
-        
-        Include `social-auth-app-django` in your project's dependencies.
-        
-        Add `social_django` into your `INSTALLED_APPS` setting:
-        
-        ```python
-        # myproject/settings.py
-        INSTALLED_APPS = (
-            ...
-            'social_django',
-            ...
-        )
-        ```
-        
-        Typically you would want to support authenticating using both OIDC and local
-        database tables. Local users are useful for initial django admin login, before
-        you've delegated permissions to users coming through OIDC.
-        
-        Add backend configuration to your `settings.py`:
-        
-        ```python
-        AUTHENTICATION_BACKENDS = [
-            'helusers.tunnistamo_oidc.TunnistamoOIDCAuth',
-            'django.contrib.auth.backends.ModelBackend',
-        ]
-        LOGIN_REDIRECT_URL = '/'
-        LOGOUT_REDIRECT_URL = '/'
-        ```
-        
-        `LOGIN_REDIRECT_URL` is the default landing URL after succesful login, if your
-        form did not specify anything else.
-        
-        `LOGOUT_REDIRECT_URL` is the same for logout. django-helusers requires this
-        to be set.
-        
-        You will also need to add URLs for `social_django` & `helusers` to your URL
-        dispatcher configuration (`urls.py`):
-        
-        ```python
-        urlpatterns = [
-            ...
-            path('pysocial/', include('social_django.urls', namespace='social')),
-            path('helauth/', include('helusers.urls')),
-            ...
-        ]
-        ```
-        
-        You can change the paths if they conflict with your application.
-        
-        Finally, you will need to configure your SESSION_SERIALIZER. helusers stores
-        the access token expiration time as a datetime which is not serializable
-        to JSON, so Django needs to be configured to use the built-in
-        PickleSerializer:
-        
-        ```python
-        SESSION_SERIALIZER = 'django.contrib.sessions.serializers.PickleSerializer'
-        ```
-        
-        #### Django session login
-        
-        Django session login is the usual login to Django that sets up a session
-        and is typically implemented using a browser cookie. This is usually done
-        using form with username & password fields. Django-helusers adds another
-        path that delegates the login to an OIDC provider. User logs in at the
-        provider and, upon successful return, a Django session is created for them.
-        For us, the main use case has been allowing logins to Django admin.
-        
-        To support session login Django-helusers needs three settings that must
-        be configured both at Helsinki OIDC provider and your project instance.
-        The settings are:
-        * client ID
-        * client secret
-        * Tunnistamo OIDC endpoint
-        
-        `Client` is OAuth2 / OIDC name for anything wanting to authenticate
-        users. Thus your application would be a `client`
-        
-        Additionally you will need to provide your "callback URL" to the folks
-        configuring Tunnistamo. This is implemented by `python-social-auth` and
-        will, by default, be `https://app.domain/auth/complete/tunnistamo/`. During
-        development on your own laptop your `app.domain` would be `localhost`.
-        
-        After you've received your client ID, client secret and Tunnistamo OIDC
-        endpoint you would configure them as follows:
-        ```python
-        SOCIAL_AUTH_TUNNISTAMO_KEY = 'https://i/am/clientid/in/url/style'
-        SOCIAL_AUTH_TUNNISTAMO_SECRET = 'iamyoursecret'
-        SOCIAL_AUTH_TUNNISTAMO_OIDC_ENDPOINT = 'https://tunnistamo.example.com/'
-        ```
-        
-        Note that `client ID` becomes `KEY` and `client secret` becomes `SECRET`.
-        
-        #### Active Directory groups
-        
-        Helusers can sync users AD groups to local Django groups when using an AD 
-        login method in Tunnistamo. To enable groups sync you should add "ad_groups" 
-        scope to the Tunnistamo OIDC authorize call. It can be done by adding
-        the following to the settings:
-        
-        ```python
-        SOCIAL_AUTH_TUNNISTAMO_SCOPE = 'ad_groups'
-        ```
-        
-        That setting will add "ad_groups" scope to the default social auth scopes
-        "openid profile email". If you would like to modify the default social
-        auth scopes you can set all of the scopes in the `SOCIAL_AUTH_TUNNISTAMO_SCOPE` 
-        setting and set `SOCIAL_AUTH_TUNNISTAMO_IGNORE_DEFAULT_SCOPE` to `True`.
-        
-        Additionally, the client in Tunnistamo should be configured with AD groups
-        enabled.
-        
-        When the users returns from Tunnistamo with "ad_groups" claim set Helusers will 
-        add all of the groups as an instance of `ADGroup` model to the database.
-        
-        Then, Helusers will add any missing ADGroups to the users' ad_groups-relation
-        and remove any ADGroups the user is not a member of anymore.
-        
-        To use groups in Django permissions, you should use the Django admin view 
-        (HELSINKI USERS > AD Group Mappings) to set mappings between ADGroups and 
-        Groups. Helusers will then add the user to Django groups that are mapped
-        to their AD Groups.
-        
-        Note that after creating mappings you cannot manually add a user to a mapped
-        group if they are not a member of the corresponding AD group because the
-        group will be removed the next time the user logs in.
-        
-        #### Adding tunnistamo URL to template context
-        
-        If you need to access the Tunnistamo API from your JS code, you can include
-        the Tunnistamo base URL in your template context using helusers's context processor:
-        
-        ```python
-        TEMPLATES = [
-            {
-                'OPTIONS': {
-                    'context_processors': [
-                        'helusers.context_processors.settings'
-                    ]
-                }
-            }
-        ]
-        ```
-        
-        #### Carrying language preference from your application to Tunnistamo
-        
-        Tunnistamo (per the OIDC specs) allows clients to specify the language used for
-        the login process. This allows you to carry your applications language setting
-        to the login screens presented by Tunnistamo.
-        
-        Configure `python-social-auth` to pass the necessary argument through its
-        login view:
-        ```python
-        SOCIAL_AUTH_TUNNISTAMO_AUTH_EXTRA_ARGUMENTS = {'ui_locales': 'fi'}
-        ```
-        `fi` there is the language code that will be used when no language is requested, so change it if you you prefer some
-        other default language. If you don't want to set a default language at all, use an empty string `""` as the language
-        code.
-        
-        When this setting is in place, languages can be requested using query param `ui_locales=<language code>` when starting
-        the login process, for example in your template
-        ```
-        <a href="{% url 'helusers:auth_login' %}?next=/foobar/&ui_locales=en">Login in English</a>
-        ```
-        
-        #### Disabling password logins
-        
-        If you're not allowing users to log in with passwords, you may disable the
-        username/password form from Django admin login page by setting `HELUSERS_PASSWORD_LOGIN_DISABLED`
-        to `True`.
-        
-        # Development
-        
-        Virtual Python environment can be used. For example:
-        
-        ```bash
-        python3 -m venv .venv
-        source .venv/bin/activate
-        ```
-        
-        Install package requirements:
-        
-        ```bash
-        pip install -e .
-        ```
-        
-        Install development requirements:
-        
-        ```bash
-        pip install -r requirements-test.txt
-        ```
-        
-        ## Running tests
-        
-        ```bash
-        pytest
-        ```
-        
-        You can run the tests against multiple environments by using [tox](https://tox.readthedocs.io/en/latest/).
-        Install `tox` globally and run:
-        
-        ```bash
-        tox
-        ```
-        
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Description-Content-Type: text/markdown
+    }
+]
+```
+
+#### Carrying language preference from your application to Tunnistamo
+
+Tunnistamo (per the OIDC specs) allows clients to specify the language used for
+the login process. This allows you to carry your applications language setting
+to the login screens presented by Tunnistamo.
+
+Configure `python-social-auth` to pass the necessary argument through its
+login view:
+```python
+SOCIAL_AUTH_TUNNISTAMO_AUTH_EXTRA_ARGUMENTS = {'ui_locales': 'fi'}
+```
+`fi` there is the language code that will be used when no language is requested, so change it if you you prefer some
+other default language. If you don't want to set a default language at all, use an empty string `""` as the language
+code.
+
+When this setting is in place, languages can be requested using query param `ui_locales=<language code>` when starting
+the login process, for example in your template
+```
+<a href="{% url 'helusers:auth_login' %}?next=/foobar/&ui_locales=en">Login in English</a>
+```
+
+#### Disabling password logins
+
+If you're not allowing users to log in with passwords, you may disable the
+username/password form from Django admin login page by setting `HELUSERS_PASSWORD_LOGIN_DISABLED`
+to `True`.
+
+# Development
+
+Virtual Python environment can be used. For example:
+
+```bash
+python3 -m venv .venv
+source .venv/bin/activate
+```
+
+Install package requirements:
+
+```bash
+pip install -e .
+```
+
+Install development requirements:
+
+```bash
+pip install -r requirements-test.txt
+```
+
+## Running tests
+
+```bash
+pytest
+```
+
+You can run the tests against multiple environments by using [tox](https://tox.readthedocs.io/en/latest/).
+Install `tox` globally and run:
+
+```bash
+tox
+```
```

### Comparing `django-helusers-0.8.1/README.md` & `django-helusers-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: django-helusers
+Version: 0.9.0
+Summary: Django app for the user infrastructure of the City of Helsinki
+Home-page: https://github.com/City-of-Helsinki/django-helusers
+Author: City of Helsinki
+Author-email: dev@hel.fi
+License: BSD License
+Platform: UNKNOWN
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Run tests](https://github.com/City-of-Helsinki/django-helusers/actions/workflows/test.yml/badge.svg)](https://github.com/City-of-Helsinki/django-helusers/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/City-of-Helsinki/django-helusers/branch/master/graph/badge.svg?token=bOfnYCJsWW)](https://codecov.io/gh/City-of-Helsinki/django-helusers)
 
 # Django app for City of Helsinki user infrastructure
 
 Django-helusers is your friendly app for bolting authentication into Django projects for City of Helsinki. Authentication schemes are based on [OAuth2](https://oauth.net/2/) and [OpenID Connect (OIDC)](https://openid.net/connect/).
 
@@ -88,91 +114,76 @@
 If you have a REST API implemented using Django REST Framework and you want to authorize access to your API using JWTs, then this might be useful to you.
 
 API token authentication is a stateless authentication method, where every request is
 authenticated by checking the signature of the included JWT token. It still
 creates a persistent Django user, which is updated with the information
 from the token with every request.
 
-- Include `drf-oidc-auth` in your project's dependencies.
 - Configure REST framework to use the `ApiTokenAuthentication` class in `settings.py`:
 
 ```python
 REST_FRAMEWORK = {
     'DEFAULT_AUTHENTICATION_CLASSES': (
         'helusers.oidc.ApiTokenAuthentication',
     ),
 }
 ```
 
-- Set your deployment-specific variables in `local_settings.py`, e.g.:
-
-```python
-OIDC_API_TOKEN_AUTH = {
-    # Audience that must be present in the token for the request to be
-    # accepted. Value must be agreed between your SSO service and your
-    # application instance. Essentially this allows your application to
-    # know that the token in meant to be used with it.
-    'AUDIENCE': 'https://api.hel.fi/auth/projects',
-    # Who we trust to sign the tokens. The library will request the
-    # public signature keys from standard locations below this URL
-    'ISSUER': 'https://api.hel.fi/sso/openid'
-    # The following can be used if you need certain OAuth2 scopes
-    # for any functionality of the API. The request will be denied
-    # if scopes starting with API_SCOPE_PREFIX are not present
-    # in the token claims. Usually this is not needed, as checking
-    # the audience is enough.
-    'REQUIRE_API_SCOPE_FOR_AUTHENTICATION': True,
-    'API_SCOPE_PREFIX': 'projects',
-}
-```
+- Set your deployment-specific variables in your project settings. See [Token authentication settings](#token-authentication-settings)
 
 ### API authentication using JWT in any setup
 
 If you want to authorize access to your API using JWTs, but you are not using Django REST Framework, then this might be useful to you.
 
 API token authentication is a stateless authentication method, where every request is authenticated by checking the signature of the included JWT token.
 It still creates a persistent Django user, which is updated with the information from the token with every request.
 
 Django-helusers contains a `helusers.oidc.RequestJWTAuthentication` class.
 It has a method called `authenticate` that takes a [Django HttpRequest](https://docs.djangoproject.com/en/3.1/ref/request-response/#django.http.HttpRequest) as an argument, looks for a JWT from that request and performs authentication.
 User of this class can use it in any way they need to perform authentication and/or authorization.
 Check the class documentation for more details.
 
-Some settings are needed (and some are optional) that affect how the `RequestJWTAuthentication` class works.
+
+### Token authentication settings
+
+Some settings are needed (and some are optional) that affect how the `ApiTokenAuthentication` and `RequestJWTAuthentication` classes work.
 
 ```python
 OIDC_API_TOKEN_AUTH = {
     # Audience that must be present in the token for it to be
     # accepted. Value must be agreed between your SSO service and your
     # application instance. Essentially this allows your application to
     # know that the token is meant to be used with it.
-    # RequestJWTAuthentication supports multiple acceptable audiences,
+    # Multiple acceptable audiences are supported,
     # so this setting can also be a list of strings.
     # This setting is required.
     'AUDIENCE': 'https://api.hel.fi/auth/projects',
 
     # Who we trust to sign the tokens. The library will request the
     # public signature keys from standard locations below this URL.
-    # RequestJWTAuthentication supports multiple issuers, so this
+    # Multiple issuers are supported, so this
     # setting can also be a list of strings.
     # Default is https://tunnistamo.hel.fi.
-    'ISSUER': 'https://api.hel.fi/sso/openid'
+    'ISSUER': 'https://api.hel.fi/sso/openid',
 
     # The following can be used if you need certain scopes for any
     # functionality of the API. Usually this is not needed, as checking
     # the audience is enough. Default is False.
     'REQUIRE_API_SCOPE_FOR_AUTHENTICATION': True,
     # The name of the claim that is used to read in the scopes from the JWT.
+    # Supports multiple fields as a list. If the field is deeper in the claims
+    # use dot notation. e.g. "authorization.permissions.scopes"
     # Default is https://api.hel.fi/auth.
     'API_AUTHORIZATION_FIELD': 'scope_field',
     # The request will be denied if scopes don't contain anything starting
-    # with the value provided here.
+    # with the value provided here. Supports multiple scope prefixes as a list.
+    # Only one scope needs to match if multiple prefixes are provided.
     'API_SCOPE_PREFIX': 'projects',
 
-    # In order to do the authentication RequestJWTAuthentication needs
+    # In order to do the authentication the token authentication classes need
     # some facts from the authorization server, mainly its public keys for
     # verifying the JWT's signature. This setting controls the time how long
     # authorization server configuration and public keys are "remembered".
     # The value is in seconds. Default is 24 hours.
     'OIDC_CONFIG_EXPIRATION_TIME': 600,
 }
 ```
@@ -190,15 +201,15 @@
 # These settings specify which authentication server(s) are trusted
 # to send back channel logout requests.
 OIDC_API_TOKEN_AUTH = {
     # Who we trust to sign the logout tokens. The library will request
     # the public signature keys from standard locations below this URL.
     # Multiple issuers are supported, so this setting can also be a list
     # of strings. Default is https://tunnistamo.hel.fi.
-    'ISSUER': 'https://api.hel.fi/sso/openid'
+    'ISSUER': 'https://api.hel.fi/sso/openid',
 
     # Audience that must be present in the logout token for it to
     # be accepted. Value must be agreed between your SSO service
     # and your application instance. Essentially this allows your
     # application to know that the token is meant to be used with
     # it. Multiple acceptable audiences are supported, so this
     # setting can also be a list of strings. This setting is required.
@@ -276,14 +287,27 @@
 
 `LOGIN_REDIRECT_URL` is the default landing URL after succesful login, if your
 form did not specify anything else.
 
 `LOGOUT_REDIRECT_URL` is the same for logout. django-helusers requires this
 to be set.
 
+Configure `social_django` [authentication pipeline](https://python-social-auth.readthedocs.io/en/latest/pipeline.html)
+to handle the users. Django-helusers provides a default pipeline that could well
+suit your needs. Use it by importing it into your `settings.py`:
+
+```python
+from helusers.defaults import SOCIAL_AUTH_PIPELINE
+```
+
+If the default pipeline isn't suitable for your needs as is, build your pipeline
+by hand and set the `SOCIAL_AUTH_PIPELINE` setting to it. You can use the default
+pipeline as an inspiration and use the functions from `helusers.pipeline` in your
+own pipeline.
+
 You will also need to add URLs for `social_django` & `helusers` to your URL
 dispatcher configuration (`urls.py`):
 
 ```python
 urlpatterns = [
     ...
     path('pysocial/', include('social_django.urls', namespace='social')),
@@ -444,7 +468,9 @@
 
 You can run the tests against multiple environments by using [tox](https://tox.readthedocs.io/en/latest/).
 Install `tox` globally and run:
 
 ```bash
 tox
 ```
+
+
```

### Comparing `django-helusers-0.8.1/django_helusers.egg-info/SOURCES.txt` & `django-helusers-0.9.0/django_helusers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 helusers/pipeline.py
 helusers/settings.py
 helusers/tunnistamo_oidc.py
 helusers/urls.py
 helusers/user_utils.py
 helusers/utils.py
 helusers/views.py
+helusers/locale/fi/LC_MESSAGES/django.mo
 helusers/locale/fi/LC_MESSAGES/django.po
 helusers/management/commands/sync_helusers.py
 helusers/migrations/0001_add_ad_groups.py
 helusers/migrations/0002_add_oidcbackchannellogoutevent.py
 helusers/migrations/__init__.py
 helusers/providers/__init__.py
 helusers/providers/helsinki/__init__.py
```

### Comparing `django-helusers-0.8.1/helusers/_oidc_auth_impl.py` & `django-helusers-0.9.0/helusers/_oidc_auth_impl.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 import logging
-import requests
+
+from cachetools.func import ttl_cache
 from django.utils.encoding import smart_str
-from django.utils.functional import cached_property
 from django.utils.translation import gettext as _
-from oidc_auth.authentication import JSONWebTokenAuthentication
-from oidc_auth.util import cache
-from rest_framework.authentication import get_authorization_header
+from jose import JWTError
+from rest_framework.authentication import BaseAuthentication, get_authorization_header
 from rest_framework.exceptions import AuthenticationFailed
 
 from .authz import UserAuthorization
+from .jwt import JWT, ValidationError
 from .settings import api_token_auth_settings
 from .user_utils import get_or_create_user
 
 logger = logging.getLogger(__name__)
 
 
-class ApiTokenAuthentication(JSONWebTokenAuthentication):
+class ApiTokenAuthentication(BaseAuthentication):
+    www_authenticate_realm = "api"
+
     def __init__(self, settings=None, **kwargs):
         self.settings = settings or api_token_auth_settings
         super(ApiTokenAuthentication, self).__init__(**kwargs)
 
-    @cached_property
-    def auth_scheme(self):
-        return self.settings.AUTH_SCHEME or 'Bearer'
-
     @property
-    def oidc_config(self):
-        return self.get_oidc_config()
+    def auth_scheme(self):
+        return self.settings.AUTH_SCHEME or "Bearer"
 
-    @cache(ttl=api_token_auth_settings.OIDC_CONFIG_EXPIRATION_TIME)
-    def get_oidc_config(self):
-        issuer = self.settings.ISSUER
-        if not isinstance(issuer, str):
-            issuer = issuer[0]
-        url = issuer + '/.well-known/openid-configuration'
-        return requests.get(url).json()
+    @ttl_cache(ttl=api_token_auth_settings.OIDC_CONFIG_EXPIRATION_TIME)
+    def get_oidc_config(self, issuer):
+        from helusers.oidc import OIDCConfig
+        return OIDCConfig(issuer)
 
     def authenticate(self, request):
         jwt_value = self.get_jwt_value(request)
         if jwt_value is None:
             return None
 
         try:
             payload = self.decode_jwt(jwt_value)
-        except AuthenticationFailed as e:
-            logger.debug("Invalid token signature")
-            raise
-
-        # Some OPs may provide the "amr" incorrectly as a string, while the
-        # specification dictates it must be an array of strings. Fix that here.
-        if isinstance(payload.get("amr"), str):
-            payload["amr"] = [payload["amr"]]
-            logger.debug(
-                'Modified "amr" claim to be an array of strings instead of a string.'
-            )
+        except JWTError:
+            return None
 
         logger.debug("Token payload decoded as: {}".format(payload))
 
-        self.validate_claims(payload)
-
         user_resolver = self.settings.USER_RESOLVER  # Default: resolve_user
         try:
             user = user_resolver(request, payload)
         except ValueError as e:
             raise AuthenticationFailed(str(e)) from e
         auth = UserAuthorization(user, payload, self.settings)
 
-        if self.settings.REQUIRE_API_SCOPE_FOR_AUTHENTICATION:
-            api_scope = self.settings.API_SCOPE_PREFIX
-            if not auth.has_api_scope_with_prefix(api_scope):
-                raise AuthenticationFailed(
-                    _("Not authorized for API scope \"{api_scope}\"")
-                    .format(api_scope=api_scope))
+        return user, auth
+
+    def decode_jwt(self, jwt_value):
+        jwt = JWT(jwt_value, settings=self.settings)
 
-        return (user, auth)
+        try:
+            jwt.validate_issuer()
+        except ValidationError as e:
+            raise AuthenticationFailed(str(e)) from e
+
+        keys = self.get_oidc_config(jwt.issuer).keys()
+        try:
+            jwt.validate(keys, self.settings.AUDIENCE)
+            jwt.validate_api_scope()
+            jwt.validate_session()
+            self.validate_claims(jwt.claims)
+        except ValidationError as e:
+            raise AuthenticationFailed(str(e)) from e
+        except Exception:
+            raise AuthenticationFailed("JWT verification failed.")
+
+        return jwt.claims
 
     def get_jwt_value(self, request):
         auth = get_authorization_header(request).split()
 
         logger.debug("Authorization header: {}".format(auth))
 
         if not auth or smart_str(auth[0]).lower() != self.auth_scheme.lower():
@@ -89,18 +87,18 @@
         elif len(auth) > 2:
             raise AuthenticationFailed(
                 _("Invalid Authorization header. "
                   "Credentials string should not contain spaces."))
 
         return auth[1]
 
+    def validate_claims(self, id_token):
+        """Not in use. Only for backwards compatibility"""
+
     def authenticate_header(self, request):
         return '{auth_scheme} realm="{realm}"'.format(
             auth_scheme=self.auth_scheme,
             realm=self.www_authenticate_realm)
 
-    def get_audiences(self, api_token):
-        return {self.settings.AUDIENCE}
-
 
 def resolve_user(request, payload):
     return get_or_create_user(payload, oidc=True)
```

### Comparing `django-helusers-0.8.1/helusers/_rest_framework_jwt_impl.py` & `django-helusers-0.9.0/helusers/_rest_framework_jwt_impl.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/adapter.py` & `django-helusers-0.9.0/helusers/adapter.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/admin.py` & `django-helusers-0.9.0/helusers/admin.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/admin_site.py` & `django-helusers-0.9.0/helusers/admin_site.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/authz.py` & `django-helusers-0.9.0/helusers/authz.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.utils.functional import cached_property
 
 from .settings import api_token_auth_settings
+from .utils import get_scopes_from_claims
 
 
 class UserAuthorization(object):
     def __init__(self, user, api_token_payload, settings=None):
         """
         Initialize authorization info from user and API Token payload.
         """
@@ -38,16 +39,8 @@
             return None
         return any(
             x == prefix or x.startswith(prefix + '.')
             for x in self._authorized_api_scopes)
 
     @cached_property
     def _authorized_api_scopes(self):
-        api_scopes = self.data.get(self.settings.API_AUTHORIZATION_FIELD)
-        return (set(api_scopes)
-                if is_list_of_non_empty_strings(api_scopes) else None)
-
-
-def is_list_of_non_empty_strings(value):
-    if not isinstance(value, list):
-        return False
-    return all(isinstance(x, str) and x for x in value)
+        return get_scopes_from_claims(self.settings.API_AUTHORIZATION_FIELD, self.data)
```

### Comparing `django-helusers-0.8.1/helusers/defaults.py` & `django-helusers-0.9.0/helusers/defaults.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/jwt.py` & `django-helusers-0.9.0/helusers/jwt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+from .utils import get_scopes_from_claims
+
 try:
     from ._rest_framework_jwt_impl import (JWTAuthentication,
                                            get_user_id_from_payload_handler,
                                            patch_jwt_settings)
 except ImportError:
     pass
 
 from django.utils.functional import cached_property
 from jose import jwt
 
+from .models import OIDCBackChannelLogoutEvent
 from .settings import api_token_auth_settings
 
 
 _NOT_PROVIDED = object()
 
 
 class ValidationError(Exception):
     pass
 
 
 class JWT:
-    def __init__(self, encoded_jwt):
+    def __init__(self, encoded_jwt, settings=None):
         """The constructor checks that a JWT can be extracted from the
         provided input but it doesn't validate it in any way. If the
         input is invalid, an exception is raised."""
         self._encoded_jwt = encoded_jwt
         self._claims = jwt.get_unverified_claims(encoded_jwt)
+        self.settings = settings or api_token_auth_settings
 
     def validate(self, keys, audience, required_claims=_NOT_PROVIDED):
         """Verifies the JWT's signature using the provided keys,
         and validates the claims, raising an exception if anything fails.
         Required claims can be specified using the required_claims argument
         and it defaults to ["aud", "exp"]."""
 
@@ -56,14 +60,46 @@
             if isinstance(claim_audiences, str):
                 claim_audiences = {claim_audiences}
             if isinstance(audience, str):
                 audience = {audience}
             if len(set(audience).intersection(claim_audiences)) == 0:
                 raise ValidationError("Invalid audience.")
 
+    def validate_issuer(self):
+        try:
+            issuer = self.issuer
+        except KeyError:
+            raise ValidationError('Required "iss" claim is missing.')
+
+        issuers = self.settings.ISSUER
+        if isinstance(issuers, str):
+            issuers = [issuers]
+
+        if issuer not in issuers:
+            raise ValidationError("Unknown JWT issuer {}.".format(issuer))
+
+    def validate_api_scope(self):
+        if not self.settings.REQUIRE_API_SCOPE_FOR_AUTHENTICATION:
+            return
+
+        api_scopes = self.settings.API_SCOPE_PREFIX
+        if isinstance(api_scopes, str):
+            api_scopes = [api_scopes]
+
+        if not any(
+            [self.has_api_scope_with_prefix(api_scope) for api_scope in api_scopes]
+        ):
+            raise ValidationError(
+                'Not authorized for any of the API scopes "{}"'.format(api_scopes)
+            )
+
+    def validate_session(self):
+        if OIDCBackChannelLogoutEvent.objects.is_session_terminated_for_token(self):
+            raise ValidationError("Session has been terminated.")
+
     @property
     def issuer(self):
         """Returns the "iss" claim value."""
         return self.claims["iss"]
 
     @property
     def claims(self):
@@ -78,14 +114,11 @@
         return any(
             x == prefix or x.startswith(prefix + ".")
             for x in self._authorized_api_scopes
         )
 
     @cached_property
     def _authorized_api_scopes(self):
-        def is_list_of_non_empty_strings(value):
-            return isinstance(value, list) and all(
-                isinstance(x, str) and x for x in value
-            )
-
-        api_scopes = self.claims.get(api_token_auth_settings.API_AUTHORIZATION_FIELD)
-        return set(api_scopes) if is_list_of_non_empty_strings(api_scopes) else set()
+        return get_scopes_from_claims(
+            self.settings.API_AUTHORIZATION_FIELD,
+            self.claims
+        )
```

### Comparing `django-helusers-0.8.1/helusers/locale/fi/LC_MESSAGES/django.po` & `django-helusers-0.9.0/helusers/locale/fi/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,72 +4,68 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-09 12:32+0200\n"
+"POT-Creation-Date: 2023-06-20 23:51-0500\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+#: helusers/_oidc_auth_impl.py
+msgid "Invalid Authorization header. No credentials provided"
+msgstr ""
+
+#: helusers/_oidc_auth_impl.py
+msgid ""
+"Invalid Authorization header. Credentials string should not contain spaces."
+msgstr ""
+
+#: helusers/_rest_framework_jwt_impl.py
+msgid "User account is disabled."
+msgstr "Käyttäjätunnus on pois käytöstä."
+
 #: helusers/admin_site.py
 msgid "Django admin"
 msgstr "Ylläpito"
 
 #: helusers/admin_site.py
 #, python-format
 msgid "%(site_name)s admin"
 msgstr "Sivuston %(site_name)s ylläpito"
 
 #: helusers/apps.py
 msgid "Helsinki Users"
 msgstr "Käyttäjät"
 
-#: helusers/jwt.py
-msgid "User account is disabled."
-msgstr "Käyttäjätunnus on pois käytöstä."
-
 #: helusers/models.py
 #, fuzzy
 #| msgid "AD Group Mapping"
 msgid "AD group mapping"
 msgstr "AD-ryhmätaulu"
 
 #: helusers/models.py
 msgid "AD group mappings"
 msgstr "AD-ryhmätaulut"
 
-#: helusers/oidc.py
-#, python-brace-format
-msgid "Not authorized for API scope \"{api_scope}\""
-msgstr ""
-
-#: helusers/oidc.py
-msgid "Invalid Authorization header. No credentials provided"
-msgstr ""
-
-#: helusers/oidc.py
-msgid "Invalid Authorization header. Credentials string should not contain spaces."
-msgstr ""
-
 #: helusers/templates/admin/base_site_default.html
 msgid "Django site admin"
 msgstr "Sivuston ylläpito"
 
 #: helusers/templates/admin/base_site_default.html
 msgid "Django administration"
 msgstr "Ylläpito"
 
 #: helusers/user_utils.py
-msgid "Invalid payload."
+msgid "Invalid payload. sub missing"
 msgstr ""
 
 #: helusers/views.py
 msgid "You have been successfully logged out."
 msgstr "Sinut on nyt kirjattu ulos."
```

### Comparing `django-helusers-0.8.1/helusers/management/commands/sync_helusers.py` & `django-helusers-0.9.0/helusers/management/commands/sync_helusers.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/migrations/0001_add_ad_groups.py` & `django-helusers-0.9.0/helusers/migrations/0001_add_ad_groups.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/migrations/0002_add_oidcbackchannellogoutevent.py` & `django-helusers-0.9.0/helusers/migrations/0002_add_oidcbackchannellogoutevent.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/models.py` & `django-helusers-0.9.0/helusers/models.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/oidc.py` & `django-helusers-0.9.0/helusers/oidc.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from cachetools.func import ttl_cache
 from django.core.exceptions import ImproperlyConfigured
 from django.core.signals import setting_changed
 from django.dispatch import receiver
 from django.utils.functional import cached_property
 
 from .authz import UserAuthorization
-from .jwt import JWT
-from .models import OIDCBackChannelLogoutEvent
+from .jwt import JWT, ValidationError
 from .settings import api_token_auth_settings
 from .user_utils import get_or_create_user
 
 
 class OIDCConfig:
     def __init__(self, issuer):
         self._issuer = issuer
@@ -122,33 +121,24 @@
             if auth_scheme.lower() != "bearer":
                 return None
             jwt = JWT(jwt_value)
         except Exception:
             return None
 
         try:
-            issuer = jwt.issuer
-        except KeyError:
-            raise AuthenticationError('Required "iss" claim is missing.')
+            jwt.validate_issuer()
+        except ValidationError as e:
+            raise AuthenticationError(str(e)) from e
 
-        if issuer not in _defaults.issuers:
-            raise AuthenticationError("Unknown JWT issuer {}.".format(issuer))
-
-        keys = _defaults.key_provider(issuer)
+        keys = _defaults.key_provider(jwt.issuer)
         try:
             jwt.validate(keys, _defaults.audience)
+            jwt.validate_api_scope()
+            jwt.validate_session()
+        except ValidationError as e:
+            raise AuthenticationError(str(e)) from e
         except Exception:
             raise AuthenticationError("JWT verification failed.")
 
-        if api_token_auth_settings.REQUIRE_API_SCOPE_FOR_AUTHENTICATION:
-            api_scope = api_token_auth_settings.API_SCOPE_PREFIX
-            if not jwt.has_api_scope_with_prefix(api_scope):
-                raise AuthenticationError(
-                    'Not authorized for API scope "{}"'.format(api_scope)
-                )
-
-        if OIDCBackChannelLogoutEvent.objects.is_session_terminated_for_token(jwt):
-            raise AuthenticationError("Session has been terminated.")
-
         claims = jwt.claims
         user = get_or_create_user(claims, oidc=True)
         return UserAuthorization(user, claims)
```

### Comparing `django-helusers-0.8.1/helusers/pipeline.py` & `django-helusers-0.9.0/helusers/pipeline.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/providers/helsinki/provider.py` & `django-helusers-0.9.0/helusers/providers/helsinki/provider.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/providers/helsinki/views.py` & `django-helusers-0.9.0/helusers/providers/helsinki/views.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/providers/helsinki_oidc/provider.py` & `django-helusers-0.9.0/helusers/providers/helsinki_oidc/provider.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/providers/helsinki_oidc/views.py` & `django-helusers-0.9.0/helusers/providers/helsinki_oidc/views.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/templates/admin/base_site_default.html` & `django-helusers-0.9.0/helusers/templates/admin/base_site_default.html`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/templates/admin/base_site_grappelli.html` & `django-helusers-0.9.0/helusers/templates/admin/base_site_grappelli.html`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/templates/admin/hel_login.html` & `django-helusers-0.9.0/helusers/templates/admin/hel_login.html`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/tunnistamo_oidc.py` & `django-helusers-0.9.0/helusers/tunnistamo_oidc.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/urls.py` & `django-helusers-0.9.0/helusers/urls.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/user_utils.py` & `django-helusers-0.9.0/helusers/user_utils.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/helusers/views.py` & `django-helusers-0.9.0/helusers/views.py`

 * *Files identical despite different names*

### Comparing `django-helusers-0.8.1/setup.py` & `django-helusers-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-helusers',
-    version='0.8.1',
+    version='0.9.0',
     packages=['helusers'],
     include_package_data=True,
     license='BSD License',
     description='Django app for the user infrastructure of the City of Helsinki',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/City-of-Helsinki/django-helusers',
```

