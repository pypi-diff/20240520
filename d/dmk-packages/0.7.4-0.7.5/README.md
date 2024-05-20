# Comparing `tmp/dmk_packages-0.7.4.tar.gz` & `tmp/dmk_packages-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.7.4.tar", last modified: Sat May 18 16:17:59 2024, max compression
+gzip compressed data, was "dmk_packages-0.7.5.tar", last modified: Mon May 20 03:33:50 2024, max compression
```

## Comparing `dmk_packages-0.7.4.tar` & `dmk_packages-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 16:17:59.273525 dmk_packages-0.7.4/
--rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.7.4/LICENSE
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-18 16:17:59.272599 dmk_packages-0.7.4/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.7.4/README.md
--rw-r--r--   0 layla      (501) staff       (20)      584 2024-05-18 16:16:08.000000 dmk_packages-0.7.4/pyproject.toml
--rw-r--r--   0 layla      (501) staff       (20)       38 2024-05-18 16:17:59.273788 dmk_packages-0.7.4/setup.cfg
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 16:17:59.254801 dmk_packages-0.7.4/src/
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 16:17:59.258165 dmk_packages-0.7.4/src/dmk_packages/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.4/src/dmk_packages/__init__.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 16:17:59.268232 dmk_packages-0.7.4/src/dmk_packages/crawler/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3534 2024-05-04 15:01:16.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 layla      (501) staff       (20)     6580 2024-05-04 15:01:16.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 layla      (501) staff       (20)     6685 2024-05-04 15:01:16.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 layla      (501) staff       (20)    18165 2024-05-18 16:16:08.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 layla      (501) staff       (20)     1382 2024-05-04 15:01:16.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/pdf_to_text.py
--rw-r--r--   0 layla      (501) staff       (20)    14699 2024-05-05 04:51:03.000000 dmk_packages-0.7.4/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 16:17:59.269927 dmk_packages-0.7.4/src/dmk_packages/database/
--rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.7.4/src/dmk_packages/database/__init__.py
--rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.7.4/src/dmk_packages/database/database.py
--rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.7.4/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-18 16:17:59.271226 dmk_packages-0.7.4/src/dmk_packages.egg-info/
--rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-18 16:17:59.000000 dmk_packages-0.7.4/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 layla      (501) staff       (20)      677 2024-05-18 16:17:59.000000 dmk_packages-0.7.4/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 layla      (501) staff       (20)        1 2024-05-18 16:17:59.000000 dmk_packages-0.7.4/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 layla      (501) staff       (20)       41 2024-05-18 16:17:59.000000 dmk_packages-0.7.4/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 layla      (501) staff       (20)       13 2024-05-18 16:17:59.000000 dmk_packages-0.7.4/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.935014 dmk_packages-0.7.5/
+-rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/LICENSE
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-05-20 03:33:50.934749 dmk_packages-0.7.5/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/README.md
+-rw-r--r--   0 tommie     (501) staff       (20)      584 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/pyproject.toml
+-rw-r--r--   0 tommie     (501) staff       (20)       38 2024-05-20 03:33:50.935073 dmk_packages-0.7.5/setup.cfg
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.928168 dmk_packages-0.7.5/src/
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.929472 dmk_packages-0.7.5/src/dmk_packages/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/src/dmk_packages/__init__.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.932607 dmk_packages-0.7.5/src/dmk_packages/crawler/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-30 04:52:14.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6462 2024-05-20 03:29:38.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 tommie     (501) staff       (20)     6685 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 tommie     (501) staff       (20)    18165 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 tommie     (501) staff       (20)    14699 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.933157 dmk_packages-0.7.5/src/dmk_packages/database/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/src/dmk_packages/database/database.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.7.5/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.933999 dmk_packages-0.7.5/src/dmk_packages/utils/
+-rw-r--r--   0 tommie     (501) staff       (20)        0 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/src/dmk_packages/utils/__init__.py
+-rw-r--r--   0 tommie     (501) staff       (20)      975 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/src/dmk_packages/utils/day_off.py
+-rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-05-20 03:28:59.000000 dmk_packages-0.7.5/src/dmk_packages/utils/pdf_to_text.py
+drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-20 03:33:50.934425 dmk_packages-0.7.5/src/dmk_packages.egg-info/
+-rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-05-20 03:33:50.000000 dmk_packages-0.7.5/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 tommie     (501) staff       (20)      744 2024-05-20 03:33:50.000000 dmk_packages-0.7.5/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 tommie     (501) staff       (20)        1 2024-05-20 03:33:50.000000 dmk_packages-0.7.5/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       41 2024-05-20 03:33:50.000000 dmk_packages-0.7.5/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 tommie     (501) staff       (20)       13 2024-05-20 03:33:50.000000 dmk_packages-0.7.5/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.7.4/LICENSE` & `dmk_packages-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/PKG-INFO` & `dmk_packages-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.7.4
+Version: 0.7.5
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.7.4/README.md` & `dmk_packages-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/pyproject.toml` & `dmk_packages-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.7.4"
+version = "0.7.5"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.7.5/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.7.5/src/dmk_packages/crawler/clien.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,15 @@
         게시물들의 기본적인 내용 크롤링
         """
         items = soup.select(".list_item.symph_row.jirum")
         results = []
 
         for item in items:
             board_sn = int(item["data-board-sn"])
-            _regist_date = pendulum.parse(item.select_one(".timestamp").text)
-            regist_date = _regist_date.add(hours=18)
+            regist_date = pendulum.parse(item.select_one(".timestamp").text)
 
             title = item.select_one(".subject_fixed").text
             if "헤드라인 모음" in title:
                 continue
 
             if self._min_board_sn <= board_sn <= self._max_board_sn:
                 continue
@@ -122,15 +121,14 @@
         pages = soup.select(".board-nav-page")
         if len(pages) <= 1:
             return None
         next_btn_exists = bool(soup.select_one(".board-nav-next"))
 
         last_item = soup.select(".list_item.symph_row.jirum")[-1]
         last_item_timestamp = pendulum.parse(last_item.select_one(".timestamp").text)
-        last_item_timestamp = last_item_timestamp.add(hours=18)
 
         if self._date_from > last_item_timestamp:
             return None
 
         for idx, page in enumerate(pages):
             if "active" in page.get("class", []):
                 if next_btn_exists or idx + 1 < len(pages):
```

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.7.5/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.7.5/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.7.5/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/pdf_to_text.py` & `dmk_packages-0.7.5/src/dmk_packages/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.7.5/src/dmk_packages/crawler/youtube.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/database/database.py` & `dmk_packages-0.7.5/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.7.5/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.7.4/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.7.5/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.7.4
+Version: 0.7.5
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.7.4/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.7.5/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 src/dmk_packages.egg-info/top_level.txt
 src/dmk_packages/crawler/__init__.py
 src/dmk_packages/crawler/bigkinds.py
 src/dmk_packages/crawler/clien.py
 src/dmk_packages/crawler/fnguide.py
 src/dmk_packages/crawler/naver_blog.py
 src/dmk_packages/crawler/naver_search_volume.py
-src/dmk_packages/crawler/pdf_to_text.py
 src/dmk_packages/crawler/youtube.py
 src/dmk_packages/database/__init__.py
-src/dmk_packages/database/database.py
+src/dmk_packages/database/database.py
+src/dmk_packages/utils/__init__.py
+src/dmk_packages/utils/day_off.py
+src/dmk_packages/utils/pdf_to_text.py
```

