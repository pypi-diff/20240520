# Comparing `tmp/wawona-1.1.2.tar.gz` & `tmp/wawona-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wawona-1.1.2.tar", last modified: Wed May  1 12:32:18 2024, max compression
+gzip compressed data, was "wawona-1.2.0.tar", last modified: Mon May 20 12:45:40 2024, max compression
```

## Comparing `wawona-1.1.2.tar` & `wawona-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.289623 wawona-1.1.2/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.1.2/LICENSE
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5112 2024-05-01 12:32:18.288014 wawona-1.1.2/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     4073 2024-04-25 12:25:34.000000 wawona-1.1.2/README.md
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-05-01 12:31:27.000000 wawona-1.1.2/pyproject.toml
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-05-01 12:32:18.298871 wawona-1.1.2/setup.cfg
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.246239 wawona-1.1.2/src/
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.264372 wawona-1.1.2/src/wawona/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.1.2/src/wawona/__init__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.1.2/src/wawona/__main__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)    19794 2024-04-25 12:22:33.000000 wawona-1.1.2/src/wawona/wawona.py
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-01 12:32:18.286066 wawona-1.1.2/src/wawona.egg-info/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5112 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/SOURCES.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/dependency_links.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/entry_points.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/requires.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-05-01 12:32:18.000000 wawona-1.1.2/src/wawona.egg-info/top_level.txt
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.863347 wawona-1.2.0/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.2.0/LICENSE
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5440 2024-05-20 12:45:40.862640 wawona-1.2.0/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     4327 2024-05-20 12:43:00.000000 wawona-1.2.0/README.md
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1132 2024-05-20 12:44:31.000000 wawona-1.2.0/pyproject.toml
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-05-20 12:45:40.863508 wawona-1.2.0/setup.cfg
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.852120 wawona-1.2.0/src/
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.856878 wawona-1.2.0/src/wawona/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.2.0/src/wawona/__init__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.2.0/src/wawona/__main__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)    22382 2024-05-20 12:43:00.000000 wawona-1.2.0/src/wawona/wawona.py
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-05-20 12:45:40.861935 wawona-1.2.0/src/wawona.egg-info/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5440 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/SOURCES.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/dependency_links.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/entry_points.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       96 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/requires.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-05-20 12:45:40.000000 wawona-1.2.0/src/wawona.egg-info/top_level.txt
```

### Comparing `wawona-1.1.2/LICENSE` & `wawona-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wawona-1.1.2/PKG-INFO` & `wawona-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.1.2
+Version: 1.2.0
 Summary: Easily make office reservations in sequoia from the command line.
-Author-email: yuzawa-san <jtyuzawa@gmail.com>
+Author-email: yuzawa-san <jtyuzawa+wawona@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
 Project-URL: Documentation, https://github.com/yuzawa-san/wawona/blob/master/README.md
 Project-URL: Repository, https://github.com/yuzawa-san/wawona.git
 Project-URL: Funding, http://paypal.me/yuzawasan
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: inquirer>=3.2.4
 Requires-Dist: texttable>=1.7.0
-Requires-Dist: keyring>=24.3.1
+Requires-Dist: keyring>=25.2.1
 Requires-Dist: pytz>=2024.1
+Requires-Dist: selenium>=4.21.0
 
 # 🌲 wawona 🌲
 
 by [@yuzawa-san](https://github.com/yuzawa-san/)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wawona)](https://pypi.org/project/wawona/)
 
@@ -78,30 +80,40 @@
   Mar 27 New York Reservation
   Complete Self-Screening
   Seat Not Selected
 
 [?] Complete task? (Y/n): 
 [?] I am healthy and not sick?: Yes (only choice)
 [?] Floor: Floor 2 (only choice)
+
+ X X
+ X X   X X
+ X O   O X   O O O X O
+ X X   O O   O * $ O $
+ O O   O O
+ O O   O O   O O O O O
+ O O   O O   O X O O O
+
+* preferred    O free    $ booked by someone you are following    X booked
 [?] Space: 
-   Desk 35
-   Desk 36
-   Desk 37
-   Desk 38
-   Desk 39
-   Desk 40
- > Desk 41
-   Desk 42 (Juan Fnulwoln)
-   Desk 43
-   Desk 44 (Maeve Melwosniwnaiko)
-   Desk 45
-   Desk 46
-   Desk 47
+   Desk 5
+   Desk 6
+   Desk 7
+   Desk 8 (Guillaume Rucpelzsva)
+   Desk 9
+   Desk 10
+ > Desk 11
+   Desk 12 (Juan Fnulwoln)
+   Desk 13
+   Desk 14 (Maeve Melwosniwnaiko)
+   Desk 15
+   Desk 16
+   Desk 17
 
-You have booked 'Desk 41'
+You have booked 'Desk 11'
 ```
 
 ## Install
 
 The easiest way is probably using [Homebrew](https://brew.sh/).
 A self-maintained tap is available for use. To install tap:
 ```console
@@ -122,16 +134,17 @@
 # update just this
 brew upgrade wawona
 ```
 
 ## Usage 
 
 - Run it from your terminal: `wawona`
-- On initial run, you will be asked provide configuration: email and password.
-- You may be prompted to for an MFA token periodically.
+- On initial run, you will be asked to provide configuration details and to do an initial login.
+- Login uses a standalone chrome powered by selenium.
+- Periodically, you will be asked to re-login.
 - Use the up/down arrows, spacebar, and return keys to select items in lists
 - Troubleshooting errors with `wawona --verbose`
 
 ### Reset
 
 If you need to reset to factory defaults (maybe if you changed your password), remove the configuration:
 
@@ -144,14 +157,13 @@
 ```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
-- Does not support SSO
 - Uses public endpoints discovered from the web UI
 - No warranty or stability guarantees, could break one day if something changes on their end
 - Password/token is stored in system keychain
 - Add/remove followers using the app.
 - Basically if it is not here or it breaks here, use the real app/site.
 - Named for the [drive-thru sequoia](https://en.wikipedia.org/wiki/Wawona_Tree)
```

### Comparing `wawona-1.1.2/README.md` & `wawona-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,30 +53,40 @@
   Mar 27 New York Reservation
   Complete Self-Screening
   Seat Not Selected
 
 [?] Complete task? (Y/n): 
 [?] I am healthy and not sick?: Yes (only choice)
 [?] Floor: Floor 2 (only choice)
+
+ X X
+ X X   X X
+ X O   O X   O O O X O
+ X X   O O   O * $ O $
+ O O   O O
+ O O   O O   O O O O O
+ O O   O O   O X O O O
+
+* preferred    O free    $ booked by someone you are following    X booked
 [?] Space: 
-   Desk 35
-   Desk 36
-   Desk 37
-   Desk 38
-   Desk 39
-   Desk 40
- > Desk 41
-   Desk 42 (Juan Fnulwoln)
-   Desk 43
-   Desk 44 (Maeve Melwosniwnaiko)
-   Desk 45
-   Desk 46
-   Desk 47
+   Desk 5
+   Desk 6
+   Desk 7
+   Desk 8 (Guillaume Rucpelzsva)
+   Desk 9
+   Desk 10
+ > Desk 11
+   Desk 12 (Juan Fnulwoln)
+   Desk 13
+   Desk 14 (Maeve Melwosniwnaiko)
+   Desk 15
+   Desk 16
+   Desk 17
 
-You have booked 'Desk 41'
+You have booked 'Desk 11'
 ```
 
 ## Install
 
 The easiest way is probably using [Homebrew](https://brew.sh/).
 A self-maintained tap is available for use. To install tap:
 ```console
@@ -97,16 +107,17 @@
 # update just this
 brew upgrade wawona
 ```
 
 ## Usage 
 
 - Run it from your terminal: `wawona`
-- On initial run, you will be asked provide configuration: email and password.
-- You may be prompted to for an MFA token periodically.
+- On initial run, you will be asked to provide configuration details and to do an initial login.
+- Login uses a standalone chrome powered by selenium.
+- Periodically, you will be asked to re-login.
 - Use the up/down arrows, spacebar, and return keys to select items in lists
 - Troubleshooting errors with `wawona --verbose`
 
 ### Reset
 
 If you need to reset to factory defaults (maybe if you changed your password), remove the configuration:
 
@@ -119,14 +130,13 @@
 ```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
-- Does not support SSO
 - Uses public endpoints discovered from the web UI
 - No warranty or stability guarantees, could break one day if something changes on their end
 - Password/token is stored in system keychain
 - Add/remove followers using the app.
 - Basically if it is not here or it breaks here, use the real app/site.
 - Named for the [drive-thru sequoia](https://en.wikipedia.org/wiki/Wawona_Tree)
```

### Comparing `wawona-1.1.2/pyproject.toml` & `wawona-1.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wawona"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
-  { name="yuzawa-san", email="jtyuzawa@gmail.com" },
+  { name="yuzawa-san", email="jtyuzawa+wawona@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Easily make office reservations in sequoia from the command line."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3.8",
   "Operating System :: OS Independent",
+  "Environment :: Console",
 ]
 dependencies = [
   "requests>=2.31.0",
   "inquirer>=3.2.4",
   "texttable>=1.7.0",
-  "keyring>=24.3.1",
+  "keyring>=25.2.1",
   "pytz>=2024.1",
+  "selenium>=4.21.0",
 ]
 
 [project.scripts]
 wawona = "wawona.wawona:run"
 
 [project.urls]
 Homepage = "https://github.com/yuzawa-san/wawona"
```

### Comparing `wawona-1.1.2/src/wawona/wawona.py` & `wawona-1.2.0/src/wawona/wawona.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,41 +2,55 @@
 import locale
 import os
 import re
 import sys
 from datetime import date, datetime, time, timedelta
 from os.path import isfile, isdir
 from time import sleep
+from urllib.parse import unquote
 
 import inquirer
 import keyring
 import pytz
 import requests
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
 from texttable import Texttable
 
 config_path = "%s/.config/wawona" % os.environ["HOME"]
 config_file = "%s/config.json" % config_path
 
+TERMINAL_CHAR_ASPECT_RATIO = 8 / 10
+FLOOR_PLAN_BUFFER = 4
+FLOOR_PLAN_COLS = 120
+COLOR_AVAILABLE = "32"
+COLOR_BOOKED_FOLLOWING = "36"
+COLOR_BOOKED = "31"
+COLOR_PREFERRED = "35"
+DOT = "\u25CF"
+
 BROWSER_HASH = "1032275734"
 HEADERS = {
     'authority': 'hrx-backend.sequoia.com',
     'accept': 'application/json',
     'agent': 'admin',
     'content-type': 'application/json;charset=UTF-8',
     'devicetype': '4',
     'locale-timezone': 'America/New_York',
     'origin': 'https://login.sequoia.com',
     'referer': 'https://login.sequoia.com/',
     'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) '
                   'Chrome/122.0.0.0 Safari/537.36'
 }
-KEYRING_EMAIL = "login.sequoia.com"
 KEYRING_TOKEN = "hrx-backend.sequoia.com"
 CHECK_MARK = "\u2705"
 CONFIG_VERSION = 1
+YOU = "You"
 
 VERBOSE = False
 for arg in sys.argv:
     if arg == "reset":
         print("Removing config file")
         os.remove(config_file)
     elif arg == "--verbose":
@@ -63,54 +77,39 @@
         if status_code == 400 and not response_json.get("success"):
             raise ApiException(response_json.get("message"))
         raise ApiException("%s %s %s %s %s %s" %
                            (method, url, kwargs.get("headers"), status_code, response_headers, response_json))
     return response_json
 
 
-def get_token(config, refresh=False):
-    email = config["email"]
-    token = keyring.get_password(KEYRING_TOKEN, email)
+def get_token(refresh=False):
+    token = keyring.get_password(KEYRING_TOKEN, KEYRING_TOKEN)
     if token and not refresh:
         return token
-    api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/v1/contacts/verify-email", headers=HEADERS,
-             json={"email": email})
-    password = keyring.get_password(KEYRING_EMAIL, email)
-    if not password:
-        password = inquirer.password(message='Password')
-    login_json = api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login", headers=HEADERS,
-                          json={"email": email, "password": password, "browserHash": BROWSER_HASH,
-                                "userType": "employee"})
-    login_data = login_json["data"]
-    user_details = login_data["userDetails"]
-    token = user_details["apiToken"]
-    okta_status = user_details["oktaStatus"]
-    if okta_status == "MFA_CHALLENGE":
-        factors = login_data.get("factors")
-        if factors:
-            factor = factors[0]
-            print(
-                "Using MFA %s %s" % (factor.get("factorType", "unknown"), factor.get("profile", {}).get("phoneNumber")))
-        while True:
-            mfa_code = inquirer.text(message="MFA Code")
-            headers = {"apitoken": token}
-            headers.update(HEADERS)
-            try:
-                api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login/verify-mfa",
-                         headers=headers, json={"passCode": mfa_code, "browserHash": BROWSER_HASH})
-                break
-            except ApiException as e:
-                print("MFA Verification Failed", e)
-    elif okta_status != "SUCCESS":
-        # https://developer.okta.com/docs/reference/api/authn/#transaction-state
-        raise ApiException("Invalid okta status %s: "
-                           "Please authenticate via https://px.sequoia.com/workplace before retrying." % okta_status)
-    keyring.set_password(KEYRING_EMAIL, email, password)
-    keyring.set_password(KEYRING_TOKEN, email, token)
-    return token
+    print("Loading auth flow in standalone Chrome...")
+    print("NOTE: If you get the alert with 'chromedriver cannot be opened because the developer cannot be verified.',"
+          "select 'Cancel' to proceed.")
+    print("PROTIP: Enable 'Remember Me' and 'Keep me signed in' and 'Trusted Device' to speed up subsequent logins.")
+    chrome_options = Options()
+    chrome_options.add_argument("user-data-dir=%s/selenium" % config_path)
+    driver = webdriver.Chrome(options=chrome_options)
+    driver.get("https://login.sequoia.com/?redirect=https://px.sequoia.com/workplace/")
+    try:
+        WebDriverWait(driver, 300).until(EC.url_to_be("https://px.sequoia.com/workplace/"))
+        cookies = driver.get_cookies()
+        if VERBOSE:
+            print("COOKIES", cookies)
+        for cookie in cookies:
+            if cookie["name"] == "_sc":
+                token = json.loads(unquote(cookie["value"]))["sessionToken"]
+                keyring.set_password(KEYRING_TOKEN, KEYRING_TOKEN, token)
+                return token
+        raise ApiException("Failed to fetch token")
+    finally:
+        driver.quit()
 
 
 def get_config():
     config: dict[str, str] = {}
     if isfile(config_file):
         with open(config_file) as f:
             config = json.load(f)
@@ -118,18 +117,14 @@
         return config
     config["version"] = str(CONFIG_VERSION)
     hours = []
     for hour in range(24):
         formatted = datetime.combine(date.today(), time(hour)).strftime(locale.nl_langinfo(locale.T_FMT_AMPM))
         hours.append((formatted, hour))
     questions = [
-        inquirer.Text(
-            "email",
-            message="Email",
-        ),
         # NOTE: this does not have location
         inquirer.Text(
             "preferred_space_id",
             message="Preferred space ID (press return for none)",
         ),
         inquirer.List(
             "start_hour",
@@ -142,23 +137,19 @@
             message="End of Day (for reservations)",
             choices=hours,
             default=18
         ),
     ]
     answers = inquirer.prompt(questions)
     config.update(answers)
-    email = config["email"]
-    password = keyring.get_password(KEYRING_EMAIL, email)
-    if password:
-        keyring.delete_password(KEYRING_EMAIL, email)
-    token = keyring.get_password(KEYRING_TOKEN, email)
+    token = keyring.get_password(KEYRING_TOKEN, KEYRING_TOKEN)
     if token:
-        keyring.delete_password(KEYRING_TOKEN, email)
+        keyring.delete_password(KEYRING_TOKEN, KEYRING_TOKEN)
     # test configuration
-    get_token(config)
+    get_token()
     # only persist configuration if test worked
     if not isdir(config_path):
         os.makedirs(config_path, exist_ok=True)
     with open(config_file, 'w') as f:
         json.dump(config, f)
     return config
 
@@ -194,29 +185,29 @@
     return out
 
 
 def get_followings(token, start, end):
     response = api_call(method='GET',
                         url="https://hrx-backend.sequoia.com/rtw/client/followings?startDate=%s&endDate=%s" % (
                             format_date(start), format_date(end)), headers=token_headers(token))
-    out = []
+    out = {}
     followings = response["data"]["followings"]
     if not followings:
         print("You are not following any coworkers.\n"
               "Add them in https://px.sequoia.com/workplace or the app, and they will appear calendar below.")
     for user in followings:
         name = user["fullName"]
         reservations = user.get("reservationsMetadata", [])
         days = set()
+        out[name] = days
         if reservations:
             for reservation in reservations:
                 year, month, day = reservation["reservationStartTime"].split(" ")[0].split("-")
                 dt = date(int(year), int(month), int(day))
                 days.add(dt)
-            out.append((name, days))
     return out
 
 
 def pretty_time(dt):
     return dt.astimezone(pytz.utc).isoformat().replace('+00:00', 'Z')
 
 
@@ -292,76 +283,146 @@
              json={"taskId": task_id, "response": answers})
 
 
 def get_floors(token, task_id):
     response = api_call(
         method='GET', url="https://hrx-backend.sequoia.com/rtw/client/space-bookings/floors?taskId=%s" % task_id,
         headers=token_headers(token))
-    return [(x["floorName"], x["floorId"]) for x in response["data"]["floors"] if x["status"] == "active"]
+    return [(x["floorName"], x) for x in response["data"]["floors"] if x["status"] == "active"]
 
 
 def get_spaces(token, adjective, task_id, floor_id, start_time, end_time):
     url = ("https://hrx-backend.sequoia.com/rtw/client/space-bookings/%s/spaces?taskId=%s&floorId=%s&startTime=%s"
            "&endTime=%s") % (
               adjective, task_id, floor_id, start_time, end_time)
     response = api_call(method='GET', url=url, headers=token_headers(token))
-    return response["data"]["spaces"]
+    return response["data"]["spaces"] or []
 
 
 def reserve_space(token, task_id, start_time, end_time, space_id, user_id, reservation_id):
     response = api_call(method='POST', url="https://hrx-backend.sequoia.com/rtw/client/space-bookings/space",
                         headers=token_headers(token),
                         json={"taskId": task_id, "startTime": start_time, "endTime": end_time, "spaceId": space_id,
                               "userId": user_id, "reservationId": reservation_id}
                         )
     return response["data"]["label"]
 
 
-def get_space(token, task, floor_id, config):
+def draw_floor_plan(floor, spaces):
+    if 'blueprintUrl' not in floor:
+        return
+    spaces = [x for x in spaces if 'Rx' in x]
+    if not spaces:
+        return
+
+    base_width = floor['baseWidth']
+    aspect_ratio = floor["aspectRatio"]
+    base_height = round(base_width * aspect_ratio)
+
+    min_x = base_width
+    min_y = base_height
+    max_x = 0
+    max_y = 0
+    for space in spaces:
+        x = space['Rx']
+        min_x = min(min_x, x)
+        max_x = max(max_x, x)
+        y = space['Ry']
+        min_y = min(min_y, y)
+        max_y = max(max_y, y)
+
+    new_width = (max_x - min_x)
+    new_height = (max_y - min_y)
+
+    w = min(FLOOR_PLAN_COLS, os.get_terminal_size()[0]) - FLOOR_PLAN_BUFFER
+    h = round(w * (new_height / new_width) * TERMINAL_CHAR_ASPECT_RATIO)
+
+    grid = []
+    for _ in range(h + FLOOR_PLAN_BUFFER):
+        grid.append([" "] * (w + FLOOR_PLAN_BUFFER))
+
+    for space in spaces:
+        x = round((space['Rx'] - min_x) / new_width * w)
+        y = round((space['Ry'] - min_y) / new_height * h)
+        color = space['color']
+        grid[y][x] = "\033[%sm%s\033[0m" % (color, DOT)
+
+    for row in grid:
+        print("".join(row))
+    print(
+        "\033[%sm%s\033[0m preferred    "
+        "\033[%sm%s\033[0m free    "
+        "\033[%sm%s\033[0m booked by someone you are following    "
+        "\033[%sm%s\033[0m booked" % (
+            COLOR_PREFERRED, DOT, COLOR_AVAILABLE, DOT, COLOR_BOOKED_FOLLOWING, DOT, COLOR_BOOKED, DOT))
+
+
+def get_space(token, task, floor, config, followings):
+    floor_id = floor["floorId"]
     task_id = task["taskId"]
     start_time = task["reservationStartTime"]
     end_time = task["reservationEndTime"]
     available_spaces = get_spaces(token, "available", task_id, floor_id, start_time, end_time)
     default = None
     preferred_space_id = config.get("preferred_space_id")
     if not preferred_space_id:
         preferred_space_id = inquirer.text(message="Preferred space ID (press return for none)")
     all_spaces = []
     available_space_set = set()
     for available_space in available_spaces:
+        available_space["color"] = COLOR_AVAILABLE
         space_id = available_space["spaceId"]
         unique_space_id = available_space["uniqueSpaceId"]
         if space_id == preferred_space_id:
+            available_space["color"] = COLOR_PREFERRED
             default = unique_space_id
         all_spaces.append(available_space)
         available_space_set.add(unique_space_id)
     booked_spaces = get_spaces(token, "booked", task_id, floor_id, start_time, end_time)
     for booked_space in booked_spaces:
         space_id = booked_space["spaceId"]
         if space_id == preferred_space_id:
             default = booked_space["uniqueSpaceId"]
+        full_name = "%s %s" % (booked_space.get("firstName"), booked_space.get("lastName"))
+        booked_space["fullName"] = full_name
+        booked_space["color"] = COLOR_BOOKED_FOLLOWING if full_name in followings else COLOR_BOOKED
         all_spaces.append(booked_space)
     all_spaces.sort(key=lambda s: [int(t) if t.isdigit() else t.lower() for t in re.split(r'(\d+)', s["label"])])
     choices = []
     for space in all_spaces:
         raw_label = space["label"]
-        first_name = space.get("firstName")
-        if first_name:
-            label = "\033[31m%s (%s %s)\033[0m" % (raw_label, first_name, space["lastName"])
-        else:
-            label = "\033[32m%s\033[0m" % raw_label
+        color = space["color"]
+        label: str = "\033[%sm%s\033[0m" % (color, raw_label)
+        full_name = space.get("fullName")
+        if full_name:
+            label = "\033[%sm%s (%s)\033[0m" % (color, raw_label, full_name)
         choices.append((label, space["uniqueSpaceId"]))
+    try:
+        draw_floor_plan(floor, all_spaces)
+    except Exception as e:
+        print("Failed to draw floor plan: ", e)
     while True:
         unique_space_id = do_inquiry("Space", choices, default)
         if unique_space_id in available_space_set:
-            return unique_space_id
+            return booked_spaces, unique_space_id
         print("Invalid selection")
 
 
-def run_tasks(token, config, pending_task_ids):
+def get_booking_map(bookings, space_id=-1):
+    out = {}
+    for booking in bookings:
+        key = "%s %s" % (booking['firstName'], booking['lastName'])
+        if space_id == booking["spaceId"]:
+            key = YOU
+        out[key] = booking['label']
+    return out
+
+
+def run_tasks(token, config, pending_task_ids, followings):
+    out = {}
     for pending_task_id in pending_task_ids:
         task = get_task(token, pending_task_id)
         task_id = task["taskId"]
         task_metadata = task["taskMetadata"]
         task_data = task_metadata.get("data")
         card_info = task_metadata["cardInfo"]
         print("%s:\n\n\t%s %s %s\n\t%s\n\t%s\n" % (
@@ -369,14 +430,20 @@
             card_info.get("displayTitle", ""),
             card_info.get("title", ""),
             card_info.get("heading", ""),
             card_info.get("basicSubtitle", ""),
             card_info.get("caption", "")
         ))
         if not task_data:
+            floor_id = task.get("floorId")
+            start_time = task.get("reservationStartTime")
+            end_time = task.get("reservationEndTime")
+            if floor_id and start_time and end_time:
+                out = get_booking_map(get_spaces(token, "booked", task_id, floor_id, start_time, end_time),
+                                      task.get("spaceId"))
             continue
         if not inquirer.confirm("Complete task?", default=True):
             continue
         questions = task_data["questions"]
         if not questions or not task_data["hasQuestionnaire"]:
             raise Exception("Task without questionnaire not supported")
         if task_data["hasDocumentAck"]:
@@ -401,51 +468,63 @@
                 choices.append([raw_choice["choiceLabel"], raw_choice["choiceId"]])
             choice_id = do_inquiry(question["questionTitle"].strip(), choices)
             answers.append({"questionId": question_id, "choice_id": choice_id})
         respond_to_task(token, task_id, answers)
         if not task["spaceBookingEnabled"]:
             continue
         floors = get_floors(token, task_id)
-        floor_id = do_inquiry("Floor", floors)
-        space_id = get_space(token, task, floor_id, config)
+        floor = do_inquiry("Floor", floors)
+        (bookings, space_id) = get_space(token, task, floor, config, followings)
         start_time = task["reservationStartTime"]
         end_time = task["reservationEndTime"]
         user_id = task["recipientId"]
         reservation_id = task["reservationId"]
         space_label = reserve_space(token, task_id, start_time, end_time, space_id, user_id, reservation_id)
         print("You have booked '%s'" % space_label)
+        out = get_booking_map(bookings)
+        out[YOU] = space_label
+    return out
 
 
-def print_weeks(weeks, today, booked, followings, choices):
+def print_weeks(weeks, today, booked, followings, choices, current_spaces):
     rows = []
     for week in weeks:
         label = "WEEK OF %s" % week[0].strftime('%d %b').upper()
         header = [label]
-        booking_row = ["Me"]
+        booking_row = [YOU]
         rows.append(header)
         rows.append(booking_row)
         for day in week:
             day_label = day.strftime('%a\n%d')
             if day == today:
                 day_label = "%s*" % day_label
             header.append(day_label)
             is_booked = day in booked
             booking_row.append(CHECK_MARK if is_booked else "")
             if not is_booked and day >= today:
                 choices.append((day.strftime('%a %d %b'), day))
-        for name, days in followings:
+        if current_spaces:
+            header.append("Today's\nSpace" if today in week else "")
+            booking_row.append(current_spaces.get(YOU, ""))
+        for name, days in followings.items():
             user_row = [name]
             add_row = False
             for day in week:
                 if day in days:
                     entry = CHECK_MARK
                     add_row = True
                 else:
                     entry = ""
                 user_row.append(entry)
+            if current_spaces:
+                space = current_spaces.get(name)
+                if space and today in week:
+                    user_row.append(space)
+                else:
+                    user_row.append("")
             if add_row:
                 rows.append(user_row)
     t = Texttable(max_width=0)
     t.add_rows(rows, header=False)
     print(t.draw())
 
 
@@ -453,39 +532,39 @@
     try:
         from . import __version__
     except ImportError:
         __version__ = None
     version = "unknown" if not __version__ else "v%s" % __version__
     print("\U0001F332 \033[32mW A W O N A\033[0m \U0001F332\n\n%s - https://github.com/yuzawa-san/wawona\n" % version)
     config = get_config()
-    token = get_token(config)
+    token = get_token()
     try:
         pending_task_ids = get_pending_tasks(token)
     except ApiException:
-        token = get_token(config, True)
+        token = get_token(True)
         pending_task_ids = get_pending_tasks(token)
-    run_tasks(token, config, pending_task_ids)
     today = date.today()
     weekday = today.weekday()
     if weekday < 5:
         start = today - timedelta(days=weekday)
     else:
         start = today + timedelta(days=7 - weekday)
     days = 14
     end = start + timedelta(days=days)
     booked = get_summary(token, start, end)
     followings = get_followings(token, start, end)
+    current_spaces = run_tasks(token, config, pending_task_ids, followings)
     choices = []
     weeks = [[], []]
     for day_offset in range(days):
         day = start + timedelta(days=day_offset)
         weekday = day.weekday()
         if weekday < 5:
             weeks[day_offset // 7].append(day)
-    print_weeks(weeks, today, booked, followings, choices)
+    print_weeks(weeks, today, booked, followings, choices, current_spaces)
     if not choices:
         return
 
     locations = get_locations(token)
     location = do_inquiry("Office", locations)
 
     questions = [
@@ -501,21 +580,21 @@
         return
     to_book = answers["dates"]
     if not to_book:
         print("No reservations added.")
         return
     check_tasks = add_reservations(token, location, to_book, config)
     booked = get_summary(token, start, end)
-    print_weeks(weeks, today, booked, [], [])
+    print_weeks(weeks, today, booked, {}, [], {})
     if check_tasks:
         for i in range(5):
             print("Waiting for pending tasks...")
             sleep(1)
             pending_task_ids = get_pending_tasks(token)
             if pending_task_ids:
-                run_tasks(token, config, pending_task_ids)
+                run_tasks(token, config, pending_task_ids, followings)
                 return
         print("Unable to find pending tasks.")
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `wawona-1.1.2/src/wawona.egg-info/PKG-INFO` & `wawona-1.2.0/src/wawona.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.1.2
+Version: 1.2.0
 Summary: Easily make office reservations in sequoia from the command line.
-Author-email: yuzawa-san <jtyuzawa@gmail.com>
+Author-email: yuzawa-san <jtyuzawa+wawona@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
 Project-URL: Documentation, https://github.com/yuzawa-san/wawona/blob/master/README.md
 Project-URL: Repository, https://github.com/yuzawa-san/wawona.git
 Project-URL: Funding, http://paypal.me/yuzawasan
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: inquirer>=3.2.4
 Requires-Dist: texttable>=1.7.0
-Requires-Dist: keyring>=24.3.1
+Requires-Dist: keyring>=25.2.1
 Requires-Dist: pytz>=2024.1
+Requires-Dist: selenium>=4.21.0
 
 # 🌲 wawona 🌲
 
 by [@yuzawa-san](https://github.com/yuzawa-san/)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/wawona)](https://pypi.org/project/wawona/)
 
@@ -78,30 +80,40 @@
   Mar 27 New York Reservation
   Complete Self-Screening
   Seat Not Selected
 
 [?] Complete task? (Y/n): 
 [?] I am healthy and not sick?: Yes (only choice)
 [?] Floor: Floor 2 (only choice)
+
+ X X
+ X X   X X
+ X O   O X   O O O X O
+ X X   O O   O * $ O $
+ O O   O O
+ O O   O O   O O O O O
+ O O   O O   O X O O O
+
+* preferred    O free    $ booked by someone you are following    X booked
 [?] Space: 
-   Desk 35
-   Desk 36
-   Desk 37
-   Desk 38
-   Desk 39
-   Desk 40
- > Desk 41
-   Desk 42 (Juan Fnulwoln)
-   Desk 43
-   Desk 44 (Maeve Melwosniwnaiko)
-   Desk 45
-   Desk 46
-   Desk 47
+   Desk 5
+   Desk 6
+   Desk 7
+   Desk 8 (Guillaume Rucpelzsva)
+   Desk 9
+   Desk 10
+ > Desk 11
+   Desk 12 (Juan Fnulwoln)
+   Desk 13
+   Desk 14 (Maeve Melwosniwnaiko)
+   Desk 15
+   Desk 16
+   Desk 17
 
-You have booked 'Desk 41'
+You have booked 'Desk 11'
 ```
 
 ## Install
 
 The easiest way is probably using [Homebrew](https://brew.sh/).
 A self-maintained tap is available for use. To install tap:
 ```console
@@ -122,16 +134,17 @@
 # update just this
 brew upgrade wawona
 ```
 
 ## Usage 
 
 - Run it from your terminal: `wawona`
-- On initial run, you will be asked provide configuration: email and password.
-- You may be prompted to for an MFA token periodically.
+- On initial run, you will be asked to provide configuration details and to do an initial login.
+- Login uses a standalone chrome powered by selenium.
+- Periodically, you will be asked to re-login.
 - Use the up/down arrows, spacebar, and return keys to select items in lists
 - Troubleshooting errors with `wawona --verbose`
 
 ### Reset
 
 If you need to reset to factory defaults (maybe if you changed your password), remove the configuration:
 
@@ -144,14 +157,13 @@
 ```console
 rm -rf ~/.config/wawona/
 ```
 
 ## Notes
 
 - Not affliated with sequoia
-- Does not support SSO
 - Uses public endpoints discovered from the web UI
 - No warranty or stability guarantees, could break one day if something changes on their end
 - Password/token is stored in system keychain
 - Add/remove followers using the app.
 - Basically if it is not here or it breaks here, use the real app/site.
 - Named for the [drive-thru sequoia](https://en.wikipedia.org/wiki/Wawona_Tree)
```

