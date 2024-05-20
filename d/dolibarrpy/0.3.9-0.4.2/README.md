# Comparing `tmp/dolibarrpy-0.3.9.tar.gz` & `tmp/dolibarrpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibarrpy-0.3.9.tar", last modified: Mon Apr 22 21:26:52 2024, max compression
+gzip compressed data, was "dolibarrpy-0.4.2.tar", last modified: Mon May 20 12:59:14 2024, max compression
```

## Comparing `dolibarrpy-0.3.9.tar` & `dolibarrpy-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-22 21:26:52.440897 dolibarrpy-0.3.9/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.3.9/LICENSE.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      868 2024-04-22 21:26:52.441067 dolibarrpy-0.3.9/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      441 2024-04-20 10:12:59.000000 dolibarrpy-0.3.9/README.md
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-22 21:26:52.438854 dolibarrpy-0.3.9/dolibarrpy/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)    58744 2024-04-22 21:22:54.000000 dolibarrpy-0.3.9/dolibarrpy/Dolibarrpy.py
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.3.9/dolibarrpy/__init__.py
-drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-04-22 21:26:52.440616 dolibarrpy-0.3.9/dolibarrpy.egg-info/
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      868 2024-04-22 21:26:52.000000 dolibarrpy-0.3.9/dolibarrpy.egg-info/PKG-INFO
--rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-04-22 21:26:52.000000 dolibarrpy-0.3.9/dolibarrpy.egg-info/SOURCES.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-04-22 21:26:52.000000 dolibarrpy-0.3.9/dolibarrpy.egg-info/dependency_links.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-04-22 21:26:52.000000 dolibarrpy-0.3.9/dolibarrpy.egg-info/top_level.txt
--rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-04-22 21:26:52.441578 dolibarrpy-0.3.9/setup.cfg
--rw-r--r--   0 jonbendtsen   (501) staff       (20)     1261 2024-04-22 21:26:34.000000 dolibarrpy-0.3.9/setup.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-05-20 12:59:14.907082 dolibarrpy-0.4.2/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1062 2024-04-20 10:12:59.000000 dolibarrpy-0.4.2/LICENSE.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      868 2024-05-20 12:59:14.907231 dolibarrpy-0.4.2/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      587 2024-04-29 20:27:21.000000 dolibarrpy-0.4.2/README.md
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-05-20 12:59:14.904868 dolibarrpy-0.4.2/dolibarrpy/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)    66481 2024-05-20 12:50:29.000000 dolibarrpy-0.4.2/dolibarrpy/Dolibarrpy.py
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       45 2024-04-20 12:08:04.000000 dolibarrpy-0.4.2/dolibarrpy/__init__.py
+drwxr-xr-x   0 jonbendtsen   (501) staff       (20)        0 2024-05-20 12:59:14.906784 dolibarrpy-0.4.2/dolibarrpy.egg-info/
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      868 2024-05-20 12:59:14.000000 dolibarrpy-0.4.2/dolibarrpy.egg-info/PKG-INFO
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)      249 2024-05-20 12:59:14.000000 dolibarrpy-0.4.2/dolibarrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)        1 2024-05-20 12:59:14.000000 dolibarrpy-0.4.2/dolibarrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       11 2024-05-20 12:59:14.000000 dolibarrpy-0.4.2/dolibarrpy.egg-info/top_level.txt
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)       79 2024-05-20 12:59:14.907662 dolibarrpy-0.4.2/setup.cfg
+-rw-r--r--   0 jonbendtsen   (501) staff       (20)     1261 2024-05-20 12:56:48.000000 dolibarrpy-0.4.2/setup.py
```

### Comparing `dolibarrpy-0.3.9/LICENSE.txt` & `dolibarrpy-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolibarrpy-0.3.9/PKG-INFO` & `dolibarrpy-0.4.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.3.9
+Version: 0.4.2
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: This project is a python wrapper for the API for Dolibarr ERP & CRM found at dolibarr.org. It is not yet complete, but most major GET endpoints has been implemented. In the beginning I will mostly focus on implementing the API endpoints that I use.
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.3.9/dolibarrpy/Dolibarrpy.py` & `dolibarrpy-0.4.2/dolibarrpy/Dolibarrpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,14 +121,25 @@
     sortorder: Optional[str] = None
     limit: Optional[int] = None
     page: Optional[int] = None
     thirdparty_ids: Optional[str] = None
     sqlfilters: Optional[str] = None    # Syntax example "(t.statut:=:1)
     properties: Optional[str] = None        # Restrict the data returned to theses properties. Ignored if empty. Comma separated list of properties names
 
+@dataclass
+class UserFilter():
+    sortfield: Optional[str] = None
+    sortorder: Optional[str] = None
+    limit: Optional[int] = None
+    page: Optional[int] = None
+    user_ids: Optional[str] = None
+    category: Optional[int] = None      # only get members with this status: draft | unpaid | paid | cancelled
+    sqlfilters: Optional[str] = None    # Syntax example "(t.statut:=:1)
+    properties: Optional[str] = None        # Restrict the data returned to theses properties. Ignored if empty. Comma separated list of properties names
+
 
 class Dolibarrpy():
     url = 'https://dolibarr.example.com/api/index.php/'
     token = 'your token'
     timeout = 16
     debug = False
 
@@ -173,17 +184,23 @@
     def call_get_api(self, object, objid):
         url = self.url + object + '/' + str(objid)
         headers = self.get_headers()
         response = requests.get(url, headers=headers, timeout=self.timeout)
         if self.debug:
             ic(url)
             ic(response)
-        json_result = json.loads(response.text)
-
-        return json_result
+            ic(response.text)
+        try:
+            result = json.loads(response.text)
+        except json.decoder.JSONDecodeError:
+            result = { "error": response }
+        except:
+            _logger.error('LIST API ERROR: ' + object)
+            result = response.text
+        return result
 
     def call_create_api(self, object, params={}):
         url = self.url + object
         headers = self.get_headers()
         response = requests.post(url, json=params, headers=headers, timeout=self.timeout)
         try:
             result = json.loads(response.text)
@@ -225,33 +242,38 @@
             result = json.loads(response.text)
         except:
             result = False
         return result
 
     def get_orders_by_status(self, status):
         """
+        @endpoint 'get /orders'
         Get orders by status
         @param status: 0 => draft, 1 => validated
         @return: list of orders
         """
         params = {
             'limit': 500,
             'sqlfilters': "(fk_statut:=:{})".format(status)
         }
 
         result = self.call_list_api('orders', params=params)
         return result
 
     def get_order_by_id(self, objid):
+        """
+        @endpoint 'get /orders/{id}'
+        """
         result = self.call_get_api('orders', objid=objid)
         return result
 
     # SHIPMENTS
     def find_all_shipments(self, from_ShipmentFilter = None):
         """
+        @endpoint 'get /shipments'
         Get all shipments
         @param from_ShipmentFilter:
         @return: list of a shipments
         """
         if self.debug:
             ic()
             ic(from_ShipmentFilter)
@@ -287,42 +309,49 @@
             search_filter = from_ShipmentFilter
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('shipments', params)
         return result
 
     def get_shipment_by_id(self, objid):
+        """
+        @endpoint 'get /shipments/{id}'
+        """
         result = self.call_get_api('shipments', objid=objid)
         return result
 
     def update_shipment_tracking(self, objid, tracking_id, shipping_method=0):
         params = {
             'tracking_number': tracking_id
         }
 
         if shipping_method:
             params.update({'shipping_method_id': shipping_method})
 
         self.call_update_api('shipments', objid, params=params)
 
     def get_shipments_by_orderid(self, order_id):
+        """
+        @endpoint 'get /orders/{id}/shipment'
+        """
         order = self.get_order_by_id(order_id)
         links = order.get('linkedObjectsIds')
         if links:
             shipment_list = links.get('shipping')
         else:
             shipment_list = self.call_list_api('shipments', params={})
         shipments = []
         for item in shipment_list:
             ship = self.get_shipment_by_id(shipment_list[item])
             shipments.append(ship)
         return shipments
 
     def get_shipments_by_status(self, status):
         """
+        @endpoint 'get /shipments'
         Get shipments by status
         @param status: 0 => draft, 1 => validated
         @return: list of shipments
         """
         params = {
             'limit': 500,
             'origin_id': 440,
@@ -330,14 +359,17 @@
         }
 
         # and (fk_shipping_method:=:9)
         erp_shipments = self.call_list_api('shipments', params=params)
         return erp_shipments
 
     def create_shipment_from_order(self, order_id, address_id=0, shipping_method_id=0, date_delivery=0, tracking_number=''):
+        """
+        @endpoint 'post /orders/{id}/shipment/{warehouse_id}'
+        """
         # This creates a complete fulfillment shipment for an order
         # get order
         order = self.get_order_by_id(order_id)
         # set defaults
         shipment_data = {
             'socid': order.get('socid'),
             "origin_type": "commande",
@@ -384,47 +416,60 @@
         #add lines to shipment
         shipment_data['lines'] = shiplines
         ship_id = self.call_create_api('shipments', shipment_data)
         return ship_id
 
 
     def set_shipment_to_validated(self, shipment_id):
+        """
+        @endpoint 'post /shipments/{id}/validate'
+        """
         params = {
           "notrigger": 0
         }
         return self.call_action_api('shipments', shipment_id, 'validate', params=params)
 
     # ORDERS
     def set_order_to_draft(self, order_id, idwarehouse=1):
+        """
+        @endpoint 'post /orders/{id}/settodraft'
+        """
         params = {
           "idwarehouse": idwarehouse
         }
         return self.call_action_api('orders', order_id, 'settodraft', params=params)
 
     def set_order_to_validated(self, order_id, idwarehouse=1):
+        """
+        @endpoint 'post /orders/{id}/validate'
+        """
         params = {
           "idwarehouse": idwarehouse
         }
         return self.call_action_api('orders', order_id, 'validate', params=params)
 
     # PRODUCTS
     def get_product_by_id(self, objid, includestockdata=1):
+        """
+        @endpoint 'get /products/{id}'
+        """
         if includestockdata == 1:
             objid = str(objid) + '?includestockdata=1'
         result = self.call_get_api('products', objid=objid)
         return result
 
     # Factory
     def get_factory_order_by_id(self, objid):
         result = self.call_get_api('factory', objid=objid)
         return result
 
     # PROJECTS
     def find_all_projects(self, with_status = ''):
         """
+        @endpoint 'get /projects'
         Get projects with status
         @param with_status: 0 => draft, 1 => open, 2=> closed
         @return: list of projects
         """
         all_projects=[]
         page = 0
         some_projects = self.find_some_projects(with_status, page)
@@ -456,42 +501,46 @@
             )
         params = asdict(search_filter)
         result = self.call_list_api('projects', params=params)
         return result
 
     def get_project_by_pid(self, objid):
         """
+        @endpoint 'get /projects/{id}'
         Get project based on project id
         @return: project 
         """
         result = self.call_get_api('projects', objid=objid)
         return result
 
     def get_project_tasks_by_pid(self, objid, includetimespent=0):
         """
+        @endpoint 'get /projects/{id}/tasks'
         Get project tasks based on project id
         @param includetimespent: 0 => Return only list of tasks, 1 => Include a summary of time spent, 2=> Include details of time spent lines
         @return: list of project tasks
         """
         objid = str(objid) + '/tasks?includetimespent=' + str(includetimespent)
         result = self.call_get_api('projects', objid)
         return result
 
     def get_project_roles_by_pid(self, objid, userid=0):
         """
+        @endpoint 'get /projects/{id}/roles'
         Get project roles based on project id
         @param userid: 0 => connected user, Any other number than 0 is interpretated as a user id and if that user has roles on that project, they are shown.
         @return: list of project roles
         """
         objid = str(objid) + '/roles?userid=' + str(userid)
         result = self.call_get_api('projects', objid)
         return result
 
     def get_project_by_ref(self, ref):
         """
+        @endpoint 'get /projects/ref/{ref}'
         Get project tasks based on project ref
         @return: project
         """
         if ref:
             ref = 'ref/' + urllib.parse.quote(ref)
             result = self.call_get_api('projects', ref)
             return result
@@ -500,14 +549,15 @@
         elif ref is None:
             raise Exception("ref can not be None")
         else:
             raise Exception("ref is wrong")
 
     def get_project_by_ref_ext(self, ref_ext):
         """
+        @endpoint 'get /projects/ref_ext/{ref_ext}'
         Get project tasks based on project ref_ext
         @return: project
         """
         if ref_ext:
             ref_ext = 'ref_ext/' + urllib.parse.quote(ref_ext)
             result = self.call_get_api('projects', ref_ext)
             return result
@@ -516,14 +566,15 @@
         elif ref_ext is None:
             raise Exception("ref_ext can not be None")
         else:
             raise Exception("ref_ext is wrong")
 
     def get_project_by_email_msgid(self, email_msgid):
         """
+        @endpoint 'get /projects/email_msgid/{email_msgid}'
         Get project tasks based on project email_msgid
         @return: project
         """
         if email_msgid:
             email_msgid = 'email_msgid/' + urllib.parse.quote(email_msgid)
             result = self.call_get_api('projects', email_msgid)
             return result
@@ -534,14 +585,15 @@
         else:
             raise Exception("email_msgid is wrong")
 
 
     # MEMBERS
     def find_all_members(self, from_MemberFilter = None):
         """
+        @endpoint 'get /members'
         Get members with status
         @param from_MemberFilter: 0 => draft, 1 => open, 2=> closed
         @return: list of members
         """
         if self.debug:
             ic()
             ic(from_MemberFilter)
@@ -579,58 +631,64 @@
         if 0 == limit:
             raise Exception("sorry, but a limit if 0 does not make sense, be sensible")
         result = self.call_list_api('members', params=params)
         return result
 
     def get_member_by_mid(self, objid):
         """
+        @endpoint 'get /members/{id}'
         Get member based on member id
         @return: member
         """
         result = self.call_get_api('members', objid=objid)
         return result
 
     def get_member_subscriptions_by_mid(self, objid):
         """
+        @endpoint 'get /members/{id}/subscriptions'
         Get member subscriptions based on member id
         @return: list of member subscriptions
         """
         objid = str(objid) + '/subscriptions'
         result = self.call_get_api('members', objid)
         return result
 
     def get_member_by_thirdparty_id(self, objid):
         """
+        @endpoint 'get /members/thirdparty/{thirdparty}'
         Get member based on thirdparty id
         @return: member
         """
         objid = 'thirdparty/' + str(objid)
         result = self.call_get_api('members', objid)
         return result
 
     def get_member_by_thirdparty_barcode(self, barcode):
         """
+        @endpoint 'get /members/thirdparty/barcode/{barcode}'
         Get member based on thirdparty barcode
         @return: member
         """
         objid = 'thirdparty/barcode/' + str(barcode)
         result = self.call_get_api('members', objid)
         return result
 
     def get_member_by_thirdparty_email(self, email):
         """
+        @endpoint 'get /members/thirdparty/email/{email}'
         Get member based on thirdparty email
         @return: member
         """
         objid = 'thirdparty/email/' + str(email)
         result = self.call_get_api('members', objid)
         return result
 
     def find_all_member_types(self, from_MemberFilter = None):
         """
+        @endpoint 'get /members/types'
         Get member_types
         @param from_MemberFilter: 0 => draft, 1 => open, 2=> closed
         @return: list of member_types
         """
         if self.debug:
             ic()
             ic(from_MemberFilter)
@@ -674,14 +732,15 @@
         if typeid:
             raise Exception("sorry, you can not use typeid in this filter, try without")
         result = self.call_list_api('members/types', params=params)
         return result
 
     def get_all_member_categories_by_mid(self, objid, from_MemberFilter = None):
         """
+        @endpoint 'get /members/{id}/categories'
         Get all categories for a member
         @param from_MemberFilter:
         @return: list of a members categories
         """
         if self.debug:
             ic()
             ic(from_MemberFilter)
@@ -740,14 +799,15 @@
             ic(result)
         return result
 
 
     # THIRDPARTIES
     def find_all_thirdparty(self, from_ThirdpartyFilter = None):
         """
+        @endpoint 'get /thirdparties'
         Get all thirdparties
         @param from_ThirdpartyFilter:
         @return: list of a thirdparties
         """
         if self.debug:
             ic()
             ic(from_ThirdpartyFilter)
@@ -784,116 +844,130 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('thirdparties', params)
         return result
 
     def get_thirdparty_by_tid(self, objid):
         """
+        @endpoint 'get /thirdparties/{id}'
         Get thirdparty based on thirdparty id
         @return: thirdparty
         """
         result = self.call_get_api('thirdparties', objid=objid)
         return result
 
     def get_thirdparty_by_barcode(self, barcode):
         """
+        @endpoint 'get /thirdparties/barcode/{barcode}'
         Get thirdparty from barcode
         @return: thirdparty
         """
         objid = 'barcode/' + str(barcode)
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparty_by_email(self, email):
         """
-        Get member based on thirdparty email
+        @endpoint 'get /thirdparties/email/{email}'
+        Get thirdparty based on thirdparty email
         @return: thirdparty
         """
         objid = 'email/' + str(email)
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_bankaccounts_by_tid(self, objid):
         """
+        @endpoint 'get /thirdparties/{id}/bankaccounts'
         Get thirdparty bankaccounts based on thirdparty id
         @return: list of thirdparty bankaccounts
         """
         objid = str(objid) + '/bankaccounts'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_getinvoicesqualifiedforcreditnote_by_tid(self, objid):
         """
+        @endpoint 'get /thirdparties/{id}/getinvoicesqualifiedforcreditnote'
         Get thirdparty invoices qualifiedforcreditnote based on thirdparty id
         @return: list of thirdparty invoices qualifiedforcreditnote
         """
         objid = str(objid) + '/getinvoicesqualifiedforcreditnote'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_getinvoicesqualifiedforreplacement_by_tid(self, objid):
         """
+        @endpoint 'get /thirdparties/{id}/getinvoicesqualifiedforreplacement'
         Get thirdparty invoices qualifiedforreplacement based on thirdparty id
         @return: list of thirdparty invoices qualifiedforreplacement
         """
         objid = str(objid) + '/getinvoicesqualifiedforreplacement'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_notifications_by_tid(self, objid):
         """
+        @endpoint 'get /thirdparties/{id}/notifications'
         Get thirdparty notifications based on thirdparty id
         @return: list of thirdparty notifications
         """
         objid = str(objid) + '/notifications'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_outstanding_by_tid(self, objid, otype, mode):
         """
+        @endpoint 'get /thirdparties/{id}/outstandinginvoices'
+        @endpoint 'get /thirdparties/{id}/outstandingorders'
+        @endpoint 'get /thirdparties/{id}/outstandingproposals'
         Get thirdparty outstanding <otype> based on thirdparty id, otype and mode
         @otype string 'invoices', 'orders' or 'proposals' 
         @mode string 'customer' or 'supplier'
         @return: list of thirdparty's <otype> invoices
         """
         if mode:
             objid = str(objid) + '/outstanding' + otype + '?mode=' + mode
         else:
             objid = str(objid) + '/outstanding' + otype
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_representatives_by_tid(self, objid, mode):
         """
+        @endpoint 'get /thirdparties/{id}/representatives'
         Get thirdparty representatives based on thirdparty id and mode
         @mode string 0=Array with properties, 1=Array of id.
         @return: list of thirdparty's representatives
         """
         if mode:
             objid = str(objid) + '/representatives?mode=' + mode
         else:
             objid = str(objid) + '/representatives'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_accounts_by_tid(self, objid, site):
         """
+        @endpoint 'get /thirdparties/{id}/accounts'
         Get thirdparty accounts based on thirdparty id and site
         @mode string 0=Array with properties, 1=Array of id.
         @return: list of thirdparty's accounts
         """
         if site:
             objid = str(objid) + '/accounts?site=' + site
         else:
             objid = str(objid) + '/accounts'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_all_thirdparties_categories_by_tid(self, objid, from_ThirdpartyFilter = None, mode = 'customer'):
         """
+        @endpoint 'get /thirdparties/{id}/categories'
+        @endpoint 'get /thirdparties/{id}/supplier_categories'
         Get all categories for a thirdparties based on it's thirdparty_id
         @param from_ThirdpartyFilter:
         @mode string 'customer' or 'supplier'
         @return: list of a thirdpartiess categories
         """
         if self.debug:
             ic()
@@ -953,40 +1027,43 @@
             # assuming that they ask for customer
             api_path = 'thirdparties/' + str(objid) + '/categories'
         result = self.call_list_api(api_path, params)
         return result
 
     def get_thirdparties_fixedamountdiscounts_by_tid(self, objid, filter):
         """
+        @endpoint 'get /thirdparties/{id}/fixedamountdiscounts'
         Get thirdparty fixedamountdiscounts based on thirdparty id and filter
         @filter Filter exceptional discount. "none" will return every discount, "available" returns unapplied discounts, "used" returns applied discounts
         @return: list of thirdparty's fixedamountdiscounts
         """
         if filter:
             objid = str(objid) + '/fixedamountdiscounts?filter=' + filter
         else:
             objid = str(objid) + '/fixedamountdiscounts'
         result = self.call_get_api('thirdparties', objid)
         return result
 
     def get_thirdparties_generateBankAccountDocument_by_tid(self, objid, companybankid, model = 'sepamandate'):
         """
+        @endpoint 'get /thirdparties/{id}/generateBankAccountDocument/{companybankid}/{model}'
         Get thirdparty generateBankAccountDocument based on thirdparty id, companybankid and model
         @companybankid
         @model default is 'sepamandate'
         @return: list of thirdparty's accounts
         """
         objid = str(objid) + '/generateBankAccountDocument/' + str(companybankid) + '/' + str(model)
         result = self.call_get_api('thirdparties', objid)
         return result
 
 
     # CONTACTS
     def find_all_contacts(self, from_ContactFilter = None):
         """
+        @endpoint 'get /contacts'
         Get all contacts
         @param from_ContactFilter:
         @return: list of a contacts
         """
         if self.debug:
             ic()
             ic(from_ContactFilter)
@@ -1023,36 +1100,39 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('contacts', params)
         return result
 
     def get_contact_by_cid(self, objid, includecount = 0, includeroles = 0):
         """
+        @endpoint 'get /contacts/{id}'
         Get contact based on contact id
         @includecount Count and return also number of elements the contact is used as a link for
         @includeroles Includes roles of the contact
         @return: contact
         """
         objid = str(objid) + '?includecount=' + str(includecount) + '&includeroles=' + str(includeroles)
         result = self.call_get_api('contacts', objid=objid)
         return result
 
     def get_contact_by_email(self, email, includecount = 0, includeroles = 0):
         """
+        @endpoint 'get /contacts/email/{email}'
         Get contact based on contact email
         @includecount Count and return also number of elements the contact is used as a link for
         @includeroles Includes roles of the contact
         @return: contact
         """
         email = urllib.parse.quote(email) + '?includecount=' + str(includecount) + '&includeroles=' + str(includeroles)
         result = self.call_get_api('contacts/email', email)
         return result
 
     def get_all_contacts_categories_by_cid(self, objid, from_ContactFilter = None):
         """
+        @endpoint 'get /contacts/{id}/categories'
         Get all categories for a contact based on it's contact_id
         @param from_ContactFilter:
         @return: list of a contacts categories
         """
         if self.debug:
             ic()
             ic(from_ContactFilter)
@@ -1110,14 +1190,15 @@
         api_path = 'contacts/' + str(objid) + '/categories'
         result = self.call_list_api(api_path, params)
         return result
 
     # SUBSCRIPTIONS
     def find_all_subscriptions(self, from_SubscriptionFilter = None):
         """
+        @endpoint 'get /subscriptions'
         Get all subscriptions
         @param from_SubscriptionFilter:
         @return: list of a subscriptions
         """
         if self.debug:
             ic()
             ic(from_SubscriptionFilter)
@@ -1154,23 +1235,25 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('subscriptions', params)
         return result
 
     def get_subscription_by_sid(self, objid):
         """
+        @endpoint 'get /subscriptions/{id}'
         Get subscription based on subscription id
         @return: subscription
         """
         result = self.call_get_api('subscriptions', objid=objid)
         return result
 
     # PROPOSALS
     def find_all_proposals(self, from_ProposalFilter = None):
         """
+        @endpoint 'get /proposals'
         Get all proposals
         @param from_ProposalFilter:
         @return: list of a proposals
         """
         if self.debug:
             ic()
             ic(from_ProposalFilter)
@@ -1207,56 +1290,61 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('proposals', params)
         return result
 
     def get_proposal_by_pid(self, objid, contact_list = 1):
         """
+        @endpoint 'get /proposals/{id}'
         Get proposal based on proposal id
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: proposal
         """
         objid = str(objid) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('proposals', objid=objid)
         return result
 
     def get_proposal_by_ref(self, objref, contact_list = 1):
         """
+        @endpoint 'get /proposals/ref/{ref}'
         Get proposal based on proposal ref
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: proposal
         """
         objref = 'ref/' + urllib.parse.quote(objref) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('proposals', objid=objref)
         return result
 
     # 2024-04-22 doesn't work for me in my Dolibarr
     def get_proposal_by_ref_ext(self, objref_ext, contact_list = 1):
         """
+        @endpoint 'get /proposals/ref_ext/{ref_ext}'
         Get proposal based on proposal ref_ext
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: proposal
         """
         objref_ext = 'ref_ext/' + urllib.parse.quote(objref_ext) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('proposals', objid=objref_ext)
         return result
 
     def get_proposal_lines_by_pid(self, objid, sqlfilters):
         """
+        @endpoint 'get /proposals/{id}/lines'
         Get proposal lines based on proposal id
         @sqlfilters string Other criteria to filter answers separated by a comma. d is the alias for proposal lines table, p is the alias for product table. "Syntax example "(p.ref:like:'SO-%') AND (d.date_start:
         @return: proposal lines
         """
         objid = str(objid) + '/lines?sqlfilters=' + str(sqlfilters)
         result = self.call_get_api('proposals', objid=objid)
         return result
 
     # ORDERS
     def find_all_orders(self, from_OrderFilter = None):
         """
+        @endpoint 'get /orders'
         Get all orders
         @param from_OrderFilter:
         @return: list of a orders
         """
         if self.debug:
             ic()
             ic(from_OrderFilter)
@@ -1293,74 +1381,81 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('orders', params)
         return result
 
     def get_order_by_oid(self, objid, contact_list = 1):
         """
+        @endpoint 'get /orders/{id}'
         Get order based on order id
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: order
         """
         objid = str(objid) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('orders', objid=objid)
         return result
 
     def get_order_contacts_by_oid(self, objid, ctype = ''):
         """
+        @endpoint 'get /orders/{id}/contacts'
         Get order based on order id and contact type
         @ctype string Type of the contact (BILLING, SHIPPING, CUSTOMER)
         @return: order
         """
         objid = str(objid) + '/contacts?type=' + str(ctype)
         result = self.call_get_api('orders', objid=objid)
         return result
 
     def get_order_by_ref(self, objref, contact_list = 1):
         """
+        @endpoint 'get /orders/ref/{ref}'
         Get order based on order ref
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: order
         """
         objref = 'ref/' + urllib.parse.quote(objref) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('orders', objid=objref)
         return result
 
     # 2024-04-22 doesn't work for me in my Dolibarr
     def get_order_by_ref_ext(self, objref_ext, contact_list = 1):
         """
+        @endpoint 'get /orders/ref_ext/{ref_ext}'
         Get order based on order ref_ext
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: order
         """
         objref_ext = 'ref_ext/' + urllib.parse.quote(objref_ext) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('orders', objid=objref_ext)
         return result
 
     def get_order_lines_by_oid(self, objid):
         """
+        @endpoint 'get /orders/{id}/lines'
         Get order lines based on order id
         @return: order lines
         """
         objid = str(objid) + '/lines'
         result = self.call_get_api('orders', objid=objid)
         return result
 
     def get_order_shipment_by_oid(self, objid):
         """
+        @endpoint 'get /orders/{id}/shipment'
         Get order shipment based on order id
         @return: order shipment
         """
         objid = str(objid) + '/shipment'
         result = self.call_get_api('orders', objid=objid)
         return result
 
     # INVOICES
     def find_all_invoices(self, from_InvoiceFilter = None):
         """
+        @endpoint 'get /invoices'
         Get all invoices
         @param from_InvoiceFilter:
         @return: list of a invoices
         """
         if self.debug:
             ic()
             ic(from_InvoiceFilter)
@@ -1397,84 +1492,92 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('invoices', params)
         return result
 
     def get_invoice_by_iid(self, objid, contact_list = 1):
         """
+        @endpoint 'get /invoices/{id}'
         Get invoice based on invoice id
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: invoice
         """
         objid = str(objid) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('invoices', objid=objid)
         return result
 
     def get_invoice_discounts_by_iid(self, objid):
         """
+        @endpoint 'get /invoices/{id}/discount'
         Get invoice discounts based on invoice id
         @return: discount
         """
         objid = str(objid) + '/discount'
         result = self.call_get_api('invoices', objid=objid)
         return result
 
     def get_invoice_by_ref(self, objref, contact_list = 1):
         """
+        @endpoint 'get /invoices/ref/{ref}'
         Get invoice based on invoice ref
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: invoice
         """
         objref = 'ref/' + urllib.parse.quote(objref) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('invoices', objid=objref)
         return result
 
     # 2024-04-22 doesn't work for me in my Dolibarr
     def get_invoice_by_ref_ext(self, objref_ext, contact_list = 1):
         """
+        @endpoint 'get /invoices/ref_ext/{ref_ext}'
         Get invoice based on invoice ref_ext
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: invoice
         """
         objref_ext = 'ref_ext/' + urllib.parse.quote(objref_ext) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('invoices', objid=objref_ext)
         return result
 
     def get_invoice_lines_by_iid(self, objid):
         """
+        @endpoint 'get /invoices/{id}/lines'
         Get invoice lines based on invoice id
         @return: invoice lines
         """
         objid = str(objid) + '/lines'
         result = self.call_get_api('invoices', objid=objid)
         return result
 
     def get_invoice_payments_by_iid(self, objid):
         """
+        @endpoint 'get /invoices/{id}/payments'
         Get invoice payments based on invoice id
         @return: invoice payments
         """
         objid = str(objid) + '/payments'
         result = self.call_get_api('invoices', objid=objid)
         return result
 
     def get_invoice_template_by_tid(self, objid, contact_list = 1):
         """
+        @endpoint 'get /invoices/templates/{id}'
         Get invoice payments based on invoice template id
         @contact_list int 1: Return array contains just id (default), 0: Returned array of contacts/addresses contains all properties
         @return: invoice payments
         """
         objid = 'payments/' + str(objid) + '?contact_list=' + str(contact_list)
         result = self.call_get_api('invoices', objid=objid)
         return result
 
 
     # INTERVENTIONS
     def find_all_interventions(self, from_InterventionFilter = None):
         """
+        @endpoint 'get /interventions'
         Get all interventions
         @param from_InterventionFilter:
         @return: list of a interventions
         """
         if self.debug:
             ic()
             ic(from_InterventionFilter)
@@ -1511,25 +1614,27 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('interventions', params)
         return result
 
     def get_intervention_by_iid(self, objid):
         """
+        @endpoint 'get /interventions/{id}'
         Get intervention based on intervention id
         @return: invoice
         """
         objid = str(objid)
         result = self.call_get_api('interventions', objid=objid)
         return result
 
 
     # TICKETS
     def find_all_tickets(self, from_TicketFilter = None):
         """
+        @endpoint 'get /tickets'
         Get all tickets
         @param from_TicketFilter:
         @return: list of a tickets
         """
         if self.debug:
             ic()
             ic(from_TicketFilter)
@@ -1566,31 +1671,131 @@
         search_filter.page = page
         params = asdict(search_filter)
         result = self.call_list_api('tickets', params)
         return result
 
     def get_ticket_by_iid(self, objid):
         """
+        @endpoint 'get /tickets/{id}'
         Get ticket based on ticket id
-        @return: invoice
+        @return: ticket
         """
         objid = str(objid)
         result = self.call_get_api('tickets', objid=objid)
         return result
 
     def get_ticket_by_ref(self, objref):
         """
+        @endpoint 'get /tickets/ref/{ref}'
         Get ticket based on ticket ref
-        @return: invoice
+        @return: ticket
         """
         objref = 'ref/' + str(objref)
         result = self.call_get_api('tickets', objid=objref)
         return result
 
     def get_ticket_by_track_id(self, objtrack_id):
         """
+        @endpoint 'get /tickets/track_id/{track_id}'
         Get ticket based on ticket track_id
-        @return: invoice
+        @return: ticket
         """
         objtrack_id = 'track_id/' + str(objtrack_id)
         result = self.call_get_api('tickets', objid=objtrack_id)
         return result
+
+
+    # USERS
+    def find_all_users(self, from_UserFilter = None):
+        """
+        @endpoint 'get /users'
+        Get all users
+        @param from_UserFilter:
+        @return: list of a users
+        """
+        if self.debug:
+            ic()
+            ic(from_UserFilter)
+        if from_UserFilter is None:
+            search_filter = UserFilter()
+        else:
+            search_filter = from_UserFilter
+        all_users=[]
+        page = 0
+        while True:
+            some_users = self.find_some_users(search_filter, page)
+            if "error" in some_users:
+                break
+            elif [] == some_users:
+                break
+            elif {} == some_users:
+                break
+            else:
+                page += 1
+                if some_users == all_users:
+                    break
+                all_users = all_users + list(some_users)
+        return all_users
+
+    def find_some_users(self, from_UserFilter = None, page = 0):
+        if self.debug:
+            ic()
+            ic(page)
+            ic(from_UserFilter)
+        if from_UserFilter is None:
+            search_filter = UserFilter()
+        else:
+            search_filter = from_UserFilter
+        search_filter.page = page
+        params = asdict(search_filter)
+        result = self.call_list_api('users', params)
+        return result
+
+    def get_user_by_uid(self, objid, includepermissions = 0):
+        """
+        @endpoint 'get /users/{id}'
+        Get user based on user id
+        @includepermissions int default 0, Set this to 1 to have the array of permissions loaded (not done by default for performance purpose)
+        @return: user
+        """
+        if includepermissions:
+            objid = str(objid)  + '?includepermissions=' + includepermissions
+        else:
+            objid = str(objid)
+        result = self.call_get_api('users', objid=objid)
+        return result
+
+    def get_user_groups_uid(self, objid):
+        """
+        @endpoint 'get /users/{id}/groups'
+        Get user groups based on user id
+        @return: list of user groups
+        """
+        objid = str(objid) + '/groups'
+        result = self.call_get_api('users', objid)
+        return result
+
+    def setgroup_user_uid(self, objid, groupid, entity = 1):
+        """
+        @endpoint 'get /users/{id}/setGroup/{group}'
+        Set group for user based on user and group id
+        @groupid int Group ID
+        @entity int Entity ID (valid only for superadmin in multicompany transverse mode) default = 1
+        @return: int
+        """
+        objid = str(objid) + '/setGroup/' + str(groupid) + '?entity=' + str(entity)
+        result = self.call_get_api('users', objid)
+        return result
+
+    def get_user_by_email(self, email, includepermissions = 0):
+        """
+        @endpoint 'get /users/email/{email}'
+        Get properties of an user object by Email
+        @return: user object
+        """
+        if includepermissions:
+            objid = 'email/' + urllib.parse.quote(email)  + '?includepermissions=' + includepermissions
+        else:
+            objid = str(objid)
+        result = self.call_get_api('users', objid=objid)
+        return result
+
```

### Comparing `dolibarrpy-0.3.9/dolibarrpy.egg-info/PKG-INFO` & `dolibarrpy-0.4.2/dolibarrpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolibarrpy
-Version: 0.3.9
+Version: 0.4.2
 Summary: Python wrapper for Dolibarr API
 Home-page: https://github.com/JonBendtsen/dolibarrpy.git
 Author: Jon Bendtsen
 Author-email: jon.bendtsen.github@jonb.dk
 License: MIT
 Description: This project is a python wrapper for the API for Dolibarr ERP & CRM found at dolibarr.org. It is not yet complete, but most major GET endpoints has been implemented. In the beginning I will mostly focus on implementing the API endpoints that I use.
 Keywords: Dolibarr,python
```

### Comparing `dolibarrpy-0.3.9/setup.py` & `dolibarrpy-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import os
 
 setup(
     name='dolibarrpy',
     packages=['dolibarrpy'],
-    version="0.3.9",
+    version="0.4.2",
     license='MIT',
     description='Python wrapper for Dolibarr API',
     long_description='This project is a python wrapper for the API for Dolibarr ERP & CRM found at dolibarr.org. It is not yet complete, but most major GET endpoints has been implemented. In the beginning I will mostly focus on implementing the API endpoints that I use.',
     long_description_content_type='text/markdown',
     author='Jon Bendtsen',
     author_email='jon.bendtsen.github@jonb.dk',
     url='https://github.com/JonBendtsen/dolibarrpy.git',
```

