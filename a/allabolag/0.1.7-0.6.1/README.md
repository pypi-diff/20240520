# Comparing `tmp/allabolag-0.1.7.tar.gz` & `tmp/allabolag-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/allabolag-0.1.7.tar", last modified: Mon Dec 16 07:01:10 2019, max compression
+gzip compressed data, was "allabolag-0.6.1.tar", last modified: Mon May 20 18:32:59 2024, max compression
```

## Comparing `allabolag-0.1.7.tar` & `allabolag-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2019-12-16 07:01:10.000000 allabolag-0.1.7/
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag.egg-info/
--rw-r--r--   0 jens      (1000) jens      (1000)       39 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag.egg-info/requires.txt
--rw-r--r--   0 jens      (1000) jens      (1000)     2577 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag.egg-info/PKG-INFO
--rw-r--r--   0 jens      (1000) jens      (1000)      387 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag.egg-info/SOURCES.txt
--rw-r--r--   0 jens      (1000) jens      (1000)        1 2019-09-18 18:05:01.000000 allabolag-0.1.7/allabolag.egg-info/not-zip-safe
--rw-r--r--   0 jens      (1000) jens      (1000)       10 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag.egg-info/top_level.txt
--rw-r--r--   0 jens      (1000) jens      (1000)        1 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag.egg-info/dependency_links.txt
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2019-12-16 07:01:10.000000 allabolag-0.1.7/test/
--rw-r--r--   0 jens      (1000) jens      (1000)      153 2019-09-18 18:37:43.000000 allabolag-0.1.7/test/test_company.py
--rw-r--r--   0 jens      (1000) jens      (1000)     2577 2019-12-16 07:01:10.000000 allabolag-0.1.7/PKG-INFO
--rw-r--r--   0 jens      (1000) jens      (1000)      109 2019-12-16 07:01:10.000000 allabolag-0.1.7/setup.cfg
--rw-r--r--   0 jens      (1000) jens      (1000)     1492 2019-12-16 07:00:30.000000 allabolag-0.1.7/README.rst
-drwxr-xr-x   0 jens      (1000) jens      (1000)        0 2019-12-16 07:01:10.000000 allabolag-0.1.7/allabolag/
--rw-r--r--   0 jens      (1000) jens      (1000)      975 2019-09-10 19:11:27.000000 allabolag-0.1.7/allabolag/utils.py
--rw-r--r--   0 jens      (1000) jens      (1000)     5745 2019-10-03 11:41:50.000000 allabolag-0.1.7/allabolag/company.py
--rw-r--r--   0 jens      (1000) jens      (1000)     1965 2019-12-16 06:59:01.000000 allabolag-0.1.7/allabolag/liquidated_companies.py
--rw-r--r--   0 jens      (1000) jens      (1000)     4634 2019-09-18 18:37:51.000000 allabolag-0.1.7/allabolag/parsers.py
--rw-r--r--   0 jens      (1000) jens      (1000)      107 2019-09-18 18:37:10.000000 allabolag-0.1.7/allabolag/__init__.py
--rw-r--r--   0 jens      (1000) jens      (1000)     1066 2019-12-16 07:00:50.000000 allabolag-0.1.7/setup.py
--rw-r--r--   0 jens      (1000) jens      (1000)     1089 2019-09-18 11:26:58.000000 allabolag-0.1.7/LICENSE.txt
--rw-r--r--   0 jens      (1000) jens      (1000)        0 2019-09-18 11:27:21.000000 allabolag-0.1.7/MANIFEST.in
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2024-05-20 18:32:59.526916 allabolag-0.6.1/
+-rw-rw-r--   0 jens      (1001) jens      (1001)     1089 2024-05-20 18:21:10.000000 allabolag-0.6.1/LICENSE.txt
+-rw-rw-r--   0 jens      (1001) jens      (1001)        0 2022-01-24 07:39:59.000000 allabolag-0.6.1/MANIFEST.in
+-rw-rw-r--   0 jens      (1001) jens      (1001)     2563 2024-05-20 18:32:59.526916 allabolag-0.6.1/PKG-INFO
+-rw-rw-r--   0 jens      (1001) jens      (1001)     2143 2024-05-20 18:31:10.000000 allabolag-0.6.1/README.rst
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2024-05-20 18:32:59.526916 allabolag-0.6.1/allabolag/
+-rw-rw-r--   0 jens      (1001) jens      (1001)      232 2024-05-20 18:21:10.000000 allabolag-0.6.1/allabolag/__init__.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)     7278 2024-05-20 18:30:08.000000 allabolag-0.6.1/allabolag/company.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)     1312 2024-05-20 18:21:10.000000 allabolag-0.6.1/allabolag/liquidated_companies.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)     1271 2024-05-20 18:26:59.000000 allabolag-0.6.1/allabolag/list.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)     4647 2024-05-20 18:21:10.000000 allabolag-0.6.1/allabolag/parsers.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)      987 2024-05-20 18:28:21.000000 allabolag-0.6.1/allabolag/utils.py
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2024-05-20 18:32:59.526916 allabolag-0.6.1/allabolag.egg-info/
+-rwxrwxrwx   0 jens      (1001) jens      (1001)     2563 2024-05-20 18:32:59.000000 allabolag-0.6.1/allabolag.egg-info/PKG-INFO
+-rwxrwxrwx   0 jens      (1001) jens      (1001)      457 2024-05-20 18:32:59.000000 allabolag-0.6.1/allabolag.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jens      (1001) jens      (1001)        1 2024-05-20 18:32:59.000000 allabolag-0.6.1/allabolag.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jens      (1001) jens      (1001)        1 2019-09-18 18:05:01.000000 allabolag-0.6.1/allabolag.egg-info/not-zip-safe
+-rwxrwxrwx   0 jens      (1001) jens      (1001)       39 2024-05-20 18:32:59.000000 allabolag-0.6.1/allabolag.egg-info/requires.txt
+-rwxrwxrwx   0 jens      (1001) jens      (1001)       10 2024-05-20 18:32:59.000000 allabolag-0.6.1/allabolag.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1001) jens      (1001)      140 2024-05-20 18:32:59.526916 allabolag-0.6.1/setup.cfg
+-rw-rw-r--   0 jens      (1001) jens      (1001)     1067 2024-05-20 18:31:41.000000 allabolag-0.6.1/setup.py
+drwxrwxr-x   0 jens      (1001) jens      (1001)        0 2024-05-20 18:32:59.526916 allabolag-0.6.1/test/
+-rw-rw-r--   0 jens      (1001) jens      (1001)      595 2024-05-20 18:21:10.000000 allabolag-0.6.1/test/test_company.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)      287 2022-01-24 07:42:50.000000 allabolag-0.6.1/test/test_liquidated_companies.py
+-rw-rw-r--   0 jens      (1001) jens      (1001)      568 2024-05-20 18:21:10.000000 allabolag-0.6.1/test/test_list.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `allabolag-0.1.7/README.rst` & `allabolag-0.6.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -56,14 +56,48 @@
 4. Upload: `python3 -m twine upload dist/allabolag-X.Y.X*`
 
 ...assuming you have Twine installed (`pip install twine`) and configured.
 
 Changelog
 ---------
 
+- 0.6.1
+  - Bug fix: Actually use header in requests.
+
+- 0.6.0
+  - Add headers to request
+  - Minor dependency updates
+  - Use logger for debugging
+
+- 0.5.1
+  - Fix return type for `Company.liquidation`
+
+- 0.5.0
+  - Add `Company.liquidation`
+
+- 0.4.1
+  - Remove debug output
+  - Don't crash when we reach the end of a list
+
+- 0.4.0
+  - Add option to start from page N
+  - Add custom exception for missing company
+
+- 0.3.1
+  - Add cache for company data
+
+- 0.3.0
+  - Add `Company.remarks` (a list of remarks, e.g. “Konkurs”)
+
+- 0.2.1
+  - Make `iter_list()` more generic, by accepting the while url fragment
+
+- 0.2.0
+  - Add `iter_list()` function
+
 - 0.1.7
 
   - Bug fix: Add encoding for Python 2.7 
 
 - 0.1.6
 
   - Fixes bug when company has remark about Svensk Handels Varningslistan
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `allabolag-0.1.7/allabolag/utils.py` & `allabolag-0.6.1/allabolag/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,28 @@
         key = dt.text.strip()
         # Assumption that the value is the next sibling
         # this is not always a dd tag (sometimes li tag for example)
         value = dt.find_next_sibling().text.strip()
         d[key] = value
     return d
 
+
 def _prefix_keys(old_dict, prefix):
     """Adds a prefix to all keys in a dict"""
     new_dict = {}
     for key, value in old_dict.items():
         new_key = u"{} - {}".format(prefix, key)
         new_dict[new_key] = old_dict[key]
     return new_dict
 
+
 def _table_to_dict(table):
     data = {}
     years = [x.text.strip() for x in table.select("thead th.data-pager__page")]
     for tr in table.select("tbody tr"):
         try:
             key = tr.select_one("th").text.strip()
-        except:
+        except Exception:
             continue
         values = [x.text.strip() for x in tr.select("td.data-pager__page")]
         data[key] = list(zip(years, values))
     return data
```

### Comparing `allabolag-0.1.7/allabolag/company.py` & `allabolag-0.6.1/allabolag/company.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-# encoding: utf-8
 import requests
 from bs4 import BeautifulSoup
 import re
 from allabolag.utils import _dl_to_dict, _table_to_dict, _prefix_keys
 from allabolag.parsers import PARSERS
+import os
+import logging
+
+logging.basicConfig(level=os.environ.get("LOGLEVEL", "WARNING"))
+logger = logging.getLogger(__name__)
+
+
+class NoSuchCompany(Exception):
+    """Raised when trying to access a copmany that doesn't exist"""
+    pass
+
 
 class Company():
     """Represents a single company.
 
     Usage:
         c = Company("559006-6642")
         print(c.data) # get all cleaned data
         print(c.raw_data) # get all uncleaned data
     """
     def __init__(self, company_code):
         self.company_code = company_code
-        self.url = "https://www.allabolag.se/{}".format(company_code.replace("-",""))
+        self.url = f"https://www.allabolag.se/{company_code.replace('-', '')}"
         self._data = {}
         self._overview_data = {}
         self._activity_data = {}
         self._accounts_data = {}
+        self._cache = {}
 
     @property
     def raw_data(self):
         """Get data from all sections
         """
         data = {}
         data.update(self.overview_data)
@@ -32,24 +43,22 @@
 
         return data
 
     @property
     def data(self):
         return self._clean_data(self.raw_data)
 
-
     @property
     def overview_data(self):
         """Collect data from 'Översikt'
         """
         if self._overview_data == {}:
             s = self._get_soup()
             data = {
                 "Namn": s.select_one("h1").text.strip(),
-
             }
 
             # Parse "Information" box
             information_elem = s.find(text="Information").parent.parent
             info_list = information_elem.select_one("dl")
             information = _dl_to_dict(info_list)
             data.update(information)
@@ -59,16 +68,17 @@
             dl = elem.select_one("dl")
             contacts = _dl_to_dict(dl)
             data.update(contacts)
 
             # Parse "Nyckeltal"
             account_fig_summary_soup = s.select_one(".company-account-figures")
             if account_fig_summary_soup is not None:
-                data["account_figures_year"] = account_fig_summary_soup.select_one("h2").text.strip()
-                account_fig_table =  account_fig_summary_soup.select_one("table")
+                data["account_figures_year"] = account_fig_summary_soup \
+                    .select_one("h2").text.strip()
+                account_fig_table = account_fig_summary_soup.select_one("table")
                 keys = [x.text.strip() for x in account_fig_table.select("th")]
                 values = [x.text.strip() for x in account_fig_table.select("td")]
                 account_figures = dict(zip(keys, values))
                 data.update(account_figures)
             data = _prefix_keys(data, u"Översikt")
 
             self._overview_data = data
@@ -86,15 +96,16 @@
             # hova in alla dt-dd-taggar
             for dl in s.select("dl"):
                 data.update(_dl_to_dict(dl))
 
             # "Verksamhet & ändamål" följer annan struktur (h3 + initliggande tagg)
             verksamhet_header = s.find(text=re.compile(u"^.*Verksamhet & ändamål.*"))
             if verksamhet_header:
-                data[u"Verksamhet & ändamål"] = verksamhet_header.parent.find_next_sibling().text.strip()
+                data[u"Verksamhet & ändamål"] = verksamhet_header \
+                    .parent.find_next_sibling().text.strip()
 
             # SNI-koden ligger som kod (dt) + etikett (dd)
             sni_dl = s.select_one(".accordion-body.sni")
             if sni_dl:
                 if sni_dl.select_one("dt"):
                     data[u"SNI-kod"] = sni_dl.select_one("dt").text.strip()
                     data[u"SNI-bransch"] = sni_dl.select_one("dd").text.strip()
@@ -102,29 +113,47 @@
             data = _prefix_keys(data, "Aktivitet och status")
 
             self._activity_data = data
 
         return self._activity_data
 
     @property
+    def remarks(self):
+        """Get a list of remarks"""
+        s = self._get_soup()
+        ul = s.find("ul", {"class": "remarks"})
+        if not ul:
+            return []
+        lis = ul.find_all("li")
+        return [li.text.strip() for li in lis]
+
+    @property
+    def liquidated(self):
+        """Check if company is liquidated"""
+        konkurs = [r for r in self.remarks if r.startswith("Konkurs")]
+        likvidation = [r for r in self.remarks if r.startswith("Likvidation")]
+        return True if len(konkurs) or len(likvidation) else False
+
+    @property
     def accounts_data(self):
         """Collect data from "Bokslut & nyckeltal" """
         if self._accounts_data == {}:
             data = {}
             s = self._get_soup("bokslut")
             for table in s.select("table"):
-                #print _table_to_dict(table)
-                table_caption = table.select_one("thead th.company-table__pager-button-cell").text.strip()
+                table_caption = table \
+                    .select_one("thead th.company-table__pager-button-cell").text.strip()
                 if table_caption != u"Nyckeltal":
                     table_data = _table_to_dict(table)
                     table_data = _prefix_keys(table_data, table_caption)
                     data.update(table_data)
                 else:
                     # Nyckeltal behöver egen parsing
-                    # Hack Nyckeltalstabellen saknar år, därför tar vi dem från föregående år
+                    # Hack Nyckeltalstabellen saknar år,
+                    # därför tar vi dem från föregående år
                     years = [x[0] for x in list(table_data.values())[0]]
 
                     table_data = {}
                     for tr in table.select("tbody tr"):
                         try:
                             # Celler med
                             key = tr.select_one("span.row-title > span.tooltip > span").text
@@ -145,14 +174,29 @@
             if key in PARSERS:
                 parser = PARSERS[key]
                 dict_[key] = parser(value)
 
         return dict_
 
     def _get_soup(self, endpoint=None):
+        cache_key = endpoint
+        if not cache_key:
+            cache_key = "INDEX"
+        if cache_key in self._cache:
+            return self._cache[cache_key]
         url = self.url
         if endpoint:
             url += "/{}".format(endpoint)
-        print("/GET {}".format(url))
-        r = requests.get(url)
+        # TODO: Allow user to set custom header
+        # As of May 2024 querying without a head does not work
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
+        }
+        logger.info("/GET {}".format(url))
+        r = requests.get(url, headers=headers)
+        if r.status_code == 404:
+            raise NoSuchCompany(f"Company {self.company_code} not found")
+        # forward any other expection
         r.raise_for_status()
-        return BeautifulSoup(r.content, "html.parser")
+        soup = BeautifulSoup(r.content, "html.parser")
+        self._cache[cache_key] = soup
+        return soup
```

### Comparing `allabolag-0.1.7/allabolag/parsers.py` & `allabolag-0.6.1/allabolag/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-# encoding: utf-8
 from datetime import datetime
 
+
 def value(s):
     """Parse float
     """
     if s is None or s == "-" or s == "":
         return None
-    s = s.replace(",",".").replace(" ","").replace(" ","")
+    s = s.replace(",", ".").replace(" ", "").replace(" ", "")
     if s.endswith("%"):
         s = s.replace("%", "")
         return float(s) / 100.0
     else:
         return float(s)
 
     raise Exception(u"Unable to parse value from '{}'".format(s))
 
+
 def date(s):
     """Parse datetime"""
     return datetime.strptime(s, "%Y-%m-%d")
 
-def date_value(l):
+
+def date_value(list_):
     """Parse [YEAR, VALUE] pair.
 
     date_value("2018-02", 25%) => [datetime(2018,2,1), 0.25]
     """
     return [
-        #datetime.strptime(l[0], "%Y-%m"),
-        l[0],
-        value(l[1])
+        # datetime.strptime(l[0], "%Y-%m"),
+        list_[0],
+        value(list_[1]),
     ]
 
+
 def date_value_list(ll):
-    return [date_value(l) for l in ll]
+    return [date_value(list_) for list_ in ll]
+
 
 def text(s):
     if s.endswith(u"Läs mer"):
         s = s.replace(u"Läs mer", "").strip()
     return s
 
+
 # Define parser for specific data fields
 PARSERS = {
     u"Aktivitet och status - Anledning till avregistrering": text,
     u"Aktivitet och status - Anmärkning": text,
     u"Aktivitet och status - Bolaget registrerat": text,
     u"Aktivitet och status - Bolagsform": text,
     u"Aktivitet och status - F-Skatt": text,
```

### Comparing `allabolag-0.1.7/setup.py` & `allabolag-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ###
 # Versioning
 ###
 from datetime import date
 
 name = "allabolag"
 
-short_version = "0.1.7"
+short_version = "0.6.1"
 long_version = short_version
 
 short_desc = """\
 Scrape data from allabolag.se.\
 """
 authors = u"Jens Finnäs, Newsworthy"
 year = date.today().year
@@ -21,14 +21,15 @@
 
 version = long_version
 
 ###
 # Setup
 ###
 
+
 def readme():
     """Import README for use as long_description."""
     with open("README.rst") as f:
         return f.read()
 
 
 repo = "https://github.com/marple-newsrobot/allabolag"
```

### Comparing `allabolag-0.1.7/LICENSE.txt` & `allabolag-0.6.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Journalism Robotics Ab Stockholm
+Copyright (c) 2019 Journalism Robotics AB Stockholm
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

