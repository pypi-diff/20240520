# Comparing `tmp/pyslth-0.4.0.tar.gz` & `tmp/pyslth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.4.0.tar", last modified: Sun May 19 21:09:05 2024, max compression
+gzip compressed data, was "pyslth-0.4.1.tar", last modified: Sun May 19 21:33:45 2024, max compression
```

## Comparing `pyslth-0.4.0.tar` & `pyslth-0.4.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.699151 pyslth-0.4.0/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.0/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 21:09:05.698912 pyslth-0.4.0/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.665763 pyslth-0.4.0/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 21:09:05.000000 pyslth-0.4.0/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.0/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 21:09:05.699212 pyslth-0.4.0/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 21:08:17.000000 pyslth-0.4.0/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.672954 pyslth-0.4.0/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.0/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.4.0/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.673620 pyslth-0.4.0/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.0/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.0/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.4.0/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.0/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.4.0/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.673910 pyslth-0.4.0/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.674588 pyslth-0.4.0/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.0/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.0/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.677395 pyslth-0.4.0/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.0/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.0/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.0/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.0/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.0/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.0/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.0/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.0/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.0/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.0/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.677859 pyslth-0.4.0/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.0/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.0/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.4.0/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.678162 pyslth-0.4.0/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.680299 pyslth-0.4.0/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.0/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.684548 pyslth-0.4.0/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.0/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.0/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.0/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.0/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.0/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.0/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.0/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.687106 pyslth-0.4.0/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.0/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.0/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.0/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.0/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.0/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.697823 pyslth-0.4.0/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.0/slth/static/js/default-passive-events.min.js
--rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.0/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 21:08:37.000000 pyslth-0.4.0/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.0/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.0/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 21:08:37.000000 pyslth-0.4.0/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   102225 2024-05-19 21:08:37.000000 pyslth-0.4.0/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.0/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.0/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:09:05.698467 pyslth-0.4.0/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.4.0/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.0/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.0/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.0/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.0/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.0/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.497803 pyslth-0.4.1/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.1/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 21:33:45.497567 pyslth-0.4.1/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.455262 pyslth-0.4.1/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-19 21:33:45.000000 pyslth-0.4.1/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1904 2024-05-19 21:33:45.000000 pyslth-0.4.1/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-19 21:33:45.000000 pyslth-0.4.1/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-19 21:33:45.000000 pyslth-0.4.1/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-19 21:33:45.000000 pyslth-0.4.1/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.1/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-19 21:33:45.497870 pyslth-0.4.1/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-19 21:33:39.000000 pyslth-0.4.1/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.462252 pyslth-0.4.1/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.1/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9685 2024-05-16 10:19:55.000000 pyslth-0.4.1/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.462926 pyslth-0.4.1/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.1/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.1/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    24698 2024-05-18 09:59:43.000000 pyslth-0.4.1/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.1/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.1/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26476 2024-05-16 10:18:46.000000 pyslth-0.4.1/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.463235 pyslth-0.4.1/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.1/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.463938 pyslth-0.4.1/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.1/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.1/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.1/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.469084 pyslth-0.4.1/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.1/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.1/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.1/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.1/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.1/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.1/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.1/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.1/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.1/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.1/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.1/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.1/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.469654 pyslth-0.4.1/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.1/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.1/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15898 2024-05-13 01:13:17.000000 pyslth-0.4.1/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.470464 pyslth-0.4.1/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.472843 pyslth-0.4.1/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.1/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.1/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.483989 pyslth-0.4.1/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.1/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.1/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.1/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.1/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.1/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.1/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.1/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.1/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.486827 pyslth-0.4.1/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.1/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.1/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.1/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.1/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.1/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.496469 pyslth-0.4.1/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.1/slth/static/js/default-passive-events.min.js
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.1/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-19 21:33:31.000000 pyslth-0.4.1/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.1/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.1/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.1/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.1/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-19 21:33:31.000000 pyslth-0.4.1/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   102258 2024-05-19 21:33:31.000000 pyslth-0.4.1/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.1/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.1/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.1/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-19 21:33:45.497125 pyslth-0.4.1/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3227 2024-05-19 17:16:43.000000 pyslth-0.4.1/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.1/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.1/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.1/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.1/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.1/slth/views.py
```

### Comparing `pyslth-0.4.0/PKG-INFO` & `pyslth-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.4.0
+Version: 0.4.1
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.4.0/pyslth.egg-info/PKG-INFO` & `pyslth-0.4.1/pyslth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.4.0
+Version: 0.4.1
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.4.0/pyslth.egg-info/SOURCES.txt` & `pyslth-0.4.1/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/setup.py` & `pyslth-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.4.0',
+    version='0.4.1',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.4.0/slth/__init__.py` & `pyslth-0.4.1/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/components.py` & `pyslth-0.4.1/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/db/models.py` & `pyslth-0.4.1/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/endpoints.py` & `pyslth-0.4.1/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/factory.py` & `pyslth-0.4.1/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/forms.py` & `pyslth-0.4.1/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/management/commands/integration_test.py` & `pyslth-0.4.1/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/management/commands/sync.py` & `pyslth-0.4.1/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/migrations/0001_initial.py` & `pyslth-0.4.1/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.4.1/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.4.1/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/migrations/0006_user.py` & `pyslth-0.4.1/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/models.py` & `pyslth-0.4.1/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/notifications.py` & `pyslth-0.4.1/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/oauth.py` & `pyslth-0.4.1/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/permissions.py` & `pyslth-0.4.1/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/queryset.py` & `pyslth-0.4.1/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/roles.py` & `pyslth-0.4.1/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/selenium/__init__.py` & `pyslth-0.4.1/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/selenium/browser.py` & `pyslth-0.4.1/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/serializer.py` & `pyslth-0.4.1/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/.DS_Store` & `pyslth-0.4.1/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/fontawesome.min.css` & `pyslth-0.4.1/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/fonts/.DS_Store` & `pyslth-0.4.1/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.4.1/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.4.1/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.4.1/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.4.1/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/slth.css` & `pyslth-0.4.1/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/css/solid.min.css` & `pyslth-0.4.1/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/images/logo.png` & `pyslth-0.4.1/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/images/logo.svg` & `pyslth-0.4.1/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/images/user.png` & `pyslth-0.4.1/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/default-passive-events.min.js` & `pyslth-0.4.1/slth/static/js/default-passive-events.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/echarts.min.js` & `pyslth-0.4.1/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/index.min.js` & `pyslth-0.4.1/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/ios-splash.min.js` & `pyslth-0.4.1/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/peerjs.min.js` & `pyslth-0.4.1/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/qrcode.min.js` & `pyslth-0.4.1/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/react-trigger-change.js` & `pyslth-0.4.1/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/react.min.js` & `pyslth-0.4.1/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/slth.min.js` & `pyslth-0.4.1/slth/static/js/slth.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -141,21 +141,21 @@
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
-function le() {
+function oe() {
     document.querySelectorAll(".message").forEach(function(e) {
         e.remove()
     })
 }
 
-function oe(e) {
+function le(e) {
     function n() {
         const a = {
             color: j.colors.info,
             backgroundColor: j.background.info,
             padding: 20,
             display: "flex",
             justifyContent: "space-between",
@@ -187,42 +187,42 @@
 
 function U(e) {
     return e.replace("/api/", "/app/")
 }
 
 function q(e, n, a, r) {
     const i = localStorage.getItem("token");
-    var l = {
+    var o = {
         Accept: "application/json"
     };
-    i && (l.Authorization = "Token " + i);
+    i && (o.Authorization = "Token " + i);
     const d = A(n);
     var c = {
         method: e,
-        headers: new Headers(l),
+        headers: new Headers(o),
         ajax: 1
     };
     r && (c.body = r);
     var s = null,
         u = null;
-    fetch(d, c).then(function(o) {
-        if (s = o, u = s.headers.get("Content-Type"), u == "application/json") return o.text();
-        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return o.arrayBuffer();
-        o.text()
-    }).then(o => {
+    fetch(d, c).then(function(l) {
+        if (s = l, u = s.headers.get("Content-Type"), u == "application/json") return l.text();
+        if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) return l.arrayBuffer();
+        l.text()
+    }).then(l => {
         if (u == "application/json") {
-            var h = JSON.parse(o || "{}");
+            var h = JSON.parse(l || "{}");
             typeof h == "object" && h.type == "redirect" ? document.location.href = U(h.url) : a && a(h, s)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
-            var g = window.URL.createObjectURL(new Blob([new Uint8Array(o)], {
+            var g = window.URL.createObjectURL(new Blob([new Uint8Array(l)], {
                     type: u
                 })),
                 w = document.createElement("a");
             w.href = g, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, s)
-        } else a && a(o, s)
+        } else a && a(l, s)
     })
 }
 
 function W(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
@@ -240,15 +240,15 @@
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
                 a = n[0],
                 r = n[1];
             return r == "00:00:00" ? a : a + " " + r
         } else if (e.indexOf(`
 `) >= 0) return e.split(`
-`).map(function(i, l) {
+`).map(function(i, o) {
             return t.jsx("div", {
                 children: i
             }, Math.random())
         });
         return e
     }
     return typeof e == "object" && e.type ? t.jsx(x, {
@@ -273,38 +273,38 @@
 }
 
 function de() {
     document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {}))
 }
 
 function pe(e, n) {
-    le(), de(), window.reloader = n;
+    oe(), de(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
     H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
         url: A(e)
     }))
 }
 
 function Ae(e) {
-    le(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
+    oe(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Fe, {
         url: A(e)
     }))
 }
 
 function Y(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
 function Re(e) {
-    le(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
+    oe(), de(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(ze, {
         actions: e
     }))
 }
 
 function Oe(e) {
     const n = {
         backgroundColor: "black",
@@ -324,18 +324,18 @@
         style: n
     })
 }
 
 function _e(e) {
     const [n, a] = B.useState(null), [r, i] = B.useState(0);
     B.useEffect(() => {
-        l(A(e.url)), document.querySelector(".layer").style.display = "block"
+        o(A(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
-    function l(s) {
+    function o(s) {
         q("GET", A(s), function(u) {
             a(u), i(r + 1)
         })
     }
 
     function d() {
         const s = {
@@ -418,38 +418,38 @@
 function ze(e) {
     const n = Math.random();
     B.useEffect(() => {
         document.querySelector(".layer").style.display = "block"
     }, []);
 
     function a() {
-        const l = {
+        const o = {
             width: "100%",
             borderBottom: "solid 1px #DDDD",
             padding: 20
         };
         return t.jsx("div", {
             align: "center",
             style: {},
             children: e.actions.map(function(d) {
                 return t.jsx("div", {
-                    style: l,
+                    style: o,
                     onClick: r,
                     children: t.jsx(_, {
                         data: d,
                         strech: !0
                     })
                 }, Math.random())
             })
         })
     }
 
     function r() {
-        const l = document.getElementById(n);
-        l.close(), l.classList.remove("opened"), l.remove(), document.querySelector(".layer").style.display = "none"
+        const o = document.getElementById(n);
+        o.close(), o.classList.remove("opened"), o.remove(), document.querySelector(".layer").style.display = "none"
     }
     const i = {
         width: "auto",
         display: "block",
         position: "fixed",
         bottom: 0,
         border: 0,
@@ -472,15 +472,15 @@
 
     function i(c) {
         c.preventDefault();
         var s = e.data.url;
         e.data.urlfunc && (s = e.data.urlfunc()), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(U(s)) : pe(s)
     }
 
-    function l() {
+    function o() {
         return e.strech ? e.data.name : e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(S, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
@@ -503,42 +503,42 @@
             c[s] = e.style[s]
         }), t.jsx("a", {
             id: n,
             href: U(e.data.url) || "#",
             onClick: i,
             style: c,
             "data-label": E(e.data.name),
-            children: l()
+            children: o()
         })
     }
     return d()
 }
 
 function Z(e) {
-    function n(l) {
-        var d = l.target.parentNode.querySelector(".dropdown");
-        return d == null && (d = l.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = l.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
+    function n(o) {
+        var d = o.target.parentNode.querySelector(".dropdown");
+        return d == null && (d = o.target.parentNode.parentNode.querySelector(".dropdown")), d == null && (d = o.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), d
     }
 
-    function a(l) {
-        const d = n(l);
+    function a(o) {
+        const d = n(o);
         if (d.style.display == "block") d.style.display = "none";
         else {
-            const c = l.target.getBoundingClientRect();
+            const c = o.target.getBoundingClientRect();
             document.querySelectorAll(".dropdown").forEach(s => s.style.display = "none"), d.style.left = c.left - 150 + c.width + "px", d.style.display = "block"
         }
     }
 
-    function r(l) {
-        const d = n(l);
+    function r(o) {
+        const d = n(o);
         d.style.display = "none"
     }
 
     function i() {
-        const l = {
+        const o = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
                 boxShadow: "15px 15px 10px -15px #DDD",
@@ -553,15 +553,15 @@
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
                 "data-label": E(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
-                style: l,
+                style: o,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(c => t.jsx("li", {
                     style: d,
                     children: t.jsx(_, {
                         data: c,
                         style: {
@@ -577,35 +577,35 @@
 
 function O({
     id: e,
     href: n,
     modal: a,
     imodal: r,
     children: i,
-    onClick: l,
+    onClick: o,
     dataLabel: d,
     style: c
 }) {
     const s = n && n.indexOf("/media/") < 0 ? U(n) : n;
 
     function u(h) {
         s.indexOf("http") == 0 ? document.location.href = s : (h.preventDefault(), a ? pe(s) : r ? Ae(s) : window.load(s))
     }
 
-    function o() {
+    function l() {
         return t.jsx("a", {
             id: e,
-            onClick: l || u,
+            onClick: o || u,
             href: s || "#",
             "data-label": E(d),
             style: c,
             children: i
         })
     }
-    return o()
+    return l()
 }
 
 function P(e) {
     function n() {
         const r = {
             display: "grid",
             gridGap: 0,
@@ -684,25 +684,25 @@
 
     function i(d) {
         q("GET", d, function(c) {
             r(c)
         })
     }
 
-    function l() {
+    function o() {
         return window[n] = () => i(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
             children: t.jsx(je, {
                 data: a,
                 width: 100
             })
         })
     }
-    return l()
+    return o()
 }
 
 function se(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 verticalAlign: "center",
@@ -741,20 +741,20 @@
         })
     }
     return n()
 }
 
 function He(e) {
     function n() {
-        const l = {
+        const o = {
             marginTop: 5,
             marginBottom: 5
         };
         return t.jsx("h3", {
-            style: l,
+            style: o,
             children: e.data.title
         })
     }
 
     function a() {
         return t.jsx(ce, {
             data: e.data.data
@@ -764,21 +764,21 @@
     function r() {
         return t.jsx(se, {
             data: e.data.actions
         })
     }
 
     function i() {
-        const l = {
+        const o = {
             border: "solid 1px #DDD",
             padding: 10,
             borderStyle: "dashed"
         };
         return t.jsxs("div", {
-            style: l,
+            style: o,
             children: [n(), a(), r()]
         })
     }
     return i()
 }
 
 function Pe(e) {
@@ -883,15 +883,15 @@
 
     function i() {
         return t.jsx(se, {
             data: e.data.actions
         })
     }
 
-    function l() {
+    function o() {
         const d = {
                 borderBottom: "solid 1px #DDD",
                 padding: 0,
                 borderBottomStyle: "dashed",
                 marginLeft: 140,
                 borderLeft: "3px solid #1151b3",
                 marginBottom: -10
@@ -903,15 +903,15 @@
             style: d,
             children: [r(), t.jsxs("div", {
                 style: c,
                 children: [n(), a(), i()]
             })]
         })
     }
-    return l()
+    return o()
 }
 
 function Ge(e) {
     const n = Math.random(),
         [a, r] = B.useState(e.data);
     F(`
     .object-fieldset{
@@ -921,15 +921,15 @@
 
     function i() {
         return t.jsx(ke, {
             data: a
         })
     }
 
-    function l() {
+    function o() {
         const u = {
             backgroundColor: "white",
             padding: 15,
             marginBottom: 15
         };
         return t.jsx("div", {
             style: u,
@@ -939,65 +939,65 @@
 
     function d() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
             children: "Nenhum registro encontrado."
         }) : a.data.map(function(u) {
             return Array.isArray(u) ? t.jsx(P, {
                 width: 300,
-                children: u.map(o => t.jsx(X, {
-                    data: o,
+                children: u.map(l => t.jsx(X, {
+                    data: l,
                     width: 100 / u.length
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
                 children: t.jsx(X, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
         }) : t.jsx(x, {
             data: a.data
         })
     }
 
     function c(u) {
-        q("GET", u, function(o) {
-            r(o)
+        q("GET", u, function(l) {
+            r(l)
         })
     }
 
     function s() {
         return e.data.url ? (window[n] = () => c(e.data.url), t.jsxs("div", {
             className: e.data.url ? "reloadable object-fieldset" : "object-fieldset",
             id: n,
-            children: [i(), l()]
+            children: [i(), o()]
         })) : t.jsxs("div", {
             className: "object-fieldset",
-            children: [i(), l()]
+            children: [i(), o()]
         })
     }
     return s()
 }
 
 function Ye(e) {
     const n = Math.random(),
         [a, r] = B.useState(e.data.actions);
 
     function i() {
         const c = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + c + "only=actions"
     }
 
-    function l() {
+    function o() {
         q("GET", i(), function(c) {
             r(c)
         })
     }
 
     function d() {
-        return window[n] = () => l(), t.jsx("div", {
+        return window[n] = () => o(), t.jsx("div", {
             className: "reloadable",
             id: n,
             children: a.map(function(c) {
                 return t.jsx(_, {
                     data: c,
                     default: !0
                 }, Math.random())
@@ -1075,15 +1075,15 @@
     function n() {
         return t.jsx(Xe, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(i, l) {
+        return e.data.data.map(function(i, o) {
             return t.jsx(x, {
                 data: i
             }, Math.random())
         })
     }
 
     function r() {
@@ -1102,19 +1102,19 @@
         })
     }
 
     function a() {
         const i = {
             backgroundColor: "white"
         };
-        return e.data.data.map(function(l, d) {
+        return e.data.data.map(function(o, d) {
             return t.jsx("div", {
                 style: i,
                 children: t.jsx(x, {
-                    data: l
+                    data: o
                 }, Math.random())
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
@@ -1143,27 +1143,27 @@
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20,
                 overflowX: "auto"
             },
-            children: e.data.map(function(i, l) {
+            children: e.data.map(function(i, o) {
                 return t.jsx(O, {
                     href: i.url,
                     style: {
                         padding: 5,
-                        fontWeight: n == l ? "bold" : "normal",
-                        borderBottom: n == l ? "solid 3px #2670e8" : "solid 3px inherite",
+                        fontWeight: n == o ? "bold" : "normal",
+                        borderBottom: n == o ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(d) {
-                        d.preventDefault(), a(l), e.loadContent(i.url)
+                        d.preventDefault(), a(o), e.loadContent(i.url)
                     },
                     dataLabel: E(i.title),
                     children: i.title
                 }, Math.random())
             })
         })
     }
@@ -1177,61 +1177,61 @@
     function i() {
         return e.data.title != "Top" && t.jsx("h2", {
             "data-label": E(e.data.title),
             children: e.data.title
         })
     }
 
-    function l() {
+    function o() {
         return t.jsx(Je, {
             data: e.data.data,
             loadContent: s
         })
     }
 
     function d() {
-        var o = {
+        var l = {
             ...a
         };
-        o.title = null;
+        l.title = null;
         const h = {
             padding: 0
         };
         return t.jsx("div", {
             style: h,
             children: t.jsx(x, {
-                data: o
+                data: l
             }, Math.random())
         })
     }
 
     function c() {
-        const o = {
+        const l = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
-            style: o
+            style: l
         })
     }
 
-    function s(o) {
-        q("GET", o, function(h) {
+    function s(l) {
+        q("GET", l, function(h) {
             r(h)
         })
     }
 
     function u() {
         return window[n] = () => s(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [i(), l(), d(), c()]
+            children: [i(), o(), d(), c()]
         })
     }
     return u()
 }
 
 function Ke() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
@@ -1241,15 +1241,15 @@
 
 function R({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: i,
-    primary: l,
+    primary: o,
     compact: d,
     spin: c
 }) {
     function s() {
         return a ? d || !r ? t.jsx(S, {
             icon: a
         }) : t.jsxs(t.Fragment, {
@@ -1264,28 +1264,28 @@
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
 
     function u() {
-        const o = {
+        const l = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
             display: i || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
-        return l ? (o.backgroundColor = j.colors.primary, o.color = "white") : (o.border = "solid 1px " + j.colors.primary, o.color = j.colors.primary), t.jsx("a", {
+        return o ? (l.backgroundColor = j.colors.primary, l.color = "white") : (l.border = "solid 1px " + j.colors.primary, l.color = j.colors.primary), t.jsx("a", {
             id: e,
-            style: o,
+            style: l,
             "data-label": E(r || a),
             onClick: h => {
                 h.preventDefault(), a && c && (h.target.dataset.spinning = a, h.target.querySelector("i.fa-spin").style.display = "inline-block", h.target.querySelector("i.fa-" + a).style.display = "none"), n(h)
             },
             children: s()
         })
     }
@@ -1329,55 +1329,55 @@
         scrolling: "no",
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
 function nt(e) {
-    function n(l) {
-        return e.data.icon ? l.done ? t.jsx(S, {
+    function n(o) {
+        return e.data.icon ? o.done ? t.jsx(S, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
             style: {
                 marginTop: 6
             },
-            children: l.number
+            children: o.number
         })
     }
 
-    function a(l) {
+    function a(o) {
         return {
             border: "3px solid " + j.colors.primary,
             borderRadius: "50%",
-            background: l.done ? j.colors.primary : "white",
-            color: l.done ? "white" : j.colors.primary,
+            background: o.done ? j.colors.primary : "white",
+            color: o.done ? "white" : j.colors.primary,
             textAlign: "center",
             width: 50,
             height: 50,
             margin: "auto",
             fontSize: "1.5rem"
         }
     }
 
-    function r(l) {
+    function r(o) {
         return {
             listStyleType: "none",
             display: "flex",
             justifyContent: "center",
-            minWidth: l.length * 100
+            minWidth: o.length * 100
         }
     }
 
     function i() {
-        const l = {
+        const o = {
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
             },
@@ -1391,15 +1391,15 @@
                 borderBottom: "2px solid #1151b3",
                 top: -28,
                 width: 45,
                 left: 77
             };
         return t.jsx("div", {
             children: t.jsx("div", {
-                style: l,
+                style: o,
                 children: t.jsx("ul", {
                     style: r(e.data.steps),
                     children: e.data.steps.map((s, u) => t.jsxs("li", {
                         style: d,
                         children: [t.jsx("div", {
                             style: a(s),
                             children: n(s)
@@ -1507,15 +1507,15 @@
                 textDecoration: "none"
             },
             i = {
                 marginTop: 30,
                 fontSize: "3rem",
                 color: j.colors.auxiliary
             },
-            l = {
+            o = {
                 marginTop: 40,
                 fontWeight: "bold",
                 fontSize: "1.2rem",
                 textTransform: "uppercase",
                 height: 70,
                 color: j.colors.primary
             };
@@ -1534,25 +1534,25 @@
                     dataLabel: d.label,
                     children: [t.jsx("div", {
                         children: t.jsx(S, {
                             style: i,
                             icon: d.icon
                         })
                     }), t.jsx("div", {
-                        style: l,
+                        style: o,
                         children: d.label
                     })]
                 }, Math.random()))
             })]
         }) : null
     }
     return n()
 }
 
-function lt(e) {
+function ot(e) {
     function n() {
         return t.jsx("div", {
             style: {
                 backgroundColor: "black",
                 color: "white",
                 padding: "10px",
                 minHeight: "300px",
@@ -1564,15 +1564,15 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function ot(e) {
+function lt(e) {
     function n() {
         return e.data.url ? t.jsx(O, {
             href: e.data.url,
             imodal: !!e.data.modal,
             children: e.data.icon ? t.jsx(S, {
                 icon: e.data.icon
             }) : e.data.url
@@ -1642,30 +1642,30 @@
             className: "indicators",
             style: a,
             children: [t.jsx("h1", {
                 "data-label": E(e.data.title),
                 children: e.data.title
             }), t.jsx(P, {
                 width: 300,
-                children: e.data.items.map(l => t.jsxs("div", {
+                children: e.data.items.map(o => t.jsxs("div", {
                     children: [t.jsx("div", {
                         style: r,
-                        children: W(l.value)
+                        children: W(o.value)
                     }), t.jsx("div", {
                         style: i,
-                        children: l.name
+                        children: o.name
                     })]
                 }, Math.random()))
             }, Math.random()), t.jsx("div", {
                 className: "actions",
-                children: e.data.actions.map(l => t.jsx(O, {
-                    href: A(l.url),
-                    label: l.label,
-                    modal: l.modal,
-                    children: l.label
+                children: e.data.actions.map(o => t.jsx(O, {
+                    href: A(o.url),
+                    label: o.label,
+                    modal: o.modal,
+                    children: o.label
                 }, Math.random()))
             })]
         })
     }
     return n()
 }
 
@@ -1703,35 +1703,35 @@
 }
 
 function Ce(e) {
     const n = Math.random();
     var a = !1;
     const r = "rgb(219, 237, 255)",
         i = "rgb(89, 154, 242)",
-        l = "rgb(246, 123, 135)",
+        o = "rgb(246, 123, 135)",
         d = [],
         c = [];
 
     function s(y) {
-        return e.data.readonly ? y == null ? r : i : y == null ? r : y.text == null ? i : l
+        return e.data.readonly ? y == null ? r : i : y == null ? r : y.text == null ? i : o
     }
 
     function u(y) {
         a = !0, y.preventDefault()
     }
 
-    function o(y) {
+    function l(y) {
         a = !1, document.getElementById("input" + n).value = JSON.stringify({
             select: d,
             deselect: c
         })
     }
 
     function h(y) {
-        e.data.readonly || e.data.single_selection && g().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != l && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
+        e.data.readonly || e.data.single_selection && g().length > 0 && y.target.style.backgroundColor != i || a && y.target.style.backgroundColor != o && (y.target.style.backgroundColor == r ? (y.target.style.backgroundColor = i, console.log("MARCOU", y.target.dataset.day, y.target.dataset.time), d.push([y.target.dataset.day, y.target.dataset.time])) : (y.target.style.backgroundColor = r, console.log("DEMARCOU", y.target.dataset.day, y.target.dataset.time), c.push([y.target.dataset.day, y.target.dataset.time])))
     }
 
     function g() {
         const y = [];
         return document.getElementById(n).querySelectorAll("td").forEach(function(I) {
             I.style.backgroundColor == i && y.push(I.dataset.day, I.dataset.time)
         }), y
@@ -1757,15 +1757,15 @@
             children: [t.jsx("input", {
                 id: "input" + n,
                 type: "hidden",
                 name: e.data.input_name
             }), t.jsxs("table", {
                 style: I,
                 onMouseDown: u,
-                onMouseUp: o,
+                onMouseUp: l,
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: e.data.matrix[0].map(function(k) {
                             return t.jsx("th", {
                                 className: "bold",
                                 style: m,
                                 children: k.text
@@ -2065,15 +2065,15 @@
         return t.jsx("div", {
             children: t.jsx(pt, {
                 id: e.data.name + "_error"
             })
         })
     }
 
-    function l() {
+    function o() {
         return e.data.help_text && t.jsx(jt, {
             text: e.data.help_text
         })
     }
 
     function d() {
         const c = {
@@ -2081,28 +2081,28 @@
             flexDirection: "column",
             padding: 5,
             width: "calc(100%-5px)"
         };
         return t.jsxs("div", {
             id: n,
             style: c,
-            children: [a(), r(), l(), i()]
+            children: [a(), r(), o(), i()]
         })
     }
     return d()
 }
 
 function ye(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), B.useEffect(() => {
-        function d(u, o, h) {
+        function d(u, l, h) {
             var g = h.target,
                 w = g.value.replace(/\D/g, ""),
-                y = g.value.length > o ? 1 : 0;
+                y = g.value.length > l ? 1 : 0;
             VMasker(g).unMask(), VMasker(g).maskPattern(u[y]), g.value = VMasker.toPattern(w, u[y])
         }
         if (e.data.mask) {
             var c = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
@@ -2122,49 +2122,49 @@
     function i(d) {
         if (e.data.type == "file" && d.target.files) {
             let s = d.target.files[0];
             var c = new FileReader;
             c.onload = function(u) {
                 if (re(s.name)) {
                     const w = "display" + a;
-                    var o = document.createElement("img");
-                    o.id = d.target.id + "img", o.style.width = "200px", o.style.display = "block", o.style.margin = "auto", o.style.marginTop = "20px", o.onload = function(y) {
-                        const I = e.data.width > e.data.height ? e.data.width / o.width : e.data.height / o.height;
+                    var l = document.createElement("img");
+                    l.id = d.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(y) {
+                        const I = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
                         var m = document.createElement("canvas");
                         const k = m.getContext("2d");
-                        m.height = m.width * (o.height / o.width);
+                        m.height = m.width * (l.height / l.width);
                         const v = document.createElement("canvas"),
                             D = v.getContext("2d");
-                        v.width = o.width * I, v.height = o.height * I, D.drawImage(o, 0, 0, v.width, v.height), k.drawImage(v, 0, 0, v.width * I, v.height * I, 0, 0, m.width, m.height), v.toBlob(function(C) {
+                        v.width = l.width * I, v.height = l.height * I, D.drawImage(l, 0, 0, v.width, v.height), k.drawImage(v, 0, 0, v.width * I, v.height * I, 0, 0, m.width, m.height), v.toBlob(function(C) {
                             const T = new DataTransfer;
                             T.items.add(new File([C], s.name)), d.target.files = T.files
                         });
                         var b = document.getElementById(w);
-                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(o), d.target.parentNode.appendChild(b)
-                    }, o.src = u.target.result
+                        b == null ? (b = document.createElement("div"), b.id = w) : b.removeChild(b.childNodes[0]), b.appendChild(l), d.target.parentNode.appendChild(b)
+                    }, l.src = u.target.result
                 }
                 const h = document.getElementById("fileinfo" + a);
                 var g = s.size / 1024;
                 g < 1024 ? g = parseInt(g) + " Kb" : g = (g / 1024).toFixed(2) + " Mb", h.innerHTML = s.name + " / " + g, e.data.max_size && s.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + g + ". Por favor, adicione um arquivo menor.")
             }, c.readAsDataURL(s)
         }
     }
 
-    function l() {
+    function o() {
         var d = e.data.type;
         if (d == "datetime" && (d = "datetime-regional"), d == "decimal" && (d = "text"), d == "file") {
             const u = {
                 alignContent: "center",
                 minHeight: 75,
                 padding: 5,
                 maxWidth: "100%",
                 margin: "auto"
             };
             var c = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (c = e.data.extensions.map(o => "." + o).join(", ")), t.jsxs(t.Fragment, {
+            return e.data.extensions && e.data.extensions.length > 0 && (c = e.data.extensions.map(l => "." + l).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
                         display: window.innerWidth < 800 ? "block" : "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
@@ -2193,15 +2193,15 @@
                             style: {
                                 textAlign: "center"
                             },
                             children: e.data.value
                         }), "Selecione um arquivo clicando no botão ao lado.", t.jsxs("div", {
                             className: "bold",
                             id: "fileinfo" + a,
-                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(o => "." + o).join(" ou "), "."]
+                            children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
                         children: t.jsx(R, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
@@ -2237,15 +2237,15 @@
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: i,
                 style: s
             })
         }
     }
-    return l()
+    return o()
 }
 
 function Me(e) {
     var n = [];
     Array.isArray(e.data.value) ? e.data.value.forEach(function(b, C) {
         n.push({
             id: b.id,
@@ -2254,18 +2254,18 @@
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
         i = Array.isArray(e.data.value),
-        [l, d] = B.useState(!1),
+        [o, d] = B.useState(!1),
         [c, s] = B.useState(null);
     var u = !1;
-    let o;
+    let l;
     B.useEffect(() => {
         k(n, !0), document.getElementById(a).addEventListener("customchange", function(b) {
             k(b.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function h() {
@@ -2375,15 +2375,15 @@
                 },
                 onChange: m,
                 onMouseLeave: y,
                 onBlur: y,
                 defaultValue: L,
                 style: b,
                 "data-label": E(e.data.label)
-            }), c && l && t.jsxs("ul", {
+            }), c && o && t.jsxs("ul", {
                 style: C,
                 onMouseLeave: I,
                 onMouseEnter: function(N) {
                     u = !0
                 },
                 children: [c.length == 0 && t.jsx("li", {
                     style: M,
@@ -2412,15 +2412,15 @@
         if (C) {
             const T = document.getElementById(r);
             i || C.options.length > 0 && T.value != C.options[0].innerHTML && (C.innerHTML = "", T.value = "", d(!1), e.data.onchange && $(T, e.data.onchange)), b.target.tagName == "UL" ? d(!1) : u || d(!1)
         }
     }
 
     function m(b) {
-        clearTimeout(o), o = setTimeout(function() {
+        clearTimeout(l), l = setTimeout(function() {
             const C = b.target.closest("form"),
                 T = e.data.choices.indexOf("?") < 0 ? "?" : "&";
             d(!0), q("GET", J(e.data.choices + T + "term=" + b.target.value, C), function(p) {
                 s(p)
             })
         }, 1e3)
     }
@@ -2476,60 +2476,60 @@
 }
 
 function ie(e) {
     const [n, a] = B.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
-    function l(u) {
+    function o(u) {
         return i.value != null ? i.value == u.id ? !0 : i.value.id == u.id : !1
     }
 
     function d(u) {
-        var o = document.getElementById(u);
-        i.checked && (o.checked = !1), e.data.onchange && $(o, e.data.onchange)
+        var l = document.getElementById(u);
+        i.checked && (l.checked = !1), e.data.onchange && $(l, e.data.onchange)
     }
 
     function c(u) {
-        var o = document.getElementById(u);
-        i.checked = o.checked
+        var l = document.getElementById(u);
+        i.checked = l.checked
     }
 
     function s() {
         return window["reload-" + i.name + "-field"] = function() {
-            q("GET", J(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(o) {
-                a(o)
+            q("GET", J(e.data.pick, document.querySelector(".radio-group." + i.name).closest("form")), function(l) {
+                a(l)
             })
         }, n.length > 0 ? t.jsx("div", {
             className: "radio-group " + i.name,
-            children: n.map((u, o) => (u.id || u.id === !1) && t.jsxs("div", {
+            children: n.map((u, l) => (u.id || u.id === !1) && t.jsxs("div", {
                 style: {
                     paddingTop: 10,
                     display: "inline-block",
                     marginRight: 25,
                     width: window.innerWidth > 800 ? "auto" : "100%"
                 },
                 children: [t.jsx("input", {
-                    id: i.name + r + o,
+                    id: i.name + r + l,
                     type: "radio",
                     name: i.name,
                     defaultValue: u.id,
-                    defaultChecked: l(u),
+                    defaultChecked: o(u),
                     "data-label": E(u.value),
                     onClick: function() {
-                        d(i.name + r + o)
+                        d(i.name + r + l)
                     },
                     onMouseEnter: function() {
-                        c(i.name + r + o)
+                        c(i.name + r + l)
                     }
                 }), t.jsx("label", {
-                    htmlFor: i.name + r + o,
+                    htmlFor: i.name + r + l,
                     children: u.value
                 })]
-            }, r + o))
+            }, r + l))
         }) : t.jsx("div", {
             className: "radio-group " + i.name,
             children: t.jsx("i", {
                 children: "Nenhuma opção disponível para seleção."
             })
         })
     }
@@ -2537,19 +2537,19 @@
 }
 
 function ve(e) {
     const [n, a] = B.useState(e.data.choices);
     var r = Math.random(),
         i = e.data;
 
-    function l(s) {
+    function o(s) {
         var u = !1;
         if (i.value)
-            for (var o = 0; o < i.value.length; o++) {
-                var h = i.value[o];
+            for (var l = 0; l < i.value.length; l++) {
+                var h = i.value[l];
                 (h == s.id || h.id == s.id) && (u = !0)
             }
         return u
     }
 
     function d(s) {
         e.data.onchange && $(s.target, e.data.onchange)
@@ -2571,15 +2571,15 @@
                 },
                 children: [t.jsx("input", {
                     id: i.name + r + u,
                     type: "checkbox",
                     name: i.name,
                     onClick: d,
                     defaultValue: s.id,
-                    defaultChecked: l(s),
+                    defaultChecked: o(s),
                     "data-label": E(s.value)
                 }), t.jsx("label", {
                     htmlFor: i.name + r + u,
                     children: s.value
                 })]
             }, r + u))
         }) : t.jsx("div", {
@@ -2614,41 +2614,41 @@
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
     function i() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
-            children: t.jsxs(oe, {
+            children: t.jsxs(le, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "pen-clip",
-                    onClick: () => l(!0),
+                    onClick: () => o(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
-                    onClick: () => l(!1),
+                    onClick: () => o(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
         })
     }
 
-    function l(s) {
+    function o(s) {
         const u = document.querySelector("input[name=" + r.name + "]"),
-            o = document.getElementById("inline-form-" + n),
+            l = document.getElementById("inline-form-" + n),
             h = document.getElementById("show-" + n),
             g = document.getElementById("hide-" + n);
-        o.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", g.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
+        l.style.display = s ? "block" : "none", h.style.display = s ? "none" : "inline", g.style.display = s ? "inline" : "none", s ? u.value === "" ? u.value = 0 : u.value = -parseInt(u.value) : parseInt(u.value) == 0 ? u.value = "" : u.value = -parseInt(u.value)
     }
 
     function d() {
         const s = {
             display: r.value ? "block" : "none"
         };
         return e.data.required && (s.display = "block", r.value === "" && (r.value = 0)), t.jsx("div", {
@@ -2680,111 +2680,111 @@
 }
 
 function Mt(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
-    function r(o, h) {
+    function r(l, h) {
         const g = n;
         return n += 1, t.jsxs("div", {
             style: {
                 display: "block"
             },
             id: "form-" + g + "-" + a,
             children: [t.jsx(ue, {
-                data: o
+                data: l
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
                 children: [t.jsx(R, {
                     primary: !0,
                     icon: "plus",
-                    onClick: () => l(),
+                    onClick: () => o(),
                     id: "extra-add-" + g + "-",
                     display: h
                 }), t.jsx(R, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => d(g),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function i() {
-        const o = c(),
-            h = o.length > 0 ? "none" : "inline";
+        const l = c(),
+            h = l.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = h;
         for (var g = 0; g < n; g++) {
             var w = document.getElementById("extra-add-" + g + "-");
             w.style.display = "none"
         }
-        if (o.length > 0) {
-            var w = document.getElementById("extra-add-" + o[o.length - 1] + "-");
+        if (l.length > 0) {
+            var w = document.getElementById("extra-add-" + l[l.length - 1] + "-");
             w.style.display = "inline"
         }
     }
 
-    function l() {
+    function o() {
         i();
-        var o = JSON.parse(JSON.stringify(e.data.template));
-        o.fields ? (o.fields.map(function(h) {
+        var l = JSON.parse(JSON.stringify(e.data.template));
+        l.fields ? (l.fields.map(function(h) {
             h.name = h.name.replace("__n__", "__" + n + "__")
-        }), o.fields[0].value = 0) : o.fieldsets.map(function(h) {
+        }), l.fields[0].value = 0) : l.fieldsets.map(function(h) {
             h.fields.map(function(g) {
                 g.map(function(w) {
                     w.name = w.name.replace("__n__", "__" + n + "__")
                 }), g[0].value = 0
             })
-        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(o, "inline")), setTimeout(i, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(i, 100)
     }
 
-    function d(o) {
+    function d(l) {
         const h = e.data.template,
-            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + o + "__"),
+            w = (h.fields ? h.fields[0] : h.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
             y = document.querySelector("input[name=" + w + "]");
-        parseInt(y.value) == 0 ? y.value = "" : y.value = -parseInt(y.value), document.getElementById("form-" + o + "-" + a).style.display = "none", i()
+        parseInt(y.value) == 0 ? y.value = "" : y.value = -parseInt(y.value), document.getElementById("form-" + l + "-" + a).style.display = "none", i()
     }
 
     function c() {
-        for (var o = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && o.push(h);
-        return o
+        for (var l = [], h = 0; h < n; h++) document.getElementById("form-" + h + "-" + a).style.display == "block" && l.push(h);
+        return l
     }
 
     function s() {
         return t.jsx("div", {
             id: "info-" + a,
-            children: t.jsx(oe, {
+            children: t.jsx(le, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
                 children: t.jsx(R, {
                     primary: !0,
                     icon: "add",
-                    onClick: () => l(),
+                    onClick: () => o(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
         })
     }
 
     function u() {
-        const o = {
+        const l = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
-                style: o,
+                style: l,
                 "data-label": E(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
@@ -2822,21 +2822,21 @@
                 children: [t.jsx("h2", {
                     "data-label": E(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), r.fields.map(i => t.jsx("div", {
-                    children: i.map(l => t.jsx("div", {
-                        className: "form-group " + l.name,
+                    children: i.map(o => t.jsx("div", {
+                        className: "form-group " + o.name,
                         style: {
                             width: 100 / i.length + "%",
-                            display: l.type == "hidden" ? "none" : "inline-block"
+                            display: o.type == "hidden" ? "none" : "inline-block"
                         },
-                        children: n(l)
+                        children: n(o)
                     }, Math.random()))
                 }, Math.random()))]
             })
         }, Math.random()))
     }
     return a()
 }
@@ -2871,15 +2871,15 @@
                 style: {
                     marginTop: 30
                 }
             })]
         })
     }
 
-    function l() {
+    function o() {
         return t.jsx(ue, {
             data: e.data
         })
     }
 
     function d() {
         return t.jsxs("div", {
@@ -2889,15 +2889,15 @@
             },
             children: [t.jsx(R, {
                 onClick: u,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
             }), t.jsx(R, {
-                onClick: o,
+                onClick: l,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
@@ -2924,24 +2924,24 @@
             method: e.data.method,
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 5
                 },
-                children: [a(), r(), i(), l(), d(), c()]
+                children: [a(), r(), i(), o(), d(), c()]
             })]
         })
     }
 
     function u() {
         Y()
     }
 
-    function o(h) {
+    function l(h) {
         h.preventDefault();
         var g = e.data.url,
             w = document.getElementById(n),
             y = new FormData(w);
         if (w.method.toUpperCase() == "GET") {
             const I = g.indexOf("?") >= 0 ? "&" : "?";
             g = g + I + "form=" + e.data.title + "&" + new URLSearchParams(y).toString(), y = null
@@ -3016,24 +3016,24 @@
             margin: 0px;
         }       
     `);
     const n = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
         a = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
         r = new Date,
         i = e.data.day ? new Date(e.data.year, e.data.month - 1, e.data.day) : null;
-    for (var l = [
+    for (var o = [
             [],
             [],
             [],
             [],
             [],
             []
         ], d = e.data.month - 1, c = new Date(e.data.year, e.data.month - 1, 1); c.getDay() > 1;) c.setDate(c.getDate() - 1);
     for (var s = 0;
-        (c.getMonth() <= d || l[s].length < 7) && (l[s].length == 7 && (s += 1), s != 5);) l[s].push({
+        (c.getMonth() <= d || o[s].length < 7) && (o[s].length == 7 && (s += 1), s != 5);) o[s].push({
         date: c.getDate(),
         total: e.data.total[c.toLocaleDateString("pt-BR")],
         today: c.getDate() === r.getDate(),
         selected: i ? c.getDate() == i.getDate() : !1
     }), c.setDate(c.getDate() + 1);
 
     function u() {
@@ -3070,21 +3070,21 @@
                         icon: "arrow-right",
                         onClick: () => e.onChange(null, e.data.next.month, e.data.next.year)
                     })
                 })]
             }), t.jsxs("table", {
                 children: [t.jsx("thead", {
                     children: t.jsx("tr", {
-                        children: n.map(o => t.jsx("th", {
-                            children: o
+                        children: n.map(l => t.jsx("th", {
+                            children: l
                         }, Math.random()))
                     })
                 }), t.jsx("tbody", {
-                    children: l.map(o => t.jsx("tr", {
-                        children: o.map(h => t.jsxs("td", {
+                    children: o.map(l => t.jsx("tr", {
+                        children: l.map(h => t.jsxs("td", {
                             children: [t.jsx("div", {
                                 className: "day",
                                 children: h.today ? t.jsx("span", {
                                     style: {
                                         textDecoration: "underline"
                                     },
                                     children: h.date
@@ -3271,15 +3271,15 @@
             children: [r(), t.jsx("i", {
                 id: "loader-" + e.data.id,
                 className: "fa-solid fa-circle-notch fa-spin fa-1x"
             })]
         })
     }
 
-    function l(f) {
+    function o(f) {
         document.getElementById("loader-" + e.data.id).style.display = f ? "block" : "none"
     }
 
     function d() {
         return n.subsets && t.jsx("div", {
             className: "tabs",
             children: n.subsets.map(function(f, p) {
@@ -3315,15 +3315,15 @@
     function u() {
         if (n.calendar) return t.jsx(It, {
             data: n.calendar,
             onChange: s
         })
     }
 
-    function o(f) {
+    function l(f) {
         const p = {
             textAlign: "left",
             verticalAlign: "top",
             lineHeight: "1.2rem",
             color: j.colors.primary,
             padding: 5
         };
@@ -3410,15 +3410,15 @@
                 marginBottom: 15
             },
             children: n.data.map(function(f) {
                 return f.type = n.renderer, t.jsx(x, {
                     data: f
                 }, Math.random())
             })
-        }) : w()) : t.jsx(oe, {
+        }) : w()) : t.jsx(le, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function w() {
@@ -3432,15 +3432,15 @@
                 borderSpacing: 0
             };
         return t.jsx("div", {
             style: f,
             children: t.jsxs("table", {
                 style: p,
                 children: [t.jsx("thead", {
-                    children: o(n.data[0].data)
+                    children: l(n.data[0].data)
                 }), t.jsx("tbody", {
                     children: n.data.map(function(M) {
                         return h(M)
                     })
                 })]
             })
         })
@@ -3534,19 +3534,19 @@
                     }, Math.random())
                 })]
             })
         }
     }
 
     function D() {
-        l(!0);
+        o(!0);
         var f;
         const p = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
         e.data.url.indexOf("?") > 0 ? f = e.data.url + "&" + p : f = e.data.url + "?" + p, q("GET", f, function(M) {
-            a(M), l(!1)
+            a(M), o(!1)
         })
     }
 
     function b() {
         const f = {
             color: j.colors.primary
         };
@@ -3639,33 +3639,33 @@
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(i, l) {
+        return e.headers ? e.headers.slice(1).map(function(i, o) {
             return {
                 name: i,
                 type: "pie",
-                radius: n[l],
+                radius: n[o],
                 emphasis: {
                     label: {
                         show: !0,
                         formatter: function(d) {
                             return d.value.toLocaleString("pt-BR")
                         },
                         fontWeight: "bold"
                     }
                 },
                 roseType: null,
                 data: e.rows.map(function(d) {
                     return {
                         name: d[0],
-                        value: d[l + 1]
+                        value: d[o + 1]
                     }
                 })
             }
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
@@ -3675,36 +3675,36 @@
                     formatter: function(i) {
                         return i.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(i, l) {
+            data: e.rows.map(function(i, o) {
                 return {
                     name: i[0],
                     value: i[1]
                 }
             })
         }
     }
 
     function r() {
         var i = {
             tooltip: {
                 trigger: "item",
-                formatter: function(l) {
-                    return `${l.name}: <b>${l.data.value.toLocaleString("pt-BR")}</b> (${l.percent.toLocaleString("pt-BR")}%)`
+                formatter: function(o) {
+                    return `${o.name}: <b>${o.data.value.toLocaleString("pt-BR")}</b> (${o.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(l) {
-                    return l.name + " (" + l.percent.toLocaleString("pt-BR") + "%)"
+                formatter(o) {
+                    return o.name + " (" + o.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
         return t.jsx(ne, {
             option: i
         })
@@ -3731,15 +3731,15 @@
 function G(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
         i = {
             type: "value"
         },
-        l = {
+        o = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
                 },
                 saveAsImage: {
                     show: !0
@@ -3750,43 +3750,43 @@
 
     function c() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
-            data: e.rows.map(function(o) {
-                return o[0]
+            data: e.rows.map(function(l) {
+                return l[0]
             })
         }
     }
 
     function s() {
-        return e.headers ? e.rows.map(function(o) {
+        return e.headers ? e.rows.map(function(l) {
             return {
-                name: o[0],
-                data: o.slice(1),
+                name: l[0],
+                data: l.slice(1),
                 type: a,
                 stack: r,
                 areaStyle: d
             }
         }) : [{
             name: null,
-            data: e.rows.map(function(o) {
-                return o[1]
+            data: e.rows.map(function(l) {
+                return l[1]
             }),
             type: a,
             stack: r,
             areaStyle: d
         }]
     }
 
     function u() {
-        var o = {
-            toolbox: l,
+        var l = {
+            toolbox: o,
             tooltip: {
                 trigger: "axis",
                 axisPointer: {
                     type: "shadow"
                 },
                 formatter: function(h) {
                     return `${h[0].name}: <b>${h[0].value.toLocaleString("pt-BR")}</b>`
@@ -3800,15 +3800,15 @@
                 }
             },
             xAxis: n ? i : c(),
             yAxis: n ? c() : i,
             series: s()
         };
         return t.jsx(ne, {
-            option: o
+            option: l
         })
     }
     return u()
 }
 
 function At(e) {
     return t.jsx(G, {
@@ -3865,18 +3865,18 @@
             type: "treemap",
             roam: "move",
             nodeClick: !0,
             data: e.headers.slice(1).map(function(r, i) {
                 return {
                     name: r,
                     type: "pie",
-                    children: e.rows.map(function(l) {
+                    children: e.rows.map(function(o) {
                         return {
-                            name: l[0],
-                            value: l[i + 1]
+                            name: o[0],
+                            value: o[i + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -4061,16 +4061,16 @@
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%",
                     borderSpacing: 0
                 },
                 children: t.jsx("tbody", {
-                    children: r.map((l, d) => t.jsx("tr", {
-                        children: l.map((c, s) => s == 0 ? t.jsx("th", {
+                    children: r.map((o, d) => t.jsx("tr", {
+                        children: o.map((c, s) => s == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left",
                                 lineHeight: "2rem",
                                 padding: 5
                             },
                             className: d % 2 == 0 ? "even" : "odd",
                             children: c
@@ -4081,19 +4081,19 @@
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], i = [], l = Object.keys(e.data.series), d = [], c = 0; c < l.length; c++) {
+        for (var r = [], i = [], o = Object.keys(e.data.series), d = [], c = 0; c < o.length; c++) {
             c == 0 && r.push("");
-            for (var s = [l[c]], u = 0, o = 0; o < e.data.series[l[c]].length; o++) {
-                var h = e.data.series[l[c]];
-                c == 0 && r.push(h[o][0]), s.push(h[o][1]), u += h[o][1], l.length > 1 && (c == 0 ? d.push(h[o][1]) : d[o] += h[o][1], o > 0 && o == e.data.series[l[c]].length - 1 && (c == 0 ? d.push(u) : d[o + 1] += u))
+            for (var s = [o[c]], u = 0, l = 0; l < e.data.series[o[c]].length; l++) {
+                var h = e.data.series[o[c]];
+                c == 0 && r.push(h[l][0]), s.push(h[l][1]), u += h[l][1], o.length > 1 && (c == 0 ? d.push(h[l][1]) : d[l] += h[l][1], l > 0 && l == e.data.series[o[c]].length - 1 && (c == 0 ? d.push(u) : d[l + 1] += u))
             }
             s.length > 2 && (c == 0 && r.push(""), s.push(u)), i.push(s)
         }
         return e.data.chart ? t.jsx(be, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
@@ -4145,158 +4145,158 @@
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
 
 function Ut() {
     function e() {
-        const l = {
+        const o = {
             width: 150,
             height: 150,
             borderRadius: "50%",
             objectFit: "cover",
             backgroundColor: j.colors.success
         };
         return window.application.menu.user && t.jsxs("div", {
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
-                    style: l
+                    style: o
                 })
             }), t.jsx("div", {
                 children: t.jsx(O, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
             })]
         })
     }
 
-    function n(l) {
-        var d = l.target;
+    function n(o) {
+        var d = o.target;
         const c = d.querySelector(":scope > ul, :scope > li");
         if (c) {
-            c.offsetParent === null ? d.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(o) {
-                o.style.display = "block"
-            }) : d.querySelectorAll(":scope > ul, :scope > li").forEach(function(o) {
-                o.style.display = "none"
+            c.offsetParent === null ? d.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(l) {
+                l.style.display = "block"
+            }) : d.querySelectorAll(":scope > ul, :scope > li").forEach(function(l) {
+                l.style.display = "none"
             });
             const s = d.querySelector(":scope > i.fa-solid.fa-chevron-right"),
                 u = d.querySelector(":scope > i.fa-solid.fa-chevron-up");
-            return s && (s.classList.remove("fa-chevron-right"), s.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), l.preventDefault(), l.stopPropagation(), l.cancelBubble = !0, !1
+            return s && (s.classList.remove("fa-chevron-right"), s.classList.add("fa-chevron-up")), u && (u.classList.remove("fa-chevron-up"), u.classList.add("fa-chevron-right")), o.preventDefault(), o.stopPropagation(), o.cancelBubble = !0, !1
         } else {
             const s = document.querySelector("aside");
             s.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
-    function a(l, d) {
+    function a(o, d) {
         const c = {
                 display: d == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 15,
                 paddingRight: 20,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem",
                 color: j.colors.primary
             },
             s = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
-        return l.url ? t.jsx("li", {
+        return o.url ? t.jsx("li", {
             style: c,
             onClick: n,
             className: "item",
             children: t.jsxs(O, {
-                href: l.url,
-                dataLabel: E(l.label),
+                href: o.url,
+                dataLabel: E(o.label),
                 style: {
                     textDecoration: "none"
                 },
                 children: [d == 0 && t.jsx(S, {
-                    icon: l.icon || "dot-circle",
+                    icon: o.icon || "dot-circle",
                     style: s
-                }), l.label]
+                }), o.label]
             })
-        }, Math.random()) : l.items.length > 0 && t.jsxs("li", {
+        }, Math.random()) : o.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: c,
-            "data-label": E(l.label),
+            "data-label": E(o.label),
             children: [d == 0 && t.jsx(S, {
-                icon: l.icon || "dot-circle",
+                icon: o.icon || "dot-circle",
                 style: s
-            }), l.label, t.jsx(S, {
+            }), o.label, t.jsx(S, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
                     display: "none",
                     paddingLeft: 15
                 },
-                children: l.items.map(function(u) {
+                children: o.items.map(function(u) {
                     return a(u, d + 1)
                 })
             })]
         }, Math.random())
     }
 
     function r() {
-        const l = {
+        const o = {
             padding: 0
         };
         return window.application.menu.items.length > 0 && t.jsx("ul", {
-            style: l,
+            style: o,
             children: window.application.menu.items.map(function(d) {
                 return a(d, 0)
             })
         })
     }
 
     function i() {
-        const l = {
+        const o = {
             marginTop: 10,
             height: "100%",
             borderRight: "solid 1px #EEE"
         };
         return t.jsxs("div", {
-            style: l,
+            style: o,
             className: "menu",
             children: [e(), r()]
         })
     }
     return i()
 }
 
 function Gt(e) {
     var n;
 
-    function a(l) {
-        const d = "=".repeat((4 - l.length % 4) % 4),
-            c = (l + d).replace(/\-/g, "+").replace(/_/g, "/"),
+    function a(o) {
+        const d = "=".repeat((4 - o.length % 4) % 4),
+            c = (o + d).replace(/\-/g, "+").replace(/_/g, "/"),
             s = window.atob(c),
             u = new Uint8Array(s.length);
-        for (let o = 0; o < s.length; ++o) u[o] = s.charCodeAt(o);
+        for (let l = 0; l < s.length; ++l) u[l] = s.charCodeAt(l);
         return u
     }
 
     function r() {
-        "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(l) {
-            if (l) {
+        "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(o) {
+            if (o) {
                 const d = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
-                l.pushManager.subscribe({
+                o.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: d
                 }).then(function(c) {
                     if (console.log(c), n = JSON.stringify(c), console.log(n), c) {
                         alert("Notificação ativada com sucesso.");
                         var s = new FormData;
                         s.append("subscription", n), q("POST", "/api/pushsubscribe/", function(u) {
@@ -4306,16 +4306,16 @@
                         alert("Problema ao ativar notificações.");
                         return
                     }
                 }).catch(function(c) {
                     alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", c)
                 })
             } else console.log("No registered service worker.")
-        }).catch(function(l) {
-            alert("Erro"), console.error("Service Worker Error", l)
+        }).catch(function(o) {
+            alert("Erro"), console.error("Service Worker Error", o)
         }) : alert("Push messaging is not supported")
     }
 
     function i() {
         return t.jsx(S, {
             onClick: r,
             icon: "bell",
@@ -4337,19 +4337,19 @@
             minX: 30,
             maxX: 30,
             minY: 50,
             maxY: 60
         },
         r = null;
     e.addEventListener("touchstart", function(i) {
-        var l = i.touches[0];
-        a.startX = l.screenX, a.startY = l.screenY
+        var o = i.touches[0];
+        a.startX = o.screenX, a.startY = o.screenY
     }), e.addEventListener("touchmove", function(i) {
-        var l = i.touches[0];
-        a.endX = l.screenX, a.endY = l.screenY
+        var o = i.touches[0];
+        a.endX = o.screenX, a.endY = o.screenY
     }), e.addEventListener("touchend", function(i) {
         Math.abs(a.endX - a.startX) > a.minX && Math.abs(a.endY - a.startY) < a.maxY ? r = a.endX > a.startX ? "right" : "left" : Math.abs(a.endY - a.startY) > a.minY && Math.abs(a.endX - a.startX) < a.maxX && (r = a.endY > a.startY ? "down" : "up"), r !== null && typeof n == "function" && n(e, r)
     })
 }
 
 function Xt(e) {
     function n() {
@@ -4418,35 +4418,35 @@
         })
     }
     return r()
 }
 
 function $t(e) {
     B.useEffect(() => {
-        const o = localStorage.getItem("message");
-        o && (localStorage.removeItem("message"), z(o)), window.addEventListener("resize", () => {
+        const l = localStorage.getItem("message");
+        l && (localStorage.removeItem("message"), z(l)), window.addEventListener("resize", () => {
             const h = document.querySelector("aside");
             h && (h.style.display = window.innerWidth < 800 ? "none" : "block")
         }), Yt(document.querySelector("main"), function(h, g) {
             console.log(h, g)
         })
     }, []);
 
     function a() {
-        const o = document.querySelector("aside");
-        o.style.display = o.style.display == "none" ? "block" : "none"
+        const l = document.querySelector("aside");
+        l.style.display = l.style.display == "none" ? "block" : "none"
     }
 
-    function r(o) {
-        const h = o.target.tagName == "A" ? o.target : o.target.closest("a");
-        o.preventDefault(), window.load(h.href)
+    function r(l) {
+        const h = l.target.tagName == "A" ? l.target : l.target.closest("a");
+        l.preventDefault(), window.load(h.href)
     }
 
     function i() {
-        const o = {
+        const l = {
                 display: "flex",
                 width: "100%",
                 justifyContent: "space-between",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 overflowX: "hidden"
             },
             h = {
@@ -4456,15 +4456,15 @@
                 mask: null,
                 name: "search",
                 required: !1,
                 type: "choice",
                 icon: "search"
             };
         return e.data.navbar ? t.jsxs("div", {
-            style: o,
+            style: l,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
                 children: [e.data.menu && t.jsx(S, {
                     icon: "navicon",
                     style: {
@@ -4591,37 +4591,37 @@
                         })
                     })
                 })]
             })]
         }) : null
     }
 
-    function l() {
+    function o() {
         return window.application.menu && window.application.menu.items.length > 0 && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
             children: t.jsx(Ut, {})
         })
     }
 
     function d() {
-        const o = {
+        const l = {
                 margin: 15,
                 display: "flex",
                 justifyContent: "space-between"
             },
             h = {
                 color: j.colors.primary
             };
         return e.data.navbar && e.data.navbar.user && t.jsxs("div", {
-            style: o,
+            style: l,
             children: [t.jsxs("div", {
                 children: [t.jsx(O, {
                     href: "/app/dashboard/",
                     style: {
                         marginRight: 10
                     },
                     children: t.jsx(S, {
@@ -4650,17 +4650,17 @@
     }
 
     function s() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
                 children: window.application.sponsors && window.application.sponsors.length > 0 && t.jsx("div", {
-                    children: window.application.sponsors.map(function(o) {
+                    children: window.application.sponsors.map(function(l) {
                         return t.jsx("img", {
-                            src: o,
+                            src: l,
                             style: {
                                 height: 30,
                                 padding: 5
                             }
                         }, Math.random())
                     })
                 })
@@ -4678,27 +4678,27 @@
                 children: i()
             }), t.jsxs("div", {
                 style: {
                     width: "100%",
                     display: "flex",
                     minHeight: window.innerHeight - 70
                 },
-                children: [l(), c()]
+                children: [o(), c()]
             })]
         })
     }
     return u()
 }
 
 function Jt(e) {
     var n = null,
         a = null,
         r = null,
         i = !1,
-        l = null,
+        o = null,
         d = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
         c = {
             constraints: {
                 mandatory: {
                     OfferToReceiveAudio: !0,
                     OfferToReceiveVideo: !0
                 },
@@ -4706,28 +4706,33 @@
                 offerToReceiveVideo: 1
             },
             sdpTransform: m => m.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
         };
 
     function s() {
         console.log("Trying to connect..."), n = new Peer("999123" + e.data.caller.replaceAll(".", "").replaceAll("-", "")), n.on("open", function(m) {
-            document.getElementById("callerid").innerHTML = e.data.caller, y(), l = setInterval(function() {
+            document.getElementById("callerid").innerHTML = e.data.caller, y(), o = setInterval(function() {
                 i ? z("Em conexão com " + e.data.receiver + ".") : (z("Tentando estabeler conexão com " + e.data.receiver + "..."), y())
             }, 15e3)
         }), n.on("call", function(m) {
             d({
                 video: {
                     width: {
                         exact: 320
                     },
                     height: {
                         exact: 240
                     }
                 },
-                audio: !0
+                audio: {
+                    autoGainControl: !1,
+                    echoCancellation: !1,
+                    googGainControl: !1,
+                    noiseSuppression: !1
+                }
             }, function(k) {
                 a = k;
                 var v = document.getElementById("video2");
                 v.addEventListener("loadedmetadata", function(D) {
                     v.style.width = this.videoWidth / 4 + "px", v.style.height = this.videoHeight / 4 + "px", v.style.marginLeft = -this.videoWidth / 4 + "px", v.style.visibility = "visible"
                 }, !1), v.srcObject = a, m.answer(k), m.on("stream", function(D) {
                     r = D, document.getElementById("video1").srcObject = r, i = !0
@@ -4738,25 +4743,25 @@
                 console.log("Failed to get local stream", k)
             })
         }), n.on("error", function(m) {
             m.type == "browser-incompatible" ? alert("Navegador incompatível.") : m.type == "invalid-id" ? alert("Usuário inexistente.") : m.type == "network" ? (i = !1, console.log("Problema na conexão do usuário. Tentando novamente em 5 segundos."), setTimeout(s, 5e3)) : m.type == "peer-unavailable" && (console.log("Usuário indisponível!"), i = !1)
         })
     }
     B.useEffect(() => (s(), function() {
-        clearInterval(l), u(), z("Desconectado!")
+        clearInterval(o), u(), z("Desconectado!")
     }), []);
 
     function u() {
-        o(a, "audio"), o(a, "video"), o(r, "audio"), o(r, "video"), a = null, r = null;
+        l(a, "audio"), l(a, "video"), l(r, "audio"), l(r, "video"), a = null, r = null;
         const m = document.getElementById("video1"),
             k = document.getElementById("video2");
         m && (m.srcObject = null), k && (k.srcObject = null), console.log("Stopped!"), i = !1
     }
 
-    function o(m, k) {
+    function l(m, k) {
         m != null && m.getTracks().forEach(v => {
             v.kind === k && v.stop()
         })
     }
 
     function h() {
         var m = document.getElementById("video1");
@@ -4784,27 +4789,23 @@
                 width: {
                     exact: 320
                 },
                 height: {
                     exact: 240
                 },
                 frameRate: {
-                    ideal: 5,
-                    max: 10
+                    ideal: 15,
+                    max: 30
                 }
             },
             audio: {
                 autoGainControl: !1,
-                channelCount: 2,
                 echoCancellation: !1,
-                latency: 0,
-                noiseSuppression: !1,
-                sampleRate: 48e3,
-                sampleSize: 16,
-                volume: 1
+                googGainControl: !1,
+                noiseSuppression: !1
             }
         }, function(m) {
             a = m;
             var k = document.getElementById("video2");
             k.addEventListener("loadedmetadata", function(v) {
                 k.style.width = this.videoWidth / 4 + "px", k.style.height = this.videoHeight / 4 + "px", k.style.marginLeft = -this.videoWidth / 4 + "px", k.style.visibility = "visible"
             }, !1), k.srcObject = a, w()
@@ -4924,16 +4925,16 @@
 x.register(st, "QrCode");
 x.register(Se, "Badge");
 x.register(rt, "Status");
 x.register(at, "Progress");
 x.register(Ie, "Color");
 x.register(it, "Boxes");
 x.register(ct, "Indicators");
-x.register(lt, "Shell");
-x.register(ot, "FileLink");
+x.register(ot, "Shell");
+x.register(lt, "FileLink");
 x.register(dt, "FilePreview");
 x.register(Le, "Response");
 x.register($t, "Application");
 x.register(De, "IconSet");
 x.register(ut, "Grid");
 x.register(He, "Rows");
 x.register(Pe, "Cards");
```

### Comparing `pyslth-0.4.0/slth/static/js/vanilla-masker.js` & `pyslth-0.4.1/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/static/js/vanilla-masker.min.js` & `pyslth-0.4.1/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/statistics.py` & `pyslth-0.4.1/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/templates/index.html` & `pyslth-0.4.1/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/templates/service-worker.js` & `pyslth-0.4.1/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/tests.py` & `pyslth-0.4.1/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/urls.py` & `pyslth-0.4.1/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/utils.py` & `pyslth-0.4.1/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.0/slth/views.py` & `pyslth-0.4.1/slth/views.py`

 * *Files identical despite different names*

