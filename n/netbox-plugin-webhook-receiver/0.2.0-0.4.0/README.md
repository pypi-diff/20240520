# Comparing `tmp/netbox_plugin_webhook_receiver-0.2.0.tar.gz` & `tmp/netbox_plugin_webhook_receiver-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_webhook_receiver-0.2.0.tar", max compression
+gzip compressed data, was "netbox_plugin_webhook_receiver-0.4.0.tar", max compression
```

## Comparing `netbox_plugin_webhook_receiver-0.2.0.tar` & `netbox_plugin_webhook_receiver-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1076 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/LICENSE
--rw-r--r--   0        0        0     1980 2023-07-04 22:34:07.960443 netbox_plugin_webhook_receiver-0.2.0/README.md
--rw-r--r--   0        0        0      502 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 09:47:06.597516 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/api/__init__.py
--rw-r--r--   0        0        0     1446 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/api/serializers.py
--rw-r--r--   0        0        0      274 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/api/urls.py
--rw-r--r--   0        0        0      621 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/api/views.py
--rw-r--r--   0        0        0      441 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/choices.py
--rw-r--r--   0        0        0      733 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/filtersets.py
--rw-r--r--   0        0        0     2895 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/forms.py
--rw-r--r--   0        0        0     4903 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/migrations/0001_initial.py
--rw-r--r--   0        0        0      428 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/migrations/0002_webhookreceiver_hash_algorithm.py
--rw-r--r--   0        0        0        0 2023-07-03 12:00:32.102516 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/migrations/__init__.py
--rw-r--r--   0        0        0     3261 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/models.py
--rw-r--r--   0        0        0      969 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/navigation.py
--rw-r--r--   0        0        0     1172 2023-07-04 15:19:05.740989 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/tables.py
--rw-r--r--   0        0        0     2981 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html
--rw-r--r--   0        0        0     1375 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html
--rw-r--r--   0        0        0     1789 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/urls.py
--rw-r--r--   0        0        0      133 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/__init__.py
--rw-r--r--   0        0        0     3819 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/views.py
--rw-r--r--   0        0        0      765 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/webhookreceiver.py
--rw-r--r--   0        0        0     1122 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/webhookreceivergroup.py
--rw-r--r--   0        0        0      735 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 netbox_plugin_webhook_receiver-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2311 2023-07-06 10:02:50.221980 netbox_plugin_webhook_receiver-0.4.0/README.md
+-rw-r--r--   0        0        0      502 2024-05-17 09:36:34.482282 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:47:06.597516 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/__init__.py
+-rw-r--r--   0        0        0     1358 2024-05-17 10:32:54.491861 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/serializers.py
+-rw-r--r--   0        0        0      274 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/urls.py
+-rw-r--r--   0        0        0      621 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/views.py
+-rw-r--r--   0        0        0      441 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/choices.py
+-rw-r--r--   0        0        0      733 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/filtersets.py
+-rw-r--r--   0        0        0     2930 2024-05-17 09:51:37.476254 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/forms.py
+-rw-r--r--   0        0        0     4903 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/0001_initial.py
+-rw-r--r--   0        0        0      428 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/0002_webhookreceiver_hash_algorithm.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:00:32.102516 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/__init__.py
+-rw-r--r--   0        0        0     3261 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/models.py
+-rw-r--r--   0        0        0      840 2024-05-17 09:55:22.379420 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/navigation.py
+-rw-r--r--   0        0        0     1172 2023-07-04 15:19:05.740989 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/tables.py
+-rw-r--r--   0        0        0     2929 2024-05-17 13:01:52.483716 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html
+-rw-r--r--   0        0        0     1264 2024-05-17 10:02:32.566523 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html
+-rw-r--r--   0        0        0     1789 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/urls.py
+-rw-r--r--   0        0        0      133 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/__init__.py
+-rw-r--r--   0        0        0     3819 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/views.py
+-rw-r--r--   0        0        0      765 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceiver.py
+-rw-r--r--   0        0        0     1122 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceivergroup.py
+-rw-r--r--   0        0        0      736 2024-05-17 12:06:08.905691 netbox_plugin_webhook_receiver-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 netbox_plugin_webhook_receiver-0.4.0/PKG-INFO
```

### Comparing `netbox_plugin_webhook_receiver-0.2.0/LICENSE` & `netbox_plugin_webhook_receiver-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/README.md` & `netbox_plugin_webhook_receiver-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 <h1 align="center">NetBox Webhook Receiver</h1>
 
 <p align="center"><i>NetBox Webhook Receiver is a NetBox plugin for managing webhook receiver endpoints and executing assigned actions.</i></p>
 
-This plugin aims mainly to streamline the deployment process of scripts and export templates to Netbox by triggering the synchronisation of its Data Sources through incomming webhooks. Adding the receiver capability to Netbox opens other possible use cases, which might be worth exploring further. One exemple could be running Netbox Scripts triggered by remote events where it is not easy to execute a direct API call.
+This plugin aims mainly to streamline the deployment process of scripts and export templates to Netbox by triggering the synchronisation of its Data Sources through incoming webhooks. Adding the receiver capability to Netbox opens other possible use cases, which might be worth exploring further. One example could be running Netbox Scripts triggered by remote events where it is not easy to execute a direct API call.
 
 ## Features
 - [x] Per endpoint authentication (signature validation or custom header) on receiving webhooks
 - [x] Webhook url enriched with automaticaly generated uuid value for additional security
 - [x] Dedicated view to configure each webhook receiver url
 - [x] Logical grouping of the receivers
-- [x] Optionally store incomming webhook payload
+- [x] Optionally store incoming webhook payload
 - [x] Custom actions execution on successfully receving authenticated webhook message. Currently only one action available: Synchronize Netbox git 'Data Source'
-- [x] Use of standard Netbox jobs to enqueue webhook actions in the workers.
+- [x] Use of standard Netbox jobs to queue webhook actions in the workers.
 - [ ] Additional actions to be implemented
 - [ ] Plugin configuration parameters
 
 ## Requirements
 
 * NetBox 3.5 or higher
 * Python 3.10 or higher
 
 ## Installation & Configuration
 
-For all netbox plugin installations please refer to the oficial guide: [Using Plugins - NetBox Documentation](https://netbox.readthedocs.io/en/stable/plugins/)
+For general knowledge about netbox plugin installation please refer to the official guide: [Using Plugins - NetBox Documentation](https://netbox.readthedocs.io/en/stable/plugins/)
 
-Please remember that this plugin introduces new database models, therefore you must run the provided database schema migrations:
+Install NetBox Webhook Receiver:
+```bash
+$ source /opt/netbox/venv/bin/activate
+(venv) $ pip install netbox-plugin-webhook-receiver
 ```
+
+To register this plugin in NetBox, add _netbox_webhook_receiver_ to the config file. `~/netbox/configuration.py`
+
+```python
+PLUGINS = [
+    "netbox_webhook_receiver",
+]
+```
+
+Please remember that this plugin introduces new database models, therefore you must run the provided database schema migrations:
+```bash
 $ source /opt/netbox/venv/bin/activate
 (venv) $ cd /opt/netbox/netbox/
 (venv) $ python3 manage.py migrate
 ```
 
 ## Screenshots
```

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/api/serializers.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from rest_framework import serializers
 
-# from ipam.api.serializers import NestedPrefixSerializer
-from netbox.api.serializers import NetBoxModelSerializer  # , WritableNestedSerializer
+from netbox.api.serializers import NetBoxModelSerializer
 from ..models import WebhookReceiver, WebhookReceiverGroup
 
 
 class WebhookReceiverSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_webhook_receiver-api:webhookreceiver-detail"
     )
```

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/api/views.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/filtersets.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/forms.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/forms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from django import forms
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
 from utilities.forms.fields import CommentField
+from utilities.forms.rendering import FieldSet
 from utilities.forms.utils import get_field_value
 from utilities.forms.widgets import HTMXSelect
 from .choices import WebhookAuthMethodChoices
 from .models import WebhookReceiver, WebhookReceiverGroup
 
 
 class WebhookReceiverForm(NetBoxModelForm):
     comments = CommentField()
 
     fieldsets = (
-        (
-            "Webhook definition",
-            (
+        FieldSet(
                 "name",
                 "receiver_group",
                 "description",
                 "uuid",
                 "store_payload",
+                name="Webhook definition"
             ),
-        ),
-        (
-            "Authentication",
-            ("auth_method", "auth_header", "secret_key", "token", "hash_algorithm"),
-        ),
-        ("Trigger action", ("datasource",)),
-        ("Extra", ("tags")),
+        FieldSet("auth_method", "auth_header", "secret_key", "token", "hash_algorithm", name="Authentication"),
+        FieldSet("datasource", name="Trigger action"),
+        FieldSet("tags", name="Extra"),
     )
 
     # Thanks to Dillon Henschen for his netbox pull #12675
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         auth_method = get_field_value(self, "auth_method")
```

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/migrations/0001_initial.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/models.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/tables.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 {% load render_table from django_tables2 %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Webhook Receiver</h5>
-        <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
               <th scope="row">Description</th>
@@ -43,22 +42,20 @@
               <td>{{ object.hash_algorithm|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Secret Key</th>
               <td>{{ object.secret_key|placeholder }}</td>
             </tr>
           </table>
-        </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Webhook actions</h5>
-        <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Store payload</th>
               <td>{{ object.store_payload|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Update datasource</th>
@@ -67,26 +64,27 @@
               </td>
             </tr>
             <tr>
               <th scope="row">Run Custom Script</th>
               <td>{{ object.customscript|placeholder }}</td>
             </tr>
           </table>
-        </div>
       </div>
     <!-- </div> -->
     <!-- <div class="col col-md-6"> -->
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Webhook Receiver URL</h5>
-        <div class="card-body">
-          {{request.headers.referer | split:"/" | slice:"5" | join:"/" }}/webhooks/{{ object.uuid}}/
-        </div>
+        <table class="table">
+          <tr>
+            <td>{{request.headers.referer | split:"/" | slice:"5" | join:"/" }}/webhooks/{{ object.uuid}}/</td>
+          </tr>
+        </table>
       </div>
     </div>
   </div>
 {% endblock content %}
```

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 {% load render_table from django_tables2 %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Webhook Receiver Group</h5>
-        <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
             <tr>
               <th scope="row">Description</th>
@@ -21,27 +20,24 @@
               <td>{{ object.tenant }}</td>
             </tr>
             <tr>
               <th scope="row">Related receivers</th>
               <td>{{ object.receivers.count }}</td>
             </tr>
           </table>
-        </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Receivers</h5>
-        <div class="card-body table-responsive">
           {% render_table receivers_table %}
-        </div>
       </div>
     </div>
   </div>
 {% endblock content %}
```

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/urls.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/views.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/webhookreceiver.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceiver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/netbox_webhook_receiver/views/webhookreceivergroup.py` & `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceivergroup.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.2.0/PKG-INFO` & `netbox_plugin_webhook_receiver-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-webhook-receiver
-Version: 0.2.0
+Version: 0.4.0
 Summary: NetBox Webhook is a plugin for managing webhook receivers in NetBox.
 Home-page: https://github.com/LuPo/netbox-plugin-webhook-receiver
 License: MIT
 Keywords: netbox,netbox-plugin,webhook
 Author: Łukasz Polański
 Author-email: wookasz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/LuPo/netbox-plugin-webhook-receiver
 Description-Content-Type: text/markdown
 
 <h1 align="center">NetBox Webhook Receiver</h1>
 
 <p align="center"><i>NetBox Webhook Receiver is a NetBox plugin for managing webhook receiver endpoints and executing assigned actions.</i></p>
 
-This plugin aims mainly to streamline the deployment process of scripts and export templates to Netbox by triggering the synchronisation of its Data Sources through incomming webhooks. Adding the receiver capability to Netbox opens other possible use cases, which might be worth exploring further. One exemple could be running Netbox Scripts triggered by remote events where it is not easy to execute a direct API call.
+This plugin aims mainly to streamline the deployment process of scripts and export templates to Netbox by triggering the synchronisation of its Data Sources through incoming webhooks. Adding the receiver capability to Netbox opens other possible use cases, which might be worth exploring further. One example could be running Netbox Scripts triggered by remote events where it is not easy to execute a direct API call.
 
 ## Features
 - [x] Per endpoint authentication (signature validation or custom header) on receiving webhooks
 - [x] Webhook url enriched with automaticaly generated uuid value for additional security
 - [x] Dedicated view to configure each webhook receiver url
 - [x] Logical grouping of the receivers
-- [x] Optionally store incomming webhook payload
+- [x] Optionally store incoming webhook payload
 - [x] Custom actions execution on successfully receving authenticated webhook message. Currently only one action available: Synchronize Netbox git 'Data Source'
-- [x] Use of standard Netbox jobs to enqueue webhook actions in the workers.
+- [x] Use of standard Netbox jobs to queue webhook actions in the workers.
 - [ ] Additional actions to be implemented
 - [ ] Plugin configuration parameters
 
 ## Requirements
 
 * NetBox 3.5 or higher
 * Python 3.10 or higher
 
 ## Installation & Configuration
 
-For all netbox plugin installations please refer to the oficial guide: [Using Plugins - NetBox Documentation](https://netbox.readthedocs.io/en/stable/plugins/)
+For general knowledge about netbox plugin installation please refer to the official guide: [Using Plugins - NetBox Documentation](https://netbox.readthedocs.io/en/stable/plugins/)
 
-Please remember that this plugin introduces new database models, therefore you must run the provided database schema migrations:
+Install NetBox Webhook Receiver:
+```bash
+$ source /opt/netbox/venv/bin/activate
+(venv) $ pip install netbox-plugin-webhook-receiver
 ```
+
+To register this plugin in NetBox, add _netbox_webhook_receiver_ to the config file. `~/netbox/configuration.py`
+
+```python
+PLUGINS = [
+    "netbox_webhook_receiver",
+]
+```
+
+Please remember that this plugin introduces new database models, therefore you must run the provided database schema migrations:
+```bash
 $ source /opt/netbox/venv/bin/activate
 (venv) $ cd /opt/netbox/netbox/
 (venv) $ python3 manage.py migrate
 ```
 
 ## Screenshots
```

