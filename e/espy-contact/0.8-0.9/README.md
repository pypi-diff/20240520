# Comparing `tmp/espy_contact-0.8.tar.gz` & `tmp/espy_contact-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_contact-0.8.tar", last modified: Mon May  6 01:51:55 2024, max compression
+gzip compressed data, was "espy_contact-0.9.tar", last modified: Mon May  6 02:35:40 2024, max compression
```

## Comparing `espy_contact-0.8.tar` & `espy_contact-0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.346603 espy_contact-0.8/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.8/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-06 01:51:55.346424 espy_contact-0.8/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-0.8/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.338578 espy_contact-0.8/espy_contact/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.8/espy_contact/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.341015 espy_contact-0.8/espy_contact/model/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.8/espy_contact/model/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     9835 2024-04-28 04:32:29.000000 espy_contact-0.8/espy_contact/model/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-0.8/espy_contact/model/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2616 2024-05-04 04:42:58.000000 espy_contact-0.8/espy_contact/model/models.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2681 2024-05-06 01:51:03.000000 espy_contact-0.8/espy_contact/model/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-0.8/espy_contact/model/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.343463 espy_contact-0.8/espy_contact/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.8/espy_contact/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2200 2024-04-28 03:20:57.000000 espy_contact-0.8/espy_contact/schema/campus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-0.8/espy_contact/schema/messaging.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-0.8/espy_contact/schema/mgcampus.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      984 2024-05-05 22:52:13.000000 espy_contact-0.8/espy_contact/schema/reach.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3204 2024-04-28 03:14:05.000000 espy_contact-0.8/espy_contact/schema/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-0.8/espy_contact/schema/tranx.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.344026 espy_contact-0.8/espy_contact/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-0.8/espy_contact/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.8/espy_contact/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.345267 espy_contact-0.8/espy_contact/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.8/espy_contact/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.8/espy_contact/util/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      184 2024-04-28 03:04:46.000000 espy_contact-0.8/espy_contact/util/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3797 2024-05-04 04:43:43.000000 espy_contact-0.8/espy_contact/util/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4356 2024-05-04 17:13:08.000000 espy_contact-0.8/espy_contact/util/pg.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.339177 espy_contact-0.8/espy_contact.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-06 01:51:55.000000 espy_contact-0.8/espy_contact.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      887 2024-05-06 01:51:55.000000 espy_contact-0.8/espy_contact.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-06 01:51:55.000000 espy_contact-0.8/espy_contact.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       76 2024-05-06 01:51:55.000000 espy_contact-0.8/espy_contact.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-06 01:51:55.000000 espy_contact-0.8/espy_contact.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-06 01:51:55.346666 espy_contact-0.8/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      655 2024-05-06 01:51:46.000000 espy_contact-0.8/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 01:51:55.346220 espy_contact-0.8/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.8/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.8/tests/test_copyright.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.8/tests/test_service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.628529 espy_contact-0.9/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-04-26 01:29:16.000000 espy_contact-0.9/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-06 02:35:40.628401 espy_contact-0.9/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      109 2024-05-05 21:34:51.000000 espy_contact-0.9/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.621308 espy_contact-0.9/espy_contact/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.9/espy_contact/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.623600 espy_contact-0.9/espy_contact/model/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:34:03.000000 espy_contact-0.9/espy_contact/model/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     9835 2024-04-28 04:32:29.000000 espy_contact-0.9/espy_contact/model/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      558 2024-04-28 03:38:46.000000 espy_contact-0.9/espy_contact/model/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2616 2024-05-04 04:42:58.000000 espy_contact-0.9/espy_contact/model/models.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2870 2024-05-06 02:29:42.000000 espy_contact-0.9/espy_contact/model/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1821 2024-04-28 03:38:03.000000 espy_contact-0.9/espy_contact/model/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.625909 espy_contact-0.9/espy_contact/schema/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-27 05:18:23.000000 espy_contact-0.9/espy_contact/schema/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2200 2024-04-28 03:20:57.000000 espy_contact-0.9/espy_contact/schema/campus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      295 2024-04-28 00:12:40.000000 espy_contact-0.9/espy_contact/schema/messaging.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     5759 2024-04-28 03:39:29.000000 espy_contact-0.9/espy_contact/schema/mgcampus.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      984 2024-05-05 22:52:13.000000 espy_contact-0.9/espy_contact/schema/reach.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3204 2024-04-28 03:14:05.000000 espy_contact-0.9/espy_contact/schema/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      932 2024-04-28 03:35:00.000000 espy_contact-0.9/espy_contact/schema/tranx.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.626334 espy_contact-0.9/espy_contact/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-28 00:08:44.000000 espy_contact-0.9/espy_contact/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1574 2024-04-27 02:59:30.000000 espy_contact-0.9/espy_contact/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.627440 espy_contact-0.9/espy_contact/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-04-26 03:59:10.000000 espy_contact-0.9/espy_contact/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 16:33:54.000000 espy_contact-0.9/espy_contact/util/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      184 2024-04-28 03:04:46.000000 espy_contact-0.9/espy_contact/util/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3797 2024-05-04 04:43:43.000000 espy_contact-0.9/espy_contact/util/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4356 2024-05-04 17:13:08.000000 espy_contact-0.9/espy_contact/util/pg.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.621894 espy_contact-0.9/espy_contact.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      348 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      887 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       76 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       19 2024-05-06 02:35:40.000000 espy_contact-0.9/espy_contact.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-06 02:35:40.628576 espy_contact-0.9/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      655 2024-05-06 02:35:35.000000 espy_contact-0.9/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 02:35:40.628239 espy_contact-0.9/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.9/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1621 2024-04-26 01:31:37.000000 espy_contact-0.9/tests/test_copyright.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-04-26 01:31:37.000000 espy_contact-0.9/tests/test_service.py
```

### Comparing `espy_contact-0.8/LICENSE` & `espy_contact-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/model/campus.py` & `espy_contact-0.9/espy_contact/model/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/model/messaging.py` & `espy_contact-0.9/espy_contact/model/messaging.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/model/models.py` & `espy_contact-0.9/espy_contact/model/models.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/model/reach.py` & `espy_contact-0.9/espy_contact/model/reach.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,15 +43,20 @@
     business_email = Column(String) 
     contact_name = Column(String)
     contact_phone = Column(String)
     contact_email = Column(String)
     address_id = Column(String, ForeignKey("addresses.id"))
     address = relationship("Address")
 
-    staff = relationship("Appuser", secondary=customer_appuser_association, backref="customers")
+    staff = relationship(
+        "Appuser", 
+        secondary=customer_appuser_association,primaryjoin="Customer.id == customer_appuser_association.c.customer_id",
+        secondaryjoin="Appuser.id == customer_appuser_association.c.appuser_id", 
+        backref="customers"
+        )
     products = relationship("Product", back_populates="customer")
 
 # customer_staff = Table(
 #     "customer_staff",
 #     Base.metadata,
 #     Column("customer_id", ForeignKey("customer.id"), primary_key=True),
 #     Column("appuser_id", ForeignKey("appuser.id"), primary_key=True)
```

### Comparing `espy_contact-0.8/espy_contact/model/tranx.py` & `espy_contact-0.9/espy_contact/model/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/schema/campus.py` & `espy_contact-0.9/espy_contact/schema/campus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/schema/mgcampus.py` & `espy_contact-0.9/espy_contact/schema/mgcampus.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/schema/reach.py` & `espy_contact-0.9/espy_contact/schema/reach.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/schema/schema.py` & `espy_contact-0.9/espy_contact/schema/schema.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/schema/tranx.py` & `espy_contact-0.9/espy_contact/schema/tranx.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/service/service.py` & `espy_contact-0.9/espy_contact/service/service.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/util/CONSTANTS.py` & `espy_contact-0.9/espy_contact/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/util/enums.py` & `espy_contact-0.9/espy_contact/util/enums.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact/util/pg.py` & `espy_contact-0.9/espy_contact/util/pg.py`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/espy_contact.egg-info/SOURCES.txt` & `espy_contact-0.9/espy_contact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espy_contact-0.8/setup.py` & `espy_contact-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 VERSION = '0.0.2'
 DESCRIPTION = 'ESSL users management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL users management'
 setup(
     name='espy_contact',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
         'pydantic==2.7.1',
         'sqlalchemy==2.0.29',
         'bson==0.5.10'
```

### Comparing `espy_contact-0.8/tests/test_copyright.py` & `espy_contact-0.9/tests/test_copyright.py`

 * *Files identical despite different names*

