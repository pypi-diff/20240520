# Comparing `tmp/mad_notifications-2.3.0.tar.gz` & `tmp/mad_notifications-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mad_notifications-2.3.0.tar", last modified: Mon May 20 09:53:48 2024, max compression
+gzip compressed data, was "mad_notifications-3.0.0.tar", last modified: Mon May 20 18:55:32 2024, max compression
```

## Comparing `mad_notifications-2.3.0.tar` & `mad_notifications-3.0.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.961889 mad_notifications-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 09:53:48.961889 mad_notifications-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/VERSION.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.953889 mad_notifications-2.3.0/mad_notifications/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.955888 mad_notifications-2.3.0/mad_notifications/api/
--rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/api/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.959889 mad_notifications-2.3.0/mad_notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0002_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0003_auto_20211019_1206.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0004_auto_20211022_1847.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0005_auto_20211022_1908.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0006_auto_20211022_1917.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0007_auto_20211025_1927.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0008_auto_20211026_1408.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0009_emailtemplate_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0010_auto_20211102_2232.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0011_auto_20211129_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0012_emailtemplate_subject.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0014_auto_20220530_1815.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0015_usernotificationconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0016_alter_emailtemplate_slug.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0018_alter_notification_template.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6742 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.960888 mad_notifications-2.3.0/mad_notifications/notify/
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notify/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notify/firebase.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notify/twilio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.960888 mad_notifications-2.3.0/mad_notifications/senders/
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/senders/email.py
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/senders/firebase.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/senders/twilio.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/shorthand.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/signals.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/user.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.960888 mad_notifications-2.3.0/mad_notifications.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2151 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-20 09:53:48.962889 mad_notifications-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/VERSION.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.491872 mad_notifications-3.0.0/mad_notifications/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.493872 mad_notifications-3.0.0/mad_notifications/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/api/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.497872 mad_notifications-3.0.0/mad_notifications/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0002_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0003_auto_20211019_1206.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0004_auto_20211022_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0005_auto_20211022_1908.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0006_auto_20211022_1917.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0007_auto_20211025_1927.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0008_auto_20211026_1408.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0009_emailtemplate_from_email.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0010_auto_20211102_2232.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0011_auto_20211129_1024.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0012_emailtemplate_subject.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0014_auto_20220530_1815.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0015_usernotificationconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0016_alter_emailtemplate_slug.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0018_alter_notification_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0021_notificationtemplate.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/0022_delete_emailtemplate.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6812 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.498872 mad_notifications-3.0.0/mad_notifications/notify/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notify/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notify/firebase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/notify/twilio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/mad_notifications/senders/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/senders/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/senders/firebase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/senders/twilio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4914 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/shorthand.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/mad_notifications/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:55:32.499872 mad_notifications-3.0.0/mad_notifications.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-20 18:55:32.000000 mad_notifications-3.0.0/mad_notifications.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-20 18:55:32.500872 mad_notifications-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 18:55:23.000000 mad_notifications-3.0.0/setup.py
```

### Comparing `mad_notifications-2.3.0/LICENSE.md` & `mad_notifications-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/PKG-INFO` & `mad_notifications-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad_notifications
-Version: 2.3.0
+Version: 3.0.0
 Summary: A Django app to send push notifications to to users.
 Home-page: https://www.madithouse.com/
 Author: Haseeb Ur Rehman
 Author-email: code@madithouse.com
 License: Other/Proprietary License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `mad_notifications-2.3.0/README.md` & `mad_notifications-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/admin.py` & `mad_notifications-3.0.0/mad_notifications/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from mad_notifications.models import get_device_admin_class, get_device_model, get_email_template_admin_class, get_email_template_model, get_notification_admin_class, get_notification_model, get_user_notification_config_admin_class, get_user_notification_config_model
+from mad_notifications.models import get_device_admin_class, get_device_model, get_notification_template_admin_class, get_notification_template_model, get_notification_admin_class, get_notification_model, get_user_notification_config_admin_class, get_user_notification_config_model
 from django.contrib import admin
 
 # Register your models here.
 
 
 class UserNotificationConfigAdmin(admin.ModelAdmin):
     list_display = [field.name for field in get_user_notification_config_model()._meta.get_fields()]
     list_filter = ('created_at',)
     ordering = ('-created_at',)
 
 
-class EmailTemplateAdmin(admin.ModelAdmin):
+class NotificationTemplateAdmin(admin.ModelAdmin):
     list_display = ['id', 'name', 'slug', 'created_at']
     list_filter = ('created_at',)
     ordering = ('-created_at',)
 
 class DeviceAdmin(admin.ModelAdmin):
     list_display = ['id', 'user', 'created_at']
     list_filter = ('created_at',)
@@ -26,20 +26,20 @@
     list_filter = ('created_at',)
     ordering = ('-created_at',)
     raw_id_fields = ('user', 'template')
 
 
 #show admin
 userConfig_model = get_user_notification_config_model()
-emailTemplate_model = get_email_template_model()
+notificationTemplate_model = get_notification_template_model()
 device_model = get_device_model()
 notification_model = get_notification_model()
 
 userConfig_admin_class = get_user_notification_config_admin_class()
-emailTemplate_admin_class = get_email_template_admin_class()
+emailTemplate_admin_class = get_notification_template_admin_class()
 device_admin_class = get_device_admin_class()
 notification_admin_class = get_notification_admin_class()
 
 admin.site.register(userConfig_model, userConfig_admin_class)
-admin.site.register(emailTemplate_model, emailTemplate_admin_class)
+admin.site.register(notificationTemplate_model, emailTemplate_admin_class)
 admin.site.register(device_model, device_admin_class)
 admin.site.register(notification_model, notification_admin_class)
```

### Comparing `mad_notifications-2.3.0/mad_notifications/api/serializers.py` & `mad_notifications-3.0.0/mad_notifications/api/serializers.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/api/urls.py` & `mad_notifications-3.0.0/mad_notifications/api/urls.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/api/views.py` & `mad_notifications-3.0.0/mad_notifications/api/views.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0001_initial.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0006_auto_20211022_1917.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0006_auto_20211022_1917.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0007_auto_20211025_1927.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0007_auto_20211025_1927.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0008_auto_20211026_1408.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0008_auto_20211026_1408.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0010_auto_20211102_2232.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0010_auto_20211102_2232.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0011_auto_20211129_1024.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0011_auto_20211129_1024.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0014_auto_20220530_1815.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0014_auto_20220530_1815.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0015_usernotificationconfig.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0015_usernotificationconfig.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0018_alter_notification_template.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0018_alter_notification_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,10 +11,10 @@
         ('mad_notifications', '0017_alter_usernotificationconfig_user'),
     ]
 
     operations = [
         migrations.AlterField(
             model_name='notification',
             name='template',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to=notification_settings.EMAIL_TEMPLATE_MODEL),
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, to=notification_settings.NOTIFICATION_TEMPLATE_MODEL),
         ),
     ]
```

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py` & `mad_notifications-3.0.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/models.py` & `mad_notifications-3.0.0/mad_notifications/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class UserNotificationConfig(UserNotificationConfigAbstract):
     pass
 
 
 # ================================================================================================================================================
 
 
-class EmailTemplateAbstract(models.Model):
+class NotificationTemplateAbstract(models.Model):
     id = models.BigAutoField(unique=True, primary_key=True)
     name = models.CharField(
         max_length=225, blank=False, null=False, help_text="Template Name"
     )
     slug = models.SlugField(
         max_length=225,
         blank=False,
@@ -83,15 +83,15 @@
         abstract = True
         ordering = ["-id"]
 
     def __str__(self):
         return str(self.name) + " - " + str(self.slug)
 
 
-class EmailTemplate(EmailTemplateAbstract):
+class NotificationTemplate(NotificationTemplateAbstract):
     pass
 
 
 # ================================================================================================================================================
 class DeviceAbstract(models.Model):
     id = models.BigAutoField(unique=True, primary_key=True)
     user = models.ForeignKey(
@@ -138,15 +138,15 @@
     actions = models.JSONField(default=dict, blank=True, help_text="")
     data = models.JSONField(
         default=dict,
         blank=True,
         help_text="All keys and values in the dictionary must be strings.",
     )
     template = models.ForeignKey(
-        notification_settings.EMAIL_TEMPLATE_MODEL,
+        notification_settings.NOTIFICATION_TEMPLATE_MODEL,
         blank=True,
         null=True,
         on_delete=models.SET_NULL,
     )
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
@@ -172,33 +172,33 @@
 
 
 def get_notification_model():
     """Return the Notification model that is active in this project."""
     return apps.get_model(notification_settings.NOTIFICATION_MODEL)
 
 
-def get_email_template_model():
+def get_notification_template_model():
     """Return the Notification model that is active in this project."""
-    return apps.get_model(notification_settings.EMAIL_TEMPLATE_MODEL)
+    return apps.get_model(notification_settings.NOTIFICATION_TEMPLATE_MODEL)
 
 
 def get_device_model():
     """Return the Notification model that is active in this project."""
     return apps.get_model(notification_settings.DEVICE_MODEL)
 
 
 ## Admin classes
 def get_user_notification_config_admin_class():
     config_admin_class = notification_settings.USER_NOTIFICATION_CONFIG_ADMIN_CLASS
     return config_admin_class
 
 
-def get_email_template_admin_class():
-    email_template_admin_class = notification_settings.EMAIL_TEMPLATE_ADMIN_CLASS
-    return email_template_admin_class
+def get_notification_template_admin_class():
+    notification_template_admin_class = notification_settings.NOTIFICATION_TEMPLATE_ADMIN_CLASS
+    return notification_template_admin_class
 
 
 def get_device_admin_class():
     device_admin_class = notification_settings.DEVICE_ADMIN_CLASS
     return device_admin_class
```

### Comparing `mad_notifications-2.3.0/mad_notifications/notification.py` & `mad_notifications-3.0.0/mad_notifications/notification.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/notify/email.py` & `mad_notifications-3.0.0/mad_notifications/notify/email.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/notify/firebase.py` & `mad_notifications-3.0.0/mad_notifications/notify/firebase.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/notify/twilio.py` & `mad_notifications-3.0.0/mad_notifications/notify/twilio.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/senders/email.py` & `mad_notifications-3.0.0/mad_notifications/senders/email.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/senders/firebase.py` & `mad_notifications-3.0.0/mad_notifications/senders/firebase.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/senders/twilio.py` & `mad_notifications-3.0.0/mad_notifications/senders/twilio.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/settings.py` & `mad_notifications-3.0.0/mad_notifications/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 USER_SETTINGS = getattr(settings, "MAD_NOTIFICATIONS", None)
 
 
 USER_NOTIFICATION_CONFIG_MODEL = "mad_notifications.UserNotificationConfig"
 
 NOTIFICATION_MODEL = getattr(settings, "MAD_NOTIFICATIONS_NOTIFICATION_MODEL", "mad_notifications.Notification")
-EMAIL_TEMPLATE_MODEL = getattr(settings, "MAD_NOTIFICATIONS_EMAIL_TEMPLATE_MODEL", "mad_notifications.EmailTemplate")
+NOTIFICATION_TEMPLATE_MODEL = getattr(settings, "MAD_NOTIFICATIONS_TEMPLATE_MODEL", "mad_notifications.NotificationTemplate")
 DEVICE_MODEL = getattr(settings, "MAD_NOTIFICATIONS_DEVICE_MODEL", "mad_notifications.Device")
 
 TWILIO_ACCOUNT_SID = getattr(settings, "TWILIO_ACCOUNT_SID", None)
 TWILIO_ACCOUNT_AUTH_TOKEN = getattr(settings, "TWILIO_ACCOUNT_AUTH_TOKEN", None)
 TWILIO_ACCOUNT_PHONE_NUMBER = getattr(settings, "TWILIO_ACCOUNT_PHONE_NUMBER", None)
 
 
 DEFAULTS = {
     "NOTIFICATION_MODEL": NOTIFICATION_MODEL,
-    "EMAIL_TEMPLATE_MODEL": EMAIL_TEMPLATE_MODEL,
+    "NOTIFICATION_TEMPLATE_MODEL": NOTIFICATION_TEMPLATE_MODEL,
     "DEVICE_MODEL": DEVICE_MODEL,
     'USER_NOTIFICATION_CONFIG_MODEL': USER_NOTIFICATION_CONFIG_MODEL,
 
     # Firebase Defaults
     "FIREBASE_MOBILE_PUSH_NOTIFICATION_CLASS": "mad_notifications.senders.firebase.FirebaseMobilePushNotification",
 
     # Email Defaults
@@ -33,28 +33,28 @@
     "TWILIO_NOTIFICATION_CLASS": "mad_notifications.senders.twilio.TwilioNotification",
     'TWILIO_ACCOUNT_SID': TWILIO_ACCOUNT_SID,
     'TWILIO_ACCOUNT_AUTH_TOKEN': TWILIO_ACCOUNT_AUTH_TOKEN,
     'TWILIO_ACCOUNT_PHONE_NUMBER': TWILIO_ACCOUNT_PHONE_NUMBER,
 
 
     "USER_NOTIFICATION_CONFIG_ADMIN_CLASS": "mad_notifications.admin.UserNotificationConfigAdmin",
-    "EMAIL_TEMPLATE_ADMIN_CLASS": "mad_notifications.admin.EmailTemplateAdmin",
+    "NOTIFICATION_TEMPLATE_ADMIN_CLASS": "mad_notifications.admin.NotificationTemplateAdmin",
     "DEVICE_ADMIN_CLASS": "mad_notifications.admin.DeviceAdmin",
     "NOTIFICATION_ADMIN_CLASS": "mad_notifications.admin.NotificationAdmin",
 
     # Add more as required.
 }
 
 IMPORT_STRINGS = (
     "FIREBASE_MOBILE_PUSH_NOTIFICATION_CLASS",
     "EMAIL_NOTIFICATION_CLASS",
     'TWILIO_NOTIFICATION_CLASS',
 
     "USER_NOTIFICATION_CONFIG_ADMIN_CLASS",
-    "EMAIL_TEMPLATE_ADMIN_CLASS",
+    "NOTIFICATION_TEMPLATE_ADMIN_CLASS",
     "DEVICE_ADMIN_CLASS",
     "NOTIFICATION_ADMIN_CLASS",
 )
 
 MANDATORY = IMPORT_STRINGS
```

### Comparing `mad_notifications-2.3.0/mad_notifications/shorthand.py` & `mad_notifications-3.0.0/mad_notifications/shorthand.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from mad_notifications.models import get_email_template_model
+from mad_notifications.models import get_notification_template_model
 from mad_notifications.notification import Notification
 
 logger = logging.getLogger(__name__)
 
 
 def newNotification(user, title, content, template_slug=None, data={}, actions={}):
     """
@@ -12,15 +12,15 @@
 
     `title`, `content` will be overridden if `template_slug` is provided
 
     """
     # get email template from db
     if template_slug is not None:
         try:
-            notification_template = get_email_template_model().objects.get(
+            notification_template = get_notification_template_model().objects.get(
                 slug=template_slug
             )
         except Exception as e:
             logger.warning("mad_notifications.shorthand.newNotification: %s", str(e))
     else:
         notification_template = None
```

### Comparing `mad_notifications-2.3.0/mad_notifications/signals.py` & `mad_notifications-3.0.0/mad_notifications/signals.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/user.py` & `mad_notifications-3.0.0/mad_notifications/user.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications/utils.py` & `mad_notifications-3.0.0/mad_notifications/utils.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/mad_notifications.egg-info/PKG-INFO` & `mad_notifications-3.0.0/mad_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad_notifications
-Version: 2.3.0
+Version: 3.0.0
 Summary: A Django app to send push notifications to to users.
 Home-page: https://www.madithouse.com/
 Author: Haseeb Ur Rehman
 Author-email: code@madithouse.com
 License: Other/Proprietary License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `mad_notifications-2.3.0/mad_notifications.egg-info/SOURCES.txt` & `mad_notifications-3.0.0/mad_notifications.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 mad_notifications/migrations/0014_auto_20220530_1815.py
 mad_notifications/migrations/0015_usernotificationconfig.py
 mad_notifications/migrations/0016_alter_emailtemplate_slug.py
 mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
 mad_notifications/migrations/0018_alter_notification_template.py
 mad_notifications/migrations/0019_notification_mobile_content_and_more.py
 mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
+mad_notifications/migrations/0021_notificationtemplate.py
+mad_notifications/migrations/0022_delete_emailtemplate.py
 mad_notifications/migrations/__init__.py
 mad_notifications/notify/email.py
 mad_notifications/notify/firebase.py
 mad_notifications/notify/twilio.py
 mad_notifications/senders/email.py
 mad_notifications/senders/firebase.py
 mad_notifications/senders/twilio.py
```

### Comparing `mad_notifications-2.3.0/requirements.txt` & `mad_notifications-3.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.3.0/setup.cfg` & `mad_notifications-3.0.0/setup.cfg`

 * *Files identical despite different names*

