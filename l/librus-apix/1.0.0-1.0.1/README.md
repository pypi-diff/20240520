# Comparing `tmp/librus_apix-1.0.0.tar.gz` & `tmp/librus_apix-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-1.0.0.tar", last modified: Sat May 18 20:21:14 2024, max compression
+gzip compressed data, was "librus_apix-1.0.1.tar", last modified: Mon May 20 16:33:59 2024, max compression
```

## Comparing `librus_apix-1.0.0.tar` & `librus_apix-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:21:14.008468 librus_apix-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 20:21:10.000000 librus_apix-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 20:21:14.008468 librus_apix-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-18 20:21:10.000000 librus_apix-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:21:14.008468 librus_apix-1.0.0/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:21:14.008468 librus_apix-1.0.0/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 20:21:10.000000 librus_apix-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-18 20:21:14.008468 librus_apix-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:21:10.000000 librus_apix-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:59.734650 librus_apix-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 16:33:53.000000 librus_apix-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 16:33:59.734650 librus_apix-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-20 16:33:53.000000 librus_apix-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:59.734650 librus_apix-1.0.1/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:59.734650 librus_apix-1.0.1/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 16:33:53.000000 librus_apix-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 16:33:59.734650 librus_apix-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:33:53.000000 librus_apix-1.0.1/setup.py
```

### Comparing `librus_apix-1.0.0/LICENSE` & `librus_apix-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/README.md` & `librus_apix-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/__init__.py` & `librus_apix-1.0.1/librus_apix/__init__.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/announcements.py` & `librus_apix-1.0.1/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/attendance.py` & `librus_apix-1.0.1/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/client.py` & `librus_apix-1.0.1/librus_apix/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         HOMEWORK_URL (str): The URL for homework.
         HOMEWORK_DETAILS_URL (str): The URL for homework details.
         INFO_URL (str): The URL for information.
         COMPLETED_LESSONS_URL (str): The URL for completed lessons.
         GATEWAY_API_ATTENDANCE (str): The URL for gateway API attendance.
         RECIPIENTS_URL (str): The URL for recipients.
         RECIPIENT_GROUPS_URL (str): The URL for recipient groups.
+        INDEX_URL (str): Url for student index
         cookies (RequestsCookieJar): additional cookies
         _session (Session): The requests session for making HTTP calls.
 
     Methods:
         refresh_oauth() -> str:
             Refreshes the OAuth token then returns it.
         post(url: str, data: Dict[str, str]) -> Response:
@@ -172,14 +173,15 @@
         homework_details_url: str = urls.HOMEWORK_DETAILS_URL,
         info_url: str = urls.INFO_URL,
         recipients_url: str = urls.RECIPIENTS_URL,
         recipient_groups_url: str = urls.RECIPIENT_GROUPS_URL,
         completed_lessons_url: str = urls.COMPLETED_LESSONS_URL,
         gateway_api_attendance: str = urls.GATEWAY_API_ATTENDANCE,
         refresh_oauth_url: str = urls.REFRESH_OAUTH_URL,
+        index_url: str = urls.INDEX_URL,
         proxy: Dict[str, str] = {},
         extra_cookies: RequestsCookieJar = RequestsCookieJar(),
     ):
         self.token = token
         self.proxy = proxy
         self.BASE_URL = base_url
         self.API_URL = api_url
@@ -195,14 +197,15 @@
         self.HOMEWORK_DETAILS_URL = homework_details_url
         self.INFO_URL = info_url
         self.COMPLETED_LESSONS_URL = completed_lessons_url
         self.GATEWAY_API_ATTENDANCE = gateway_api_attendance
         self.RECIPIENTS_URL = recipients_url
         self.RECIPIENT_GROUPS_URL = recipient_groups_url
         self.REFRESH_URL = refresh_oauth_url
+        self.INDEX_URL = index_url
         self.cookies = extra_cookies
         self._session = Session()
         """
         Initializes a new instance of Client.
 
         Args:
             token (Token): The authentication token required for API access.
@@ -355,14 +358,15 @@
     homework_details_url: str = urls.HOMEWORK_DETAILS_URL,
     info_url: str = urls.INFO_URL,
     recipients_url: str = urls.RECIPIENTS_URL,
     recipient_groups_url: str = urls.RECIPIENT_GROUPS_URL,
     completed_lessons_url: str = urls.COMPLETED_LESSONS_URL,
     gateway_api_attendance: str = urls.GATEWAY_API_ATTENDANCE,
     refresh_oauth_url: str = urls.REFRESH_OAUTH_URL,
+    index_url: str = urls.INDEX_URL,
     proxy: dict[str, str] = {},
 ):
     """
     Creates a new instance of the Client class.
 
     Args:
         token (Optional[Token], optional): The authentication token. Defaults to None.
@@ -380,14 +384,15 @@
         homework_details_url (str, optional): The URL of the homework details endpoint. Defaults to urls.HOMEWORK_DETAILS_URL.
         info_url (str, optional): The URL of the info endpoint. Defaults to urls.INFO_URL.
         recipients_url (str, optional): The URL of the recipients endpoint. Defaults to urls.RECIPIENTS_URL.
         recipient_groups_url (str, optional): The URL of the recipient groups endpoint. Defaults to urls.RECIPIENT_GROUPS_URL.
         completed_lessons_url (str, optional): The URL of the completed lessons endpoint. Defaults to urls.COMPLETED_LESSONS_URL.
         gateway_api_attendance (str, optional): The URL of the gateway API attendance endpoint. Defaults to urls.GATEWAY_API_ATTENDANCE.
         refresh_oauth_url (str, optional): The URL of the refresh OAuth endpoint. Defaults to urls.REFRESH_OAUTH_URL.
+        index_url (str, optional): The url for student index
         proxy (dict[str, str], optional): A dictionary containing proxy settings. Defaults to an empty dictionary.
 
     Returns:
         Client: A new instance of the Client class.
     """
     if not isinstance(token, Token):
         token = Token()
@@ -407,9 +412,10 @@
         homework_details_url,
         info_url,
         recipients_url,
         recipient_groups_url,
         completed_lessons_url,
         gateway_api_attendance,
         refresh_oauth_url,
+        index_url,
         proxy,
     )
```

### Comparing `librus_apix-1.0.0/librus_apix/completed_lessons.py` & `librus_apix-1.0.1/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/exceptions.py` & `librus_apix-1.0.1/librus_apix/exceptions.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/grades.py` & `librus_apix-1.0.1/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/helpers.py` & `librus_apix-1.0.1/librus_apix/helpers.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/homework.py` & `librus_apix-1.0.1/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/messages.py` & `librus_apix-1.0.1/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/schedule.py` & `librus_apix-1.0.1/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/student_information.py` & `librus_apix-1.0.1/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/timetable.py` & `librus_apix-1.0.1/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.0/librus_apix/urls.py` & `librus_apix-1.0.1/librus_apix/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Constants:
     ```python
     - HEADERS: A dictionary containing HTTP headers for making requests.
     - BASE_URL: The base URL for the Librus website.
     - API_URL: The base URL for the Librus API.
+    - INDEX_URL: Student Index url
     - GRADES_URL: URL for accessing grades.
     - TIMETABLE_URL: URL for accessing the timetable.
     - ANNOUNCEMENTS_URL: URL for accessing announcements.
     - MESSAGE_URL: URL for accessing messages.
     - RECIPIENT_GROUPS_URL: URL for retrieving recipient groups for messages.
     - RECIPIENTS_URL: URL for retrieving recipients for messages.
     - SEND_MESSAGE_URL: URL for sending messages.
@@ -28,14 +29,15 @@
 
 HEADERS: Dict[str, Union[str, bytes]] = {
     "User-Agent": "Mozilla/5.0 (Windows NT x.y; Win64; x64; rv:10.0) Gecko/20100101 Firefox/10.0",
     "Content-Type": "application/x-www-form-urlencoded",
 }
 BASE_URL = "https://synergia.librus.pl"
 API_URL = "https://api.librus.pl"
+INDEX_URL = BASE_URL + "/uczen/index"
 GRADES_URL = BASE_URL + "/przegladaj_oceny/uczen"
 TIMETABLE_URL = f"{BASE_URL}/przegladaj_plan_lekcji"
 ANNOUNCEMENTS_URL = f"{BASE_URL}/ogloszenia"
 MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/5"
 RECIPIENT_GROUPS_URL = f"{BASE_URL}/wiadomosci/2/6"
 RECIPIENTS_URL = f"{BASE_URL}/getRecipients"
 SEND_MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/6"
```

### Comparing `librus_apix-1.0.0/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.1/librus_apix.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 librus_apix/client.py
 librus_apix/completed_lessons.py
 librus_apix/exceptions.py
 librus_apix/grades.py
 librus_apix/helpers.py
 librus_apix/homework.py
 librus_apix/messages.py
+librus_apix/notifications.py
 librus_apix/schedule.py
 librus_apix/student_information.py
 librus_apix/timetable.py
 librus_apix/urls.py
 librus_apix.egg-info/PKG-INFO
 librus_apix.egg-info/SOURCES.txt
 librus_apix.egg-info/dependency_links.txt
```

### Comparing `librus_apix-1.0.0/setup.cfg` & `librus_apix-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v1.0.0
+version = v1.0.1
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

