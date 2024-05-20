# Comparing `tmp/comun_va-3.6.tar.gz` & `tmp/comun_va-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-3.6.tar", last modified: Tue May 14 09:16:27 2024, max compression
+gzip compressed data, was "comun_va-3.7.tar", last modified: Mon May 20 14:36:48 2024, max compression
```

## Comparing `comun_va-3.6.tar` & `comun_va-3.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 09:16:27.452512 comun_va-3.6/
--rw-rw-rw-   0        0        0       53 2024-05-14 09:16:27.450909 comun_va-3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 09:16:27.447861 comun_va-3.6/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2024-05-14 09:16:27.000000 comun_va-3.6/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-14 09:16:27.000000 comun_va-3.6/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 09:16:27.000000 comun_va-3.6/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-14 09:16:27.000000 comun_va-3.6/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-14 09:16:27.000000 comun_va-3.6/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8935 2024-05-14 09:10:19.000000 comun_va-3.6/comun_va.py
--rw-rw-rw-   0        0        0       42 2024-05-14 09:16:27.453465 comun_va-3.6/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-05-14 09:16:25.000000 comun_va-3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:36:47.990530 comun_va-3.7/
+-rw-rw-rw-   0        0        0      141 2024-05-20 14:36:47.989944 comun_va-3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 14:36:47.988699 comun_va-3.7/comun_va.egg-info/
+-rw-rw-rw-   0        0        0      141 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-20 14:36:47.000000 comun_va-3.7/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8931 2024-05-20 14:35:45.000000 comun_va-3.7/comun_va.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:36:47.990530 comun_va-3.7/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-05-20 14:35:45.000000 comun_va-3.7/setup.py
```

### Comparing `comun_va-3.6/comun_va.py` & `comun_va-3.7/comun_va.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,16 @@
     Function that connect to an IP camera and return all the barcodes or QRs that can be read (without repeat)
     :param camera_url: need to be the RTSP URL
     :param intents: how much tries to connect to the camera and read the barcode, must to be greater than 0
     :return: list of all barcodes read without repeat
     """
     try:
         barcodes = set()
+        cap = cv2.VideoCapture(camera_url)  # IP Camera
         for _ in range(intents):
-            cap = cv2.VideoCapture(camera_url)  # IP Camera
             success, frame = cap.read()
             if not success:
                 raise Exception
             detected_barcodes = decode(frame)
             if detected_barcodes:
                 for barcode in detected_barcodes:
                     if barcode.data != "":
```

