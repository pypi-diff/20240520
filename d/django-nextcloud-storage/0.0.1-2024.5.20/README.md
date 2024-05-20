# Comparing `tmp/django-nextcloud-storage-0.0.1.tar.gz` & `tmp/django_nextcloud_storage-2024.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nextcloud-storage-0.0.1.tar", last modified: Thu May 13 20:33:59 2021, max compression
+gzip compressed data, was "django_nextcloud_storage-2024.5.20.tar", last modified: Mon May 20 19:15:11 2024, max compression
```

## Comparing `django-nextcloud-storage-0.0.1.tar` & `django_nextcloud_storage-2024.5.20.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 abtin     (1000) users      (100)        0 2021-05-13 20:33:59.924766 django-nextcloud-storage-0.0.1/
--rw-r--r--   0 abtin     (1000) users      (100)      722 2021-05-13 20:33:59.924766 django-nextcloud-storage-0.0.1/PKG-INFO
-drwxr-xr-x   0 abtin     (1000) users      (100)        0 2021-05-13 20:33:59.924766 django-nextcloud-storage-0.0.1/django_nextcloud_storage/
--rw-r--r--   0 abtin     (1000) users      (100)        0 2021-05-13 20:32:52.000000 django-nextcloud-storage-0.0.1/django_nextcloud_storage/__init__.py
-drwxr-xr-x   0 abtin     (1000) users      (100)        0 2021-05-13 20:33:59.924766 django-nextcloud-storage-0.0.1/django_nextcloud_storage.egg-info/
--rw-r--r--   0 abtin     (1000) users      (100)      722 2021-05-13 20:33:59.000000 django-nextcloud-storage-0.0.1/django_nextcloud_storage.egg-info/PKG-INFO
--rw-r--r--   0 abtin     (1000) users      (100)      237 2021-05-13 20:33:59.000000 django-nextcloud-storage-0.0.1/django_nextcloud_storage.egg-info/SOURCES.txt
--rw-r--r--   0 abtin     (1000) users      (100)        1 2021-05-13 20:33:59.000000 django-nextcloud-storage-0.0.1/django_nextcloud_storage.egg-info/dependency_links.txt
--rw-r--r--   0 abtin     (1000) users      (100)       25 2021-05-13 20:33:59.000000 django-nextcloud-storage-0.0.1/django_nextcloud_storage.egg-info/top_level.txt
--rw-r--r--   0 abtin     (1000) users      (100)       38 2021-05-13 20:33:59.924766 django-nextcloud-storage-0.0.1/setup.cfg
--rw-r--r--   0 abtin     (1000) users      (100)      738 2021-05-13 20:33:06.000000 django-nextcloud-storage-0.0.1/setup.py
+drwxr-xr-x   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:15:11.106928 django_nextcloud_storage-2024.5.20/
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)     1009 2024-05-20 19:15:11.106731 django_nextcloud_storage-2024.5.20/PKG-INFO
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:11:12.000000 django_nextcloud_storage-2024.5.20/README.md
+drwxr-xr-x   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:15:11.105544 django_nextcloud_storage-2024.5.20/backend/
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)     5766 2024-05-20 18:39:42.000000 django_nextcloud_storage-2024.5.20/backend/storage.py
+drwxr-xr-x   0 abtinmiheban   (501) staff       (20)        0 2024-05-20 19:15:11.106551 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)     1009 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/PKG-INFO
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)      282 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)        1 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)       43 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/requires.txt
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)        8 2024-05-20 19:15:11.000000 django_nextcloud_storage-2024.5.20/django_nextcloud_storage.egg-info/top_level.txt
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)     1360 2024-05-20 19:15:08.000000 django_nextcloud_storage-2024.5.20/pyproject.toml
+-rw-r--r--   0 abtinmiheban   (501) staff       (20)       38 2024-05-20 19:15:11.106966 django_nextcloud_storage-2024.5.20/setup.cfg
```

