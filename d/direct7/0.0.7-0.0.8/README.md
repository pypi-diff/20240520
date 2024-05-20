# Comparing `tmp/direct7-0.0.7.tar.gz` & `tmp/direct7-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May 16 05:23:36 2024, from Unix
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `direct7-0.0.7.tar` & `direct7-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 direct7-0.0.7/main.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/__init__.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/client.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/errors.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/number_lookup.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/slack.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/sms.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/verify.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/viber.py
--rw-r--r--   0        0        0    10572 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/whatsapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 direct7-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    14774 2020-02-02 00:00:00.000000 direct7-0.0.7/tests/test_sdk.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 direct7-0.0.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 direct7-0.0.7/LICENSE
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 direct7-0.0.7/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 direct7-0.0.7/pyproject.toml
--rw-r--r--   0 sisira    (1000) sisira    (1000)     7264 2024-05-16 05:23:35.000000 direct7-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 direct7-0.0.8/main.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/__init__.py
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/client.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/errors.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/number_lookup.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/slack.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/sms.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/verify.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/viber.py
+-rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 direct7-0.0.8/src/direct7/whatsapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 direct7-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 direct7-0.0.8/tests/test_sdk.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 direct7-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 direct7-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 direct7-0.0.8/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 direct7-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 direct7-0.0.8/PKG-INFO
```

### Comparing `direct7-0.0.7/src/direct7/client.py` & `direct7-0.0.8/src/direct7/client.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/src/direct7/number_lookup.py` & `direct7-0.0.8/src/direct7/number_lookup.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/src/direct7/slack.py` & `direct7-0.0.8/src/direct7/slack.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/src/direct7/sms.py` & `direct7-0.0.8/src/direct7/sms.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/src/direct7/verify.py` & `direct7-0.0.8/src/direct7/verify.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/src/direct7/viber.py` & `direct7-0.0.8/src/direct7/viber.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/src/direct7/whatsapp.py` & `direct7-0.0.8/src/direct7/whatsapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 
     def __init__(self, client):
         self._client = client
 
     def send_whatsapp_freeform_message(self, originator: str, recipient: str, message_type: str, first_name: str = None,
                                        last_name: str = None, formatted_name: str = None, middle_name: str = None,
                                        suffix: str = None, prefix: str = None, birthday: str = None,
-                                       phones: list = None,
-                                       emails: list = None, urls: list = None, latitude: str = None,
-                                       longitude: str = None,
-                                       name: str = None, address: str = None,
-                                       type: str = None, url: str = None, caption: str = None, body: str = None,
-                                       message_id: uuid.UUID = None, emoji: str = None,
-                                       contact_addresses: list = None, ):
+                                       phones: list = None, emails: list = None, urls: list = None,
+                                       latitude: str = None, longitude: str = None, name: str = None,
+                                       address: str = None, type: str = None, url: str = None, caption: str = None,
+                                       filename: str = None, body: str = None, message_id: uuid.UUID = None,
+                                       emoji: str = None, contact_addresses: list = None, ):
         """
         Send a WhatsApp message to a single/multiple recipients.
+        :param filename:
         :param prefix: Prefix for the contact's name, such as Mr., Ms., Dr., etc.
         :param suffix: Suffix for the contact's name, if applicable.
         :param middle_name: Contact's middle name.
         :param contact_addresses:
         :param emoji:
         :param message_id:
         :param birthday: Contact's birthday in YYYY-MM-DD format.
@@ -74,19 +73,27 @@
             message["content"]["location"] = {
                 "latitude": latitude,
                 "longitude": longitude,
                 "name": name,
                 "address": address
             }
         elif message_type == "ATTACHMENT":
-            message["content"]["attachment"] = {
-                "type": type,
-                "url": url,
-                "caption": caption
-            }
+            if type == "document":
+                message["content"]["attachment"] = {
+                    "type": type,
+                    "url": url,
+                    "caption": caption,
+                    "filename": filename
+                }
+            else:
+                message["content"]["attachment"] = {
+                    "type": type,
+                    "url": url,
+                    "caption": caption
+                }
         elif message_type == "TEXT":
             message["content"]["text"] = {
                 "body": body
             }
 
         elif message_type == "REACTION":
             message["content"]["reaction"] = {
@@ -95,19 +102,19 @@
             }
 
         response = self._client.post(
             self._client.host(), "/whatsapp/v2/send", params={"messages": [message]})
         log.info("Message sent successfully.")
         return response
 
-    def send_whatsapp_templated_message(self, originator: str, recipient: str, template_id: str,
+    def send_whatsapp_templated_message(self, originator: str, recipient: str, template_id: str, language: str,
                                         body_parameter_values: dict = {}, media_type: str = None,
-                                        media_url: str = None,
-                                        latitude: str = None, longitude: str = None, location_name: str = None,
-                                        location_address: str = None, lto_expiration_time_ms: str = None,
+                                        text_header_title: str = None, media_url: str = None,
+                                        latitude: str = None, longitude: str = None, name: str = None,
+                                        address: str = None, lto_expiration_time_ms: str = None,
                                         coupon_code: str = None, quick_replies: dict = None, actions: dict = None,
                                         carousel_cards: list = []):
         """
         Send a WhatsApp message to a single/multiple recipients.
         :param originator: str - The message originator.
         :param recipient: str - The message recipient.
         :param template_id: str - The template ID for text messages.
@@ -116,29 +123,33 @@
         :param media_url: str - The URL of the media content.
         """
         message = {
             "originator": originator,
             "recipients": [{"recipient": recipient}],
             "content": {
                 "message_type": "TEMPLATE",
-                "template": {"template_id": template_id, "body_parameter_values": body_parameter_values}
+                "template": {"template_id": template_id, "language": language,
+                             "body_parameter_values": body_parameter_values}
             }
         }
 
         if media_type:
             if media_type == "location":
                 message["content"]["template"]["media"] = {
                     "media_type": "location",
                     "location": {
                         "latitude": latitude,
                         "longitude": longitude,
-                        "name": location_name,
-                        "address": location_address
+                        "name": name,
+                        "address": address
                     }
                 }
+            elif media_type == "text":
+                message["content"]["template"]["media"] = {
+                    "media_type": media_type, "text_header_title": text_header_title}
             else:
                 message["content"]["template"]["media"] = {
                     "media_type": media_type, "media_url": media_url}
         if lto_expiration_time_ms:
             message["content"]["template"]["limited_time_offer"] = {
                 "expiration_time_ms": lto_expiration_time_ms
             }
```

### Comparing `direct7-0.0.7/tests/test_sdk.py` & `direct7-0.0.8/tests/test_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,24 +89,44 @@
     # attachment: Sticker
     response_send_messages = client.whatsapp.send_whatsapp_freeform_message(originator="+XXXXXXXXXXXX",
                                                                             recipient="XXXXXXXXXXXX",
                                                                             message_type="ATTACHMENT", type="sticker",
                                                                             url="https://raw.githubusercontent.com/sagarbhavsar4328/dummys3bucket/master/sample3.webp")
     # location
     response_send_messages = client.whatsapp.send_whatsapp_freeform_message(originator="+XXXXXXXXXXXX",
-                                                                           recipient="XXXXXXXXXXXX",
-                                                                            message_type="LOCATION", latitude="12.93803129081362",
+                                                                            recipient="XXXXXXXXXXXX",
+                                                                            message_type="LOCATION",
+                                                                            latitude="12.93803129081362",
                                                                             longitude="77.61088653615994",
-                                                                            name="Mobile Pvt Ltd", address="30, Hosur Rd, 7th Block, Koramangala, Bengaluru, Karnataka 560095")
+                                                                            name="Mobile Pvt Ltd",
+                                                                            address="30, Hosur Rd, 7th Block, Koramangala, Bengaluru, Karnataka 560095")
+
+    # templated: location
+    response_send_messages = client.whatsapp.send_whatsapp_templated_message(originator="+971563287051",
+                                                                             recipient="+918086757074",
+                                                                             template_id="location", language="en",
+                                                                             media_type="location",
+                                                                             latitude="12.93803129081362",
+                                                                             longitude="77.61088653615994",
+                                                                             name="Mobile Pvt Ltd",
+                                                                             address="30, Hosur Rd, 7th Block, Koramangala, Bengaluru, Karnataka 560095")
+
+    # templated: text
+    response_send_messages = client.whatsapp.send_whatsapp_templated_message(originator="+971563287051",
+                                                                             recipient="+918086757074",
+                                                                             template_id="header_param", language="en",
+                                                                             media_type="text",
+                                                                             text_header_title="Ds")
 
     # lto
     response_send_messages = client.whatsapp.send_whatsapp_templated_message(originator="+XXXXXXXXXXX",
                                                                              recipient="XXXXXXXXXXXXX",
                                                                              template_id="limited_time_offer",
-                                                                             media_type="image", media_url="https://upload.wikimedia.org",
+                                                                             media_type="image",
+                                                                             media_url="https://upload.wikimedia.org",
                                                                              lto_expiration_time_ms="1708804800000",
                                                                              coupon_code="DWS44")
     # Action
     actions = [
         {
             "action_type": "url",
             "action_index": "0",
@@ -188,24 +208,25 @@
                                                                             message_type="REACTION",
                                                                             message_id="f1a99798-11aa-11ef-9821-0242ac1b0030",
                                                                             emoji="\U0001F600")
 
     # interactive cta_url: text
 
     parameters = {
-              "display_text": "Visit Alpha",
-              "url": "https://www.luckyshrub.com?clickID=kqDGWd24Q5TRwoEQTICY7W1JKoXvaZOXWAS7h1P76s0R7Paec4"
-            }
+        "display_text": "Visit Alpha",
+        "url": "https://www.luckyshrub.com?clickID=kqDGWd24Q5TRwoEQTICY7W1JKoXvaZOXWAS7h1P76s0R7Paec4"
+    }
     response_send_messages = client.whatsapp.send_whatsapp_interactive_message(originator="+XXXXXXXXXXXX",
                                                                                recipient="XXXXXXXXXXXX",
                                                                                interactive_type="cta_url",
                                                                                header_type="text",
                                                                                header_text="Payment$ for D7 Whatsapp Service",
                                                                                body_text="Direct7 Networks is a messaging service provider that specializes in helping organizations efficiently communicate with their customers.",
-                                                                               footer_text="Thank You", parameters=parameters)
+                                                                               footer_text="Thank You",
+                                                                               parameters=parameters)
 
     ## interactive cta_url: image
 
     parameters = {
         "display_text": "Visit Alpha",
         "url": "https://www.luckyshrub.com?clickID=kqDGWd24Q5TRwoEQTICY7W1JKoXvaZOXWAS7h1P76s0R7Paec4"
     }
@@ -217,36 +238,36 @@
                                                                                body_text="Direct7 Networks is a messaging service provider that specializes in helping organizations efficiently communicate with their customers.",
                                                                                footer_text="Thank You",
                                                                                parameters=parameters)
 
     # interactive button: image
 
     buttons = [
-              {
-                "type": "reply",
-                "reply": {
-                  "id": "1",
-                  "title": "Debit Card"
-                }
-              },
-              {
-                "type": "reply",
-                "reply": {
-                  "id": "2",
-                  "title": "Credit Card"
-                }
-              },
-              {
-                "type": "reply",
-                "reply": {
-                  "id": "3",
-                  "title": "Cash"
-                }
-              }
-            ]
+        {
+            "type": "reply",
+            "reply": {
+                "id": "1",
+                "title": "Debit Card"
+            }
+        },
+        {
+            "type": "reply",
+            "reply": {
+                "id": "2",
+                "title": "Credit Card"
+            }
+        },
+        {
+            "type": "reply",
+            "reply": {
+                "id": "3",
+                "title": "Cash"
+            }
+        }
+    ]
     response_send_messages = client.whatsapp.send_whatsapp_interactive_message(originator="+XXXXXXXXXXXX",
                                                                                recipient="XXXXXXXXXXXX",
                                                                                interactive_type="button",
                                                                                header_type="image",
                                                                                header_link="https://karix.s3.ap-south-1.amazonaws.com/English-4.jpg",
                                                                                body_text="Direct7 Networks is a messaging service provider that specializes in helping organizations efficiently communicate with their customers.",
                                                                                footer_text="Thank You",
@@ -301,7 +322,8 @@
     print(response_get_status)
     assert response_get_status is not None
     assert response_get_status
 
 
 if __name__ == "__main__":
     test_send_messages()
+    test_get_status()
```

### Comparing `direct7-0.0.7/.gitignore` & `direct7-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/LICENSE` & `direct7-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/README.md` & `direct7-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `direct7-0.0.7/pyproject.toml` & `direct7-0.0.8/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "direct7"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Direct7 Networks", email="support@d7networks.com" },
 ]
 description = "Python SDK for Direct7  Platform REST API"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests == 2.31.0"
 
-[project.requires]
-requests = "2.31.0"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/d7networks/direct7-python-sdk"
 "Bug Tracker" = "https://github.com/d7networks/direct7-python-sdk/issues"
```

### Comparing `direct7-0.0.7/PKG-INFO` & `direct7-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.2
+Metadata-Version: 2.3
 Name: direct7
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python SDK for Direct7  Platform REST API
 Project-URL: Homepage, https://github.com/d7networks/direct7-python-sdk
 Project-URL: Bug Tracker, https://github.com/d7networks/direct7-python-sdk/issues
 Author-email: Direct7 Networks <support@d7networks.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+Requires-Dist: requests==2.31.0
 Description-Content-Type: text/markdown
 
 # Direct7 Python SDK
 
 Python SDK to seamlessly incorporate communication features into your Python applications via the Direct7 REST API. This SDK empowers you to effortlessly initiate SMS,Whatsapp, Slack, Viber  messages and 2 factor authentication features.
 
 ## Documentation
```

