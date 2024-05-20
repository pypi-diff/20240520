# Comparing `tmp/vanguard_api-0.0.9.tar.gz` & `tmp/vanguard_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.0.9.tar", last modified: Wed May 15 11:03:59 2024, max compression
+gzip compressed data, was "vanguard_api-0.1.0.tar", last modified: Mon May 20 14:02:12 2024, max compression
```

## Comparing `vanguard_api-0.0.9.tar` & `vanguard_api-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:03:59.619557 vanguard_api-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 11:03:59.619557 vanguard_api-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 11:03:59.619557 vanguard_api-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:03:59.619557 vanguard_api-0.0.9/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/vanguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 11:03:49.000000 vanguard_api-0.0.9/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 11:03:59.619557 vanguard_api-0.0.9/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 11:03:59.000000 vanguard_api-0.0.9/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 11:03:59.000000 vanguard_api-0.0.9/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 11:03:59.000000 vanguard_api-0.0.9/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 11:03:59.000000 vanguard_api-0.0.9/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 11:03:59.000000 vanguard_api-0.0.9/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.0.9/LICENSE` & `vanguard_api-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.9/PKG-INFO` & `vanguard_api-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.9
+Version: 0.1.0
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.9.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.0.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.0.9/README.md` & `vanguard_api-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.9/setup.py` & `vanguard_api-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.0.9",
+    version="0.1.0",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.9.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.0.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.0.9/vanguard/account.py` & `vanguard_api-0.1.0/vanguard/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         Args:
             selector (ElementHandle): The selector from which to retrieve the account ID.
 
         Returns:
            string: account_id
         """
         account_id = selector.query_selector("span > span > span > span").inner_text()
-        return account_id.split("—")[2].strip().replace("*", "")
+        if len(account_fields := account_id.split("—")) == 3:
+            return account_fields[2].strip().replace("*", "")
+        return None
 
     def _parse_rows(self, table_rows, account_id):
         """
         Parses the rows of a table to extract holdings information.
 
         Args:
             table_rows (ElementHandle): The rows of the table to parse.
@@ -152,14 +154,16 @@
             self.session.page.wait_for_selector(
                 '//span[contains(text(), "Expand all accounts")]', timeout=120000
             ).click()
             self.session.page.wait_for_selector("#overflow-override")
             all_selectors = self.session.page.query_selector_all("#overflow-override")
             for i, selector in enumerate(all_selectors):
                 account_id = self._get_account_id(selector)
+                if not account_id:
+                    continue
                 self.account_numbers.append(account_id)
                 table_wrapper = selector.wait_for_selector(f"#self_managed_table_{i}")
                 table_entries = table_wrapper.query_selector_all("tbody")
                 for j, entry in enumerate(table_entries):
                     if j == len(table_entries) - 1:
                         total_row = entry.query_selector_all("tr")
                         for row in total_row:
@@ -167,15 +171,14 @@
                             self.account_totals[account_id] = totals[-1].replace(
                                 "$", ""
                             )
             return True
         except PlaywrightTimeoutError:
             return False
 
-        
     def get_holdings(self):
         """
         Retrieves and sets the holdings information of the account.
 
         This method navigates to the account holdings page, waits for the holdings information to load, and then retrieves the holdings information from the page.
 
         Returns:
@@ -193,14 +196,16 @@
             self.total_value = float(
                 total_element.inner_text().split()[-1].replace(",", "").replace("$", "")
             )
             self.session.page.wait_for_selector("#overflow-override")
             all_selectors = self.session.page.query_selector_all("#overflow-override")
             for i, selector in enumerate(all_selectors):
                 account_id = self._get_account_id(selector)
+                if not account_id:
+                    continue
                 table_wrapper = selector.wait_for_selector(f"#self_managed_table_{i}")
                 table_entries = table_wrapper.query_selector_all("tbody")
                 for entry in table_entries:
                     table_rows = entry.query_selector_all("tr")
                     self._parse_rows(table_rows, account_id)
             return True
         except PlaywrightTimeoutError:
```

### Comparing `vanguard_api-0.0.9/vanguard/order.py` & `vanguard_api-0.1.0/vanguard/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,27 +93,29 @@
         """
         order_messages = {
             "ORDER INVALID": "",
             "ORDER PREVIEW": "",
             "ORDER CONFIRMATION": "",
         }
         self.session.go_url(order_page())
-
-        self.session.page.wait_for_selector(
-            "//div[text()=' Select Account ']", timeout=20000
-        ).click()
-        account_box = self.session.page.wait_for_selector(
-            ".c11n-modal-dialog-open",
-            timeout=10000,
-        )
-        account_selectors = account_box.query_selector_all("tds-list-option")
-        for account in account_selectors:
-            if account_id in account.text_content():
-                account.click()
-                break
+        try:
+            self.session.page.wait_for_selector(
+                "//div[text()=' Select Account ']", timeout=10000
+            ).click()
+            account_box = self.session.page.wait_for_selector(
+                ".c11n-modal-dialog-open",
+                timeout=10000,
+            )
+            account_selectors = account_box.query_selector_all("tds-list-option")
+            for account in account_selectors:
+                if account_id in account.text_content():
+                    account.click()
+                    break
+        except:
+            pass
         quote_box = self.session.page.wait_for_selector(
             "//input[@placeholder='Get Quote']"
         )
         quote_box.click()
         quote_box.fill("")
         quote_box.fill(symbol)
         self.session.page.press(
@@ -181,26 +183,31 @@
         try:
             if duration == "DAY":
                 self.session.page.click("xpath=//label[text()='Day']")
             elif duration == "GOOD_TILL_CANCELLED":
                 self.session.page.click("xpath=//label[text()='60-day (GTC)']")
             if order_type == "SELL":
                 self.session.page.wait_for_selector(
-                    "body > twe-root > main > twe-trade > form > div > div.row > div:nth-child(1) > twe-cost-basis-control > twe-cost-basis-modal > tds-modal > div.modal.visible > div > div.modal__content",
+                    "body > twe-root > main > twe-trade > form > div > div.row >"
+                    " div:nth-child(1) > twe-cost-basis-control > twe-cost-basis-modal"
+                    " > tds-modal > div.modal.visible > div > div.modal__content",
                     timeout=10000,
                 )
                 self.session.page.wait_for_selector(
                     "//button[text()=' Continue ']",
                     timeout=10000,
                 ).click()
         except PlaywrightTimeoutError:
             pass
         try:
             self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-trade > form > div > div.row > div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail > tds-card > div > tds-card-body > div.twe-flex-button-wrap > button:nth-child(2)",
+                "body > twe-root > main > twe-trade > form > div > div.row >"
+                " div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail"
+                " > tds-card > div > tds-card-body > div.twe-flex-button-wrap >"
+                " button:nth-child(2)",
                 timeout=5000,
             ).click()
         except PlaywrightTimeoutError:
             pass
         if after_hours:
             try:
                 sleep(2)
@@ -209,15 +216,18 @@
                     timeout=5000,
                 ).click()
             except PlaywrightTimeoutError:
                 pass
 
         try:
             warning = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-trade > form > div > div.row > div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail > tds-card > div > tds-card-body > div:nth-child(3) > div > tds-card > div > tds-card-body",
+                "body > twe-root > main > twe-trade > form > div > div.row >"
+                " div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail"
+                " > tds-card > div > tds-card-body > div:nth-child(3) > div > tds-card"
+                " > div > tds-card-body",
                 timeout=5000,
             )
             warning_header_selector = warning.query_selector("p")
             warning_header = warning_header_selector.text_content()
             warning_items = warning.query_selector_all("li")
             warning_text = {warning_header: []}
             for item in warning_items:
@@ -225,20 +235,22 @@
             order_messages["ORDER INVALID"] = warning_text
             return order_messages
         except PlaywrightTimeoutError:
             order_messages["ORDER INVALID"] = "No invalid order message found."
 
         try:
             order_preview = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-preview > div > div > div.col-lg-7 > tds-card > div > tds-card-body > twe-order-details",
+                "body > twe-root > main > twe-preview > div > div > div.col-lg-7 >"
+                " tds-card > div > tds-card-body > twe-order-details",
                 timeout=5000,
             )
             order_preview_text = order_preview.text_content()
             preview_parts = re.split(
-                r"(Account|Transaction|Shares|Security|Order type|Duration|Commission|Estimated amount|\*)",
+                r"(Account|Transaction|Shares|Security|Order"
+                r" type|Duration|Commission|Estimated amount|\*)",
                 order_preview_text,
             )
             order_preview = {
                 "Account": preview_parts[2],
                 "Transaction": preview_parts[4],
                 "Shares": preview_parts[6],
                 "Security": preview_parts[8],
@@ -259,19 +271,22 @@
             else:
                 return order_messages
         except PlaywrightTimeoutError:
             order_messages["ORDER PREVIEW"] = "No order preview page found."
 
         try:
             order_handle_one = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-confirm > div > div > div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 > h2",
+                "body > twe-root > main > twe-confirm > div > div >"
+                " div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 > h2",
                 timeout=5000,
             )
             order_handle_two = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-confirm > div > div > div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 > div.page-heading.tds-mb-7",
+                "body > twe-root > main > twe-confirm > div > div >"
+                " div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 >"
+                " div.page-heading.tds-mb-7",
                 timeout=5000,
             )
             order_number_text = order_handle_one.text_content()
             order_match = re.search(r"Received order #(\d+)", order_number_text)
             if order_match:
                 order_number = order_match.group(1)
             else:
```

### Comparing `vanguard_api-0.0.9/vanguard/session.py` & `vanguard_api-0.1.0/vanguard/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,21 +155,24 @@
                         return False
                     self.page.wait_for_selector(
                         "#username-password-submit-btn-1", timeout=1000
                     )
                     break
                 except PlaywrightTimeoutError:
                     continue
-            username_box = self.page.query_selector("#USER")
-            username_box.type(username, delay=random.randint(50, 500))
-            username_box.press("Tab")
-            password_box = self.page.query_selector("#PASSWORD-blocked")
-            password_box.type(password, delay=random.randint(50, 500))
-            sleep(random.uniform(1, 3))
-            self.page.query_selector("#username-password-submit-btn-1").click()
+            try:
+                username_box = self.page.wait_for_selector("#USER", timeout=10000)
+                username_box.type(username, delay=random.randint(50, 500))
+                username_box.press("Tab")
+                password_box = self.page.query_selector("#PASSWORD-blocked")
+                password_box.type(password, delay=random.randint(50, 500))
+                sleep(random.uniform(1, 3))
+                self.page.query_selector("#username-password-submit-btn-1").click()
+            except PlaywrightTimeoutError:
+                pass
             try:
                 self.page.wait_for_selector(
                     "button.col-md:nth-child(2) > div:nth-child(1)", timeout=5000
                 ).click()
             except PlaywrightTimeoutError:
                 pass
             try:
```

### Comparing `vanguard_api-0.0.9/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.1.0/vanguard_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.9
+Version: 0.1.0
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.9.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.0.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

