# Comparing `tmp/notifications_python_client-9.0.0-py3-none-any.whl.zip` & `tmp/notifications_python_client-9.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9334 bytes, number of entries: 12
--rw-r--r--  2.0 unx      637 b- defN 24-Jan-04 12:48 notifications_python_client/__init__.py
--rw-r--r--  2.0 unx     4662 b- defN 24-Jan-04 12:48 notifications_python_client/authentication.py
--rw-r--r--  2.0 unx     3745 b- defN 24-Jan-04 12:48 notifications_python_client/base.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Jan-04 12:48 notifications_python_client/errors.py
--rw-r--r--  2.0 unx     5435 b- defN 24-Jan-04 12:48 notifications_python_client/notifications.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-04 12:48 notifications_python_client/py.typed
--rw-r--r--  2.0 unx      542 b- defN 24-Jan-04 12:48 notifications_python_client/utils.py
--rw-r--r--  2.0 unx     1094 b- defN 24-Jan-04 12:59 notifications_python_client-9.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1084 b- defN 24-Jan-04 12:59 notifications_python_client-9.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-04 12:59 notifications_python_client-9.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Jan-04 12:59 notifications_python_client-9.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1152 b- defN 24-Jan-04 12:59 notifications_python_client-9.0.0.dist-info/RECORD
-12 files, 20909 bytes uncompressed, 7338 bytes compressed:  64.9%
+Zip file size: 9387 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      637 b- defN 24-May-20 12:54 notifications_python_client/__init__.py
+-rw-r--r--  2.0 unx     4662 b- defN 24-May-20 12:54 notifications_python_client/authentication.py
+-rw-r--r--  2.0 unx     3745 b- defN 24-May-20 12:54 notifications_python_client/base.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-20 12:54 notifications_python_client/errors.py
+-rw-r--r--  2.0 unx     5645 b- defN 24-May-20 12:54 notifications_python_client/notifications.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 12:54 notifications_python_client/py.typed
+-rw-r--r--  2.0 unx      542 b- defN 24-May-20 12:54 notifications_python_client/utils.py
+-rw-r--r--  2.0 unx     1094 b- defN 24-May-20 13:25 notifications_python_client-9.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1084 b- defN 24-May-20 13:25 notifications_python_client-9.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 13:25 notifications_python_client-9.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 13:25 notifications_python_client-9.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1152 b- defN 24-May-20 13:25 notifications_python_client-9.1.0.dist-info/RECORD
+12 files, 21119 bytes uncompressed, 7391 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: notifications_python_client/py.typed
 Comment: 
 
 Filename: notifications_python_client/utils.py
 Comment: 
 
-Filename: notifications_python_client-9.0.0.dist-info/LICENSE
+Filename: notifications_python_client-9.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: notifications_python_client-9.0.0.dist-info/METADATA
+Filename: notifications_python_client-9.1.0.dist-info/METADATA
 Comment: 
 
-Filename: notifications_python_client-9.0.0.dist-info/WHEEL
+Filename: notifications_python_client-9.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: notifications_python_client-9.0.0.dist-info/top_level.txt
+Filename: notifications_python_client-9.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: notifications_python_client-9.0.0.dist-info/RECORD
+Filename: notifications_python_client-9.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## notifications_python_client/__init__.py

```diff
@@ -3,15 +3,15 @@
 # Given a version number MAJOR.MINOR.PATCH, increment the:
 # - MAJOR version when you make incompatible API changes,
 # - MINOR version when you add functionality in a backwards-compatible manner, and
 # - PATCH version when you make backwards-compatible bug fixes.
 #
 # -- http://semver.org/
 
-__version__ = "9.0.0"
+__version__ = "9.1.0"
 
 from notifications_python_client.errors import (  # noqa
     REQUEST_ERROR_MESSAGE,
     REQUEST_ERROR_STATUS_CODE,
 )
 from notifications_python_client.notifications import NotificationsAPIClient  # noqa
 from notifications_python_client.utils import prepare_upload  # noqa
```

## notifications_python_client/notifications.py

```diff
@@ -18,23 +18,32 @@
         if reference:
             notification.update({"reference": reference})
         if sms_sender_id:
             notification.update({"sms_sender_id": sms_sender_id})
         return self.post("/v2/notifications/sms", data=notification)
 
     def send_email_notification(
-        self, email_address, template_id, personalisation=None, reference=None, email_reply_to_id=None
+        self,
+        email_address,
+        template_id,
+        personalisation=None,
+        reference=None,
+        email_reply_to_id=None,
+        one_click_unsubscribe_url=None,
     ):
         notification = {"email_address": email_address, "template_id": template_id}
         if personalisation:
             notification.update({"personalisation": personalisation})
         if reference:
             notification.update({"reference": reference})
         if email_reply_to_id:
             notification.update({"email_reply_to_id": email_reply_to_id})
+        if one_click_unsubscribe_url:
+            notification.update({"one_click_unsubscribe_url": one_click_unsubscribe_url})
+
         return self.post("/v2/notifications/email", data=notification)
 
     def send_letter_notification(self, template_id, personalisation, reference=None):
         notification = {"template_id": template_id, "personalisation": personalisation}
         if reference:
             notification.update({"reference": reference})
         return self.post("/v2/notifications/letter", data=notification)
```

## Comparing `notifications_python_client-9.0.0.dist-info/LICENSE` & `notifications_python_client-9.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `notifications_python_client-9.0.0.dist-info/METADATA` & `notifications_python_client-9.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifications-python-client
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python API client for GOV.UK Notify.
 Home-page: https://github.com/alphagov/notifications-python-client
 Author: Government Digital Service
 License: MIT
 Keywords: gds govuk notify
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `notifications_python_client-9.0.0.dist-info/RECORD` & `notifications_python_client-9.1.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-notifications_python_client/__init__.py,sha256=tTCSd_0PnzJKeF-Skytdp-VpsJJ8GlPa96kt38eO3nE,637
+notifications_python_client/__init__.py,sha256=r-sJQ-6pj7OsKjenzJoH9im4hhabdDj1Gu0tu6DbgiM,637
 notifications_python_client/authentication.py,sha256=HUOchdPtdMv20EFgD6O1xDnPqHUgpcwOSTKm772D1UU,4662
 notifications_python_client/base.py,sha256=oCxTWfhNpdTB66XSrl9rdXarADsCm4GvDg1rTKI_WLg,3745
 notifications_python_client/errors.py,sha256=Jsby_ww6xiJVpEQl-b4Psdawz9LE390rtoCuXLjxMbU,2438
-notifications_python_client/notifications.py,sha256=Ns6QOQSEVKmMtBCuWqVHyB0YyYDqdits4Yau_IY2ub0,5435
+notifications_python_client/notifications.py,sha256=c_mfGZNfmDgrOFcSQ7-RnLTY7KUkjV9GbsVrw88N2cA,5645
 notifications_python_client/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 notifications_python_client/utils.py,sha256=EiJqiLjjBGJHhsQjpyXwHcze54oaFiG0nARYggWxR5M,542
-notifications_python_client-9.0.0.dist-info/LICENSE,sha256=ArTAWSfEszf0_SxXDz1S9HbshIn78-RfUZLDF0UgULA,1094
-notifications_python_client-9.0.0.dist-info/METADATA,sha256=PZajqlxMoDIErp3NytYivvWEuZVscZbJnSX3XGAkXzs,1084
-notifications_python_client-9.0.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-notifications_python_client-9.0.0.dist-info/top_level.txt,sha256=RAa3Hvf6kd59bZGL4QBm5zVsiv6MegJquMXAQubXM3A,28
-notifications_python_client-9.0.0.dist-info/RECORD,,
+notifications_python_client-9.1.0.dist-info/LICENSE,sha256=ArTAWSfEszf0_SxXDz1S9HbshIn78-RfUZLDF0UgULA,1094
+notifications_python_client-9.1.0.dist-info/METADATA,sha256=oe8BaU4LS6Our2XKm7Q0L4jm74CJ3WBNwI1Esb7gKrA,1084
+notifications_python_client-9.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+notifications_python_client-9.1.0.dist-info/top_level.txt,sha256=RAa3Hvf6kd59bZGL4QBm5zVsiv6MegJquMXAQubXM3A,28
+notifications_python_client-9.1.0.dist-info/RECORD,,
```

