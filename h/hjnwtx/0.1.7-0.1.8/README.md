# Comparing `tmp/hjnwtx-0.1.7.tar.gz` & `tmp/hjnwtx-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hjnwtx-0.1.7.tar", last modified: Wed May 15 03:23:26 2024, max compression
+gzip compressed data, was "hjnwtx-0.1.8.tar", last modified: Mon May 20 05:53:34 2024, max compression
```

## Comparing `hjnwtx-0.1.7.tar` & `hjnwtx-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/
--rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/PKG-INFO
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       16 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/README.md
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-05-15 03:23:26.924907 hjnwtx-0.1.7/hjnwtx/
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    17426 2024-01-23 02:42:51.000000 hjnwtx-0.1.7/hjnwtx/H8mess.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      171 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/__init__.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    23455 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/cinradHJN.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1163 2024-01-06 12:54:45.000000 hjnwtx-0.1.7/hjnwtx/colormap.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    11590 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/examMeso.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      800 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnDAAS.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2927 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnFTP.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    12118 2024-03-05 02:10:16.000000 hjnwtx-0.1.7/hjnwtx/hjnGIS.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      516 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnGPU.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2362 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnIDW.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2395 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnKDTree.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1975 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/hjnLAPSTransform.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     2193 2024-04-20 09:02:38.000000 hjnwtx-0.1.7/hjnwtx/hjnLog.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     6580 2024-01-23 02:47:03.000000 hjnwtx-0.1.7/hjnwtx/hjnMiscellaneous.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     5753 2024-01-23 02:42:52.000000 hjnwtx-0.1.7/hjnwtx/hjnProj.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     1290 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/inotify.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     3343 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/matplotlibMess.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    24653 2024-01-24 03:29:07.000000 hjnwtx-0.1.7/hjnwtx/mkNCHJN.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)    23449 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/newTypeRadar.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       80 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/test.py
--rw-rw-r--   0 hjn       (1003) hjn       (1003)     5119 2024-01-03 00:18:24.000000 hjnwtx-0.1.7/hjnwtx/tlogP.py
-drwxrwxr-x   0 hjn       (1003) hjn       (1003)        0 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/hjnwtx.egg-info/
--rw-r--r--   0 hjn       (1003) hjn       (1003)      140 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/PKG-INFO
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      581 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/SOURCES.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/dependency_links.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        1 2024-01-03 00:19:56.000000 hjnwtx-0.1.7/hjnwtx.egg-info/not-zip-safe
--rw-rw-r--   0 hjn       (1003) hjn       (1003)        7 2024-05-15 03:23:26.000000 hjnwtx-0.1.7/hjnwtx.egg-info/top_level.txt
--rw-rw-r--   0 hjn       (1003) hjn       (1003)       38 2024-05-15 03:23:26.936907 hjnwtx-0.1.7/setup.cfg
--rw-rw-r--   0 hjn       (1003) hjn       (1003)      250 2024-05-15 03:21:46.000000 hjnwtx-0.1.7/setup.py
+drwxrwxr-x   0 hjn       (1014) hjn       (1014)        0 2024-05-20 05:53:34.627397 hjnwtx-0.1.8/
+-rw-r--r--   0 hjn       (1014) hjn       (1014)      140 2024-05-20 05:53:34.627397 hjnwtx-0.1.8/PKG-INFO
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)       16 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/README.md
+drwxrwxr-x   0 hjn       (1014) hjn       (1014)        0 2024-05-20 05:53:34.623397 hjnwtx-0.1.8/hjnwtx/
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)    17426 2024-01-23 02:42:51.000000 hjnwtx-0.1.8/hjnwtx/H8mess.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)      171 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/__init__.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)    23455 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/cinradHJN.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     1163 2024-01-06 12:54:45.000000 hjnwtx-0.1.8/hjnwtx/colormap.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)    11802 2024-05-20 04:57:39.000000 hjnwtx-0.1.8/hjnwtx/examMeso.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)      800 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/hjnDAAS.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     2927 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/hjnFTP.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)    12118 2024-03-05 02:10:16.000000 hjnwtx-0.1.8/hjnwtx/hjnGIS.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)      516 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/hjnGPU.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     2362 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/hjnIDW.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     2395 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/hjnKDTree.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     1975 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/hjnLAPSTransform.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     2193 2024-04-20 09:02:38.000000 hjnwtx-0.1.8/hjnwtx/hjnLog.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     6580 2024-01-23 02:47:03.000000 hjnwtx-0.1.8/hjnwtx/hjnMiscellaneous.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     5753 2024-01-23 02:42:52.000000 hjnwtx-0.1.8/hjnwtx/hjnProj.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     1290 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/inotify.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     3343 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/matplotlibMess.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)    24653 2024-01-24 03:29:07.000000 hjnwtx-0.1.8/hjnwtx/mkNCHJN.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)    23449 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/newTypeRadar.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)       80 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/test.py
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)     5119 2024-01-03 00:18:24.000000 hjnwtx-0.1.8/hjnwtx/tlogP.py
+drwxrwxr-x   0 hjn       (1014) hjn       (1014)        0 2024-05-20 05:53:34.627397 hjnwtx-0.1.8/hjnwtx.egg-info/
+-rw-r--r--   0 hjn       (1014) hjn       (1014)      140 2024-05-20 05:53:34.000000 hjnwtx-0.1.8/hjnwtx.egg-info/PKG-INFO
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)      581 2024-05-20 05:53:34.000000 hjnwtx-0.1.8/hjnwtx.egg-info/SOURCES.txt
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)        1 2024-05-20 05:53:34.000000 hjnwtx-0.1.8/hjnwtx.egg-info/dependency_links.txt
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)        1 2024-01-03 00:19:56.000000 hjnwtx-0.1.8/hjnwtx.egg-info/not-zip-safe
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)        7 2024-05-20 05:53:34.000000 hjnwtx-0.1.8/hjnwtx.egg-info/top_level.txt
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)       38 2024-05-20 05:53:34.627397 hjnwtx-0.1.8/setup.cfg
+-rw-rw-r--   0 hjn       (1014) hjn       (1014)      250 2024-05-20 05:53:24.000000 hjnwtx-0.1.8/setup.py
```

### Comparing `hjnwtx-0.1.7/hjnwtx/H8mess.py` & `hjnwtx-0.1.8/hjnwtx/H8mess.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/cinradHJN.py` & `hjnwtx-0.1.8/hjnwtx/cinradHJN.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/colormap.py` & `hjnwtx-0.1.8/hjnwtx/colormap.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/examMeso.py` & `hjnwtx-0.1.8/hjnwtx/examMeso.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
     return pre[latIdx, lonIdx].round(decimals=decimal)
 
 def getPoint(pre, df, lat0, lon0, resolution, decimal=1):
     latIdx = ((lat0 - df["Lat"]) / resolution + 0.5).astype(np.int64)
     lonIdx = ((df["Lon"] - lon0) / resolution + 0.5).astype(np.int64)
     return pre[...,latIdx, lonIdx].round(decimals=decimal)
 
+def getPointIdx(df, lat0, lon0, resolution):
+    latIdx = ((lat0 - df["Lat"]) / resolution + 0.5).astype(np.int64)
+    lonIdx = ((df["Lon"] - lon0) / resolution + 0.5).astype(np.int64)
+    return latIdx, lonIdx
+
 def getPointBilinear3D(preData,df1,latArr,lonArr,decimal=2):
     df=copy.copy(df1)
     resolution=np.abs((latArr[0]-latArr[-1])/(len(latArr)-1))
     latIdxN = ((latArr[0] - df["Lat"]) / resolution).astype(np.int64)
     lonIdxW = ((df["Lon"] - lonArr[0]) / resolution).astype(np.int64)
 
     latIdxS = ((latArr[0] - df["Lat"]) / resolution).astype(np.int64)+1
```

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnDAAS.py` & `hjnwtx-0.1.8/hjnwtx/hjnDAAS.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnFTP.py` & `hjnwtx-0.1.8/hjnwtx/hjnFTP.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnGIS.py` & `hjnwtx-0.1.8/hjnwtx/hjnGIS.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnGPU.py` & `hjnwtx-0.1.8/hjnwtx/hjnGPU.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnIDW.py` & `hjnwtx-0.1.8/hjnwtx/hjnIDW.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnKDTree.py` & `hjnwtx-0.1.8/hjnwtx/hjnKDTree.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnLAPSTransform.py` & `hjnwtx-0.1.8/hjnwtx/hjnLAPSTransform.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnLog.py` & `hjnwtx-0.1.8/hjnwtx/hjnLog.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnMiscellaneous.py` & `hjnwtx-0.1.8/hjnwtx/hjnMiscellaneous.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/hjnProj.py` & `hjnwtx-0.1.8/hjnwtx/hjnProj.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/inotify.py` & `hjnwtx-0.1.8/hjnwtx/inotify.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/matplotlibMess.py` & `hjnwtx-0.1.8/hjnwtx/matplotlibMess.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/mkNCHJN.py` & `hjnwtx-0.1.8/hjnwtx/mkNCHJN.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/newTypeRadar.py` & `hjnwtx-0.1.8/hjnwtx/newTypeRadar.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx/tlogP.py` & `hjnwtx-0.1.8/hjnwtx/tlogP.py`

 * *Files identical despite different names*

### Comparing `hjnwtx-0.1.7/hjnwtx.egg-info/SOURCES.txt` & `hjnwtx-0.1.8/hjnwtx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

