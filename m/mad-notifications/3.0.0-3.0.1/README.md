# Comparing `tmp/mad_notifications-3.0.0.tar.gz` & `tmp/mad_notifications-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mad_notifications-3.0.0.tar", last modified: Mon May 20 18:55:32 2024, max compression
+gzip compressed data, was "mad_notifications-3.0.1.tar", last modified: Mon May 20 19:31:48 2024, max compression
```

## Comparing `mad_notifications-3.0.0.tar` & `mad_notifications-3.0.1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/VERSION.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.491872 mad_notifications-3.0.0/mad_notifications/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.493872 mad_notifications-3.0.0/mad_notifications/api/
--rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/api/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.497872 mad_notifications-3.0.0/mad_notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0002_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0003_auto_20211019_1206.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0004_auto_20211022_1847.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0005_auto_20211022_1908.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0006_auto_20211022_1917.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0007_auto_20211025_1927.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0008_auto_20211026_1408.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0009_emailtemplate_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0010_auto_20211102_2232.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0011_auto_20211129_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0012_emailtemplate_subject.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0014_auto_20220530_1815.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0015_usernotificationconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0016_alter_emailtemplate_slug.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0018_alter_notification_template.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0021_notificationtemplate.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0022_delete_emailtemplate.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6812 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.498872 mad_notifications-3.0.0/mad_notifications/notify/
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notify/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notify/firebase.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notify/twilio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/mad_notifications/senders/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/senders/email.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/senders/firebase.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/senders/twilio.py
--rw-rw-rw-   0 root         (0) root         (0)     4914 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/shorthand.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/signals.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/user.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/mad_notifications.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2267 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-20 18:55:32.500872 mad_notifications-3.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.277336 mad_notifications-3.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 19:31:48.277336 mad_notifications-3.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-20 19:31:47.000000 mad_notifications-3.0.1/VERSION.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.269336 mad_notifications-3.0.1/mad_notifications/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.270336 mad_notifications-3.0.1/mad_notifications/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/api/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.275336 mad_notifications-3.0.1/mad_notifications/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0002_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0003_auto_20211019_1206.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0004_auto_20211022_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0005_auto_20211022_1908.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0006_auto_20211022_1917.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0007_auto_20211025_1927.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0008_auto_20211026_1408.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0009_emailtemplate_from_email.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0010_auto_20211102_2232.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0011_auto_20211129_1024.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0012_emailtemplate_subject.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0014_auto_20220530_1815.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0015_usernotificationconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0016_alter_emailtemplate_slug.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0018_alter_notification_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0019_notification_mobile_content_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/0021_notificationtemplate.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6890 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.275336 mad_notifications-3.0.1/mad_notifications/notify/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/notify/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/notify/firebase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/notify/twilio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.276336 mad_notifications-3.0.1/mad_notifications/senders/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/senders/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/senders/firebase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/senders/twilio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4907 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/shorthand.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/mad_notifications/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 19:31:48.276336 mad_notifications-3.0.1/mad_notifications.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 19:31:48.000000 mad_notifications-3.0.1/mad_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-05-20 19:31:48.000000 mad_notifications-3.0.1/mad_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 19:31:48.000000 mad_notifications-3.0.1/mad_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 19:31:48.000000 mad_notifications-3.0.1/mad_notifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-20 19:31:48.000000 mad_notifications-3.0.1/mad_notifications.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-20 19:31:48.277336 mad_notifications-3.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 19:31:39.000000 mad_notifications-3.0.1/setup.py
```

### Comparing `mad_notifications-3.0.0/LICENSE.md` & `mad_notifications-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/PKG-INFO` & `mad_notifications-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad_notifications
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Django app to send push notifications to to users.
 Home-page: https://www.madithouse.com/
 Author: Haseeb Ur Rehman
 Author-email: code@madithouse.com
 License: Other/Proprietary License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `mad_notifications-3.0.0/README.md` & `mad_notifications-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/admin.py` & `mad_notifications-3.0.1/mad_notifications/admin.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/api/serializers.py` & `mad_notifications-3.0.1/mad_notifications/api/serializers.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/api/urls.py` & `mad_notifications-3.0.1/mad_notifications/api/urls.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/api/views.py` & `mad_notifications-3.0.1/mad_notifications/api/views.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0001_initial.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0006_auto_20211022_1917.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0006_auto_20211022_1917.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0007_auto_20211025_1927.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0007_auto_20211025_1927.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0008_auto_20211026_1408.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0008_auto_20211026_1408.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0010_auto_20211102_2232.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0010_auto_20211102_2232.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0011_auto_20211129_1024.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0011_auto_20211129_1024.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0014_auto_20220530_1815.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0014_auto_20220530_1815.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0015_usernotificationconfig.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0015_usernotificationconfig.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0018_alter_notification_template.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0018_alter_notification_template.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0019_notification_mobile_content_and_more.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/migrations/0021_notificationtemplate.py` & `mad_notifications-3.0.1/mad_notifications/migrations/0021_notificationtemplate.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/models.py` & `mad_notifications-3.0.1/mad_notifications/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         return str(self.name) + " - " + str(self.slug)
 
 
 class NotificationTemplate(NotificationTemplateAbstract):
     pass
 
 
+class EmailTemplate(NotificationTemplateAbstract):
+    pass
+
+
 # ================================================================================================================================================
 class DeviceAbstract(models.Model):
     id = models.BigAutoField(unique=True, primary_key=True)
     user = models.ForeignKey(
         get_user_model(), on_delete=models.SET_NULL, blank=False, null=True
     )
     token = models.TextField(blank=True, null=True)
@@ -189,15 +193,17 @@
 ## Admin classes
 def get_user_notification_config_admin_class():
     config_admin_class = notification_settings.USER_NOTIFICATION_CONFIG_ADMIN_CLASS
     return config_admin_class
 
 
 def get_notification_template_admin_class():
-    notification_template_admin_class = notification_settings.NOTIFICATION_TEMPLATE_ADMIN_CLASS
+    notification_template_admin_class = (
+        notification_settings.NOTIFICATION_TEMPLATE_ADMIN_CLASS
+    )
     return notification_template_admin_class
 
 
 def get_device_admin_class():
     device_admin_class = notification_settings.DEVICE_ADMIN_CLASS
     return device_admin_class
```

### Comparing `mad_notifications-3.0.0/mad_notifications/notification.py` & `mad_notifications-3.0.1/mad_notifications/notification.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/notify/email.py` & `mad_notifications-3.0.1/mad_notifications/notify/email.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/notify/firebase.py` & `mad_notifications-3.0.1/mad_notifications/notify/firebase.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/notify/twilio.py` & `mad_notifications-3.0.1/mad_notifications/notify/twilio.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/senders/email.py` & `mad_notifications-3.0.1/mad_notifications/senders/email.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/senders/firebase.py` & `mad_notifications-3.0.1/mad_notifications/senders/firebase.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/senders/twilio.py` & `mad_notifications-3.0.1/mad_notifications/senders/twilio.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/settings.py` & `mad_notifications-3.0.1/mad_notifications/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 USER_SETTINGS = getattr(settings, "MAD_NOTIFICATIONS", None)
 
 
 USER_NOTIFICATION_CONFIG_MODEL = "mad_notifications.UserNotificationConfig"
 
 NOTIFICATION_MODEL = getattr(settings, "MAD_NOTIFICATIONS_NOTIFICATION_MODEL", "mad_notifications.Notification")
-NOTIFICATION_TEMPLATE_MODEL = getattr(settings, "MAD_NOTIFICATIONS_TEMPLATE_MODEL", "mad_notifications.NotificationTemplate")
+NOTIFICATION_TEMPLATE_MODEL = getattr(settings, "MAD_NOTIFICATIONS_TEMPLATE_MODEL", "mad_notifications.EmailTemplate")
 DEVICE_MODEL = getattr(settings, "MAD_NOTIFICATIONS_DEVICE_MODEL", "mad_notifications.Device")
 
 TWILIO_ACCOUNT_SID = getattr(settings, "TWILIO_ACCOUNT_SID", None)
 TWILIO_ACCOUNT_AUTH_TOKEN = getattr(settings, "TWILIO_ACCOUNT_AUTH_TOKEN", None)
 TWILIO_ACCOUNT_PHONE_NUMBER = getattr(settings, "TWILIO_ACCOUNT_PHONE_NUMBER", None)
```

### Comparing `mad_notifications-3.0.0/mad_notifications/shorthand.py` & `mad_notifications-3.0.1/mad_notifications/shorthand.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/signals.py` & `mad_notifications-3.0.1/mad_notifications/signals.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/user.py` & `mad_notifications-3.0.1/mad_notifications/user.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications/utils.py` & `mad_notifications-3.0.1/mad_notifications/utils.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/mad_notifications.egg-info/PKG-INFO` & `mad_notifications-3.0.1/mad_notifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad_notifications
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Django app to send push notifications to to users.
 Home-page: https://www.madithouse.com/
 Author: Haseeb Ur Rehman
 Author-email: code@madithouse.com
 License: Other/Proprietary License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `mad_notifications-3.0.0/mad_notifications.egg-info/SOURCES.txt` & `mad_notifications-3.0.1/mad_notifications.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 mad_notifications/migrations/0015_usernotificationconfig.py
 mad_notifications/migrations/0016_alter_emailtemplate_slug.py
 mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
 mad_notifications/migrations/0018_alter_notification_template.py
 mad_notifications/migrations/0019_notification_mobile_content_and_more.py
 mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
 mad_notifications/migrations/0021_notificationtemplate.py
-mad_notifications/migrations/0022_delete_emailtemplate.py
 mad_notifications/migrations/__init__.py
 mad_notifications/notify/email.py
 mad_notifications/notify/firebase.py
 mad_notifications/notify/twilio.py
 mad_notifications/senders/email.py
 mad_notifications/senders/firebase.py
 mad_notifications/senders/twilio.py
```

### Comparing `mad_notifications-3.0.0/requirements.txt` & `mad_notifications-3.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `mad_notifications-3.0.0/setup.cfg` & `mad_notifications-3.0.1/setup.cfg`

 * *Files identical despite different names*

