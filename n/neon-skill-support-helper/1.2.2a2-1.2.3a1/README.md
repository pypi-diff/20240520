# Comparing `tmp/neon-skill-support_helper-1.2.2a2.tar.gz` & `tmp/neon-skill-support_helper-1.2.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-support_helper-1.2.2a2.tar", last modified: Tue Apr  2 22:57:58 2024, max compression
+gzip compressed data, was "neon-skill-support_helper-1.2.3a1.tar", last modified: Mon May 20 16:08:42 2024, max compression
```

## Comparing `neon-skill-support_helper-1.2.2a2.tar` & `neon-skill-support_helper-1.2.3a1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.380057 neon-skill-support_helper-1.2.2a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.380057 neon-skill-support_helper-1.2.2a2/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/ask_description.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/cancelled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/confirm_support.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/email_signature.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/one_moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/support.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/dialog/yes.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/de-de/vocab/contact_support.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.380057 neon-skill-support_helper-1.2.2a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/ask_description.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/cancelled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/confirm_support.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/email_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/email_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/email_signature.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/email_title.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/no_email.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/one_moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/dialog/support.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/locale/en-us/intent/contact_support.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-02 22:57:58.000000 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-02 22:57:58.000000 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:57:58.000000 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 22:57:58.000000 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 22:57:58.000000 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 22:57:58.000000 neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:57:58.384057 neon-skill-support_helper-1.2.2a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 22:57:54.000000 neon-skill-support_helper-1.2.2a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.545404 neon-skill-support_helper-1.2.3a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.545404 neon-skill-support_helper-1.2.3a1/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.549404 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/ask_description.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/cancelled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/confirm_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/email_signature.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/one_moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/support.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/dialog/yes.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.549404 neon-skill-support_helper-1.2.3a1/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/de-de/vocab/contact_support.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.549404 neon-skill-support_helper-1.2.3a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/ask_description.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/cancelled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/confirm_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/email_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/email_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/email_signature.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/email_title.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/no_email.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/one_moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/dialog/support.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/locale/en-us/intent/contact_support.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-20 16:08:42.000000 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-20 16:08:42.000000 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:08:42.000000 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 16:08:42.000000 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-20 16:08:42.000000 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 16:08:42.000000 neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:08:42.553404 neon-skill-support_helper-1.2.3a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-20 16:08:38.000000 neon-skill-support_helper-1.2.3a1/version.py
```

### Comparing `neon-skill-support_helper-1.2.2a2/LICENSE.md` & `neon-skill-support_helper-1.2.3a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.2.2a2/PKG-INFO` & `neon-skill-support_helper-1.2.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-support_helper
-Version: 1.2.2a2
+Version: 1.2.3a1
 Home-page: https://github.com/NeonGeckoCom/skill-support_helper
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-support_helper-1.2.2a2/README.md` & `neon-skill-support_helper-1.2.3a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.2.2a2/__init__.py` & `neon-skill-support_helper-1.2.3a1/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,24 +90,24 @@
                 self.speak_dialog("one_moment", private=True)
             diagnostic_info = self._get_support_info(message, user_profile)
             user_description = self.get_response("ask_description",
                                                  num_retries=0)
             diagnostic_info["user_description"] = user_description
             attachment_files = self._parse_attachments(
                 self._get_attachments(diagnostic_info))
-            if self.send_email(self.translate("email_title"),
+            if self.send_email(self.resources.render_dialog("email_title"),
                                self._format_email_body(diagnostic_info),
                                message, email_addr,
                                attachments=attachment_files):
                 self.speak_dialog("complete",
                                   {"email": email_addr},
                                   private=True)
                 return
             LOG.error("Email failed to send, retry without attachments")
-            if self.send_email(self.translate("email_title"),
+            if self.send_email(self.resources.render_dialog("email_title"),
                                self._format_email_body(diagnostic_info),
                                message, email_addr):
                 self.speak_dialog("complete",
                                   {"email": email_addr},
                                   private=True)
             else:
                 LOG.error(f"Email Failed to send!")
@@ -144,19 +144,19 @@
 
     def _format_email_body(self, diagnostics: dict) -> str:
         """
         Format the diagnostic data with email dialog and return a string body
         :param diagnostics: diagnostic data to format into the email.
         :returns: email body to send
         """
-        return '\n\n'.join((self.translate("email_intro",
-                                           {"email": self.support_email}),
+        return '\n\n'.join((self.resources.render_dialog("email_intro",
+                                                         {"email": self.support_email}),
                             diagnostics.get('user_description') or
                             "No Description Provided",
-                            self.translate("email_signature")))
+                            self.resources.render_dialog("email_signature")))
 
     def _check_service_status(self, message: Message = None) -> dict:
         """
         Query services on the messagebus and report back their status
         """
         message = message or Message("get_status")
```

### Comparing `neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/PKG-INFO` & `neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-support-helper
-Version: 1.2.2a2
+Version: 1.2.3a1
 Home-page: https://github.com/NeonGeckoCom/skill-support_helper
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-support_helper-1.2.2a2/neon_skill_support_helper.egg-info/SOURCES.txt` & `neon-skill-support_helper-1.2.3a1/neon_skill_support_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.2.2a2/setup.py` & `neon-skill-support_helper-1.2.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.2.2a2/skill.json` & `neon-skill-support_helper-1.2.3a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.2.2a2/test/test_skill.py` & `neon-skill-support_helper-1.2.3a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-support_helper-1.2.2a2/version.py` & `neon-skill-support_helper-1.2.3a1/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.2.2a2"
+__version__ = "1.2.3a1"
```

