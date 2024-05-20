# Comparing `tmp/musclex-1.9.2.tar.gz` & `tmp/musclex-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/musclex-1.9.2.tar", last modified: Wed Dec 20 22:24:46 2017, max compression
+gzip compressed data, was "dist/musclex-1.9.3.tar", last modified: Fri Dec 22 20:39:16 2017, max compression
```

## Comparing `musclex-1.9.2.tar` & `musclex-1.9.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex/
--rw-r--r--   0 jiranun    (501) staff       (20)     1366 2017-12-20 22:24:22.000000 musclex-1.9.2/musclex/__init__.py
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex/CalibrationSettings/
--rw-r--r--   0 jiranun    (501) staff       (20)     1396 2017-12-01 21:15:50.000000 musclex-1.9.2/musclex/CalibrationSettings/__init__.py
--rw-r--r--   0 jiranun    (501) staff       (20)    21071 2017-12-07 21:42:18.000000 musclex-1.9.2/musclex/CalibrationSettings/CalibrationSettings.py
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex/csv_manager/
--rw-r--r--   0 jiranun    (501) staff       (20)     1506 2017-12-04 19:02:07.000000 musclex-1.9.2/musclex/csv_manager/__init__.py
--rw-r--r--   0 jiranun    (501) staff       (20)     5251 2017-12-01 17:41:04.000000 musclex-1.9.2/musclex/csv_manager/CP_CSVManager.py
--rw-r--r--   0 jiranun    (501) staff       (20)    23307 2017-12-04 18:22:35.000000 musclex-1.9.2/musclex/csv_manager/DC_CSVManager.py
--rw-r--r--   0 jiranun    (501) staff       (20)     7767 2017-12-08 16:45:38.000000 musclex-1.9.2/musclex/csv_manager/EQ_CVSManager.py
--rw-r--r--   0 jiranun    (501) staff       (20)     6626 2017-12-13 20:14:08.000000 musclex-1.9.2/musclex/csv_manager/PT_CSVManager.py
--rw-r--r--   0 jiranun    (501) staff       (20)     4054 2017-12-04 19:03:26.000000 musclex-1.9.2/musclex/main.py
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex/modules/
--rw-r--r--   0 jiranun    (501) staff       (20)     1343 2017-12-01 15:03:02.000000 musclex-1.9.2/musclex/modules/__init__.py
--rw-r--r--   0 jiranun    (501) staff       (20)    50726 2017-12-13 19:04:34.000000 musclex-1.9.2/musclex/modules/CircularProjection.py
--rw-r--r--   0 jiranun    (501) staff       (20)    30414 2017-12-05 19:28:02.000000 musclex-1.9.2/musclex/modules/DiffractionCentroids.py
--rw-r--r--   0 jiranun    (501) staff       (20)    39690 2017-12-20 22:23:53.000000 musclex-1.9.2/musclex/modules/EquatorImage.py
--rw-r--r--   0 jiranun    (501) staff       (20)    22936 2017-12-13 21:50:47.000000 musclex-1.9.2/musclex/modules/ProjectionProcessor.py
--rw-r--r--   0 jiranun    (501) staff       (20)    25415 2017-12-01 15:03:02.000000 musclex-1.9.2/musclex/modules/QF_utilities.pyx
--rw-r--r--   0 jiranun    (501) staff       (20)    34868 2017-12-07 20:08:03.000000 musclex-1.9.2/musclex/modules/QuadrantFolder.py
--rw-r--r--   0 jiranun    (501) staff       (20)      716 2017-12-01 15:03:02.000000 musclex-1.9.2/musclex/modules/setup2.py
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex/ui/
--rw-r--r--   0 jiranun    (501) staff       (20)     1342 2017-12-01 15:03:02.000000 musclex-1.9.2/musclex/ui/__init__.py
--rw-r--r--   0 jiranun    (501) staff       (20)     8008 2017-12-01 20:58:49.000000 musclex-1.9.2/musclex/ui/BlankImageSettings.py
--rw-r--r--   0 jiranun    (501) staff       (20)     5273 2017-12-07 21:42:48.000000 musclex-1.9.2/musclex/ui/CircularProjectionGUI.py
--rw-r--r--   0 jiranun    (501) staff       (20)    43946 2017-12-04 16:08:16.000000 musclex-1.9.2/musclex/ui/CPBatchWindow.py
--rw-r--r--   0 jiranun    (501) staff       (20)    43519 2017-12-18 16:40:26.000000 musclex-1.9.2/musclex/ui/CPBatchWindow2.py
--rw-r--r--   0 jiranun    (501) staff       (20)    60695 2017-12-04 19:07:19.000000 musclex-1.9.2/musclex/ui/CPImageWindow.py
--rw-r--r--   0 jiranun    (501) staff       (20)     8818 2017-12-04 19:07:19.000000 musclex-1.9.2/musclex/ui/ddf_processor.py
--rw-r--r--   0 jiranun    (501) staff       (20)    93926 2017-12-07 21:52:08.000000 musclex-1.9.2/musclex/ui/diffraction_centroids.py
--rw-r--r--   0 jiranun    (501) staff       (20)    13819 2017-12-08 19:52:18.000000 musclex-1.9.2/musclex/ui/EQ_FittingTab.py
--rw-r--r--   0 jiranun    (501) staff       (20)     5502 2017-12-07 21:46:22.000000 musclex-1.9.2/musclex/ui/EQStartWindow.py
--rw-r--r--   0 jiranun    (501) staff       (20)    85338 2017-12-08 19:57:33.000000 musclex-1.9.2/musclex/ui/EquatorWindow.py
--rw-r--r--   0 jiranun    (501) staff       (20)     8342 2017-12-07 21:52:08.000000 musclex-1.9.2/musclex/ui/ImageMerger.py
--rw-r--r--   0 jiranun    (501) staff       (20)    30649 2017-12-14 22:05:34.000000 musclex-1.9.2/musclex/ui/ProjectionBoxTab.py
--rw-r--r--   0 jiranun    (501) staff       (20)    46116 2017-12-07 21:50:42.000000 musclex-1.9.2/musclex/ui/ProjectionTracesGUI.py
--rw-r--r--   0 jiranun    (501) staff       (20)     2931 2017-12-12 22:00:47.000000 musclex-1.9.2/musclex/ui/pyqt_utils.py
--rw-r--r--   0 jiranun    (501) staff       (20)    80118 2017-12-07 21:50:42.000000 musclex-1.9.2/musclex/ui/QuadrantFoldingGUI.py
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex/utils/
--rw-r--r--   0 jiranun    (501) staff       (20)     1343 2017-12-01 15:03:02.000000 musclex-1.9.2/musclex/utils/__init__.py
--rw-r--r--   0 jiranun    (501) staff       (20)    15708 2017-12-07 21:30:43.000000 musclex-1.9.2/musclex/utils/file_manager.py
--rw-r--r--   0 jiranun    (501) staff       (20)    16364 2017-12-20 18:45:46.000000 musclex-1.9.2/musclex/utils/histogram_processor.py
--rw-rw-rw-   0 jiranun    (501) staff       (20)    15881 2017-12-01 22:02:56.000000 musclex-1.9.2/musclex/utils/image_processor.py
-drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/
--rw-r--r--   0 jiranun    (501) staff       (20)        1 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/dependency_links.txt
--rw-r--r--   0 jiranun    (501) staff       (20)       47 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/entry_points.txt
--rw-r--r--   0 jiranun    (501) staff       (20)       47 2017-12-01 15:03:02.000000 musclex-1.9.2/musclex.egg-info/pbr.json
--rw-r--r--   0 jiranun    (501) staff       (20)      688 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/PKG-INFO
--rw-r--r--   0 jiranun    (501) staff       (20)      142 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/requires.txt
--rw-r--r--   0 jiranun    (501) staff       (20)     1419 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/SOURCES.txt
--rw-r--r--   0 jiranun    (501) staff       (20)        8 2017-12-20 22:24:46.000000 musclex-1.9.2/musclex.egg-info/top_level.txt
--rw-r--r--   0 jiranun    (501) staff       (20)      688 2017-12-20 22:24:46.000000 musclex-1.9.2/PKG-INFO
--rw-r--r--   0 jiranun    (501) staff       (20)      426 2017-12-04 19:02:07.000000 musclex-1.9.2/README.md
--rw-r--r--   0 jiranun    (501) staff       (20)       79 2017-12-20 22:24:46.000000 musclex-1.9.2/setup.cfg
--rw-r--r--   0 jiranun    (501) staff       (20)     3639 2017-12-05 21:48:13.000000 musclex-1.9.2/setup.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex/
+-rw-r--r--   0 jiranun    (501) staff       (20)     1366 2017-12-22 20:07:59.000000 musclex-1.9.3/musclex/__init__.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex/CalibrationSettings/
+-rw-r--r--   0 jiranun    (501) staff       (20)     1396 2017-12-01 21:15:50.000000 musclex-1.9.3/musclex/CalibrationSettings/__init__.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    21058 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/CalibrationSettings/CalibrationSettings.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex/csv_manager/
+-rw-r--r--   0 jiranun    (501) staff       (20)     1506 2017-12-04 19:02:07.000000 musclex-1.9.3/musclex/csv_manager/__init__.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     5251 2017-12-01 17:41:04.000000 musclex-1.9.3/musclex/csv_manager/CP_CSVManager.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    23307 2017-12-04 18:22:35.000000 musclex-1.9.3/musclex/csv_manager/DC_CSVManager.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     7767 2017-12-08 16:45:38.000000 musclex-1.9.3/musclex/csv_manager/EQ_CVSManager.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     6626 2017-12-13 20:14:08.000000 musclex-1.9.3/musclex/csv_manager/PT_CSVManager.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     4054 2017-12-04 19:03:26.000000 musclex-1.9.3/musclex/main.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex/modules/
+-rw-r--r--   0 jiranun    (501) staff       (20)     1343 2017-12-01 15:03:02.000000 musclex-1.9.3/musclex/modules/__init__.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    50726 2017-12-13 19:04:34.000000 musclex-1.9.3/musclex/modules/CircularProjection.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    30414 2017-12-05 19:28:02.000000 musclex-1.9.3/musclex/modules/DiffractionCentroids.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    39690 2017-12-20 22:23:53.000000 musclex-1.9.3/musclex/modules/EquatorImage.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    22936 2017-12-13 21:50:47.000000 musclex-1.9.3/musclex/modules/ProjectionProcessor.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    25415 2017-12-01 15:03:02.000000 musclex-1.9.3/musclex/modules/QF_utilities.pyx
+-rw-r--r--   0 jiranun    (501) staff       (20)    34868 2017-12-07 20:08:03.000000 musclex-1.9.3/musclex/modules/QuadrantFolder.py
+-rw-r--r--   0 jiranun    (501) staff       (20)      716 2017-12-01 15:03:02.000000 musclex-1.9.3/musclex/modules/setup2.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex/ui/
+-rw-r--r--   0 jiranun    (501) staff       (20)     1342 2017-12-01 15:03:02.000000 musclex-1.9.3/musclex/ui/__init__.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     7991 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/BlankImageSettings.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     5275 2017-12-22 19:51:53.000000 musclex-1.9.3/musclex/ui/CircularProjectionGUI.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    43815 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/CPBatchWindow.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    43519 2017-12-18 16:40:26.000000 musclex-1.9.3/musclex/ui/CPBatchWindow2.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    60583 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/CPImageWindow.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     8818 2017-12-04 19:07:19.000000 musclex-1.9.3/musclex/ui/ddf_processor.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    93926 2017-12-07 21:52:08.000000 musclex-1.9.3/musclex/ui/diffraction_centroids.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    13819 2017-12-08 19:52:18.000000 musclex-1.9.3/musclex/ui/EQ_FittingTab.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     5502 2017-12-07 21:46:22.000000 musclex-1.9.3/musclex/ui/EQStartWindow.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    85302 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/EquatorWindow.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     8342 2017-12-07 21:52:08.000000 musclex-1.9.3/musclex/ui/ImageMerger.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    30611 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/ProjectionBoxTab.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    46099 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/ProjectionTracesGUI.py
+-rw-r--r--   0 jiranun    (501) staff       (20)     2931 2017-12-12 22:00:47.000000 musclex-1.9.3/musclex/ui/pyqt_utils.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    80082 2017-12-22 19:58:25.000000 musclex-1.9.3/musclex/ui/QuadrantFoldingGUI.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex/utils/
+-rw-r--r--   0 jiranun    (501) staff       (20)     1343 2017-12-01 15:03:02.000000 musclex-1.9.3/musclex/utils/__init__.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    15738 2017-12-22 19:49:52.000000 musclex-1.9.3/musclex/utils/file_manager.py
+-rw-r--r--   0 jiranun    (501) staff       (20)    16364 2017-12-20 18:45:46.000000 musclex-1.9.3/musclex/utils/histogram_processor.py
+-rw-rw-rw-   0 jiranun    (501) staff       (20)    15881 2017-12-01 22:02:56.000000 musclex-1.9.3/musclex/utils/image_processor.py
+drwxr-xr-x   0 jiranun    (501) staff       (20)        0 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/
+-rw-r--r--   0 jiranun    (501) staff       (20)        1 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/dependency_links.txt
+-rw-r--r--   0 jiranun    (501) staff       (20)       47 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/entry_points.txt
+-rw-r--r--   0 jiranun    (501) staff       (20)       47 2017-12-01 15:03:02.000000 musclex-1.9.3/musclex.egg-info/pbr.json
+-rw-r--r--   0 jiranun    (501) staff       (20)      688 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/PKG-INFO
+-rw-r--r--   0 jiranun    (501) staff       (20)      142 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/requires.txt
+-rw-r--r--   0 jiranun    (501) staff       (20)     1419 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/SOURCES.txt
+-rw-r--r--   0 jiranun    (501) staff       (20)        8 2017-12-22 20:39:16.000000 musclex-1.9.3/musclex.egg-info/top_level.txt
+-rw-r--r--   0 jiranun    (501) staff       (20)      688 2017-12-22 20:39:16.000000 musclex-1.9.3/PKG-INFO
+-rw-r--r--   0 jiranun    (501) staff       (20)      426 2017-12-04 19:02:07.000000 musclex-1.9.3/README.md
+-rw-r--r--   0 jiranun    (501) staff       (20)       79 2017-12-22 20:39:16.000000 musclex-1.9.3/setup.cfg
+-rw-r--r--   0 jiranun    (501) staff       (20)     3639 2017-12-05 21:48:13.000000 musclex-1.9.3/setup.py
```

### Comparing `musclex-1.9.2/musclex/__init__.py` & `musclex-1.9.3/musclex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 Except as contained in this notice, the name of Illinois Institute
 of Technology shall not be used in advertising or otherwise to promote
 the sale, use or other dealings in this Software without prior written
 authorization from Illinois Institute of Technology.
 """
 
-__version__ = '1.9.2'
+__version__ = '1.9.3'
```

### Comparing `musclex-1.9.2/musclex/CalibrationSettings/__init__.py` & `musclex-1.9.3/musclex/CalibrationSettings/__init__.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/CalibrationSettings/CalibrationSettings.py` & `musclex-1.9.3/musclex/CalibrationSettings/CalibrationSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if cache is not None:
             self.calFile = cache["path"]
             self.calSettings = cache["settings"]
         else:
             self.calFile = fullPath(dir_path, "calibration.tif")
             self.calSettings = None
 
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.initUI()
         self.setConnection()
         self.setAllToolTips()
 
         if exists(self.calFile) and self.calImageGrp.isChecked():
             if self.calSettings is None:
                 self.calibrate()
@@ -89,15 +89,15 @@
 
         self.pathText = QLineEdit()
         if exists(self.calFile):
             self.pathText.setText(self.calFile)
         self.pathText.setEnabled(False)
         self.browseButton = QPushButton("Browse")
         self.unsetButton = QPushButton("Unset")
-        self.calImgFigure = plt.figure(facecolor='#606060')
+        self.calImgFigure = plt.figure()
         self.calImgCanvas = FigureCanvas(self.calImgFigure)
         self.calImgCanvas.setHidden(True)
 
         self.minIntLabel = QLabel("Min intensity : ")
         self.minInt = QDoubleSpinBox()
         self.minInt.setKeyboardTracking(False)
         self.minInt.setValue(0)
@@ -126,15 +126,15 @@
         self.bottons = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel, Qt.Horizontal, self)
         self.bottons.accepted.connect(self.okClicked)
         self.bottons.rejected.connect(self.reject)
         self.bottons.setFixedWidth(100)
         grpbox_ss = "QGroupBox::title { background-color: #323232 ; subcontrol-origin: margin; subcontrol-position: top left; padding: 0 3px; }"
         self.calImageGrp = QGroupBox("Setting by Calibration Image")
         self.calImageGrp.setCheckable(True)
-        self.calImageGrp.setStyleSheet(grpbox_ss)
+        # self.calImageGrp.setStyleSheet(grpbox_ss)
         self.calImageGrp.setChecked(type == "img")
         self.calImageLayout = QGridLayout(self.calImageGrp)
         self.calImageLayout.addWidget(QLabel("Calibration File :") , 0, 0, 1, 1)
         self.calImageLayout.addWidget(self.pathText, 0, 1, 1, 1)
         self.calImageLayout.addWidget(self.browseButton, 0, 2, 1, 1)
         self.calImageLayout.addWidget(self.unsetButton, 0, 3, 1, 1)
         self.calImageLayout.addWidget(self.calImgCanvas, 1, 0, 1, 4)
@@ -146,15 +146,15 @@
         self.calImageLayout.addWidget(QLabel("Silver Behenate :"), 3, 2, 1, 1, Qt.AlignRight)
         self.calImageLayout.addWidget(self.silverBehenate, 3, 3, 1, 1)
         # self.calImageLayout.setColumnStretch(1,2)
         self.calImageLayout.setRowStretch(1, 2)
 
         self.paramGrp = QGroupBox("Setting by Parameters")
         self.paramGrp.setCheckable(True)
-        self.paramGrp.setStyleSheet(grpbox_ss)
+        # self.paramGrp.setStyleSheet(grpbox_ss)
         self.paramGrp.setChecked(type == "cont")
         self.paramLayout = QGridLayout(self.paramGrp)
 
         self.lambdaSpnBx = QDoubleSpinBox()
         self.lambdaSpnBx.setDecimals(8)
         self.lambdaSpnBx.setRange(0.00001, 5.)
         self.lambdaSpnBx.setValue(init_lambda)
```

### Comparing `musclex-1.9.2/musclex/csv_manager/__init__.py` & `musclex-1.9.3/musclex/csv_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/csv_manager/CP_CSVManager.py` & `musclex-1.9.3/musclex/csv_manager/CP_CSVManager.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/csv_manager/DC_CSVManager.py` & `musclex-1.9.3/musclex/csv_manager/DC_CSVManager.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/csv_manager/EQ_CVSManager.py` & `musclex-1.9.3/musclex/csv_manager/EQ_CVSManager.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/csv_manager/PT_CSVManager.py` & `musclex-1.9.3/musclex/csv_manager/PT_CSVManager.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/main.py` & `musclex-1.9.3/musclex/main.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/__init__.py` & `musclex-1.9.3/musclex/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/CircularProjection.py` & `musclex-1.9.3/musclex/modules/CircularProjection.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/DiffractionCentroids.py` & `musclex-1.9.3/musclex/modules/DiffractionCentroids.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/EquatorImage.py` & `musclex-1.9.3/musclex/modules/EquatorImage.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/ProjectionProcessor.py` & `musclex-1.9.3/musclex/modules/ProjectionProcessor.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/QF_utilities.pyx` & `musclex-1.9.3/musclex/modules/QF_utilities.pyx`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/QuadrantFolder.py` & `musclex-1.9.3/musclex/modules/QuadrantFolder.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/modules/setup2.py` & `musclex-1.9.3/musclex/modules/setup2.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/__init__.py` & `musclex-1.9.3/musclex/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/BlankImageSettings.py` & `musclex-1.9.3/musclex/ui/BlankImageSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,17 @@
         mask = join(path, 'mask.tif')
         if exists(blank):
             self.selected = fabio.open(blank).data
             if exists(mask):
                 self.mask = fabio.open(mask).data
 
     def initUI(self):
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.mainLayout = QGridLayout(self)
-        self.imageFigure = plt.figure(facecolor='#606060')
+        self.imageFigure = plt.figure()
         self.imageCanvas = FigureCanvas(self.imageFigure)
         self.imageAxes = self.imageFigure.add_subplot(111)
 
         self.selectImage = QPushButton("Select Blank Image(s)")
         self.drawMask = QPushButton("Draw Additional Mask")
         self.drawMask.setEnabled(self.selected is not None)
         self.maskThres = QSpinBox()
```

### Comparing `musclex-1.9.2/musclex/ui/CircularProjectionGUI.py` & `musclex-1.9.3/musclex/ui/CircularProjectionGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def __init__(self):
         QWidget.__init__(self)
         self.widgetList = []
         self.initUI()
 
     def initUI(self):
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.setWindowTitle("Muscle X Circular Projection v." + musclex.__version__)
         self.centralWidget = QWidget(self)
         self.mainLayout = QVBoxLayout(self.centralWidget)
         self.setCentralWidget(self.centralWidget)
 
         ## display browse file and folder buttons when program started
         self.browseFileButton = QPushButton("Select an Image...")
```

### Comparing `musclex-1.9.2/musclex/ui/CPBatchWindow.py` & `musclex-1.9.3/musclex/ui/CPBatchWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,21 +191,21 @@
         self.csvManager = CP_CSVManager(self.filePath)
         self.initUI()
         self.setConnections()
         self.processFolder(self.filePath)
 
     def initUI(self):
         self.setWindowTitle("Circular Projection v." + musclex.__version__)
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.centralWidget = QWidget(self)
         self.mainLayout = QGridLayout(self.centralWidget)
         self.setCentralWidget(self.centralWidget)
 
         #### IMAGE ####
-        self.imgFigure = plt.figure(facecolor='#606060')
+        self.imgFigure = plt.figure()
         self.imgAxes = self.imgFigure.add_subplot(111)
         self.imgCanvas = FigureCanvas(self.imgFigure)
         self.img_maxInt = QDoubleSpinBox()
         self.img_maxInt.setValue(1)
         self.img_maxInt.setKeyboardTracking(False)
         self.img_minInt = QDoubleSpinBox()
         self.img_minInt.setValue(0)
@@ -223,15 +223,15 @@
         self.imgFrame.setHidden(True)
 
         #### BATCHMODE - tabs
         ## BATCHMODE 1 : Total Intensity Map Tab
         self.intensityTab = QWidget()
         self.intensityTab.setContentsMargins(0, 0, 0, 0)
         self.intensityTabLayout = QGridLayout(self.intensityTab)
-        self.intensityMapFigure = plt.figure(facecolor='#606060')
+        self.intensityMapFigure = plt.figure()
         self.intensityMapAxes = self.intensityMapFigure.add_subplot(111)
         self.intensityMapCanvas = FigureCanvas(self.intensityMapFigure)
         self.intensityMapFigure.canvas.mpl_connect('button_press_event', self.plotClicked)
         self.int_maxIntMap = QDoubleSpinBox()
         self.int_maxIntMap.setMinimum(1)
         self.int_maxIntMap.setMaximum(100)
         self.int_maxIntMap.setValue(100.)
@@ -255,19 +255,19 @@
         self.intensityTabLayout.addWidget(self.intensityMapCanvas, 0, 0, 1, 1)
         self.intensityTabLayout.addLayout(self.int_MapIntSettings, 1, 0, 1, 1)
 
         ## BATCHMODE 2 : Distance btw rings map
         self.distanceMapTab = QWidget()
         self.distanceMapTab.setContentsMargins(0, 0, 0, 0)
         self.distanceMapTabLayout = QGridLayout(self.distanceMapTab)
-        self.distanceMapFigure = plt.figure(facecolor='#606060')
+        self.distanceMapFigure = plt.figure()
         self.distanceMapAxes = self.distanceMapFigure.add_subplot(111)
         self.distanceMapCanvas = FigureCanvas(self.distanceMapFigure)
         self.distanceMapFigure.canvas.mpl_connect('button_press_event', self.plotClicked)
-        self.ds_ImgFigure = plt.figure(facecolor='#606060')
+        self.ds_ImgFigure = plt.figure()
         self.ds_ImgCanvas = FigureCanvas(self.ds_ImgFigure)
 
         self.ds_maxIntMap = QDoubleSpinBox()
         self.ds_maxIntMap.setMinimum(1)
         self.ds_maxIntMap.setMaximum(100)
         self.ds_maxIntMap.setValue(100.)
         self.ds_maxIntMap.setSingleStep(5.0)
@@ -291,15 +291,15 @@
         ## BATCHMODE 3 : Angular range map (degrees)
         self.angularMapTab = QWidget()
         self.angularMapTab.setContentsMargins(0, 0, 0, 0)
         self.angularMapTabLayout = QGridLayout(self.angularMapTab)
         self.angularMapTab = QWidget()
         self.angularMapTab.setContentsMargins(0, 0, 0, 0)
         self.angularMapTabLayout = QGridLayout(self.angularMapTab)
-        self.angularMapFigure = plt.figure(facecolor='#606060')
+        self.angularMapFigure = plt.figure()
         self.angularMapAxes = self.angularMapFigure.add_subplot(111)
         self.angularMapCanvas = FigureCanvas(self.angularMapFigure)
         self.angularMapFigure.canvas.mpl_connect('button_press_event', self.plotClicked)
 
         self.ar_maxIntMap = QDoubleSpinBox()
         self.ar_maxIntMap.setMinimum(1)
         self.ar_maxIntMap.setMaximum(100)
@@ -322,15 +322,15 @@
         self.angularMapTabLayout.addWidget(self.angularMapCanvas, 0, 0, 1, 1)
         self.angularMapTabLayout.addLayout(self.ar_MapIntSettings, 1, 0, 1, 1)
 
         ## BATCHMODE 4 : Vector Fields
         self.vectorFieldTab = QWidget()
         self.vectorFieldTab.setContentsMargins(0, 0, 0, 0)
         self.vectorFieldTabLayout = QGridLayout(self.vectorFieldTab)
-        self.vectorFieldMapFigure = plt.figure(facecolor='#606060')
+        self.vectorFieldMapFigure = plt.figure()
         self.vectorFieldMapAxes = self.vectorFieldMapFigure.add_subplot(111)
         self.vectorFieldMapCanvas = FigureCanvas(self.vectorFieldMapFigure)
         self.vectorFieldMapFigure.canvas.mpl_connect('button_press_event', self.plotClicked)
         self.arrowLengthSlider = QSlider()
         self.arrowLengthSlider.setMinimum(5)
         self.arrowLengthSlider.setMaximum(25)
         self.arrowLengthSlider.setValue(5)
@@ -340,15 +340,15 @@
         self.vectorFieldTabLayout.addWidget(QLabel("Arrow Length"), 1, 0, 1, 1)
         self.vectorFieldTabLayout.addWidget(self.arrowLengthSlider, 1, 1, 1, 1)
 
         ## BATCHMODE 5 : Elliptical Presentation
         self.ellipticalTab = QWidget()
         self.ellipticalTab.setContentsMargins(0, 0, 0, 0)
         self.ellipticalTabLayout = QGridLayout(self.ellipticalTab)
-        self.ellipticalMapFigure = plt.figure(facecolor='#606060')
+        self.ellipticalMapFigure = plt.figure()
         self.ellipticalMapAxes = self.ellipticalMapFigure.add_subplot(111)
         self.ellipticalMapCanvas = FigureCanvas(self.ellipticalMapFigure)
         self.ellipticalMapFigure.canvas.mpl_connect('button_press_event', self.plotClicked)
         self.ellipticalTabLayout.addWidget(self.ellipticalMapCanvas, 0, 0, 1, 1)
 
         ## tabs
         self.tabWidget = QTabWidget()
```

### Comparing `musclex-1.9.2/musclex/ui/CPBatchWindow2.py` & `musclex-1.9.3/musclex/ui/CPBatchWindow2.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/CPImageWindow.py` & `musclex-1.9.3/musclex/ui/CPImageWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,27 +57,27 @@
                 for r in possible_vals:
                     if b==0 and g==0 and r==0:
                         continue
                     self.ring_colors.append([b,g,r])
 
     def initUI(self):
         self.setWindowTitle("Muscle X Circular Projection v." + musclex.__version__)
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.centralWidget = QWidget(self)
         self.mainLayout = QVBoxLayout(self.centralWidget)
         self.setCentralWidget(self.centralWidget)
 
         ### Image mode tabs
         ## IMAGE MODE 1 : Image tab
         self.imageTab = QWidget()
         self.imageTab.setContentsMargins(0, 0, 0, 0)
         self.imageTabLayout = QHBoxLayout(self.imageTab)
         self.displayedImgLayout = QHBoxLayout()
         self.displayedImgLayout.setAlignment(Qt.AlignCenter)
-        self.displayImgFigure = plt.figure(facecolor='#606060')
+        self.displayImgFigure = plt.figure()
         self.displayImgAxes = self.displayImgFigure.add_subplot(111)
         self.displayImgCanvas = FigureCanvas(self.displayImgFigure)
         self.imageOptionsFrame = QFrame()
         self.imageOptionsFrame.setFixedWidth(300)
         self.imageOptionsLayout = QVBoxLayout()
         self.imageOptionsLayout.setAlignment(Qt.AlignTop)
         self.centerChkbx = QCheckBox("Display Center")
@@ -203,24 +203,24 @@
         self.m1_keys_layout.setAlignment(change_label, Qt.AlignCenter)
         self.m1_keys_layout.addWidget(self.prev_range, 1, 2, 1, 1)
         self.m1_keys_layout.addWidget(self.next_range, 1, 3, 1, 1)
         self.m1_keys_layout.setAlignment(Qt.AlignTop)
         self.m1_key_group.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
         self.m1_key_group.setAlignment(Qt.AlignTop)
 
-        self.m1_partial_hist_figure = plt.figure(facecolor='#606060')
+        self.m1_partial_hist_figure = plt.figure()
         self.m1_partial_hist_figure.subplots_adjust(top=0.90, bottom=0.20)
         self.m1_partial_hist_axes = self.m1_partial_hist_figure.add_subplot(111)
         self.m1_partial_hist_canvas = FigureCanvas(self.m1_partial_hist_figure)
         # self.toolbar = NavigationToolbar(self.m1_partial_hist_canvas, self)
         # self.method1TabLayout.addWidget(self.toolbar)
-        self.m1_hist_figure = plt.figure(facecolor='#606060')
+        self.m1_hist_figure = plt.figure()
         self.m1_hist_axes = self.m1_hist_figure.add_subplot(111)
         self.m1_hist_canvas = FigureCanvas(self.m1_hist_figure)
-        self.m1_img_fig = plt.figure(facecolor='#606060')
+        self.m1_img_fig = plt.figure()
         self.m1_img_axes = self.m1_img_fig.add_subplot(111)
         self.m1_img_canvas = FigureCanvas(self.m1_img_fig)
         self.method1TabLayout.addWidget(self.m1_img_canvas, 0, 0, 3, 1)
         self.method1TabLayout.addWidget(self.m1_partial_hist_canvas, 0, 1)
         self.method1TabLayout.addWidget(self.m1_key_group, 1, 1)
         self.method1TabLayout.addWidget(self.m1_hist_canvas, 2, 1)
 
@@ -232,15 +232,15 @@
         self.method2ComboBx.addItem("2D Integration")
         self.method2ComboBx.addItem("Central Differences")
         self.method2ComboBx.addItem("Log Central Differences")
         self.method2ComboBx.setCurrentIndex(2)
         self.runsChkBx = QCheckBox("Display Runs")
         self.ringsChkBx = QCheckBox("Display Rings")
 
-        self.m2_cent_diff_fig = plt.figure(facecolor='#606060')
+        self.m2_cent_diff_fig = plt.figure()
         self.m2_cent_diff_axes = self.m2_cent_diff_fig.add_subplot(111)
         self.m2_cent_diff_canvas = FigureCanvas(self.m2_cent_diff_fig)
         self.method2Tablayout.addWidget(self.method2ComboBx, 0, 0, 1, 1)
         self.method2Tablayout.addWidget(self.runsChkBx, 0, 1, 1, 1)
         # self.method2Tablayout.setAlignment(self.runsChkBx, Qt.AlignCenter)
         self.method2Tablayout.addWidget(self.ringsChkBx, 0, 2, 1, 1)
         # self.method2Tablayout.setAlignment(self.ringsChkBx, Qt.AlignCenter)
@@ -287,15 +287,15 @@
         self.graph_options_layout.addWidget(self.fit_hist_chkbx)
         self.graph_options_layout.addWidget(self.ring_hists_chkbx)
         self.graph_options_layout.addWidget(self.g_model_chkbx)
         self.graph_options_layout.addWidget(self.average_ring_chkbx)
         self.graph_options_frame.setLayout(self.graph_options_layout)
 
         # self.graph_options_frame.setFixedWidth(200)
-        self.result_graph_figure = plt.figure(facecolor='#606060')
+        self.result_graph_figure = plt.figure()
         self.result_graph_axes = self.result_graph_figure.add_subplot(111)
         self.result_graph_canvas = FigureCanvas(self.result_graph_figure)
         self.processing_results = QTextEdit()
         self.processing_results.setReadOnly(True)
         self.processing_results.setText("Angular results : N/A")
         self.rings_results = QTextEdit()
         self.rings_results.setReadOnly(True)
```

### Comparing `musclex-1.9.2/musclex/ui/ddf_processor.py` & `musclex-1.9.3/musclex/ui/ddf_processor.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/diffraction_centroids.py` & `musclex-1.9.3/musclex/ui/diffraction_centroids.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/EQ_FittingTab.py` & `musclex-1.9.3/musclex/ui/EQ_FittingTab.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/EQStartWindow.py` & `musclex-1.9.3/musclex/ui/EQStartWindow.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/EquatorWindow.py` & `musclex-1.9.3/musclex/ui/EquatorWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self.fixedIntArea = None
         self.dir_path, self.imgList, self.currentImg = getImgFiles(str(filename))
         if len(self.imgList) == 0:
             self.inputerror()
             return
         self.csvManager = EQ_CVSManager(self.dir_path)  # Create a CSV Manager object
         self.setWindowTitle("Muscle X Equator v." + self.version)
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.initUI()  # Initial all UI
         self.setAllToolTips()  # Set tooltips for widgets
         self.setConnections()  # Set interaction for widgets
         self.setCalibrationImage()
         self.onImageChanged() # Toggle window to process current image
         self.show()
         self.resize(1000, 100)
@@ -115,15 +115,15 @@
 
         #
         ### Image Tab ###
         #
         self.imageTab = QWidget()
         self.imageTab.setContentsMargins(0, 0, 0, 0)
         self.imageTabLayout = QHBoxLayout(self.imageTab)
-        self.displayImgFigure = plt.figure(facecolor='#606060')
+        self.displayImgFigure = plt.figure()
         self.displayImgAxes = self.displayImgFigure.add_subplot(111)
         self.imageVLayout = QVBoxLayout()
         self.displayImgCanvas = FigureCanvas(self.displayImgFigure)
         self.imageVLayout.addWidget(self.displayImgCanvas)
 
         self.imgDispOptionGrp = QGroupBox('Display Options')
         self.imgDispOptLayout = QVBoxLayout()
@@ -167,24 +167,24 @@
 
         self.imgProcGrp = QGroupBox("Image Processing")
         self.imgProcLayout = QGridLayout()
         self.imgProcGrp.setLayout(self.imgProcLayout)
         self.calibrationB = QPushButton("Calibration Settings")
         self.setRotAndCentB = QPushButton("Set Rotation Angle \nand Center")
         self.setRotAndCentB.setCheckable(True)
-        self.setRotAndCentB.setFixedHeight(40)
+        self.setRotAndCentB.setFixedHeight(45)
         self.setAngleB = QPushButton("Set \nRotation Angle")
         self.setAngleB.setCheckable(True)
-        self.setAngleB.setFixedHeight(40)
+        self.setAngleB.setFixedHeight(45)
         self.setRminB = QPushButton("Set R-min")
         self.setRminB.setCheckable(True)
-        self.setRminB.setFixedHeight(40)
+        self.setRminB.setFixedHeight(45)
         self.setIntAreaB = QPushButton("Set Box Width")
         self.setIntAreaB.setCheckable(True)
-        self.setIntAreaB.setFixedHeight(40)
+        self.setIntAreaB.setFixedHeight(45)
         self.checkableButtons.extend([self.setRotAndCentB, self.setIntAreaB, self.setRminB, self.setAngleB])
         self.fixedAngleChkBx = QCheckBox("Fixed Angle")
         self.fixedAngleChkBx.setChecked(False)
         self.fixedIntAreaChkBx = QCheckBox("Fixed Box Width")
         self.fixedIntAreaChkBx.setChecked(False)
         self.fixedAngle = QSpinBox()
         self.fixedAngle.setKeyboardTracking(False)
@@ -226,15 +226,15 @@
         self.bottomLayout.addWidget(self.rejectChkBx, 0, 0, 1, 2)
         self.bottomLayout.addWidget(self.processFolderButton, 1, 0, 1, 2)
         self.bottomLayout.addWidget(self.prevButton, 2, 0, 1, 1)
         self.bottomLayout.addWidget(self.nextButton, 2, 1, 1, 1)
         self.bottomLayout.setAlignment(self.rejectChkBx, Qt.AlignLeft)
 
         self.imageOptionsFrame = QFrame()
-        self.imageOptionsFrame.setFixedWidth(300)
+        self.imageOptionsFrame.setFixedWidth(350)
         self.imageOptionsLayout = QVBoxLayout()
 
         self.imageOptionsLayout.setAlignment(Qt.AlignTop)
         self.imageOptionsLayout.addSpacing(10)
         self.imageOptionsLayout.addWidget(self.imgDispOptionGrp)
         self.imageOptionsLayout.addSpacing(10)
         self.imageOptionsLayout.addWidget(self.imgProcGrp)
@@ -249,15 +249,15 @@
         #
         ### Fitting Tab ###
         #
         self.fittingTab = QWidget()
         self.fittingTabLayout = QHBoxLayout(self.fittingTab)
 
         # Plot
-        self.fittingFigure = plt.figure(facecolor='#606060')
+        self.fittingFigure = plt.figure()
         self.fittingAxes = self.fittingFigure.add_subplot(111)
         self.fittingVLayout = QVBoxLayout()
         self.fittingCanvas = FigureCanvas(self.fittingFigure)
 
         self.generalGrp = QGroupBox("General Settings")
         self.genLayout = QGridLayout(self.generalGrp)
         self.skeletalChkBx = QCheckBox("Skeletal Muscle (Z line)")
```

### Comparing `musclex-1.9.2/musclex/ui/ImageMerger.py` & `musclex-1.9.3/musclex/ui/ImageMerger.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/ProjectionBoxTab.py` & `musclex-1.9.3/musclex/ui/ProjectionBoxTab.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,19 +79,19 @@
 
     def initUI(self):
         """
         Initial all GUIs including : 4 plots and result table
         """
         self.setContentsMargins(0, 0, 0, 0)
         self.tabLayout = QHBoxLayout(self)
-        self.graphFigure1 = plt.figure(facecolor='#606060')
+        self.graphFigure1 = plt.figure()
         self.graphAxes1 = self.graphFigure1.add_subplot(111)
         self.graphCanvas1 = FigureCanvas(self.graphFigure1)
 
-        self.graphFigure2 = plt.figure(facecolor='#606060')
+        self.graphFigure2 = plt.figure()
         self.graphAxes2 = self.graphFigure2.add_subplot(111)
         self.graphCanvas2 = FigureCanvas(self.graphFigure2)
 
         self.optionsFrame = QFrame()
         self.optionsFrame.setFixedWidth(350)
         self.optionsLayout = QVBoxLayout(self.optionsFrame)
```

### Comparing `musclex-1.9.2/musclex/ui/ProjectionTracesGUI.py` & `musclex-1.9.3/musclex/ui/ProjectionTracesGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         self.img_zoom = None
         self.function = None
         self.allboxes = {}
         self.boxtypes = {}
         self.bgsubs = {}
         self.peaks = {}
         self.hull_ranges = {}
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.checkableButtons = []
         self.initUI()
         self.setConnections()
 
     def initUI(self):
         """
         Initial all GUI
@@ -137,15 +137,15 @@
         self.tabWidget.setTabPosition(QTabWidget.North)
         self.tabWidget.setDocumentMode(False)
         self.tabWidget.setTabsClosable(True)
         self.tabWidget.setStyleSheet("QTabBar::tab { height: 20px; width: 200px; }")
 
         self.imageTab = QWidget()
         self.imageTabLayer = QHBoxLayout(self.imageTab)
-        self.displayImgFigure = plt.figure(facecolor='#606060')
+        self.displayImgFigure = plt.figure()
         self.displayImgAxes = self.displayImgFigure.add_subplot(111)
         self.imageVLayout = QVBoxLayout()
         self.displayImgCanvas = FigureCanvas(self.displayImgFigure)
         self.imageVLayout.addWidget(self.displayImgCanvas)
 
         self.imageLeftFrame = QFrame()
         self.imageLeftFrame.setFixedWidth(250)
```

### Comparing `musclex-1.9.2/musclex/ui/pyqt_utils.py` & `musclex-1.9.3/musclex/ui/pyqt_utils.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/ui/QuadrantFoldingGUI.py` & `musclex-1.9.3/musclex/ui/QuadrantFoldingGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.BGImages = []
         self.ignoreFolds = set()
         self.initUI() # initial all GUI
         self.setConnections() # set triggered function for widgets
         self.setMinimumHeight(800)
 
     def initUI(self):
-        self.setStyleSheet(getStyleSheet())
+        # self.setStyleSheet(getStyleSheet())
         self.setWindowTitle("Muscle X Quadrant Folding v." + musclex.__version__)
 
         self.centralWidget = QWidget(self)
         self.setCentralWidget(self.centralWidget)
         self.mainHLayout = QHBoxLayout(self.centralWidget)
 
         self.tabWidget = QTabWidget()
@@ -99,15 +99,15 @@
         self.selectFolder = QPushButton('Click Here to Select a Folder...')
         self.selectFolder.setFixedHeight(100)
         self.selectFolder.setFixedWidth(300)
 
         self.bgWd = QWidget()
         self.verImgLayout.addWidget(self.selectImageButton)
         self.verImgLayout.addWidget(self.selectFolder)
-        self.imageFigure = plt.figure(facecolor='#606060')
+        self.imageFigure = plt.figure()
         self.imageAxes = self.imageFigure.add_subplot(111)
         self.imageCanvas = FigureCanvas(self.imageFigure)
 
         self.imageCanvas.setHidden(True)
         self.imageTabLayout.addLayout(self.verImgLayout)
         self.imageTabLayout.addWidget(self.imageCanvas)
 
@@ -223,15 +223,15 @@
 
         self.leftLayout = QVBoxLayout()
         self.leftFrame = QFrame()
         self.leftFrame.setFixedWidth(300)
         self.leftFrame.setLayout(self.leftLayout)
         self.resultTabLayout.addWidget(self.leftFrame)
         
-        self.resultFigure = plt.figure(facecolor='#606060')
+        self.resultFigure = plt.figure()
         self.resultAxes = self.resultFigure.add_subplot(111)
         self.resultVLayout = QVBoxLayout()
         self.resultCanvas = FigureCanvas(self.resultFigure)
         self.resultTabLayout.addWidget(self.resultCanvas)
 
         self.rightLayout = QVBoxLayout()
         self.rightFrame = QFrame()
```

### Comparing `musclex-1.9.2/musclex/utils/__init__.py` & `musclex-1.9.3/musclex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/utils/file_manager.py` & `musclex-1.9.3/musclex/utils/file_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
         os.makedirs(path)
 
 def getStyleSheet():
     """
     Get style sheet from stylesheet.txt
     :return: styesheet (str) or empty string if it's not available
     """
+    return ""
     return "QToolTip{     border: 1px solid black;     background-color: #ffa02f;     padding: 1px;     border-radius: 3px;     opacity: 100;} " \
            "QWidget {    color: #cecece;    background-color: #323232; }" \
            "QWidget:item:selected{    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #ffa02f, stop: 1 #d7801a);}" \
            "QMenuBar::item{    background: transparent;}" \
            "QMenuBar::item:selected{    background: transparent;    border: 1px solid #ffaa00;}" \
            "QMenuBar::item:pressed{    background: #6d6d6d;    border: 1px solid #000;    background-color: QLinearGradient(        x1:0, y1:0,        x2:0, y2:1,        stop:1 #212121,        stop:0.4 #343434/*,        stop:0.2 #343434,        stop:0.1 #ffaa00*/    );    margin-bottom:-1px;    padding-bottom:1px;}" \
            "QMenu{    border: 1px solid #000;}" \
@@ -149,15 +150,15 @@
            "QMenu::item:selected{    color: #000000;}" \
            "QWidget:disabled{    color: #777676;    background-color: #323232;}" \
            "QAbstractItemView{    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #4d4d4d, stop: 0.1 #646464, stop: 1 #5d5d5d);}" \
            "QLineEdit{    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #4d4d4d, stop: 0 #646464, stop: 1 #5d5d5d);    padding: 1px;    border-style: solid;    border: 1px solid #1e1e1e;    border-radius: 5;}" \
            "QPushButton{    color: #cecece;    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #565656, stop: 0.1 #525252, stop: 0.5 #4e4e4e, stop: 0.9 #4a4a4a, stop: 1 #464646);    border-width: 1px;    border-color: #1e1e1e;    border-style: solid;    border-radius: 6;    padding: 3px;    font-size: 12px;    padding-left: 5px;    padding-right: 5px; height: 15px;}" \
            "QPushButton:pressed{    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #2d2d2d, stop: 0.1 #2b2b2b, stop: 0.5 #292929, stop: 0.9 #282828, stop: 1 #252525);}" \
            "QPushButton:checked{    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #2d2d2d, stop: 0.1 #2b2b2b, stop: 0.5 #292929, stop: 0.9 #282828, stop: 1 #252525);}" \
-           "QComboBox{    selection-background-color: #ffaa00;    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #565656, stop: 0.1 #525252, stop: 0.5 #4e4e4e, stop: 0.9 #4a4a4a, stop: 1 #464646);    border-style: solid;    border: 1px solid #1e1e1e;    border-radius: 5;}" \
+           "QComboBox{    color: #ffffff; selection-background-color: #ffaa00;    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #565656, stop: 0.1 #525252, stop: 0.5 #4e4e4e, stop: 0.9 #4a4a4a, stop: 1 #464646);    border-style: solid;    border: 1px solid #1e1e1e;    border-radius: 5;}" \
            "QComboBox:hover,QPushButton:hover{    border: 2px solid QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #ffa02f, stop: 1 #51300a);}" \
            "QComboBox:on{    padding-top: 3px;    padding-left: 4px;    background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #2d2d2d, stop: 0.1 #2b2b2b, stop: 0.5 #292929, stop: 0.9 #282828, stop: 1 #252525);    selection-background-color: #ffaa00;}" \
            "QComboBox QAbstractItemView{    border: 2px solid darkgray;    selection-background-color: QLinearGradient( x1: 0, y1: 0, x2: 0, y2: 1, stop: 0 #ffa02f, stop: 1 #d7801a);}" \
            "QComboBox::drop-down{     subcontrol-origin: padding;     subcontrol-position: top right;     width: 15px;     border-left-width: 0px;     border-left-color: darkgray;     border-left-style: solid; /* just a single line */     border-top-right-radius: 2px; /* same radius as the QComboBox */     border-bottom-right-radius: 2px; }" \
            "QGroupBox { border: 1px solid gray; border-radius: 2px; margin-top: 1ex; }" \
            "QGroupBox::indicator{    color: #cecece;    background-color: #323232;    border: 1px solid #cecece;    width: 9px;    height: 9px;}" \
            "QGroupBox::indicator:disabled, QRadioButton::indicator:disabled{    border: 1px solid #6d6d6d;}" \
```

### Comparing `musclex-1.9.2/musclex/utils/histogram_processor.py` & `musclex-1.9.3/musclex/utils/histogram_processor.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex/utils/image_processor.py` & `musclex-1.9.3/musclex/utils/image_processor.py`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/musclex.egg-info/PKG-INFO` & `musclex-1.9.3/musclex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: musclex
-Version: 1.9.2
+Version: 1.9.3
 Summary: Muscle X
 Home-page: https://github.com/biocatiit/musclex/wiki
 Author: Jiranun J.
 Author-email: jjiratra@hawk.iit.edu
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `musclex-1.9.2/musclex.egg-info/SOURCES.txt` & `musclex-1.9.3/musclex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musclex-1.9.2/PKG-INFO` & `musclex-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: musclex
-Version: 1.9.2
+Version: 1.9.3
 Summary: Muscle X
 Home-page: https://github.com/biocatiit/musclex/wiki
 Author: Jiranun J.
 Author-email: jjiratra@hawk.iit.edu
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `musclex-1.9.2/setup.py` & `musclex-1.9.3/setup.py`

 * *Files identical despite different names*

