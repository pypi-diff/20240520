# Comparing `tmp/mad_notifications-2.1.2.tar.gz` & `tmp/mad_notifications-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mad_notifications-2.1.2.tar", last modified: Thu Dec 14 13:01:10 2023, max compression
+gzip compressed data, was "mad_notifications-2.3.0.tar", last modified: Mon May 20 09:53:48 2024, max compression
```

## Comparing `mad_notifications-2.1.2.tar` & `mad_notifications-2.3.0.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.519560 mad_notifications-2.1.2/
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3003 2023-12-14 13:01:10.519560 mad_notifications-2.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1695 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-12-14 13:01:10.000000 mad_notifications-2.1.2/VERSION.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.511560 mad_notifications-2.1.2/mad_notifications/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.513560 mad_notifications-2.1.2/mad_notifications/api/
--rw-rw-rw-   0 root         (0) root         (0)     1175 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/api/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2962 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.517560 mad_notifications-2.1.2/mad_notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2041 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0002_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0003_auto_20211019_1206.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0004_auto_20211022_1847.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0005_auto_20211022_1908.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0006_auto_20211022_1917.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0007_auto_20211025_1927.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0008_auto_20211026_1408.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0009_emailtemplate_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0010_auto_20211102_2232.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0011_auto_20211129_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0012_emailtemplate_subject.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0014_auto_20220530_1815.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0015_usernotificationconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0016_alter_emailtemplate_slug.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/0018_alter_notification_template.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.518560 mad_notifications-2.1.2/mad_notifications/notify/
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/notify/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/notify/firebase.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/notify/twilio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.518560 mad_notifications-2.1.2/mad_notifications/senders/
--rw-rw-rw-   0 root         (0) root         (0)     2317 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/senders/email.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/senders/firebase.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/senders/twilio.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/shorthand.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/signals.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/user.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/mad_notifications/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 13:01:10.519560 mad_notifications-2.1.2/mad_notifications.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3003 2023-12-14 13:01:10.000000 mad_notifications-2.1.2/mad_notifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2006 2023-12-14 13:01:10.000000 mad_notifications-2.1.2/mad_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-14 13:01:10.000000 mad_notifications-2.1.2/mad_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      309 2023-12-14 13:01:10.000000 mad_notifications-2.1.2/mad_notifications.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-14 13:01:10.000000 mad_notifications-2.1.2/mad_notifications.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-12-14 13:01:10.520560 mad_notifications-2.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-12-14 13:01:01.000000 mad_notifications-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.961889 mad_notifications-2.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 09:53:48.961889 mad_notifications-2.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1695 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/VERSION.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.953889 mad_notifications-2.3.0/mad_notifications/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.955888 mad_notifications-2.3.0/mad_notifications/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/api/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2962 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.959889 mad_notifications-2.3.0/mad_notifications/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0002_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0003_auto_20211019_1206.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0004_auto_20211022_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0005_auto_20211022_1908.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0006_auto_20211022_1917.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0007_auto_20211025_1927.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0008_auto_20211026_1408.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0009_emailtemplate_from_email.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0010_auto_20211102_2232.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0011_auto_20211129_1024.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0012_emailtemplate_subject.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0014_auto_20220530_1815.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0015_usernotificationconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0016_alter_emailtemplate_slug.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0018_alter_notification_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0019_notification_mobile_content_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1522 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6742 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.960888 mad_notifications-2.3.0/mad_notifications/notify/
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notify/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notify/firebase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/notify/twilio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.960888 mad_notifications-2.3.0/mad_notifications/senders/
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/senders/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/senders/firebase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/senders/twilio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/shorthand.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/mad_notifications/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 09:53:48.960888 mad_notifications-2.3.0/mad_notifications.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-20 09:53:48.000000 mad_notifications-2.3.0/mad_notifications.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-20 09:53:48.962889 mad_notifications-2.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 09:53:39.000000 mad_notifications-2.3.0/setup.py
```

### Comparing `mad_notifications-2.1.2/LICENSE.md` & `mad_notifications-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/PKG-INFO` & `mad_notifications-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad_notifications
-Version: 2.1.2
+Version: 2.3.0
 Summary: A Django app to send push notifications to to users.
 Home-page: https://www.madithouse.com/
 Author: Haseeb Ur Rehman
 Author-email: code@madithouse.com
 License: Other/Proprietary License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,14 +28,16 @@
 Requires-Dist: google-api-core>=2.12.0
 Requires-Dist: google-auth>=2.23.4
 Requires-Dist: google-auth-httplib2>=0.1.1
 Requires-Dist: google-api-python-client>=2.106.0
 Requires-Dist: google-cloud-firestore>=2.13.0
 Requires-Dist: googleapis-common-protos>=1.61.0
 Requires-Dist: twilio>=8.10.0
+Requires-Dist: django-phonenumber-field>=7.3.0
+Requires-Dist: phonenumbers>=8.13.37
 
 # Mad Notifications
 
 Mad Notifications app for django to send notifications to the user
 
 ## Quick start
```

### Comparing `mad_notifications-2.1.2/README.md` & `mad_notifications-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/admin.py` & `mad_notifications-2.3.0/mad_notifications/admin.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/api/serializers.py` & `mad_notifications-2.3.0/mad_notifications/api/serializers.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/api/urls.py` & `mad_notifications-2.3.0/mad_notifications/api/urls.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/api/views.py` & `mad_notifications-2.3.0/mad_notifications/api/views.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0001_initial.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     operations = [
         migrations.CreateModel(
             name='Notification',
             fields=[
                 ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('title', models.CharField(max_length=254)),
                 ('content', models.TextField(blank=True, null=True)),
-                ('image', models.FileField(blank=True, null=True, upload_to=mad_notifications.utils.notificaion_unique_file_path)),
-                ('icon', models.FileField(blank=True, null=True, upload_to=mad_notifications.utils.notificaion_unique_file_path)),
+                ('image', models.FileField(blank=True, null=True, upload_to=mad_notifications.utils.notification_unique_file_path)),
+                ('icon', models.FileField(blank=True, null=True, upload_to=mad_notifications.utils.notification_unique_file_path)),
                 ('is_read', models.BooleanField(default=False)),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
                 ('user', models.ForeignKey(null=True, on_delete=django.db.models.deletion.SET_NULL, to=settings.AUTH_USER_MODEL)),
             ],
             options={
                 'verbose_name': 'User Notification',
```

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0006_auto_20211022_1917.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0006_auto_20211022_1917.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0007_auto_20211025_1927.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0007_auto_20211025_1927.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0008_auto_20211026_1408.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0008_auto_20211026_1408.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0010_auto_20211102_2232.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0010_auto_20211102_2232.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0011_auto_20211129_1024.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0011_auto_20211129_1024.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0014_auto_20220530_1815.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0014_auto_20220530_1815.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0015_usernotificationconfig.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0015_usernotificationconfig.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0017_alter_usernotificationconfig_user.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/migrations/0018_alter_notification_template.py` & `mad_notifications-2.3.0/mad_notifications/migrations/0018_alter_notification_template.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/models.py` & `mad_notifications-2.3.0/mad_notifications/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,180 @@
-from mad_notifications.utils import notificaion_unique_file_path
-from django.db import models
-from django.contrib.auth import get_user_model
 from django.apps import apps
-from mad_notifications.settings import notification_settings
+from django.contrib.auth import get_user_model
+from django.db import models
 
+from phonenumber_field.modelfields import PhoneNumberField
+
+from mad_notifications.settings import notification_settings
+from mad_notifications.utils import notification_unique_file_path
 
 # Create your models here.
 
+
 class UserNotificationConfigAbstract(models.Model):
     """
     Depending on the provider settings, determine if the notification should be sent or not.
     """
-    user = models.OneToOneField(get_user_model(), primary_key=True, on_delete=models.CASCADE)
+
+    user = models.OneToOneField(
+        get_user_model(), primary_key=True, on_delete=models.CASCADE
+    )
     allow_email = models.BooleanField(default=True, help_text="")
     allow_push = models.BooleanField(default=True, help_text="")
     allow_sms = models.BooleanField(default=True, help_text="")
     allow_whatsapp = models.BooleanField(default=True, help_text="")
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         abstract = True
 
 
 class UserNotificationConfig(UserNotificationConfigAbstract):
     pass
+
+
 # ================================================================================================================================================
 
+
 class EmailTemplateAbstract(models.Model):
     id = models.BigAutoField(unique=True, primary_key=True)
-    name = models.CharField(max_length=225, blank=False, null=False, help_text="Template Name")
-    slug = models.SlugField(max_length=225, blank=False, null=False, unique=True, help_text="Unique Template identifier")
-    subject = models.CharField(max_length=225, default="Email Subject here", blank=False, null=False, help_text="Email Subject")
-    content = models.TextField(blank=False, null=False, help_text='Templated content of the email. <a href="https://docs.djangoproject.com/en/dev/topics/templates/" target="_target">Refer to docs for more details</a>. Supports HTML')
-    from_email = models.CharField(max_length=225, blank=True, null=True, help_text='For example: No Reply &lt;noreply@example.com&gt;')
+    name = models.CharField(
+        max_length=225, blank=False, null=False, help_text="Template Name"
+    )
+    slug = models.SlugField(
+        max_length=225,
+        blank=False,
+        null=False,
+        unique=True,
+        help_text="Unique Template identifier",
+    )
+    subject = models.CharField(
+        max_length=225,
+        default="Email Subject here",
+        blank=False,
+        null=False,
+        help_text="Email Subject",
+    )
+    content = models.TextField(
+        blank=True,
+        null=True,
+        help_text='Templated content of the email. <a href="https://docs.djangoproject.com/en/dev/topics/templates/" target="_target">Refer to docs for more details</a>. Supports HTML',
+    )
+    mobile_content = models.TextField(
+        blank=True,
+        null=True,
+        help_text='Templated content for SMS, and Push notification etc. <a href="https://docs.djangoproject.com/en/dev/topics/templates/" target="_target">Refer to docs for more details</a>. Supports HTML',
+    )
+    from_email = models.CharField(
+        max_length=225,
+        blank=True,
+        null=True,
+        help_text="For example: No Reply &lt;noreply@example.com&gt;",
+    )
+    from_phone = PhoneNumberField(
+        blank=True, null=True, help_text="Phone number to send this message from."
+    )
     admin_note = models.TextField(blank=True, null=True, help_text="")
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
-
     class Meta:
         abstract = True
-        ordering = ['-id']
+        ordering = ["-id"]
 
     def __str__(self):
         return str(self.name) + " - " + str(self.slug)
 
 
 class EmailTemplate(EmailTemplateAbstract):
     pass
 
 
 # ================================================================================================================================================
 class DeviceAbstract(models.Model):
     id = models.BigAutoField(unique=True, primary_key=True)
-    user = models.ForeignKey(get_user_model(), on_delete=models.SET_NULL, blank=False, null=True)
+    user = models.ForeignKey(
+        get_user_model(), on_delete=models.SET_NULL, blank=False, null=True
+    )
     token = models.TextField(blank=True, null=True)
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     class Meta:
         abstract = True
-        ordering = ['-id']
+        ordering = ["-id"]
 
 
 class Device(DeviceAbstract):
     pass
 
+
 # ================================================================================================================================================
 
+
 class NotificationAbstract(models.Model):
     id = models.BigAutoField(unique=True, primary_key=True)
-    user = models.ForeignKey(get_user_model(), on_delete=models.SET_NULL, blank=False, null=True)
+    user = models.ForeignKey(
+        get_user_model(), on_delete=models.SET_NULL, blank=False, null=True
+    )
     title = models.CharField(max_length=254, blank=False, null=False)
-    content = models.TextField(blank=False, null=True)
-    image = models.FileField(upload_to=notificaion_unique_file_path, blank=True, null=True)
-    icon = models.FileField(upload_to=notificaion_unique_file_path, blank=True, null=True)
+    content = models.TextField(
+        blank=False, null=True, help_text="Notification content for web/email"
+    )
+    mobile_content = models.TextField(
+        blank=False,
+        null=True,
+        help_text="Notification content for web/email sms, push, etc.",
+    )
+    image = models.FileField(
+        upload_to=notification_unique_file_path, blank=True, null=True
+    )
+    icon = models.FileField(
+        upload_to=notification_unique_file_path, blank=True, null=True
+    )
     is_read = models.BooleanField(default=False)
     actions = models.JSONField(default=dict, blank=True, help_text="")
-    data = models.JSONField(default=dict, blank=True, help_text="All keys and values in the dictionary must be strings.")
-    template = models.ForeignKey(notification_settings.EMAIL_TEMPLATE_MODEL, blank=True, null=True, on_delete=models.SET_NULL)
+    data = models.JSONField(
+        default=dict,
+        blank=True,
+        help_text="All keys and values in the dictionary must be strings.",
+    )
+    template = models.ForeignKey(
+        notification_settings.EMAIL_TEMPLATE_MODEL,
+        blank=True,
+        null=True,
+        on_delete=models.SET_NULL,
+    )
 
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
-
     class Meta:
         abstract = True
-        ordering = ['-id']
-
+        ordering = ["-id"]
 
 
 class Notification(NotificationAbstract):
     pass
 
 
 # ================================================================================================================================================
 
 
 # Model methods
 
+
 def get_user_notification_config_model():
     """Return the Notification model that is active in this project."""
     return apps.get_model(notification_settings.USER_NOTIFICATION_CONFIG_MODEL)
 
+
 def get_notification_model():
     """Return the Notification model that is active in this project."""
     return apps.get_model(notification_settings.NOTIFICATION_MODEL)
 
 
 def get_email_template_model():
     """Return the Notification model that is active in this project."""
@@ -135,8 +200,8 @@
 def get_device_admin_class():
     device_admin_class = notification_settings.DEVICE_ADMIN_CLASS
     return device_admin_class
 
 
 def get_notification_admin_class():
     notification_admin_class = notification_settings.NOTIFICATION_ADMIN_CLASS
-    return notification_admin_class
+    return notification_admin_class
```

### Comparing `mad_notifications-2.1.2/mad_notifications/notify/email.py` & `mad_notifications-2.3.0/mad_notifications/notify/email.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/notify/firebase.py` & `mad_notifications-2.3.0/mad_notifications/notify/firebase.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,41 @@
 
 """
 https://firebase.google.com/docs/cloud-messaging/auth-server#use-credentials-to-mint-access-tokens
 https://github.com/firebase/firebase-admin-python/blob/e35a45a68885d1edfe7a28a2e75a9f1cc444f272/snippets/messaging/cloud_messaging.py
 """
 
 FIREBASE_APP = firebase_admin.initialize_app()
-SCOPES = [
-        'https://www.googleapis.com/auth/firebase.messaging'
-    ]
-
-def get_access_token():
-        """
-        Retrieve a valid access token that can be used to authorize requests.
-        :return: Access token.
-        """
-        access_token_info = FIREBASE_APP.get_access_token()
-        return access_token_info.access_token
+SCOPES = ["https://www.googleapis.com/auth/firebase.messaging"]
+
+
+def get_access_token(_firebase_app):
+    """
+    Retrieve a valid access token that can be used to authorize requests.
+    :return: Access token.
+    """
+    access_token_info = _firebase_app.get_access_token()
+    return access_token_info.access_token
 
 
 @shared_task(name="Non-Periodic: Push notification")
 def push_notification(notification_id):
     notification_obj = get_notification_model().objects.get(id=notification_id)
     # context = json.loads(notification_obj.notification_context)
     devices = notification_obj.user.device_set.all()
-    if notification_obj.content is not None:
+    if notification_obj.mobile_content is not None:
         for device in devices:
             try:
                 sendFirebaseMobilePushNotification(device, notification_obj)
                 logger.info("Push notification sent to device: " + str(device.id))
             except Exception as e:
-                logger.error( "Could not send push notification to device: " + str(device.id) + " message: " + str(e) )
+                logger.error(
+                    "Could not send push notification to device: "
+                    + str(device.id)
+                    + " message: "
+                    + str(e)
+                )
                 # TODO delete device object if notification couldn't be sent
 
         return "Push notifications sent"
     else:
         return "Error Notification has not content"
```

### Comparing `mad_notifications-2.1.2/mad_notifications/notify/twilio.py` & `mad_notifications-2.3.0/mad_notifications/notify/twilio.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/senders/firebase.py` & `mad_notifications-2.3.0/mad_notifications/senders/firebase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,75 @@
+# pylint: disable=E1123
+
 import datetime
 from firebase_admin import messaging
 from mad_notifications.settings import notification_settings
 
 
 class FirebaseMobilePushNotification:
-    
+
     def __init__(self, device, notification):
         self.device = device
         self.notification = notification
 
-
     def mobilePushNotification(self):
         device = self.device
         notification_obj = self.notification
 
         message = messaging.Message(
             token=device.token,
             notification=messaging.Notification(
                 title=notification_obj.title,
-                body=notification_obj.content,
-                image=notification_obj.image.url if notification_obj.image else '' ,
-                icon=notification_obj.icon.url if notification_obj.ion else ''
+                body=notification_obj.mobile_content,
+                image=notification_obj.image.url if notification_obj.image else "",
+                icon=notification_obj.icon.url if notification_obj.ion else "",
             ),
             android=messaging.AndroidConfig(
                 ttl=datetime.timedelta(seconds=3600),
-                priority='high',
+                priority="high",
                 notification=messaging.AndroidNotification(
-                    icon=notification_obj.icon.url if notification_obj.icon else '' ,
+                    icon=notification_obj.icon.url if notification_obj.icon else "",
                     default_sound=True,
-                    sound='default',
-                    color='#ffffff',
+                    sound="default",
+                    color="#ffffff",
                     default_light_settings=True,
-                    click_action=notification_obj.actions['click_action'] if "click_action" in notification_obj.actions else None
-                )
+                    click_action=(
+                        notification_obj.actions["click_action"]
+                        if "click_action" in notification_obj.actions
+                        else None
+                    ),
+                ),
             ),
             apns=messaging.APNSConfig(
-                headers={'apns-priority': '10'},
+                headers={"apns-priority": "10"},
                 payload=messaging.APNSPayload(
                     aps=messaging.Aps(
-                        sound=messaging.CriticalSound (
-                            name="default",
-                            volume=1.0
+                        sound=messaging.CriticalSound(name="default", volume=1.0),
+                        category=(
+                            notification_obj.actions["click_action"]
+                            if "click_action" in notification_obj.actions
+                            else None
                         ),
-                        category=notification_obj.actions['click_action'] if "click_action" in notification_obj.actions else None
                     ),
                 ),
             ),
             webpush=messaging.WebpushConfig(
                 notification=messaging.WebpushNotification(
                     icon=notification_obj.icon.url if notification_obj.icon else "",
                     # renotify=True, # ! this requires tags so think about how this will be
                     # tag = "",
                     require_interaction=True,
                 ),
             ),
             # fcm data only supports json with string values.
-            data=notification_obj.data
+            data=notification_obj.data,
         )
         return messaging.send(message)
 
 
-
 def sendFirebaseMobilePushNotification(device, notification):
-    firebase_push_notification = notification_settings.FIREBASE_MOBILE_PUSH_NOTIFICATION_CLASS(device, notification)
-    return firebase_push_notification.mobilePushNotification()
+    firebase_push_notification = (
+        notification_settings.FIREBASE_MOBILE_PUSH_NOTIFICATION_CLASS(
+            device, notification
+        )
+    )
+    return firebase_push_notification.mobilePushNotification()
```

### Comparing `mad_notifications-2.1.2/mad_notifications/senders/twilio.py` & `mad_notifications-2.3.0/mad_notifications/senders/twilio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 import datetime
+import logging
+
 from django.conf import settings
-from mad_notifications.settings import notification_settings
-from django.template import Template, Context
+from django.template import Context, Template
 from twilio.rest import Client
-from django.conf import settings
-import logging
+
+from mad_notifications.settings import notification_settings
 
 logger = logging.getLogger(__name__)
 
+
 class TwilioNotification:
-    
+
     def __init__(self, notification):
         self.notification = notification
         self.TWILIO_ACCOUNT_SID = notification_settings.TWILIO_ACCOUNT_SID
         self.TWILIO_ACCOUNT_AUTH_TOKEN = notification_settings.TWILIO_ACCOUNT_AUTH_TOKEN
-        self.TWILIO_ACCOUNT_PHONE_NUMBER = notification_settings.TWILIO_ACCOUNT_PHONE_NUMBER
-        
-        self.twilioClient = Client(self.TWILIO_ACCOUNT_SID, self.TWILIO_ACCOUNT_AUTH_TOKEN)
-        
-
+        self.TWILIO_ACCOUNT_PHONE_NUMBER = (
+            notification_settings.TWILIO_ACCOUNT_PHONE_NUMBER
+        )
+
+        self.twilioClient = Client(
+            self.TWILIO_ACCOUNT_SID, self.TWILIO_ACCOUNT_AUTH_TOKEN
+        )
 
     def smsNotification(self):
         notification_obj = self.notification
         # send SMS
         try:
             message = self.twilioClient.messages.create(
-                body = notification_obj.content,
-                from_ = str(self.TWILIO_ACCOUNT_PHONE_NUMBER),
-                to = str(notification_obj.user.phone)
+                body=notification_obj.mobile_content,
+                from_=str(self.TWILIO_ACCOUNT_PHONE_NUMBER),
+                to=str(notification_obj.user.phone),
             )
             return message
-        
+
         except Exception as e:
             logger.error(str(e))
             raise
-    
-    
+
     def WhatsAppNotification(self):
         notification_obj = self.notification
         # send SMS
         try:
             message = self.twilioClient.messages.create(
-                body = notification_obj.content,
-                from_ = 'whatsapp:' + str(self.TWILIO_ACCOUNT_PHONE_NUMBER),
-                to = 'whatsapp:' + str(notification_obj.user.phone)
+                body=notification_obj.mobile_content,
+                from_="whatsapp:" + str(self.TWILIO_ACCOUNT_PHONE_NUMBER),
+                to="whatsapp:" + str(notification_obj.user.phone),
             )
             return message
-        
+
         except Exception as e:
             logger.error(str(e))
             raise
 
 
-
 def sendTwilioSMSNotification(notification):
     twilio_notification = notification_settings.TWILIO_NOTIFICATION_CLASS(notification)
     return twilio_notification.smsNotification()
 
 
 def sendTwilioWhatsAppNotification(notification):
     twilio_notification = notification_settings.TWILIO_NOTIFICATION_CLASS(notification)
-    return twilio_notification.WhatsAppNotification()
+    return twilio_notification.WhatsAppNotification()
```

### Comparing `mad_notifications-2.1.2/mad_notifications/settings.py` & `mad_notifications-2.3.0/mad_notifications/settings.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/shorthand.py` & `mad_notifications-2.3.0/mad_notifications/shorthand.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+import logging
+
 from mad_notifications.models import get_email_template_model
 from mad_notifications.notification import Notification
 
+logger = logging.getLogger(__name__)
+
 
-def newNotification(user, title, content, template_slug = None, data = {}, actions = {}):
+def newNotification(user, title, content, template_slug=None, data={}, actions={}):
     """
     Shorthand method to create and send notification
+
+    `title`, `content` will be overridden if `template_slug` is provided
+
     """
     # get email template from db
-    try:
-        if template_slug is not None:
-            email_template = get_email_template_model().objects.get(slug=template_slug)
-            email_template = email_template
-        else:
-            raise
-    except:
-        email_template = None
+    if template_slug is not None:
+        try:
+            notification_template = get_email_template_model().objects.get(
+                slug=template_slug
+            )
+        except Exception as e:
+            logger.warning("mad_notifications.shorthand.newNotification: %s", str(e))
+    else:
+        notification_template = None
 
     # create a notification for user
     notification = Notification(
-        user = user,
-        title = title,
-        content = str(content),
-        template = email_template,
-        data = data,
-        actions = actions,
+        user=user,
+        title=title,
+        content=str(content),
+        mobile_content=str(content),
+        template=notification_template,
+        data=data,
+        actions=actions,
     )
 
-    return notification.notify()
+    return notification.notify()
```

### Comparing `mad_notifications-2.1.2/mad_notifications/signals.py` & `mad_notifications-2.3.0/mad_notifications/signals.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/user.py` & `mad_notifications-2.3.0/mad_notifications/user.py`

 * *Files identical despite different names*

### Comparing `mad_notifications-2.1.2/mad_notifications/utils.py` & `mad_notifications-2.3.0/mad_notifications/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 
 def randomString(stringLength=8):
     """Generate a random string of fixed length """
     letters = string.ascii_lowercase
     return ''.join(random.choice(letters) for i in range(stringLength))
 
 
-def notificaion_unique_file_path(instance, filename):
+def notification_unique_file_path(instance, filename):
     # Get new file name/upload path
     base, ext = splitext(filename)
     newname = "%s%s%s" % (randomString(), '-' + base, ext)
     upload_dir = 'notification_media'
     return join(upload_dir, newname)
```

### Comparing `mad_notifications-2.1.2/mad_notifications.egg-info/PKG-INFO` & `mad_notifications-2.3.0/mad_notifications.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mad-notifications
-Version: 2.1.2
+Name: mad_notifications
+Version: 2.3.0
 Summary: A Django app to send push notifications to to users.
 Home-page: https://www.madithouse.com/
 Author: Haseeb Ur Rehman
 Author-email: code@madithouse.com
 License: Other/Proprietary License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -28,14 +28,16 @@
 Requires-Dist: google-api-core>=2.12.0
 Requires-Dist: google-auth>=2.23.4
 Requires-Dist: google-auth-httplib2>=0.1.1
 Requires-Dist: google-api-python-client>=2.106.0
 Requires-Dist: google-cloud-firestore>=2.13.0
 Requires-Dist: googleapis-common-protos>=1.61.0
 Requires-Dist: twilio>=8.10.0
+Requires-Dist: django-phonenumber-field>=7.3.0
+Requires-Dist: phonenumbers>=8.13.37
 
 # Mad Notifications
 
 Mad Notifications app for django to send notifications to the user
 
 ## Quick start
```

### Comparing `mad_notifications-2.1.2/mad_notifications.egg-info/SOURCES.txt` & `mad_notifications-2.3.0/mad_notifications.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 mad_notifications/migrations/0012_emailtemplate_subject.py
 mad_notifications/migrations/0013_alter_emailtemplate_from_email.py
 mad_notifications/migrations/0014_auto_20220530_1815.py
 mad_notifications/migrations/0015_usernotificationconfig.py
 mad_notifications/migrations/0016_alter_emailtemplate_slug.py
 mad_notifications/migrations/0017_alter_usernotificationconfig_user.py
 mad_notifications/migrations/0018_alter_notification_template.py
+mad_notifications/migrations/0019_notification_mobile_content_and_more.py
+mad_notifications/migrations/0020_emailtemplate_from_phone_and_more.py
 mad_notifications/migrations/__init__.py
 mad_notifications/notify/email.py
 mad_notifications/notify/firebase.py
 mad_notifications/notify/twilio.py
 mad_notifications/senders/email.py
 mad_notifications/senders/firebase.py
 mad_notifications/senders/twilio.py
```

### Comparing `mad_notifications-2.1.2/setup.cfg` & `mad_notifications-2.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -34,12 +34,14 @@
 	google-api-core>=2.12.0 # https://pypi.org/project/google-api-core/
 	google-auth>=2.23.4 # https://pypi.org/project/google-auth/
 	google-auth-httplib2>=0.1.1 # https://pypi.org/project/google-auth-httplib2/
 	google-api-python-client>=2.106.0 # https://pypi.org/project/google-api-python-client/
 	google-cloud-firestore>=2.13.0 # https://pypi.org/project/google-cloud-firestore/
 	googleapis-common-protos>=1.61.0  # https://pypi.org/project/googleapis-common-protos/
 	twilio>=8.10.0 # https://pypi.org/project/twilio/
+	django-phonenumber-field>=7.3.0 # https://pypi.org/project/django-phonenumber-field/
+	phonenumbers>=8.13.37 # https://pypi.org/project/phonenumbers/ - dependency for the above dependency
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

