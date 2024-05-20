# Comparing `tmp/acb-0.6.0.tar.gz` & `tmp/acb-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.6.0.tar", last modified: Sun May 19 15:51:54 2024, max compression
+gzip compressed data, was "acb-0.6.1.tar", last modified: Sun May 19 20:00:46 2024, max compression
```

## Comparing `acb-0.6.0.tar` & `acb-0.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.6.0/LICENSE
--rw-r--r--   0        0        0      877 2024-02-25 15:01:48.403334 acb-0.6.0/README.md
--rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.6.0/acb/__init__.py
--rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.6.0/acb/actions/__init__.py
--rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.6.0/acb/actions/compress.py
--rw-r--r--   0        0        0     4784 2024-03-18 08:07:46.797620 acb-0.6.0/acb/actions/encode.py
--rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.6.0/acb/actions/hash.py
--rw-r--r--   0        0        0     5526 2024-03-18 07:52:52.122921 acb-0.6.0/acb/adapters/__init__.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.6.0/acb/adapters/app/__init__.py
--rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.6.0/acb/adapters/app/_base.py
--rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.6.0/acb/adapters/app/main.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.6.0/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.6.0/acb/adapters/cache/_base.py
--rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.6.0/acb/adapters/cache/memory.py
--rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.6.0/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.6.0/acb/adapters/dns/__init__.py
--rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.6.0/acb/adapters/dns/_base.py
--rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.6.0/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.6.0/acb/adapters/ftpd/__init__.py
--rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.6.0/acb/adapters/ftpd/_base.py
--rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.6.0/acb/adapters/ftpd/ftp.py
--rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.6.0/acb/adapters/ftpd/sftp.py
--rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.6.0/acb/adapters/logger/__init__.py
--rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.6.0/acb/adapters/logger/_base.py
--rw-r--r--   0        0        0     3512 2024-04-12 00:33:56.007870 acb-0.6.0/acb/adapters/logger/loguru.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.6.0/acb/adapters/logger/structlog.py
--rw-r--r--   0        0        0       63 2024-02-07 20:56:24.207919 acb-0.6.0/acb/adapters/models/__init__.py
--rw-r--r--   0        0        0      247 2024-05-19 15:42:40.075662 acb-0.6.0/acb/adapters/models/_base.py
--rw-r--r--   0        0        0     2361 2024-05-19 15:48:46.214106 acb-0.6.0/acb/adapters/models/default.py
--rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.6.0/acb/adapters/monitoring/__init__.py
--rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.6.0/acb/adapters/monitoring/_base.py
--rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.6.0/acb/adapters/monitoring/sentry.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.6.0/acb/adapters/nosql/__init__.py
--rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.6.0/acb/adapters/nosql/_base.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.6.0/acb/adapters/nosql/firestore.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.6.0/acb/adapters/nosql/mongodb.py
--rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.6.0/acb/adapters/nosql/redis.py
--rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.6.0/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.6.0/acb/adapters/requests/_base.py
--rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.6.0/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.6.0/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.6.0/acb/adapters/secret/_base.py
--rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.6.0/acb/adapters/secret/infisical.py
--rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.6.0/acb/adapters/secret/secret_manager.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.6.0/acb/adapters/smtp/__init__.py
--rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.6.0/acb/adapters/smtp/_base.py
--rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.6.0/acb/adapters/smtp/gmail.py
--rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.6.0/acb/adapters/smtp/mailgun.py
--rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.6.0/acb/adapters/sql/__init__.py
--rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.6.0/acb/adapters/sql/_backup.py
--rw-r--r--   0        0        0     6668 2024-04-02 07:53:33.461560 acb-0.6.0/acb/adapters/sql/_base.py
--rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.6.0/acb/adapters/sql/_migrate.py
--rw-r--r--   0        0        0      253 2024-03-09 15:10:21.640219 acb-0.6.0/acb/adapters/sql/mysql.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.6.0/acb/adapters/sql/pgsql.py
--rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.6.0/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.6.0/acb/adapters/storage/_base.py
--rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.6.0/acb/adapters/storage/azure.py
--rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.6.0/acb/adapters/storage/cloud_storage.py
--rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.6.0/acb/adapters/storage/file.py
--rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.6.0/acb/adapters/storage/memory.py
--rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.6.0/acb/adapters/storage/s3.py
--rw-r--r--   0        0        0    10433 2024-04-02 07:37:38.490567 acb-0.6.0/acb/config.py
--rw-r--r--   0        0        0     2212 2024-04-02 07:49:59.744042 acb-0.6.0/acb/debug.py
--rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.6.0/acb/depends.py
--rw-r--r--   0        0        0     3444 2024-05-19 15:51:54.369318 acb-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 acb-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.6.1/LICENSE
+-rw-r--r--   0        0        0      772 2024-05-19 19:52:53.054302 acb-0.6.1/README.md
+-rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.6.1/acb/__init__.py
+-rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.6.1/acb/actions/__init__.py
+-rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.6.1/acb/actions/compress.py
+-rw-r--r--   0        0        0     4784 2024-03-18 08:07:46.797620 acb-0.6.1/acb/actions/encode.py
+-rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.6.1/acb/actions/hash.py
+-rw-r--r--   0        0        0     5526 2024-03-18 07:52:52.122921 acb-0.6.1/acb/adapters/__init__.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.6.1/acb/adapters/app/__init__.py
+-rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.6.1/acb/adapters/app/_base.py
+-rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.6.1/acb/adapters/app/main.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.6.1/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.6.1/acb/adapters/cache/_base.py
+-rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.6.1/acb/adapters/cache/memory.py
+-rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.6.1/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.6.1/acb/adapters/dns/__init__.py
+-rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.6.1/acb/adapters/dns/_base.py
+-rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.6.1/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.6.1/acb/adapters/ftpd/__init__.py
+-rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.6.1/acb/adapters/ftpd/_base.py
+-rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.6.1/acb/adapters/ftpd/ftp.py
+-rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.6.1/acb/adapters/ftpd/sftp.py
+-rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.6.1/acb/adapters/logger/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.6.1/acb/adapters/logger/_base.py
+-rw-r--r--   0        0        0     3512 2024-04-12 00:33:56.007870 acb-0.6.1/acb/adapters/logger/loguru.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.6.1/acb/adapters/logger/structlog.py
+-rw-r--r--   0        0        0       63 2024-02-07 20:56:24.207919 acb-0.6.1/acb/adapters/models/__init__.py
+-rw-r--r--   0        0        0      247 2024-05-19 15:42:40.075662 acb-0.6.1/acb/adapters/models/_base.py
+-rw-r--r--   0        0        0     2361 2024-05-19 15:48:46.214106 acb-0.6.1/acb/adapters/models/default.py
+-rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.6.1/acb/adapters/monitoring/__init__.py
+-rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.6.1/acb/adapters/monitoring/_base.py
+-rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.6.1/acb/adapters/monitoring/sentry.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.6.1/acb/adapters/nosql/__init__.py
+-rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.6.1/acb/adapters/nosql/_base.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.6.1/acb/adapters/nosql/firestore.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.6.1/acb/adapters/nosql/mongodb.py
+-rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.6.1/acb/adapters/nosql/redis.py
+-rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.6.1/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.6.1/acb/adapters/requests/_base.py
+-rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.6.1/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.6.1/acb/adapters/secret/__init__.py
+-rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.6.1/acb/adapters/secret/_base.py
+-rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.6.1/acb/adapters/secret/infisical.py
+-rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.6.1/acb/adapters/secret/secret_manager.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.6.1/acb/adapters/smtp/__init__.py
+-rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.6.1/acb/adapters/smtp/_base.py
+-rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.6.1/acb/adapters/smtp/gmail.py
+-rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.6.1/acb/adapters/smtp/mailgun.py
+-rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.6.1/acb/adapters/sql/__init__.py
+-rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.6.1/acb/adapters/sql/_backup.py
+-rw-r--r--   0        0        0     6668 2024-04-02 07:53:33.461560 acb-0.6.1/acb/adapters/sql/_base.py
+-rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.6.1/acb/adapters/sql/_migrate.py
+-rw-r--r--   0        0        0      253 2024-03-09 15:10:21.640219 acb-0.6.1/acb/adapters/sql/mysql.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.6.1/acb/adapters/sql/pgsql.py
+-rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.6.1/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.6.1/acb/adapters/storage/_base.py
+-rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.6.1/acb/adapters/storage/azure.py
+-rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.6.1/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.6.1/acb/adapters/storage/file.py
+-rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.6.1/acb/adapters/storage/memory.py
+-rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.6.1/acb/adapters/storage/s3.py
+-rw-r--r--   0        0        0    10433 2024-04-02 07:37:38.490567 acb-0.6.1/acb/config.py
+-rw-r--r--   0        0        0     2212 2024-04-02 07:49:59.744042 acb-0.6.1/acb/debug.py
+-rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.6.1/acb/depends.py
+-rw-r--r--   0        0        0     3444 2024-05-19 20:00:46.441353 acb-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3528 1970-01-01 00:00:00.000000 acb-0.6.1/PKG-INFO
```

### Comparing `acb-0.6.0/LICENSE` & `acb-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/__init__.py` & `acb-0.6.1/acb/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/actions/__init__.py` & `acb-0.6.1/acb/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/actions/compress.py` & `acb-0.6.1/acb/actions/compress.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/actions/encode.py` & `acb-0.6.1/acb/actions/encode.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/actions/hash.py` & `acb-0.6.1/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/__init__.py` & `acb-0.6.1/acb/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/app/main.py` & `acb-0.6.1/acb/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/cache/_base.py` & `acb-0.6.1/acb/adapters/cache/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/cache/memory.py` & `acb-0.6.1/acb/adapters/cache/memory.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/cache/redis.py` & `acb-0.6.1/acb/adapters/cache/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/dns/_base.py` & `acb-0.6.1/acb/adapters/dns/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/dns/cloud_dns.py` & `acb-0.6.1/acb/adapters/dns/cloud_dns.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/ftpd/ftp.py` & `acb-0.6.1/acb/adapters/ftpd/ftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/ftpd/sftp.py` & `acb-0.6.1/acb/adapters/ftpd/sftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/logger/loguru.py` & `acb-0.6.1/acb/adapters/logger/loguru.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/models/default.py` & `acb-0.6.1/acb/adapters/models/default.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/monitoring/sentry.py` & `acb-0.6.1/acb/adapters/monitoring/sentry.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/nosql/redis.py` & `acb-0.6.1/acb/adapters/nosql/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/requests/_base.py` & `acb-0.6.1/acb/adapters/requests/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/requests/httpx.py` & `acb-0.6.1/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/secret/_base.py` & `acb-0.6.1/acb/adapters/secret/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/secret/secret_manager.py` & `acb-0.6.1/acb/adapters/secret/secret_manager.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/smtp/_base.py` & `acb-0.6.1/acb/adapters/smtp/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/smtp/gmail.py` & `acb-0.6.1/acb/adapters/smtp/gmail.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/smtp/mailgun.py` & `acb-0.6.1/acb/adapters/smtp/mailgun.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/sql/_backup.py` & `acb-0.6.1/acb/adapters/sql/_backup.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/sql/_base.py` & `acb-0.6.1/acb/adapters/sql/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/storage/_base.py` & `acb-0.6.1/acb/adapters/storage/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/storage/cloud_storage.py` & `acb-0.6.1/acb/adapters/storage/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/adapters/storage/file.py` & `acb-0.6.1/acb/adapters/storage/file.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/config.py` & `acb-0.6.1/acb/config.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/debug.py` & `acb-0.6.1/acb/debug.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/acb/depends.py` & `acb-0.6.1/acb/depends.py`

 * *Files identical despite different names*

### Comparing `acb-0.6.0/pyproject.toml` & `acb-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 config = [
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "crackerjack>=0.7.25",
+    "crackerjack>=0.7.33",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
@@ -37,37 +37,37 @@
 
 [tool.creosote]
 paths = [
     "acb",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pdm",
+    "pytest",
     "pdm-bump",
+    "pdm",
+    "pyfiglet",
     "pre-commit",
     "autotyping",
-    "pyfiglet",
-    "pyyaml",
     "ulid-py",
-    "pytest",
     "phonenumbers",
     "alive-progress",
+    "pyyaml",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "acb",
 ]
 skips = [
     "B603",
-    "B404",
     "B403",
+    "B404",
     "B113",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "acb",
@@ -89,35 +89,35 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "acb"
-version = "0.6.0"
+version = "0.6.1"
 description = "Asynchronous Component Base"
 dependencies = [
-    "itsdangerous>=2.1.2",
+    "itsdangerous>=2.2.0",
     "arrow>=1.3.0",
     "dill>=0.3.8",
     "blake3>=0.4.1",
     "loguru>=0.7.2",
     "msgspec[toml]>=0.18.6",
     "nest-asyncio>=1.6.0",
-    "pydantic-settings>=2.2.0",
+    "pydantic-settings>=2.2.1",
     "bevy>=2.0.2",
     "icecream>=2.1.3",
     "brotli>=1.1.0",
     "pyfiglet>=1.0.2",
     "alive-progress>=3.1.5",
     "inflection>=0.5.1",
     "aiopath>=0.7.7",
     "pyyaml>=6.0.1",
     "google-crc32c>=1.5.0",
-    "pydantic[email]>=2.6.1",
+    "pydantic[email]>=2.7.1",
     "devtools>=0.12.2",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -140,53 +140,53 @@
 [project.urls]
 Homepage = "https://github.com/lesleslie/acb"
 Documentation = "https://github.com/lesleslie/acb"
 Repository = "https://github.com/lesleslie/acb"
 
 [project.optional-dependencies]
 cache = [
-    "cashews[redis]>=7.0.0",
+    "cashews[redis]>=7.1.0",
 ]
 storage = [
-    "gcsfs>=2024.2.0",
-    "s3fs>=2024.2.0",
-    "adlfs>=2024.2.0",
+    "gcsfs>=2024.5.0",
+    "s3fs>=2024.5.0",
+    "adlfs>=2024.4.1",
 ]
 dns = [
     "google-cloud-dns>=0.35.0",
-    "validators>=0.22.0",
+    "validators>=0.28.1",
 ]
 requests = [
-    "httpx[http2]>=0.26.0",
-    "hishel>=0.0.24",
+    "httpx[http2]>=0.27.0",
+    "hishel>=0.0.26",
 ]
 email = [
     "mailgun>=0.1.1",
 ]
 sql = [
-    "sqlalchemy>=2.0.27",
-    "sqlalchemy-utils>=0.41.1",
+    "sqlalchemy>=2.0.30",
+    "sqlalchemy-utils>=0.41.2",
     "mysqlclient>=2.2.4",
     "asyncmy>=0.2.9",
-    "sqlmodel>=0.0.16",
-    "babel>=2.14.0",
+    "sqlmodel>=0.0.18",
+    "babel>=2.15.0",
 ]
 nosql = [
-    "google-cloud-firestore>=2.14.0",
-    "motor>=3.3.2",
+    "google-cloud-firestore>=2.16.0",
+    "motor>=3.4.0",
 ]
 demo = [
-    "faker>=23.2.1",
+    "faker>=25.2.0",
 ]
 ftp = [
     "aioftp>=0.22.3",
     "asyncssh>=2.14.2",
 ]
 secret = [
-    "google-cloud-secret-manager>=2.18.2",
+    "google-cloud-secret-manager>=2.20.0",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `acb-0.6.0/PKG-INFO` & `acb-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6163 620a  : 2.1.Name: acb.
-00000020: 5665 7273 696f 6e3a 2030 2e36 2e30 0a53  Version: 0.6.0.S
+00000020: 5665 7273 696f 6e3a 2030 2e36 2e31 0a53  Version: 0.6.1.S
 00000030: 756d 6d61 7279 3a20 4173 796e 6368 726f  ummary: Asynchro
 00000040: 6e6f 7573 2043 6f6d 706f 6e65 6e74 2042  nous Component B
 00000050: 6173 650a 4175 7468 6f72 2d45 6d61 696c  ase.Author-Email
 00000060: 3a20 6c65 736c 6573 6c69 6520 3c6c 6573  : lesleslie <les
 00000070: 4077 6564 6777 6f6f 6477 6562 776f 726b  @wedgwoodwebwork
 00000080: 732e 636f 6d3e 0a4c 6963 656e 7365 3a20  s.com>.License: 
 00000090: 4253 442d 332d 436c 6175 7365 0a43 6c61  BSD-3-Clause.Cla
@@ -45,30 +45,30 @@
 000002c0: 6573 6c65 736c 6965 2f61 6362 0a50 726f  esleslie/acb.Pro
 000002d0: 6a65 6374 2d55 524c 3a20 5265 706f 7369  ject-URL: Reposi
 000002e0: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
 000002f0: 7468 7562 2e63 6f6d 2f6c 6573 6c65 736c  thub.com/leslesl
 00000300: 6965 2f61 6362 0a52 6571 7569 7265 732d  ie/acb.Requires-
 00000310: 5079 7468 6f6e 3a20 3e3d 332e 3132 0a52  Python: >=3.12.R
 00000320: 6571 7569 7265 732d 4469 7374 3a20 6974  equires-Dist: it
-00000330: 7364 616e 6765 726f 7573 3e3d 322e 312e  sdangerous>=2.1.
-00000340: 320a 5265 7175 6972 6573 2d44 6973 743a  2.Requires-Dist:
+00000330: 7364 616e 6765 726f 7573 3e3d 322e 322e  sdangerous>=2.2.
+00000340: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
 00000350: 2061 7272 6f77 3e3d 312e 332e 300a 5265   arrow>=1.3.0.Re
 00000360: 7175 6972 6573 2d44 6973 743a 2064 696c  quires-Dist: dil
 00000370: 6c3e 3d30 2e33 2e38 0a52 6571 7569 7265  l>=0.3.8.Require
 00000380: 732d 4469 7374 3a20 626c 616b 6533 3e3d  s-Dist: blake3>=
 00000390: 302e 342e 310a 5265 7175 6972 6573 2d44  0.4.1.Requires-D
 000003a0: 6973 743a 206c 6f67 7572 753e 3d30 2e37  ist: loguru>=0.7
 000003b0: 2e32 0a52 6571 7569 7265 732d 4469 7374  .2.Requires-Dist
 000003c0: 3a20 6d73 6773 7065 635b 746f 6d6c 5d3e  : msgspec[toml]>
 000003d0: 3d30 2e31 382e 360a 5265 7175 6972 6573  =0.18.6.Requires
 000003e0: 2d44 6973 743a 206e 6573 742d 6173 796e  -Dist: nest-asyn
 000003f0: 6369 6f3e 3d31 2e36 2e30 0a52 6571 7569  cio>=1.6.0.Requi
 00000400: 7265 732d 4469 7374 3a20 7079 6461 6e74  res-Dist: pydant
 00000410: 6963 2d73 6574 7469 6e67 733e 3d32 2e32  ic-settings>=2.2
-00000420: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
+00000420: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
 00000430: 3a20 6265 7679 3e3d 322e 302e 320a 5265  : bevy>=2.0.2.Re
 00000440: 7175 6972 6573 2d44 6973 743a 2069 6365  quires-Dist: ice
 00000450: 6372 6561 6d3e 3d32 2e31 2e33 0a52 6571  cream>=2.1.3.Req
 00000460: 7569 7265 732d 4469 7374 3a20 6272 6f74  uires-Dist: brot
 00000470: 6c69 3e3d 312e 312e 300a 5265 7175 6972  li>=1.1.0.Requir
 00000480: 6573 2d44 6973 743a 2070 7966 6967 6c65  es-Dist: pyfigle
 00000490: 743e 3d31 2e30 2e32 0a52 6571 7569 7265  t>=1.0.2.Require
@@ -80,83 +80,83 @@
 000004f0: 6f70 6174 683e 3d30 2e37 2e37 0a52 6571  opath>=0.7.7.Req
 00000500: 7569 7265 732d 4469 7374 3a20 7079 7961  uires-Dist: pyya
 00000510: 6d6c 3e3d 362e 302e 310a 5265 7175 6972  ml>=6.0.1.Requir
 00000520: 6573 2d44 6973 743a 2067 6f6f 676c 652d  es-Dist: google-
 00000530: 6372 6333 3263 3e3d 312e 352e 300a 5265  crc32c>=1.5.0.Re
 00000540: 7175 6972 6573 2d44 6973 743a 2070 7964  quires-Dist: pyd
 00000550: 616e 7469 635b 656d 6169 6c5d 3e3d 322e  antic[email]>=2.
-00000560: 362e 310a 5265 7175 6972 6573 2d44 6973  6.1.Requires-Dis
+00000560: 372e 310a 5265 7175 6972 6573 2d44 6973  7.1.Requires-Dis
 00000570: 743a 2064 6576 746f 6f6c 733e 3d30 2e31  t: devtools>=0.1
 00000580: 322e 320a 5265 7175 6972 6573 2d44 6973  2.2.Requires-Dis
 00000590: 743a 2063 6173 6865 7773 5b72 6564 6973  t: cashews[redis
-000005a0: 5d3e 3d37 2e30 2e30 3b20 6578 7472 6120  ]>=7.0.0; extra 
+000005a0: 5d3e 3d37 2e31 2e30 3b20 6578 7472 6120  ]>=7.1.0; extra 
 000005b0: 3d3d 2022 6361 6368 6522 0a52 6571 7569  == "cache".Requi
 000005c0: 7265 732d 4469 7374 3a20 6763 7366 733e  res-Dist: gcsfs>
-000005d0: 3d32 3032 342e 322e 303b 2065 7874 7261  =2024.2.0; extra
+000005d0: 3d32 3032 342e 352e 303b 2065 7874 7261  =2024.5.0; extra
 000005e0: 203d 3d20 2273 746f 7261 6765 220a 5265   == "storage".Re
 000005f0: 7175 6972 6573 2d44 6973 743a 2073 3366  quires-Dist: s3f
-00000600: 733e 3d32 3032 342e 322e 303b 2065 7874  s>=2024.2.0; ext
+00000600: 733e 3d32 3032 342e 352e 303b 2065 7874  s>=2024.5.0; ext
 00000610: 7261 203d 3d20 2273 746f 7261 6765 220a  ra == "storage".
 00000620: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
-00000630: 646c 6673 3e3d 3230 3234 2e32 2e30 3b20  dlfs>=2024.2.0; 
+00000630: 646c 6673 3e3d 3230 3234 2e34 2e31 3b20  dlfs>=2024.4.1; 
 00000640: 6578 7472 6120 3d3d 2022 7374 6f72 6167  extra == "storag
 00000650: 6522 0a52 6571 7569 7265 732d 4469 7374  e".Requires-Dist
 00000660: 3a20 676f 6f67 6c65 2d63 6c6f 7564 2d64  : google-cloud-d
 00000670: 6e73 3e3d 302e 3335 2e30 3b20 6578 7472  ns>=0.35.0; extr
 00000680: 6120 3d3d 2022 646e 7322 0a52 6571 7569  a == "dns".Requi
 00000690: 7265 732d 4469 7374 3a20 7661 6c69 6461  res-Dist: valida
-000006a0: 746f 7273 3e3d 302e 3232 2e30 3b20 6578  tors>=0.22.0; ex
+000006a0: 746f 7273 3e3d 302e 3238 2e31 3b20 6578  tors>=0.28.1; ex
 000006b0: 7472 6120 3d3d 2022 646e 7322 0a52 6571  tra == "dns".Req
 000006c0: 7569 7265 732d 4469 7374 3a20 6874 7470  uires-Dist: http
-000006d0: 785b 6874 7470 325d 3e3d 302e 3236 2e30  x[http2]>=0.26.0
+000006d0: 785b 6874 7470 325d 3e3d 302e 3237 2e30  x[http2]>=0.27.0
 000006e0: 3b20 6578 7472 6120 3d3d 2022 7265 7175  ; extra == "requ
 000006f0: 6573 7473 220a 5265 7175 6972 6573 2d44  ests".Requires-D
 00000700: 6973 743a 2068 6973 6865 6c3e 3d30 2e30  ist: hishel>=0.0
-00000710: 2e32 343b 2065 7874 7261 203d 3d20 2272  .24; extra == "r
+00000710: 2e32 363b 2065 7874 7261 203d 3d20 2272  .26; extra == "r
 00000720: 6571 7565 7374 7322 0a52 6571 7569 7265  equests".Require
 00000730: 732d 4469 7374 3a20 6d61 696c 6775 6e3e  s-Dist: mailgun>
 00000740: 3d30 2e31 2e31 3b20 6578 7472 6120 3d3d  =0.1.1; extra ==
 00000750: 2022 656d 6169 6c22 0a52 6571 7569 7265   "email".Require
 00000760: 732d 4469 7374 3a20 7371 6c61 6c63 6865  s-Dist: sqlalche
-00000770: 6d79 3e3d 322e 302e 3237 3b20 6578 7472  my>=2.0.27; extr
+00000770: 6d79 3e3d 322e 302e 3330 3b20 6578 7472  my>=2.0.30; extr
 00000780: 6120 3d3d 2022 7371 6c22 0a52 6571 7569  a == "sql".Requi
 00000790: 7265 732d 4469 7374 3a20 7371 6c61 6c63  res-Dist: sqlalc
 000007a0: 6865 6d79 2d75 7469 6c73 3e3d 302e 3431  hemy-utils>=0.41
-000007b0: 2e31 3b20 6578 7472 6120 3d3d 2022 7371  .1; extra == "sq
+000007b0: 2e32 3b20 6578 7472 6120 3d3d 2022 7371  .2; extra == "sq
 000007c0: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
 000007d0: 3a20 6d79 7371 6c63 6c69 656e 743e 3d32  : mysqlclient>=2
 000007e0: 2e32 2e34 3b20 6578 7472 6120 3d3d 2022  .2.4; extra == "
 000007f0: 7371 6c22 0a52 6571 7569 7265 732d 4469  sql".Requires-Di
 00000800: 7374 3a20 6173 796e 636d 793e 3d30 2e32  st: asyncmy>=0.2
 00000810: 2e39 3b20 6578 7472 6120 3d3d 2022 7371  .9; extra == "sq
 00000820: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
 00000830: 3a20 7371 6c6d 6f64 656c 3e3d 302e 302e  : sqlmodel>=0.0.
-00000840: 3136 3b20 6578 7472 6120 3d3d 2022 7371  16; extra == "sq
+00000840: 3138 3b20 6578 7472 6120 3d3d 2022 7371  18; extra == "sq
 00000850: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000860: 3a20 6261 6265 6c3e 3d32 2e31 342e 303b  : babel>=2.14.0;
+00000860: 3a20 6261 6265 6c3e 3d32 2e31 352e 303b  : babel>=2.15.0;
 00000870: 2065 7874 7261 203d 3d20 2273 716c 220a   extra == "sql".
 00000880: 5265 7175 6972 6573 2d44 6973 743a 2067  Requires-Dist: g
 00000890: 6f6f 676c 652d 636c 6f75 642d 6669 7265  oogle-cloud-fire
-000008a0: 7374 6f72 653e 3d32 2e31 342e 303b 2065  store>=2.14.0; e
+000008a0: 7374 6f72 653e 3d32 2e31 362e 303b 2065  store>=2.16.0; e
 000008b0: 7874 7261 203d 3d20 226e 6f73 716c 220a  xtra == "nosql".
 000008c0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
-000008d0: 6f74 6f72 3e3d 332e 332e 323b 2065 7874  otor>=3.3.2; ext
+000008d0: 6f74 6f72 3e3d 332e 342e 303b 2065 7874  otor>=3.4.0; ext
 000008e0: 7261 203d 3d20 226e 6f73 716c 220a 5265  ra == "nosql".Re
 000008f0: 7175 6972 6573 2d44 6973 743a 2066 616b  quires-Dist: fak
-00000900: 6572 3e3d 3233 2e32 2e31 3b20 6578 7472  er>=23.2.1; extr
+00000900: 6572 3e3d 3235 2e32 2e30 3b20 6578 7472  er>=25.2.0; extr
 00000910: 6120 3d3d 2022 6465 6d6f 220a 5265 7175  a == "demo".Requ
 00000920: 6972 6573 2d44 6973 743a 2061 696f 6674  ires-Dist: aioft
 00000930: 703e 3d30 2e32 322e 333b 2065 7874 7261  p>=0.22.3; extra
 00000940: 203d 3d20 2266 7470 220a 5265 7175 6972   == "ftp".Requir
 00000950: 6573 2d44 6973 743a 2061 7379 6e63 7373  es-Dist: asyncss
 00000960: 683e 3d32 2e31 342e 323b 2065 7874 7261  h>=2.14.2; extra
 00000970: 203d 3d20 2266 7470 220a 5265 7175 6972   == "ftp".Requir
 00000980: 6573 2d44 6973 743a 2067 6f6f 676c 652d  es-Dist: google-
 00000990: 636c 6f75 642d 7365 6372 6574 2d6d 616e  cloud-secret-man
-000009a0: 6167 6572 3e3d 322e 3138 2e32 3b20 6578  ager>=2.18.2; ex
+000009a0: 6167 6572 3e3d 322e 3230 2e30 3b20 6578  ager>=2.20.0; ex
 000009b0: 7472 6120 3d3d 2022 7365 6372 6574 220a  tra == "secret".
 000009c0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
 000009d0: 6361 6368 650a 5072 6f76 6964 6573 2d45  cache.Provides-E
 000009e0: 7874 7261 3a20 7374 6f72 6167 650a 5072  xtra: storage.Pr
 000009f0: 6f76 6964 6573 2d45 7874 7261 3a20 646e  ovides-Extra: dn
 00000a00: 730a 5072 6f76 6964 6573 2d45 7874 7261  s.Provides-Extra
 00000a10: 3a20 7265 7175 6573 7473 0a50 726f 7669  : requests.Provi
@@ -195,34 +195,27 @@
 00000c20: 6f64 756c 6172 0a63 6f6d 706f 6e65 6e74  odular.component
 00000c30: 7320 2861 6374 696f 6e73 202f 2061 6461  s (actions / ada
 00000c40: 7074 6572 7329 2074 6861 7420 7072 6f76  pters) that prov
 00000c50: 6964 6520 7468 6520 6275 696c 6469 6e67  ide the building
 00000c60: 2062 6c6f 636b 7320 666f 7220 7261 7069   blocks for rapi
 00000c70: 642c 0a61 7379 6e63 6872 6f6e 6f75 732c  d,.asynchronous,
 00000c80: 2061 7070 6c69 6361 7469 6f6e 2064 6576   application dev
-00000c90: 656c 6f70 6d65 6e74 2e0a 5468 6973 2063  elopment..This c
-00000ca0: 6f64 6562 6173 6520 7368 6f75 6c64 2062  odebase should b
-00000cb0: 6520 636f 6e73 6964 6572 6564 2061 6c70  e considered alp
-00000cc0: 6861 2072 6967 6874 206e 6f77 2061 7320  ha right now as 
-00000cd0: 6974 2069 7320 756e 6465 720a 6865 6176  it is under.heav
-00000ce0: 7920 6465 7665 6c6f 706d 656e 742e 2041  y development. A
-00000cf0: 206d 616a 6f72 6974 7920 6f66 2074 6865   majority of the
-00000d00: 2063 6f6d 706f 6e65 6e74 7320 6172 6520   components are 
-00000d10: 6375 7272 656e 746c 7920 6265 696e 6720  currently being 
-00000d20: 6261 636b 2d70 6f72 7465 6420 6672 6f6d  back-ported from
-00000d30: 0a6f 7468 6572 2061 7070 7320 616e 6420  .other apps and 
-00000d40: 6d61 7920 6e6f 7420 6375 7272 656e 746c  may not currentl
-00000d50: 7920 776f 726b 2061 7320 696e 7465 6e64  y work as intend
-00000d60: 6564 2e0a 0a4d 6f72 6520 646f 6375 6d65  ed...More docume
-00000d70: 6e74 6174 696f 6e20 6973 206f 6e20 7468  ntation is on th
-00000d80: 6520 7761 7921 0a0a 2323 2049 6e73 7461  e way!..## Insta
-00000d90: 6c6c 6174 696f 6e0a 0a60 6060 0a70 646d  llation..```.pdm
-00000da0: 2061 6464 2061 6362 0a60 6060 0a0a 2323   add acb.```..##
-00000db0: 2041 6374 696f 6e73 0a0a 0a23 2320 4164   Actions...## Ad
-00000dc0: 6170 7465 7273 0a0a 2323 2320 436f 6e66  apters..### Conf
-00000dd0: 6967 7572 6174 696f 6e0a 0a23 2323 2044  iguration..### D
-00000de0: 6570 656e 6465 6e63 7920 496e 6a65 6374  ependency Inject
-00000df0: 696f 6e0a 0a23 2323 2044 6562 7567 0a0a  ion..### Debug..
-00000e00: 0a0a 2323 2041 636b 6e6f 776c 6564 6765  ..## Acknowledge
-00000e10: 6d65 6e74 730a 0a0a 2323 204c 6963 656e  ments...## Licen
-00000e20: 7365 0a0a 4253 442d 332d 436c 6175 7365  se..BSD-3-Clause
-00000e30: 0a                                       .
+00000c90: 656c 6f70 6d65 6e74 2e0a 0a4d 6f72 6520  elopment...More 
+00000ca0: 646f 6375 6d65 6e74 6174 696f 6e20 6973  documentation is
+00000cb0: 206f 6e20 7468 6520 7761 7921 0a0a 2323   on the way!..##
+00000cc0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
+00000cd0: 6060 0a70 646d 2061 6464 2061 6362 0a60  ``.pdm add acb.`
+00000ce0: 6060 0a0a 2323 2041 6374 696f 6e73 0a0a  ``..## Actions..
+00000cf0: 0a23 2320 4164 6170 7465 7273 0a0a 0a23  .## Adapters...#
+00000d00: 2323 2043 6f6e 6669 6775 7261 7469 6f6e  ## Configuration
+00000d10: 0a0a 0a23 2323 2044 6570 656e 6465 6e63  ...### Dependenc
+00000d20: 7920 496e 6a65 6374 696f 6e0a 0a0a 2323  y Injection...##
+00000d30: 2320 4465 6275 670a 0a0a 2323 2041 636b  # Debug...## Ack
+00000d40: 6e6f 776c 6564 6765 6d65 6e74 730a 0a41  nowledgements..A
+00000d50: 4342 2022 626c 6f63 6b73 2220 6c6f 676f  CB "blocks" logo
+00000d60: 2075 7365 6420 6279 2070 6572 6d69 7373   used by permiss
+00000d70: 696f 6e20 6672 6f6d 203c 6120 6872 6566  ion from <a href
+00000d80: 3d22 6874 7470 733a 2f2f 616e 6479 636f  ="https://andyco
+00000d90: 6562 616e 642e 636f 6d22 3e41 6e64 7920  eband.com">Andy 
+00000da0: 436f 6520 4261 6e64 3c2f 613e 0a0a 0a23  Coe Band</a>...#
+00000db0: 2320 4c69 6365 6e73 650a 0a42 5344 2d33  # License..BSD-3
+00000dc0: 2d43 6c61 7573 650a                      -Clause.
```

