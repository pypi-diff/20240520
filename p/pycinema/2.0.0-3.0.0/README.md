# Comparing `tmp/pycinema-2.0.0.tar.gz` & `tmp/pycinema-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycinema-2.0.0.tar", last modified: Wed Sep 20 19:58:04 2023, max compression
+gzip compressed data, was "pycinema-3.0.0.tar", last modified: Mon May 20 20:05:56 2024, max compression
```

## Comparing `pycinema-2.0.0.tar` & `pycinema-3.0.0.tar`

### file list

```diff
@@ -1,77 +1,98 @@
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.417769 pycinema-2.0.0/
--rw-r--r--   0 dhr      (24423) staff       (20)      937 2023-09-20 19:58:04.417638 pycinema-2.0.0/PKG-INFO
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.403239 pycinema-2.0.0/doc/
--rw-r--r--   0 dhr      (24423) staff       (20)      558 2023-09-20 19:55:33.000000 pycinema-2.0.0/doc/description.md
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.403827 pycinema-2.0.0/pycinema/
--rw-r--r--   0 dhr      (24423) staff       (20)     9025 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/Core.py
--rw-r--r--   0 dhr      (24423) staff       (20)       55 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/__init__.py
--rw-r--r--   0 dhr      (24423) staff       (20)       22 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/_version.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.409295 pycinema-2.0.0/pycinema/filters/
--rw-r--r--   0 dhr      (24423) staff       (20)     1718 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/CinemaDatabaseReader.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3315 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/CinemaDatabaseWriter.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3736 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ColorMapping.py
--rw-r--r--   0 dhr      (24423) staff       (20)      374 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ColorSource.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4949 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/DepthCompositing.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3516 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ImageAnnotation.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1310 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ImageBorder.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1093 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ImageCanny.py
--rw-r--r--   0 dhr      (24423) staff       (20)      690 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ImageConvertGrayscale.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1801 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ImageFilterPIL.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2801 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ImageReader.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2444 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/MaskCompositing.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3606 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/Shader.py
--rw-r--r--   0 dhr      (24423) staff       (20)     6891 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderDemoScene.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4327 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderFXAA.py
--rw-r--r--   0 dhr      (24423) staff       (20)     5390 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderIBS.py
--rw-r--r--   0 dhr      (24423) staff       (20)     8304 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderLineAO.py
--rw-r--r--   0 dhr      (24423) staff       (20)     8032 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderPBR.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3791 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderPhong.py
--rw-r--r--   0 dhr      (24423) staff       (20)     8429 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderPointAO.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3532 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/ShaderSSAO.py
--rw-r--r--   0 dhr      (24423) staff       (20)      517 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/TableEditor.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2401 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/TableQuery.py
--rw-r--r--   0 dhr      (24423) staff       (20)      794 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/TableWriter.py
--rw-r--r--   0 dhr      (24423) staff       (20)      687 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/filters/__init__.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.410454 pycinema-2.0.0/pycinema/ipy/
--rw-r--r--   0 dhr      (24423) staff       (20)     4123 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/ipy/CinemaDatabaseViewer.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4344 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/ipy/ColorMappingWidgets.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1524 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/ipy/ImageViewer.py
--rw-r--r--   0 dhr      (24423) staff       (20)      938 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/ipy/NumberWidget.py
--rw-r--r--   0 dhr      (24423) staff       (20)     7066 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/ipy/ParameterWidgets.py
--rw-r--r--   0 dhr      (24423) staff       (20)      158 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/ipy/__init__.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.412773 pycinema-2.0.0/pycinema/theater/
--rw-r--r--   0 dhr      (24423) staff       (20)     2639 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/FilterBrowser.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1566 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/Icons.py
--rw-r--r--   0 dhr      (24423) staff       (20)    12677 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/Theater.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2405 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/View.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4198 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/ViewFrame.py
--rw-r--r--   0 dhr      (24423) staff       (20)      455 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/ViewStyle.py
--rw-r--r--   0 dhr      (24423) staff       (20)      151 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/__init__.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.415577 pycinema-2.0.0/pycinema/theater/node_editor/
--rw-r--r--   0 dhr      (24423) staff       (20)      837 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/node_editor/Edge.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3320 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/node_editor/InputText.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3277 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/node_editor/Node.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2711 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/node_editor/NodeEditorStyle.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3836 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/node_editor/Port.py
--rw-r--r--   0 dhr      (24423) staff       (20)      116 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/node_editor/__init__.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.417296 pycinema-2.0.0/pycinema/theater/views/
--rw-r--r--   0 dhr      (24423) staff       (20)     5837 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/ColorMappingView.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1515 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/FilterView.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3388 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/ImageView.py
--rw-r--r--   0 dhr      (24423) staff       (20)      745 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/InspectorView.py
--rw-r--r--   0 dhr      (24423) staff       (20)    12683 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/NodeEditorView.py
--rw-r--r--   0 dhr      (24423) staff       (20)    14038 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/ParallelCoordinatesView.py
--rw-r--r--   0 dhr      (24423) staff       (20)     8352 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/ParameterView.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1128 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/SelectionView.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1876 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/TableView.py
--rw-r--r--   0 dhr      (24423) staff       (20)      375 2023-09-20 19:55:33.000000 pycinema-2.0.0/pycinema/theater/views/__init__.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.404651 pycinema-2.0.0/pycinema.egg-info/
--rw-r--r--   0 dhr      (24423) staff       (20)      937 2023-09-20 19:58:04.000000 pycinema-2.0.0/pycinema.egg-info/PKG-INFO
--rw-r--r--   0 dhr      (24423) staff       (20)     2126 2023-09-20 19:58:04.000000 pycinema-2.0.0/pycinema.egg-info/SOURCES.txt
--rw-r--r--   0 dhr      (24423) staff       (20)        1 2023-09-20 19:58:04.000000 pycinema-2.0.0/pycinema.egg-info/dependency_links.txt
--rw-r--r--   0 dhr      (24423) staff       (20)      191 2023-09-20 19:58:04.000000 pycinema-2.0.0/pycinema.egg-info/requires.txt
--rw-r--r--   0 dhr      (24423) staff       (20)        9 2023-09-20 19:58:04.000000 pycinema-2.0.0/pycinema.egg-info/top_level.txt
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-09-20 19:58:04.417436 pycinema-2.0.0/scripts/
--rw-r--r--   0 dhr      (24423) staff       (20)      895 2023-09-20 19:55:33.000000 pycinema-2.0.0/scripts/cinema
--rw-r--r--   0 dhr      (24423) staff       (20)       38 2023-09-20 19:58:04.417816 pycinema-2.0.0/setup.cfg
--rw-r--r--   0 dhr      (24423) staff       (20)     1369 2023-09-20 19:55:33.000000 pycinema-2.0.0/setup.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.575210 pycinema-3.0.0/
+-rw-r--r--   0 dhr      (24423) staff       (20)     1407 2024-05-20 20:05:56.575012 pycinema-3.0.0/PKG-INFO
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.562648 pycinema-3.0.0/doc/
+-rw-r--r--   0 dhr      (24423) staff       (20)      558 2024-05-20 19:33:04.000000 pycinema-3.0.0/doc/pycinema-description.md
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.562972 pycinema-3.0.0/pycinema/
+-rw-r--r--   0 dhr      (24423) staff       (20)    16186 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/Core.py
+-rw-r--r--   0 dhr      (24423) staff       (20)       55 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/__init__.py
+-rw-r--r--   0 dhr      (24423) staff       (20)       22 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/_version.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.568586 pycinema-3.0.0/pycinema/filters/
+-rw-r--r--   0 dhr      (24423) staff       (20)     1611 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/CSVReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1311 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/Calculator.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1911 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/CinemaDatabaseReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3355 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/CinemaDatabaseWriter.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     7835 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ColorMapping.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      374 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ColorSource.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4967 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/DepthCompositing.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      775 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/GetColumn.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3516 2024-01-18 15:47:34.000000 pycinema-3.0.0/pycinema/filters/ImageAnnotation.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1310 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ImageBorder.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1093 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ImageCanny.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      690 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ImageConvertGrayscale.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1843 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ImageFilterPIL.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2999 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ImageReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1619 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ImageSort.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     7121 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ImageView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      730 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ImagesToTable.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      602 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/InspectorView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1751 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/MLTFPredictor.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1173 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/MLTFReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2463 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/MaskCompositing.py
+-rw-r--r--   0 dhr      (24423) staff       (20)    14702 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ParallelCoordinates.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     7631 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ParametersView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1459 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/Plot.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1229 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/PlotLineItem.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1230 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/Python.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3622 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/Shader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     6891 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderDemoScene.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4327 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderFXAA.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     5390 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderIBS.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     8304 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderLineAO.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     8032 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderPBR.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3791 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderPhong.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     8429 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderPointAO.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3532 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/ShaderSSAO.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2338 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/SqliteDatabaseReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      517 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/filters/TableEditor.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2304 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/TableQuery.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     5309 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/TableView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      833 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/TableWriter.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1108 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/TextEditor.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      887 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/TextFileReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      434 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/ValueSource.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1175 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/filters/__init__.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.569237 pycinema-3.0.0/pycinema/ipy/
+-rw-r--r--   0 dhr      (24423) staff       (20)     4123 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/ipy/CinemaDatabaseViewer.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4344 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/ipy/ColorMappingWidgets.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1524 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/ipy/ImageViewer.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      938 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/ipy/NumberWidget.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     7066 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/ipy/ParameterWidgets.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      158 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/ipy/__init__.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.570118 pycinema-3.0.0/pycinema/scripts/
+-rw-r--r--   0 dhr      (24423) staff       (20)        0 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/scripts/__init__.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1899 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/scripts/browse.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3788 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/scripts/discover.py
+-rwxr-xr-x   0 dhr      (24423) staff       (20)     2305 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/scripts/explore.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2275 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/scripts/view.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.573062 pycinema-3.0.0/pycinema/theater/
+-rw-r--r--   0 dhr      (24423) staff       (20)     2671 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/FilterBrowser.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2831 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/Icons.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3725 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/SplitFrame.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3342 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/TabFrame.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     9080 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/Theater.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2555 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/View.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      455 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/theater/ViewStyle.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      184 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/__init__.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.573928 pycinema-3.0.0/pycinema/theater/node_editor/
+-rw-r--r--   0 dhr      (24423) staff       (20)      837 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/theater/node_editor/Edge.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3320 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/theater/node_editor/InputText.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4071 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/node_editor/Node.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2711 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/theater/node_editor/NodeEditorStyle.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4803 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/node_editor/Port.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      116 2023-10-25 17:24:52.000000 pycinema-3.0.0/pycinema/theater/node_editor/__init__.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.574598 pycinema-3.0.0/pycinema/theater/views/
+-rw-r--r--   0 dhr      (24423) staff       (20)     1029 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/views/FilterView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)    12333 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/views/NodeEditorView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2269 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/views/SelectionView.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      138 2024-05-20 19:33:04.000000 pycinema-3.0.0/pycinema/theater/views/__init__.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.563639 pycinema-3.0.0/pycinema.egg-info/
+-rw-r--r--   0 dhr      (24423) staff       (20)     1407 2024-05-20 20:05:56.000000 pycinema-3.0.0/pycinema.egg-info/PKG-INFO
+-rw-r--r--   0 dhr      (24423) staff       (20)     2702 2024-05-20 20:05:56.000000 pycinema-3.0.0/pycinema.egg-info/SOURCES.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)        1 2024-05-20 20:05:56.000000 pycinema-3.0.0/pycinema.egg-info/dependency_links.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)        1 2024-05-20 20:05:56.000000 pycinema-3.0.0/pycinema.egg-info/not-zip-safe
+-rw-r--r--   0 dhr      (24423) staff       (20)      245 2024-05-20 20:05:56.000000 pycinema-3.0.0/pycinema.egg-info/requires.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)        9 2024-05-20 20:05:56.000000 pycinema-3.0.0/pycinema.egg-info/top_level.txt
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2024-05-20 20:05:56.574735 pycinema-3.0.0/scripts/
+-rw-r--r--   0 dhr      (24423) staff       (20)     1667 2024-05-20 19:33:04.000000 pycinema-3.0.0/scripts/cinema
+-rw-r--r--   0 dhr      (24423) staff       (20)       38 2024-05-20 20:05:56.575279 pycinema-3.0.0/setup.cfg
+-rw-r--r--   0 dhr      (24423) staff       (20)     1514 2024-05-20 19:33:04.000000 pycinema-3.0.0/setup.py
```

### Comparing `pycinema-2.0.0/doc/description.md` & `pycinema-3.0.0/doc/pycinema-description.md`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/CinemaDatabaseReader.py` & `pycinema-3.0.0/pycinema/filters/CinemaDatabaseReader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pycinema import Filter
 
 import csv
-from os.path import exists
+import os.path
 import re
+import logging as log
 
 class CinemaDatabaseReader(Filter):
 
     def __init__(self):
         super().__init__(
           inputs={
             'path': '',
@@ -17,47 +18,50 @@
           }
         )
 
     def _update(self):
 
         table = []
         dbPath = self.inputs.path.get()
+        dbPath = os.path.expanduser(dbPath)
+
         if not dbPath:
             self.outputs.table.set([[]])
             return 0
 
-        if not exists(dbPath):
-            print('[ERROR] CDB not found:', dbPath)
+        if not os.path.exists(dbPath):
+            log.error(" CDB not found '" + dbPath + "'")
             self.outputs.table.set([[]])
             return 0
 
         try:
             dataCsvPath = dbPath + '/data.csv'
             with open(dataCsvPath, 'r+') as csvfile:
                 rows = csv.reader(csvfile, delimiter=',')
                 for row in rows:
                     table.append(row)
         except:
-            print('[ERROR] Unable to open data.csv')
+            log.error(" Unable to open data.csv")
             self.outputs.table.set([[]])
             return 0
 
         # remove empty lines
         table = list(filter(lambda row: len(row)>0, table))
 
         # # force lower case header
         # table[0] = list(map(str.lower,table[0]))
 
         # add dbPath prefix to file column
         try:
             fileColumnIdx = [i for i, item in enumerate(table[0]) if re.search(self.inputs.file_column.get(), item, re.IGNORECASE)].pop()
         except:
-            print('[ERROR] file column not found:',self.inputs.file_column.get())
+            log.error(" file column not found: '" + self.inputs.file_column.get() + "'")
             self.outputs.table.set([[]])
             return 0
 
         for i in range(1,len(table)):
-            table[i][fileColumnIdx] = dbPath + '/' + table[i][fileColumnIdx]
+            if not table[i][fileColumnIdx].startswith('http:') and not table[i][fileColumnIdx].startswith('https:'):
+                table[i][fileColumnIdx] = dbPath + '/' + table[i][fileColumnIdx]
 
         self.outputs.table.set(table)
 
         return 1
```

### Comparing `pycinema-2.0.0/pycinema/filters/CinemaDatabaseWriter.py` & `pycinema-3.0.0/pycinema/filters/CinemaDatabaseWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         file.close()
 
     def _update(self):
 
         images = self.inputs.images.get()
         path = self.inputs.path.get()
+        path = os.path.expanduser(path)
 
         if len(images)<1 or len(path)<1:
             return 1
 
         # check if path is a cdb
         filename, extension = os.path.splitext(path)
         extension = str.lower(extension[1:])
```

### Comparing `pycinema-2.0.0/pycinema/filters/DepthCompositing.py` & `pycinema-3.0.0/pycinema/filters/DepthCompositing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pycinema import Filter
 
 import numpy
 import re
+import logging as log
 
 class DepthCompositing(Filter):
 
     def __init__(self):
         super().__init__(
           inputs={
             'images_a': [],
@@ -39,15 +40,15 @@
         elif type(data) == list:
             return data
         return [data]
 
     def getKeys(self,image,compose):
         if compose[0]==None:
             return image.meta.keys()
-        ignore = [compose[0]] + ['id','file']
+        ignore = [compose[0]] + ['^id','^file']
         return [p for p in image.meta.keys() if not any([re.search(i, p, re.IGNORECASE) for i in ignore])]
 
     def getTupleKey(self,image,keys):
         meta_keys = [self.toList(image.meta[m]) for m in keys]
         return tuple(sum(meta_keys, []))
 
     def makeSet(self,data):
@@ -111,15 +112,15 @@
         imagesA = self.inputs.images_a.get()
         imagesB = self.inputs.images_b.get()
 
         results = []
 
         nImages = len(imagesA)
         if len(imagesB)>0 and nImages!=len(imagesB):
-          print('ERROR', 'Input image lists must be of equal size.' )
+          log.error("Input image lists must be of equal size.")
           self.outputs.images.set(results)
           return 0
 
         depthChannel = self.inputs.depth_channel.get()
 
         if len(imagesA)==len(imagesB):
             for i in range(0,nImages):
```

### Comparing `pycinema-2.0.0/pycinema/filters/ImageAnnotation.py` & `pycinema-3.0.0/pycinema/filters/ImageAnnotation.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ImageBorder.py` & `pycinema-3.0.0/pycinema/filters/ImageBorder.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ImageCanny.py` & `pycinema-3.0.0/pycinema/filters/ImageCanny.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ImageConvertGrayscale.py` & `pycinema-3.0.0/pycinema/filters/ImageConvertGrayscale.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ImageFilterPIL.py` & `pycinema-3.0.0/pycinema/filters/ImageFilterPIL.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pycinema import Filter
 
 import PIL
 from PIL import ImageFilter
 import numpy
+import logging as log
 
 class ImageFilterPIL(Filter):
 
     def __init__(self):
         super().__init__(
           inputs={
             'filter': 'BLUR', 
@@ -40,16 +41,16 @@
         elif filterType == 'SMOOTH': 
             imFilter = ImageFilter.SMOOTH
         elif filterType == 'SMOOTH_MORE': 
             imFilter = ImageFilter.SMOOTH_MORE
         elif filterType == 'BLUR': 
             imFilter = ImageFilter.BLUR
         else:
-            print("FILTER NOT FOUND " + filterType)
-            print("  applying default filter ...")
+            log.warning(" Filter not found: '" + filterType + "'")
+            log.warning(" applying default filter ...")
 
         for image in self.inputs.images.get():
             rgbImage = PIL.Image.fromarray(image.channels['rgba'])
             filtered = rgbImage.filter(imFilter)
 
             outImage = image.copy()
             outImage.channels['rgba'] = numpy.array(filtered)
```

### Comparing `pycinema-2.0.0/pycinema/filters/ImageReader.py` & `pycinema-3.0.0/pycinema/filters/ImageReader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from pycinema import Filter, Image
+from pycinema import Filter, Image, isURL
 
 import PIL
 import numpy
 import h5py
 import os
 import re
+import requests
+import logging as log
 
 from pycinema import getTableExtent
 
 class ImageReader(Filter):
 
     def __init__(self):
         self.cache = {}
@@ -31,16 +33,16 @@
         if tableExtent[0]<1 or tableExtent[1]<1:
             return self.outputs.images.set([])
 
         fileColumn = self.inputs.file_column.get()
 
         try:
             fileColumnIdx = [i for i, item in enumerate(table[0]) if re.search(fileColumn, item, re.IGNORECASE)].pop()
-        except ValueError as e:
-            print("table does not contain '" + fileColumn + "' column!")
+        except Exception as e:
+            log.error("table does not contain '" + fileColumn + "' column!")
             return 0
 
         images = [];
         cache = self.inputs.cache.get()
 
         for i in range(1, len(table)):
             row = table[i]
@@ -59,24 +61,28 @@
                 file = h5py.File(path, 'r')
                 for (g,v) in [('channels',image.channels), ('meta',image.meta)]:
                     group = file.get(g)
                     if group==None:
                         raise ValueError('h5 file not formatted correctly')
                     for k in group.keys():
                         data = numpy.array(group.get(k))
-                        # print('xxx',data)
                         if data.dtype == '|S10' and len(data)==1:
                             data = data[0].decode('UTF-8')
                         # elif len(data)==1:
                         #     data = data[0]
                         v[k] = data
                 file.close()
 
             elif str.lower(extension) in ['png','jpg','jpeg']:
-                rawImage = PIL.Image.open(path)
+                if isURL(path):
+                    log.debug("requesting " + path)
+                    rawImage = PIL.Image.open(requests.get(path, stream=True).raw)
+                else:
+                    rawImage = PIL.Image.open(path)
+
                 if rawImage.mode == 'RGB':
                     rawImage = rawImage.convert('RGBA')
                 image = Image({ 'rgba': numpy.asarray(rawImage) })
 
             else:
                 raise ValueError('Unable to read image: '+path)
```

### Comparing `pycinema-2.0.0/pycinema/filters/MaskCompositing.py` & `pycinema-3.0.0/pycinema/filters/MaskCompositing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pycinema import Filter
 import numpy
+import logging as log
 
 class MaskCompositing(Filter):
 
     def __init__(self):
         super().__init__(
           inputs={
             'images_a': [],
@@ -38,15 +39,15 @@
 
         for i in range(0,nImages):
             A = imagesA[min(i,len(imagesA)-1)]
             B = imagesB[min(i,len(imagesB)-1)]
             M = masks[min(i,len(masks)-1)]
 
             if type(A) is tuple and type(B) is tuple:
-                print('ERROR', 'Unable to composit just two color inputs')
+                log.error(' Unable to composite just two color inputs')
                 return 0
 
             result = None
 
             Ac = None
             Bc = None
             Mc = M.channels[maskChannel]
```

### Comparing `pycinema-2.0.0/pycinema/filters/Shader.py` & `pycinema-3.0.0/pycinema/filters/Shader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pycinema import Filter
 
 import numpy
 import moderngl
 import re
+import logging as log
 
 class Shader(Filter):
 
     ctx = None
     quad = None
     fbo = None
 
@@ -106,8 +107,8 @@
                     -1.0,  1.0,
                     -1.0, -1.0,
                      1.0, -1.0,
                      1.0,  1.0
                 ]).astype('f4').tobytes()
             )
 except:
-    print("WARNING: Unable to setup OpenGL context.")
+    log.warn("Unable to setup OpenGL context.")
```

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderDemoScene.py` & `pycinema-3.0.0/pycinema/filters/ShaderDemoScene.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderFXAA.py` & `pycinema-3.0.0/pycinema/filters/ShaderFXAA.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderIBS.py` & `pycinema-3.0.0/pycinema/filters/ShaderIBS.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderLineAO.py` & `pycinema-3.0.0/pycinema/filters/ShaderLineAO.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderPBR.py` & `pycinema-3.0.0/pycinema/filters/ShaderPBR.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderPhong.py` & `pycinema-3.0.0/pycinema/filters/ShaderPhong.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderPointAO.py` & `pycinema-3.0.0/pycinema/filters/ShaderPointAO.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/ShaderSSAO.py` & `pycinema-3.0.0/pycinema/filters/ShaderSSAO.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/TableEditor.py` & `pycinema-3.0.0/pycinema/filters/TableEditor.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/filters/TableQuery.py` & `pycinema-3.0.0/pycinema/filters/TableQuery.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,100 @@
 from pycinema import Filter, isNumber
 
 import sqlite3
 
 from pycinema import getTableExtent
+import logging as log
+
+def executeSQL(db,sql):
+  try:
+    c = db.cursor()
+    c.execute(sql)
+  except sqlite3.Error as e:
+    log.error(" sqlite3 error: " + e)
+
+def createTable(db, table, castType=False):
+  sql = 'CREATE TABLE input(id INTEGER PRIMARY KEY AUTOINCREMENT';
+  header = table[0]
+  firstRow = table[1]
+
+  if castType:
+    for i in range(0,len(header)):
+      if header[i].lower()=='id':
+        continue
+      if isNumber(firstRow[i]):
+          sql += ', "' + header[i] + '" REAL';
+      else:
+          sql += ', "' + header[i] + '" TEXT';
+  else:
+    for i in range(0,len(header)):
+      if header[i].lower()=='id':
+        continue
+      sql = sql + ', "' + header[i] + '" TEXT';
+
+  sql =  sql + ')';
+  executeSQL(db,sql)
+
+def insertData(db, table):
+  sql = 'INSERT INTO input(';
+  for x in table[0]:
+    sql = sql+ '"' + x + '", ';
+  sql = sql[0:-2] + ') VALUES\n';
+
+  for i in range(1, len(table)):
+    row = '('
+    for v in table[i]:
+      row += '"' + str(v) + '",'
+    sql += row[0:-1] + '),\n'
+  sql = sql[0:-2];
+  executeSQL(db,sql)
+
+def queryData(db, sqlQuery):
+  c = db.cursor()
+  try:
+    c.execute(sqlQuery)
+  except sqlite3.Error as er:
+    log.error(' %s' % (' '.join(er.args)))
+    return [[]]
+  res = c.fetchall()
+  columns = []
+  for d in c.description:
+    columns.append(d[0])
+  res.insert(0,columns)
+  return res
 
 class TableQuery(Filter):
 
     def __init__(self):
         super().__init__(
           inputs={
             'table': [[]],
             'sql': 'SELECT * FROM input'
           },
           outputs={
             'table': [[]]
           }
         )
 
-    def executeSQL(self,db,sql):
-        try:
-            c = db.cursor()
-            c.execute(sql)
-        except sqlite3.Error as e:
-            print(e)
-
-    def createTable(self, db, table):
-        sql = 'CREATE TABLE input(id INTEGER PRIMARY KEY AUTOINCREMENT';
-
-        header = table[0]
-        firstRow = table[1]
-
-        for i in range(0,len(header)):
-            if header[i].lower()=='id':
-                continue
-            if isNumber(firstRow[i]):
-                sql += ', ' + header[i] + ' REAL';
-            else:
-                sql += ', ' + header[i] + ' TEXT';
-        sql =  sql + ')';
-        self.executeSQL(db,sql)
-
-    def insertData(self, db, table):
-        sql = 'INSERT INTO input(';
-        for x in table[0]:
-            sql = sql + x + ', ';
-        sql = sql[0:-2] + ') VALUES\n';
-
-        for i in range(1, len(table)):
-            row = '('
-            for v in table[i]:
-              row += '"' + str(v) + '",'
-            sql += row[0:-1] + '),\n'
-        sql = sql[0:-2];
-        self.executeSQL(db,sql)
-
-    def queryData(self, db, sqlQuery):
-        c = db.cursor()
-        try:
-            c.execute(sqlQuery)
-        except sqlite3.Error as er:
-            print('[SQL ERROR] %s' % (' '.join(er.args)))
-            return [[]]
-        res = c.fetchall()
-        columns = []
-        for d in c.description:
-          columns.append(d[0])
-        res.insert(0,columns)
-        return res
-
     def _update(self):
 
       db = sqlite3.connect(":memory:")
 
       table = self.inputs.table.get()
       tableExtent = getTableExtent(table)
       if tableExtent[0]<2 or tableExtent[1]<1:
           return self.outputs.table.set([[]])
 
-      self.createTable(db, table)
-      self.insertData(db, table)
+      createTable(db, table, True)
+      insertData(db, table)
 
       sql = self.inputs.sql.get()
       if isinstance(sql, dict):
         header = table[0]
         sql2 = {k: v for k, v in sql.items() if k in header}
         sql = 'SELECT * FROM input WHERE '+ ' AND '.join(sql2.values())
 
-      output = self.queryData(db, sql)
+      output = queryData(db, sql)
 
       self.outputs.table.set(output)
 
       return 1;
```

### Comparing `pycinema-2.0.0/pycinema/filters/TableWriter.py` & `pycinema-3.0.0/pycinema/filters/TableWriter.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,17 @@
             write = csv.writer(csvfile)
             write.writerows(self.inputs.table.get())
 
 
     def _update(self):
 
         path = self.inputs.path.get()
+        path = os.path.expanduser(path)
 
-        # get path components 
+        # get path components
         directory, filename = os.path.split(path)
 
         # ensure folder exists
         if not directory == '':
             if not os.path.exists(directory):
                 os.makedirs(directory)
```

### Comparing `pycinema-2.0.0/pycinema/filters/__init__.py` & `pycinema-3.0.0/pycinema/filters/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,42 @@
+from .Calculator import *
 from .CinemaDatabaseReader import *
 from .CinemaDatabaseWriter import *
 from .ColorMapping import *
 from .ColorSource import *
+from .CSVReader import *
 from .TableQuery import *
 from .TableEditor import *
 from .DepthCompositing import *
 from .ImageAnnotation import *
 from .ImageBorder import *
 from .ImageCanny import *
 from .ImageConvertGrayscale import *
 from .ImageFilterPIL import *
 from .ImageReader import *
+from .ImageSort import *
+from .ImagesToTable import *
+from .ImageView import *
 from .MaskCompositing import *
+from .MLTFReader import *
+from .MLTFPredictor import *
+from .Plot import *
+from .PlotLineItem import *
+from .Python import *
+from .GetColumn import *
 from .ShaderDemoScene import *
 from .ShaderFXAA import *
 from .ShaderIBS import *
 from .ShaderPBR import *
 from .ShaderPhong import *
 from .Shader import *
 from .ShaderSSAO import *
 from .ShaderLineAO import *
 from .ShaderPointAO import *
+from .SqliteDatabaseReader import *
 from .TableWriter import *
+from .TableView import *
+from .TextEditor import *
+from .ParametersView import *
+from .ParallelCoordinates import *
+from .InspectorView import *
+from .ValueSource import *
```

### Comparing `pycinema-2.0.0/pycinema/ipy/CinemaDatabaseViewer.py` & `pycinema-3.0.0/pycinema/ipy/CinemaDatabaseViewer.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/ipy/ColorMappingWidgets.py` & `pycinema-3.0.0/pycinema/ipy/ColorMappingWidgets.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/ipy/ImageViewer.py` & `pycinema-3.0.0/pycinema/ipy/ImageViewer.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/ipy/NumberWidget.py` & `pycinema-3.0.0/pycinema/ipy/NumberWidget.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/ipy/ParameterWidgets.py` & `pycinema-3.0.0/pycinema/ipy/ParameterWidgets.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/theater/FilterBrowser.py` & `pycinema-3.0.0/pycinema/theater/FilterBrowser.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def keyReleaseEvent(self,event):
         super().keyReleaseEvent(event)
         if event.key()==QtCore.Qt.Key_Return:
             self.s_return.emit()
 
 class FilterBrowser(QtWidgets.QDialog):
 
-    filters = dict([(name, cls) for name, cls in pycinema.filters.__dict__.items() if isinstance(cls,type) and issubclass(cls,pycinema.Core.Filter)])
+    filters = dict([(name, cls) for name, cls in pycinema.filters.__dict__.items() if isinstance(cls,type) and issubclass(cls,pycinema.Core.Filter) and len(cls.__subclasses__())<1])
 
     def __init__(self):
         super().__init__()
 
         self.setLayout(QtWidgets.QVBoxLayout())
 
         self.query = QueryWidget()
```

### Comparing `pycinema-2.0.0/pycinema/theater/View.py` & `pycinema-3.0.0/pycinema/theater/View.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,22 @@
 
 class View(QtWidgets.QFrame):
 
     s_close = QtCore.Signal(QtWidgets.QFrame, name='close')
     s_splitH = QtCore.Signal(QtWidgets.QFrame,name='splitH')
     s_splitV = QtCore.Signal(QtWidgets.QFrame,name='splitV')
 
+    id_counter = 0
+
     def __init__(self, content_layout='V'):
         super().__init__()
 
+        self.id = 'view'+str(View.id_counter)
+        View.id_counter += 1
+
         self.setLayout(QtWidgets.QVBoxLayout())
         self.layout().setContentsMargins(4,2,4,0)
 
         # toolbar
         self.toolbar = QtWidgets.QToolBar()
         self.layout().addWidget(self.toolbar)
 
@@ -53,19 +58,19 @@
         elif content_layout == 'H':
             self.content.setLayout(QtWidgets.QHBoxLayout())
         elif content_layout == 'G':
             self.content.setLayout(QtWidgets.QGridLayout())
 
         self.layout().addWidget(self.content,1)
 
-    # def __del__(self):
-    #   print('del VIEW')
-
     def emitClose(self):
       self.s_close.emit(self)
     def emitSplitH(self):
       self.s_splitH.emit(self)
     def emitSplitV(self):
       self.s_splitV.emit(self)
 
     def setTitle(self,text):
         self.title.setText(text)
+
+    def export(self):
+      return self.id + ' = pycinema.theater.views.'+self.__class__.__name__+'()\n'
```

### Comparing `pycinema-2.0.0/pycinema/theater/ViewFrame.py` & `pycinema-3.0.0/pycinema/theater/SplitFrame.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from PySide6 import QtCore, QtWidgets, QtGui
 
 from pycinema.theater.View import View
 from pycinema.theater.ViewStyle import ViewStyle
-from pycinema.theater.views import SelectionView
-from pycinema.theater.views import FilterView
-from pycinema.theater.views import NodeEditorView
+from pycinema.theater.views import SelectionView, FilterView
+import pycinema.theater.TabFrame
 from pycinema import Filter
 
-class ViewFrame(QtWidgets.QSplitter):
+class SplitFrame(QtWidgets.QSplitter):
 
   id_counter = 0
 
-  def __init__(self, orientation=QtCore.Qt.Horizontal,root=False):
+  def __init__(self, orientation=QtCore.Qt.Horizontal):
       super().__init__()
-      self.root = root
       self.setChildrenCollapsible(False)
       self.setStyleSheet(ViewStyle.get_style_sheet())
-      self.id = 'vf'+str(ViewFrame.id_counter)
-      ViewFrame.id_counter += 1
+      self.id = 'splitFrame'+str(SplitFrame.id_counter)
+      SplitFrame.id_counter += 1
       self.setOrientation(orientation)
 
   def setVerticalOrientation(self):
       self.setOrientation(QtCore.Qt.Vertical)
 
   def setHorizontalOrientation(self):
       self.setOrientation(QtCore.Qt.Horizontal)
@@ -33,36 +31,37 @@
 
   def disconnectView(self,view):
       view.s_close.disconnect(self.s_close)
       view.s_splitH.disconnect(self.s_splitH)
       view.s_splitV.disconnect(self.s_splitV)
 
   def insertFrame(self,idx):
-      frame = ViewFrame()
+      frame = SplitFrame()
       self.insertWidget(idx, frame)
       return frame
 
   def insertView(self,idx,view):
-      self.connectView(view)
+      if isinstance(view,Filter):
+        view = FilterView(view)
+
+      if isinstance(view,View):
+        self.connectView(view)
+
       self.insertWidget(idx, view)
       return view
 
   def s_close(self, widget):
     idx = self.indexOf(widget)
     widget.setParent(None)
-    # if isinstance(widget, ViewFrame):
-    #   widget.deleteLater()
-    # else:
-    #   self.disconnectView(widget)
 
     if self.count()<1:
-      if self.root:
-        self.insertView(0, SelectionView())
-      else:
+      if isinstance(self.parent(),SplitFrame):
         self.parent().s_close(self)
+      else:
+        self.insertView(0, SelectionView())
 
   def split(self,view,orientation):
     idx = self.indexOf(view)
 
     width = view.width()
     height = view.height()
 
@@ -88,15 +87,15 @@
     else:
       for i in range(0,self.count()):
         v = self.widget(i)
         widths.append(v.width())
         heights.append(v.height())
 
       self.disconnectView(view)
-      newFrame = ViewFrame(orientation=orientation)
+      newFrame = SplitFrame(orientation=orientation)
       newFrame.insertView(0,view)
       newFrame.insertView(1,SelectionView())
       if orientation==QtCore.Qt.Horizontal:
         newFrame.setSizes([width/2,width/2])
       else:
         newFrame.setSizes([height/2,height/2])
 
@@ -109,45 +108,30 @@
 
   def s_splitH(self,view):
     self.split(view,QtCore.Qt.Horizontal)
 
   def s_splitV(self,view):
     self.split(view,QtCore.Qt.Vertical)
 
-  def replaceView(self,view,cls):
-    # print(view,cls)
-    idx = self.indexOf(view)
+  def replaceView(self,oldView,newView):
+    idx = self.indexOf(oldView)
     sizes = self.sizes()
-
-    self.disconnectView(view)
-    view.setParent(None)
-
-    newView = cls()
+    self.disconnectView(oldView)
+    oldView.setParent(None)
     self.insertView(idx,newView)
-
     self.setSizes(sizes)
 
-    if issubclass(cls,Filter) and issubclass(cls,FilterView):
-      return newView.filter
-    else:
-      return newView
-
   def export(self):
-    r = ''
+    r = self.id + ' = pycinema.theater.SplitFrame()\n'
     if self.orientation()==QtCore.Qt.Vertical:
-      r = self.id + '.setVerticalOrientation()\n'
+      r += self.id + '.setVerticalOrientation()\n'
     else:
-      r = self.id + '.setHorizontalOrientation()\n'
+      r += self.id + '.setHorizontalOrientation()\n'
 
     for i in range(0,self.count()):
       w = self.widget(i)
-      if isinstance(w,ViewFrame):
-        r += w.id + ' = ' + self.id + '.insertFrame('+str(i)+')\n'
-        r += w.export()
-      elif isinstance(w,Filter):
-        r += w.id + ' = ' + self.id+'.insertView( '+str(i)+', pycinema.theater.views.'+w.__class__.__name__+'() )\n'
-      else:
-        r += self.id+'.insertView( '+str(i)+', pycinema.theater.views.'+w.__class__.__name__+'() )\n'
+      r += w.export()
+      r += self.id+'.insertView( '+str(i)+', '+w.id+' )\n'
 
     r += self.id + '.setSizes('+str(self.sizes())+')\n'
     return r
```

### Comparing `pycinema-2.0.0/pycinema/theater/node_editor/Edge.py` & `pycinema-3.0.0/pycinema/theater/node_editor/Edge.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/theater/node_editor/InputText.py` & `pycinema-3.0.0/pycinema/theater/node_editor/InputText.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/theater/node_editor/Node.py` & `pycinema-3.0.0/pycinema/theater/node_editor/Node.py`

 * *Files 25% similar despite different names*

```diff
@@ -80,19 +80,35 @@
           NES.NODE_WIDTH,
           NES.NODE_PORT_Y + (len(self.inputPorts)+len(self.outputPorts))*NES.NODE_PORT_SPACE - 10
         )
 
     def paint(self, painter, options, widget):
 
         br = self.boundingRect()
-        br2 = QtCore.QRect(br.x(),br.y(),br.width(),NES.NODE_HEADER_HEIGHT)
+
+        corner_radius = 5
+        corner_radius2 = corner_radius*2
+
         path = QtGui.QPainterPath()
-        path.addRect(br2)
+        path.moveTo(br.x(),br.y()+NES.NODE_HEADER_HEIGHT);
+        path.lineTo(br.x()+br.width(),br.y()+NES.NODE_HEADER_HEIGHT);
+        path.lineTo(br.x()+br.width(),br.y()+corner_radius);
+        path.arcTo(br.x()+br.width()-corner_radius2,br.y(), corner_radius2, corner_radius2, 0.0, 90.0);
+        path.lineTo(br.x()+corner_radius,br.y());
+        path.arcTo(br.x(),br.y(), corner_radius2, corner_radius2, 90.0, 90.0);
+        path.lineTo(br.x(),br.y()+corner_radius);
+
         if self.isSelected():
             painter.fillPath(path,QtGui.QBrush(NES.COLOR_RED_T))
         else:
             painter.fillPath(path,QtGui.QBrush(NES.COLOR_BLUE_T))
 
-        br2 = QtCore.QRect(br.x(),br.y()+NES.NODE_HEADER_HEIGHT,br.width(),br.height()-NES.NODE_HEADER_HEIGHT)
         path = QtGui.QPainterPath()
-        path.addRect(br2)
+
+        path.moveTo(br.x(),br.y()+NES.NODE_HEADER_HEIGHT);
+        path.lineTo(br.x(),br.y()+br.height()-corner_radius);
+        path.arcTo(br.x(),br.y()+br.height()-corner_radius2,corner_radius2,corner_radius2,180,90);
+        path.lineTo(br.x()+br.width()-corner_radius,br.y()+br.height());
+        path.arcTo(br.x()+br.width()-corner_radius2,br.y()+br.height()-corner_radius2,corner_radius2,corner_radius2,270,90);
+        path.lineTo(br.x()+br.width(),br.y()+NES.NODE_HEADER_HEIGHT);
+
         painter.fillPath(path,QtGui.QBrush(NES.COLOR_BASE_T))
```

### Comparing `pycinema-2.0.0/pycinema/theater/node_editor/NodeEditorStyle.py` & `pycinema-3.0.0/pycinema/theater/node_editor/NodeEditorStyle.py`

 * *Files identical despite different names*

### Comparing `pycinema-2.0.0/pycinema/theater/node_editor/Port.py` & `pycinema-3.0.0/pycinema/theater/node_editor/Port.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,20 @@
 
         self.setCursor(QtCore.Qt.PointingHandCursor)
         self.setZValue(1000)
         self.setAcceptHoverEvents(True)
         self.setPen(QtCore.Qt.NoPen)
 
         self.representation = QtWidgets.QGraphicsEllipseItem(self)
-        # self.setPen(QtGui.QPen(NES.COLOR_NORMAL, 0))
-        # self.setBrush(NES.COLOR_NORMAL)
         self.representation.setPen(QtCore.Qt.NoPen)
         self.representation.setBrush(NES.COLOR_NORMAL)
 
     def setRect(self,rect):
-        super().setRect(rect.adjusted(-10,-10,10,10))
         self.representation.setRect(rect)
-        # return super().setRect(rect)
+        return super().setRect(rect.adjusted(-10,-10,10,10))
 
     def hoverEnterEvent(self,event):
         self.representation.setBrush(NES.COLOR_BLUE)
     def hoverLeaveEvent(self,event):
         self.representation.setBrush(NES.COLOR_NORMAL)
 
     def mousePressEvent(self,event):
@@ -37,16 +34,28 @@
         line.setP2(pos)
         ncl.setLine(line)
         ncl.show()
 
     def mouseMoveEvent(self,event):
         ncl = self.scene().node_connection_line
         line = ncl.line()
-        line.setP2( self.mapToScene(event.pos()) )
-        ncl.setLine(line)
+
+        s = self.parentItem().port
+        t = None
+        items = self.scene().items(event.scenePos());
+        for i in items:
+            if isinstance(i,Port):
+                t = i
+                break
+        if not t or s.is_input == t.port.is_input or s.parent==t.port.parent:
+          line.setP2( self.mapToScene(event.pos()) )
+          ncl.setLine(line)
+        else:
+          line.setP2( t.disc.mapToScene(t.disc.boundingRect().center()) )
+          ncl.setLine(line)
 
     def mouseReleaseEvent(self,event):
         ncl = self.scene().node_connection_line
         ncl.hide()
 
         s = self.parentItem().port
         t = None
@@ -55,25 +64,41 @@
             if isinstance(i,Port):
                 t = i.port
                 break
         if not t or s.is_input == t.is_input or s.parent==t.parent:
             return
         if t.is_input:
             s,t = t,s
-        s.set( t )
+        if event.modifiers() == QtCore.Qt.ShiftModifier:
+            if s.valueIsPortList():
+                ports = [p for p in s._value]
+                ports.append(t)
+                s.set( ports )
+            elif s.valueIsPort():
+                s.set( [s._value,t] )
+            else:
+                s.set( t )
+        else:
+            s.set( t )
 
     def mouseDoubleClickEvent(self,event):
-        self.parentItem().port.set(self.parentItem().port.default)
+        if self.parentItem().port.is_input:
+          self.parentItem().port.set(self.parentItem().port.default)
 
-class WidgetFrame(QtWidgets.QGraphicsRectItem):
-    def __init__(self, width, height, parent=None):
+class InputTextGraphicsItem(QtWidgets.QGraphicsItem):
+    def __init__(self, port, width, parent=None):
         super().__init__(parent)
-        self.width = width
-        self.height = height
-        self.setRect(QtCore.QRect(0,0,self.width,self.height))
+
+        self.widget_ = InputText(port, width)
+        self.widget = QtWidgets.QGraphicsProxyWidget(self)
+        self.widget.setWidget(self.widget_)
+        self.widget.setZValue(NES.Z_NODE_LAYER+2)
+
+    def boundingRect(self):
+        return self.widget.boundingRect()
 
     def paint(self, painter, option, widget):
         br = self.boundingRect()
         path = QtGui.QPainterPath()
         path.addRoundedRect(br,3,3)
         painter.fillPath(path,QtGui.QBrush(NES.COLOR_WIDGET_T))
 
@@ -81,39 +106,44 @@
 class Port(QtWidgets.QGraphicsItem):
 
     def __init__(self,parent,port):
         super().__init__(parent)
         self.port = port
 
         parentBR = parent.boundingRect()
+        widget_width = parentBR.width()-2*(NES.PORT_SIZE)
 
-        self.widget_ = InputText(port, parentBR.width()-2*(NES.PORT_SIZE))
+        self.widget_ = InputText(port, widget_width)
         self.widget = QtWidgets.QGraphicsProxyWidget(self)
         self.widget.setWidget(self.widget_)
-
         self.widget.setZValue(NES.Z_NODE_LAYER+2)
-        portLabelBR = self.widget.boundingRect()
+
+        widget_br = self.widget.boundingRect()
+        self.widget.setZValue(NES.Z_NODE_LAYER+1)
         if port.is_input:
           self.widget.setPos(
             NES.PORT_SIZE,
-            -portLabelBR.height()/2-1
+            -widget_br.height()/2-1
           )
         else:
           self.widget.setPos(
-            -NES.PORT_SIZE-portLabelBR.width(),
-            -portLabelBR.height()/2-1
+            -NES.PORT_SIZE-widget_br.width(),
+            -widget_br.height()/2-1
           )
 
-        self.widgetFrame = WidgetFrame(portLabelBR.width(), portLabelBR.height(), self)
-        self.widgetFrame.setZValue(NES.Z_NODE_LAYER+1)
-        self.widgetFrame.setPos(self.widget.pos())
-
         self.disc = PortDisc(self)
         self.disc.setRect(
           QtCore.QRect(-NES.PORT_SIZE/2,-NES.PORT_SIZE/2,NES.PORT_SIZE,NES.PORT_SIZE)
         )
 
     def boundingRect(self):
-        return self.widget.boundingRect().united(self.disc.boundingRect())
+        br = self.widget.boundingRect()
+        br.moveTo(self.widget.pos())
+        return br.united(self.disc.boundingRect())
 
     def paint(self, painter, option, widget):
+        br = self.widget.boundingRect()
+        br.moveTo(self.widget.pos())
+        path = QtGui.QPainterPath()
+        path.addRoundedRect(br,3,3)
+        painter.fillPath(path,QtGui.QBrush(NES.COLOR_WIDGET_T))
         return
```

### Comparing `pycinema-2.0.0/pycinema/theater/views/NodeEditorView.py` & `pycinema-3.0.0/pycinema/theater/views/NodeEditorView.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from PySide6 import QtCore, QtWidgets, QtGui
 
 import pycinema
 import pycinema.filters
+import logging as log
 
 from pycinema.theater.View import View
 from pycinema.theater.FilterBrowser import FilterBrowser
 
 use_pgv = True
 try:
     import pygraphviz as pgv
@@ -43,18 +44,18 @@
         self.setResizeAnchor(QtWidgets.QGraphicsView.AnchorUnderMouse)
         self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
         self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
         l = 10000
         self.setSceneRect(-l,-l,2*l,2*l)
 
         if not QtNodeEditorView.scene:
-          QtNodeEditorView.init_gobal()
+          QtNodeEditorView.init_global()
         self.setScene(QtNodeEditorView.scene)
 
-    def init_gobal():
+    def init_global():
         node_connection_line = QtWidgets.QGraphicsLineItem()
         node_connection_line.setPen(QtGui.QPen(NES.COLOR_NORMAL, 2, QtCore.Qt.SolidLine, QtCore.Qt.RoundCap, QtCore.Qt.RoundJoin))
         node_connection_line.setZValue(1000)
         node_connection_line.hide()
 
         QtNodeEditorView.scene = QtWidgets.QGraphicsScene()
         QtNodeEditorView.scene.addItem(node_connection_line)
@@ -101,39 +102,36 @@
         node.delete()
         QtNodeEditorView.computeLayout()
 
     def autoConnect(node_a,node_b,force=False):
         if not node_a or not node_b or (not force and not QtNodeEditorView.auto_connect):
             return
 
-        node_a_ports = node_a.filter.outputs.ports()
-        node_b_ports = node_b.filter.inputs.ports()
+        o_ports = [p for n,p in node_a.filter.outputs.ports()]
+        i_ports = [p for n,p in node_b.filter.inputs.ports()]
+        if len(o_ports)<1 or len(i_ports)<1:
+            return
+
+        matches = [(o, i) for o in o_ports for i in i_ports if o.name == i.name]
 
-        if len(node_b_ports)==1:
-          for o_portName, o_port in node_a_ports:
-              for i_portName, i_port in node_b_ports:
-                  bridge_ports = list(o_port.connections)
-                  i_port.set(o_port)
-                  for bridge_port in bridge_ports:
-                      if bridge_port.parent==node_b.filter: continue
-                      for o_portName_, o_port_ in node_b.filter.outputs.ports():
-                          if bridge_port.name == o_portName_:
-                              bridge_port.set(o_port_)
-                  return
-
-        for o_portName, o_port in node_a_ports:
-            for i_portName, i_port in node_b_ports:
-                if o_portName==i_portName:
-                    bridge_ports = list(o_port.connections)
-                    i_port.set(o_port)
-                    for bridge_port in bridge_ports:
-                        if bridge_port.parent==node_b.filter: continue
-                        for o_portName_, o_port_ in node_b.filter.outputs.ports():
-                            if bridge_port.name == o_portName_:
-                                bridge_port.set(o_port_)
+        if len(matches)<1:
+            free_i_ports = [i for i in i_ports if not isinstance(i._value, pycinema.Port)]
+            if len(free_i_ports)>0:
+                matches = [(o_ports[0],free_i_ports[0])]
+            else:
+                matches = [(o_ports[0],i_ports[0])]
+
+        for (o,i) in matches:
+            bridge_ports = list(o.connections)
+            i.set(o)
+            for b in bridge_ports:
+                if b.parent==node_b.filter: continue
+                for _, o2 in node_b.filter.outputs.ports():
+                    if b.name == o2.name:
+                        b.set(o2)
 
     def fitInView(self):
         rect = QtCore.QRectF(QtNodeEditorView.scene.itemsBoundingRect())
         if rect.isNull():
             return
 
         self.resetTransform()
@@ -269,14 +267,15 @@
                 filter = filters[key]
                 node_ = G.get_node(str(filter.id))
                 pos = [float(x) for x in node_.attr['pos'].split(',')]
                 node = QtNodeEditorView.node_map[filter]
                 node.target = QtCore.QPointF(pos[0],-pos[1])
         else:
             g = igraph.Graph(directed=True)
+
             vertices = [f for f in filters]
             g.add_vertices( [f.id for f in vertices] )
 
             edges = {}
             pycinema.Filter.computeDAG(edges)
             L = pycinema.Filter.computeTopologicalOrdering(edges)
 
@@ -291,15 +290,15 @@
             g.add_edges(edges_)
 
             layout = g.layout_reingold_tilford(mode="out")
             scale = 250
             for i, f in enumerate(vertices):
                 node = QtNodeEditorView.node_map[f]
                 coords = layout[i]
-                QtNodeEditorView.node_map[f].target = QtCore.QPointF(coords[1]*scale,coords[0]*scale*0.7)
+                QtNodeEditorView.node_map[f].target = QtCore.QPointF(coords[1]*scale,-coords[0]*scale*0.7)
 
             for f in L:
                 if not f in edgesR:
                     continue
                 previous_filters = edgesR[f]
                 max_x = -900000000
                 for pf in previous_filters:
```

### Comparing `pycinema-2.0.0/pycinema/theater/views/ParallelCoordinatesView.py` & `pycinema-3.0.0/pycinema/filters/ParallelCoordinates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,520 +1,525 @@
-from PySide6 import QtCore, QtWidgets, QtGui
-
 import sqlite3
 import re
+from copy import deepcopy
 
-from pycinema.theater.views.FilterView import FilterView
-from pycinema import Filter, getTableExtent, isNumber
-
-def executeSQL(db,sql):
-  try:
-    c = db.cursor()
-    c.execute(sql)
-  except sqlite3.Error as e:
-    print(e)
-
-def createTable(db, table):
-  sql = 'CREATE TABLE input(id INTEGER PRIMARY KEY AUTOINCREMENT';
-  header = table[0]
-  firstRow = table[1]
-  for i in range(0,len(header)):
-    if header[i].lower()=='id':
-      continue
-    sql = sql + ', ' + header[i] + ' TEXT';
-  sql =  sql + ')';
-  executeSQL(db,sql)
-
-def insertData(db, table):
-  sql = 'INSERT INTO input(';
-  for x in table[0]:
-    sql = sql + x + ', ';
-  sql = sql[0:-2] + ') VALUES\n';
-
-  for i in range(1, len(table)):
-    row = '('
-    for v in table[i]:
-      row += '"' + str(v) + '",'
-    sql += row[0:-1] + '),\n'
-  sql = sql[0:-2];
-  executeSQL(db,sql)
-
-def queryData(db, sqlQuery):
-  c = db.cursor()
-  try:
-    c.execute(sqlQuery)
-  except sqlite3.Error as er:
-    print('[SQL ERROR] %s' % (' '.join(er.args)))
-    return [[]]
-  res = c.fetchall()
-  columns = []
-  for d in c.description:
-    columns.append(d[0])
-  res.insert(0,columns)
-  return res
-
-def createLabel(parent,text):
-  _label = QtWidgets.QLabel(str(text))
-  font = QtGui.QFont()
-  font.setPointSize(10)
-  _label.setFont(font)
-
-  palette = QtCore.QCoreApplication.instance().palette()
-  color = 'color: '+palette.text().color().name()+';background:transparent;';
-  _label.setStyleSheet(color);
-  label = QtWidgets.QGraphicsProxyWidget(parent)
-  label._color = color;
-  label.setWidget(_label)
-  return label
-
-def computeValues(header,table):
-  values = []
-  for (p,idx) in header:
-    v_dic = set()
-
-    for j in range(1,len(table)):
-      v_dic.add(table[j][idx])
-
-    v_list = list(v_dic)
-    isListOfNumbers = isNumber(table[1][idx])
-    if isListOfNumbers:
-      v_list = [(float(x),x) for x in v_list]
-    v_list.sort()
-    if isListOfNumbers:
-      v_list = [x[1] for x in v_list]
+from pycinema.filters.ParametersView import computeValues
 
-    values.append(v_list)
+from pycinema import Filter, getTableExtent, getColumnIndexFromTable, isNumber
+from pycinema.filters.TableQuery import executeSQL, createTable, insertData, queryData
 
-  return values
-
-class Lines(QtWidgets.QGraphicsItem):
-  def __init__(self):
-    super().__init__()
-    self.br = QtCore.QRectF(0,0,0,0)
+try:
+  from PySide6 import QtGui, QtCore, QtWidgets
+except ImportError:
+  pass
+
+try:
+  def createLabel(parent,text):
+    _label = QtWidgets.QLabel(str(text))
+    font = QtGui.QFont()
+    font.setPointSize(10)
+    _label.setFont(font)
 
     palette = QtCore.QCoreApplication.instance().palette()
+    _label._style = 'color: '+palette.text().color().name()+';background:transparent;'
+    _label.setStyleSheet(_label._style);
+    label = QtWidgets.QGraphicsProxyWidget(parent)
+    label.setWidget(_label)
 
-    # determine theme
-    dark_theme = base_color = QtCore.QCoreApplication.instance().palette().base().color().red()<100
-    if dark_theme:
-      self.pen_line_normal = QtGui.QPen(QtGui.QColor("#555"))
-      self.pen_line_highlight = QtGui.QPen(QtGui.QColor("#fff"))
-    else:
-      self.pen_line_normal = QtGui.QPen(QtGui.QColor("#eee"))
-      self.pen_line_highlight = QtGui.QPen(QtGui.QColor("#333"))
-
-    self.pen_line_highlight.setWidth(2)
+    return label
 
-    self.lines_normal = []
-    self.lines_highlight = []
+  class Lines(QtWidgets.QGraphicsItem):
+    def __init__(self):
+      super().__init__()
+      self.br = QtCore.QRectF(0,0,0,0)
 
-    self.path_normal = QtGui.QPainterPath()
-    self.path_highlight = QtGui.QPainterPath()
+      palette = QtCore.QCoreApplication.instance().palette()
 
-  def setBoundingRect(self,br):
-    self.prepareGeometryChange()
-    self.br = br
+      # determine theme
+      dark_theme = base_color = QtCore.QCoreApplication.instance().palette().base().color().red()<100
+      if dark_theme:
+        self.pen_line_normal = QtGui.QPen(QtGui.QColor("#555"))
+        self.pen_line_highlight = QtGui.QPen(QtGui.QColor("#fff"))
+      else:
+        self.pen_line_normal = QtGui.QPen(QtGui.QColor("#eee"))
+        self.pen_line_highlight = QtGui.QPen(QtGui.QColor("#333"))
+
+      self.pen_line_highlight.setWidth(2)
+
+      self.lines_normal = []
+      self.lines_highlight = []
+
+      self.path_normal = QtGui.QPainterPath()
+      self.path_highlight = QtGui.QPainterPath()
+
+    def setBoundingRect(self,br):
+      self.prepareGeometryChange()
+      self.br = br
+
+      if len(self.lines_normal)<1: return
+
+      n2 = len(self.lines_normal[0])
+      n = n2-1
+
+      x0 = self.br.x()
+      y0 = self.br.y()
+      w = self.br.width()
+      h = self.br.height()
+
+      interpolate = lambda l,q,q0: q0+l*q
+
+      self.path_normal = QtGui.QPainterPath()
+      self.path_highlight = QtGui.QPainterPath()
+
+      for (lines,path) in [(self.lines_normal,self.path_normal),(self.lines_highlight,self.path_highlight)]:
+        for line in lines:
+          path.moveTo( interpolate(line[0],w,x0), interpolate(line[1],h,y0) )
+          path.lineTo( interpolate(line[2],w,x0), interpolate(line[3],h,y0) )
+
+    def boundingRect(self):
+      return self.br
+
+    def paint(self, painter, option, widget):
+      painter.setPen(self.pen_line_normal)
+      painter.drawPath(self.path_normal)
+      painter.setPen(self.pen_line_highlight)
+      painter.drawPath(self.path_highlight)
+
+  class Axis(QtWidgets.QGraphicsItem):
+
+    def __init__(self, parameter, filter):
+      super().__init__()
+
+      self.br = QtCore.QRectF(0,0,0,0)
+
+      self.parameter = parameter
+      self.filter = filter
+      self.values = deepcopy(filter.model[parameter])
+      self.n_values = len(self.values)
+      self.compose = False
+      self.selection_idx0 = 0
+      self.selection_idx1 = 0
+      self.mouse_state = -1
+
+      # label
+      self.label = createLabel(self,parameter)
+      self.label.setPos(-self.label.boundingRect().width()/2,0)
+      self.label.widget().setCursor(QtCore.Qt.PointingHandCursor)
+
+      # pens
+      palette = QtCore.QCoreApplication.instance().palette()
+      self.pen_grid = QtGui.QPen(palette.light().color())
+
+      # main line
+      self.line = QtWidgets.QGraphicsLineItem(
+        0, -100, 0, 100,
+        self
+      )
+      self.line.setPen(self.pen_grid)
 
-    if len(self.lines_normal)<1: return
+      # ticks
+      self.ticks = []
+      n = len(self.values)
+      if n==1:
+        self.addTick(0.5,self.values[0])
+      else:
+        d = 1/(n-1)
+        skip_d = 1 if n<20 else round(n/20)
+        self.addTick(0,self.values[0])
+        self.addTick(1,self.values[-1])
+
+        i = d
+        for t in range(1,n):
+          if t%skip_d==0:
+            self.addTick(i,self.values[t])
+          i += d
+
+      # highlight bar
+      self.bar = QtWidgets.QGraphicsRectItem(0,0,0,0,self)
+
+      dark_theme = base_color = QtCore.QCoreApplication.instance().palette().base().color().red()<100
+      if dark_theme:
+        bar_c = QtGui.QColor('#fff')
+      else:
+        bar_c = QtGui.QColor('#333')
+
+      self.bar.setBrush(bar_c)
+      bar_pen = QtGui.QPen(bar_c)
+      bar_pen.setWidth(3)
+      self.bar.setPen(bar_pen)
+      self.bar.setCursor(QtCore.Qt.PointingHandCursor)
+      self.bar.hide()
+
+    def snapToValueIdx(self,y):
+      l = (y - self.y0) / (self.y1 - self.y0)
+      l = max(min(l,1),0)
+      return round(l*(self.n_values-1))
+
+    def mousePressEvent(self,event):
+      y = event.pos().y()
+      if y<self.y0:
+        self.mouse_state = 0
+      else:
+        self.mouse_state = 1
+        idx = self.snapToValueIdx(y)
+        self.selection_idx0 = idx
+        self.selection_idx1 = idx
+        self.bar.show()
+        self.updateBar()
+
+    def mouseMoveEvent(self,event):
+      if self.mouse_state != 1: return
+      idx = self.snapToValueIdx(event.pos().y())
+      if idx!=self.selection_idx1:
+        self.selection_idx1 = idx
+        self.updateBar()
+
+    def mouseReleaseEvent(self,event):
+      if self.mouse_state == 0:
+        self.compose = not self.compose
+        if self.compose:
+          self.filter.inputs.compose.set(self.parameter)
+        else:
+          self.filter.inputs.compose.set(None)
+      else:
+        self.bar.hide()
+        self.updateSelection(event.modifiers() == QtCore.Qt.ShiftModifier)
+      self.mouse_state = -1
+
+    def updateSelection(self,grow=False):
+      if grow:
+        parameters = self.filter.computeParameterValues()
+      else:
+        parameters = {}
+      indices = sorted([self.selection_idx0, self.selection_idx1])
+      parameters[self.parameter] = {self.values[s] for s in range(indices[0],indices[1]+1)}
+      sql = 'SELECT `id` ' + self.filter.computeSQL(parameters)
+      table = queryData(self.filter.db, sql)
+      self.filter.inputs.selection.set(
+        [table[i][0]-1 for i in range(1,len(table))],
+        True,
+        True
+      )
 
-    n2 = len(self.lines_normal[0])
-    n = n2-1
+    def addTick(self, l, text):
+      tick_line = QtWidgets.QGraphicsLineItem(0,0,0,0,self)
+      tick_line.l = l
+      tick_line.setPen(self.pen_grid)
+      tick_label = createLabel(self,text)
+      self.ticks.append((tick_line,tick_label))
+
+    def updateBar(self):
+      if self.selection_idx0 < self.selection_idx1:
+        idx0, idx1 = self.selection_idx0, self.selection_idx1
+      else:
+        idx1, idx0 = self.selection_idx0, self.selection_idx1
+      barMargin = 0.25/self.n_values
+      if self.n_values>1:
+        l0 = max(0,idx0/(self.n_values-1)-barMargin)
+        l1 = min(1,idx1/(self.n_values-1)+barMargin)
+      else:
+        l0 = 0.45
+        l1 = 0.55
+      hy0 = (1-l0)*self.y0 + l0*self.y1
+      hy1 = (1-l1)*self.y0 + l1*self.y1
+      self.bar.setRect( -1, hy0, 2, hy1-hy0 )
+
+    def _resize(self,  x, y, height, axis_width):
+      self.prepareGeometryChange()
+
+      self.br = QtCore.QRectF(-axis_width/2,y,axis_width,height)
+
+      self.setPos(x,0)
+      self.label.setPos(self.label.pos().x(),y+5)
+
+      self.y0 = y+30
+      self.y1 = y+height-10
+
+      self.line.setLine(0,self.y0,0,self.y1)
+
+      for (tick_line,tick_label) in self.ticks:
+        y = (1-tick_line.l)*self.y0 + tick_line.l*self.y1
+        tick_line.setLine(-5,y,5,y)
+        lb = tick_label.boundingRect()
+        tick_label.setPos(-10-lb.width(),y-lb.height()/2)
+
+    def boundingRect(self):
+      return self.br
+
+    def paint(self, painter, option, widget):
+      return
+
+  class _ParallelCoordinates(QtWidgets.QGraphicsView):
+
+    def __init__(self,filter):
+      super().__init__()
+      self.filter = filter
+
+      self.setRenderHints(QtGui.QPainter.Antialiasing)
+      self.setDragMode(QtWidgets.QGraphicsView.DragMode.NoDrag)
+      self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+      self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+
+      self.axes = {}
+      self.lines = Lines()
+
+      scene = QtWidgets.QGraphicsScene(self)
+      scene.addItem(self.lines)
+      self.setScene(scene)
+
+    def removeAxes(self):
+      for a in self.axes:
+        axis = self.axes[a]
+        self.scene().removeItem(axis)
+      self.axes = {}
+
+    def addAxes(self):
+      model = self.filter.model
+      for p in model:
+        axis = Axis(p,self.filter)
+        self.axes[p] = axis
+        self.scene().addItem(axis)
+
+    def updatePlot(self):
+
+      self.removeAxes()
+      self.removeLines()
+
+      self.addAxes()
+      self.addBackgroundLines()
+      self._resize()
+
+    def addHighlightedLines(self):
+      selection = self.filter.inputs.selection.get()
+      table = self.filter.inputs.table.get()
+      model = self.filter.model
+      parameters = [p for p in model]
+      n = len(parameters) - 1
+      if n<1: return
 
-    x0 = self.br.x()
-    y0 = self.br.y()
-    w = self.br.width()
-    h = self.br.height()
+      dx = 1/n
+      x = 0
 
-    interpolate = lambda l,q,q0: q0+l*q
+      lines = []
+      edges = set()
+      for i in range(0,len(parameters)-1):
+        p0 = parameters[i]
+        p1 = parameters[i+1]
+        c0 = table[0].index(p0)
+        c1 = table[0].index(p1)
+        s0 = self.axes[p0].values
+        s1 = self.axes[p1].values
+        n0 = len(s0)-1
+        n1 = len(s1)-1
+
+        for r in selection:
+          edge = (str(table[r+1][c0]),str(table[r+1][c1]))
+          if not edge in edges:
+            lines.append([
+                  i*dx, s0.index(edge[0])/n0 if n0>0 else 0.5,
+              (i+1)*dx, s1.index(edge[1])/n1 if n1>0 else 0.5
+            ])
+            edges.add(edge)
+
+      self.lines.lines_highlight = lines
+      self._resize()
+
+    def removeLines(self):
+      self.lines.lines_highlight = []
+      self.lines.path_highlight = QtGui.QPainterPath()
+      self.lines.lines_normal = []
+      self.lines.path_normal = QtGui.QPainterPath()
 
-    self.path_normal = QtGui.QPainterPath()
-    self.path_highlight = QtGui.QPainterPath()
+    def addBackgroundLines(self):
 
-    for (lines,path) in [(self.lines_normal,self.path_normal),(self.lines_highlight,self.path_highlight)]:
-      for line in lines:
-        path.moveTo( x0, interpolate(line[0][1],h,y0) )
-        for i in range(1,n2):
-          path.lineTo( interpolate(line[i][0],w,x0), interpolate(line[i][1],h,y0) )
+      lines = self.lines.lines_normal
+      model = self.filter.model
+      table = self.filter.inputs.table.get()
 
-  def boundingRect(self):
-    return self.br
+      parameters = [p for p in model]
+      n = len(parameters) - 1
+      if n<1: return
 
-  def paint(self, painter, option, widget):
-    painter.setPen(self.pen_line_normal)
-    painter.drawPath(self.path_normal)
-    painter.setPen(self.pen_line_highlight)
-    painter.drawPath(self.path_highlight)
+      dx = 1/n
+      x = 0
 
-class Axis(QtWidgets.QGraphicsItem):
+      n_rows = len(table)
+      for i in range(0,len(parameters)-1):
+        p0 = parameters[i]
+        p1 = parameters[i+1]
+        c0 = table[0].index(p0)
+        c1 = table[0].index(p1)
+        s0 = self.axes[p0].values
+        s1 = self.axes[p1].values
+        n0 = len(s0)-1
+        n1 = len(s1)-1
+
+        edges = set()
+        for r in range(1,n_rows):
+          edge = (str(table[r][c0]),str(table[r][c1]))
+          if not edge in edges:
+            lines.append([
+                  i*dx, s0.index(edge[0])/n0 if n0>0 else 0.5,
+              (i+1)*dx, s1.index(edge[1])/n1 if n1>0 else 0.5
+            ])
+            edges.add(edge)
+
+    def scrollContentsBy(self,a,b):
+      return
+    def wheelEvent(self, event):
+      return
+    def fitInView(self):
+      return
+    def keyPressEvent(self,event):
+      return
+
+    def _resize(self):
+
+      model = self.filter.model
+      parameters = [p for p in model]
+      n = len(parameters)
+      if n<1: return
+
+      view_rect = self.mapToScene(self.rect()).boundingRect()
+
+      margin = 50
+      w = view_rect.width()-2*margin
+      if n>1:
+        x = view_rect.x()+margin
+        aw = w/(n-1)
+      else:
+        x = view_rect.x() + view_rect.width()/2
+        aw = w
+      y = view_rect.y()
+      h = view_rect.height()
+
+      for p in parameters:
+        axis = self.axes[p]
+        axis._resize(x,y,h,aw)
+        x+=aw
+
+      a0 = self.axes[parameters[0]]
+      a1 = self.axes[parameters[n-1]]
+      x0 = a0.pos().x()
+      x1 = a1.pos().x()
+      y0 = a0.y0
+      y1 = a0.y1
+      self.lines.setBoundingRect(QtCore.QRectF(x0,y0,x1-x0,y1-y0))
+
+    def resizeEvent(self, event):
+      super().resizeEvent(event)
+      self._resize()
 
-  def __init__(self, parameter, values, emitter):
-    super().__init__()
+except NameError:
+  pass
 
-    self.br = QtCore.QRectF(0,0,0,0)
+class ParallelCoordinates(Filter):
 
-    self.emitter = emitter
+  def __init__(self):
 
-    self.parameter = parameter
-    self.values = values
-    self.n_values = len(values)
-    self.selection_idx0 = 0
-    self.selection_idx1 = 0
-    self.compose = False
-    self.mouse_state = -1
+    self.model = {}
+    self.widgets = []
 
-    # label
-    self.label = createLabel(self,parameter)
-    self.label.setPos(-self.label.boundingRect().width()/2,0)
-    self.label.widget().setCursor(QtCore.Qt.PointingHandCursor)
+    self.db = None
 
-    # pens
-    palette = QtCore.QCoreApplication.instance().palette()
-    self.pen_grid = QtGui.QPen(palette.mid().color())
-
-    # main line
-    self.line = QtWidgets.QGraphicsLineItem(
-      0, -100, 0, 100,
-      self
+    self.inputTimes = [-1,-1]
+    Filter.__init__(
+      self,
+      inputs={
+        'table': [[]],
+        'ignore': ['^file','^id'],
+        'selection': [],
+        'compose': ''
+      },
+      outputs={
+        'table': [[]],
+        'sql': '',
+        'compose': (None,{})
+      }
     )
-    self.line.setPen(self.pen_grid)
-
-    # ticks
-    self.ticks = []
-    if len(self.values)==1:
-      self.addTick(0.5,self.values[0])
-    elif type(self.values[0])==str or len(self.values)<6:
-      i = 0
-      d = 1/(len(self.values)-1)
-      for t in self.values:
-        self.addTick(i,t)
-        i += d
-    else:
-      return print('ERROR: unsupported axis type')
-
-    # highlight bar
-    self.bar = QtWidgets.QGraphicsRectItem(0,0,0,0,self)
-
-    dark_theme = base_color = QtCore.QCoreApplication.instance().palette().base().color().red()<100
-    if dark_theme:
-      bar_c = QtGui.QColor('#fff')
-    else:
-      bar_c = QtGui.QColor('#333')
-
-    self.bar.setBrush(bar_c)
-    bar_pen = QtGui.QPen(bar_c)
-    bar_pen.setWidth(3)
-    self.bar.setPen(bar_pen)
-    self.bar.setCursor(QtCore.Qt.PointingHandCursor)
-
-  def snapToValueIdx(self,y):
-    l = (y - self.y0) / (self.y1 - self.y0)
-    l = max(min(l,1),0)
-    return round(l*(self.n_values-1))
-
-  def mousePressEvent(self,event):
-    y = event.pos().y()
-    if y<self.y0:
-      self.mouse_state = 0
-    else:
-      self.mouse_state = 1
-      idx = self.snapToValueIdx(y)
-      self.selection_idx0 = idx
-      self.selection_idx1 = idx
-      self.emitter.s_selection_changed_intermediate.emit()
-
-  def mouseMoveEvent(self,event):
-    if self.mouse_state != 1: return
-    idx = self.snapToValueIdx(event.pos().y())
-    if idx!=self.selection_idx1:
-      self.selection_idx1 = idx
-      self.emitter.s_selection_changed_intermediate.emit()
-
-  def mouseReleaseEvent(self,event):
-    if self.mouse_state == 0:
-      self.compose = not self.compose
-    self.mouse_state = -1
-    self.emitter.s_selection_changed.emit()
-
-  def addTick(self, l, text):
-    tick_line = QtWidgets.QGraphicsLineItem(0,0,0,0,self)
-    tick_line.l = l
-    tick_line.setPen(self.pen_grid)
-
-    tick_label = createLabel(self,text)
-    self.ticks.append((tick_line,tick_label))
-
-  def update(self, x, y, height, axis_width):
-    self.prepareGeometryChange()
-
-    self.br = QtCore.QRectF(-axis_width/2,y,axis_width,height)
-
-    self.setPos(x,0)
-    self.label.setPos(self.label.pos().x(),y+5)
-
-    self.y0 = y+30
-    self.y1 = y+height-10
-
-    self.line.setLine(0,self.y0,0,self.y1)
-
-    for (tick_line,tick_label) in self.ticks:
-      y = (1-tick_line.l)*self.y0 + tick_line.l*self.y1
-      tick_line.setLine(-5,y,5,y)
-      lb = tick_label.boundingRect()
-      tick_label.setPos(-10-lb.width(),y-lb.height()/2)
-
-    if self.selection_idx1 < self.selection_idx0:
-      idx0, idx1 = self.selection_idx1, self.selection_idx0
-    else:
-      idx0, idx1 = self.selection_idx0, self.selection_idx1
-
-    idx0 = max(0,idx0-0.1)
-    idx1 = min(self.n_values-1,idx1+0.1)
-
-    l0 = 0
-    l1 = 0
-    if self.n_values>1:
-      l0 = idx0/(self.n_values-1)
-      l1 = idx1/(self.n_values-1)
-
-    hy0 = (1-l0)*self.y0 + l0*self.y1
-    hy1 = (1-l1)*self.y0 + l1*self.y1
-
-    self.bar.setRect( -1, hy0, 2, hy1-hy0 )
 
-    if self.compose:
-      self.label.widget().setStyleSheet('font-weight: bold;'+self.label._color)
-    else:
-      self.label.widget().setStyleSheet('font-weight: normal;'+self.label._color)
-
-  def boundingRect(self):
-    return self.br
-
-  def paint(self, painter, option, widget):
-    return
-
-  def toSQL(self):
-    if self.selection_idx1 < self.selection_idx0:
-      idx0, idx1 = self.selection_idx1, self.selection_idx0
-    else:
-      idx0, idx1 = self.selection_idx0, self.selection_idx1
-
-    v = []
-    for i in range(idx0,idx1+1):
-      v.append(self.values[i])
-    v = tuple(v)
+  def computeParameterValues(self):
+    selection = self.inputs.selection.get()
+    table = self.inputs.table.get()
+    parameters = {}
+    for p in self.model:
+      ci = table[0].index(p)
+      values = {table[s+1][ci] for s in selection}
+      if len(values)>0:
+        parameters[p] = values
+    return parameters
+
+  def computeSQL(self,parameters):
+    sql = 'FROM `input` WHERE '
+    for p in parameters:
+      sql += '`' + p + '` IN ("'+ '","'.join([str(v) for v in parameters[p]]) +'") AND  '
+    return sql[:-6]
+
+  def generateWidgets(self):
+    widget = _ParallelCoordinates(self)
+    widget.updatePlot()
+    self.widgets.append(widget)
+    return widget
+
+  def _update(self):
+    table = self.inputs.table.get()
+    tableExtent = getTableExtent(table)
+    if tableExtent[0]<1 or tableExtent[1]<1:
+      self.outputs.table.set([[]])
+      self.outputs.sql.set('')
+      return 0
+
+    inputTimes = [self.inputs.table.getTime(),self.inputs.ignore.get()]
+    if self.inputTimes!=inputTimes:
+      self.inputTimes = inputTimes
+      ignore = self.inputs.ignore.get()
+      parameterIndices = [idx for idx in range(0,tableExtent[1]) if not any([re.search(i, table[0][idx], re.IGNORECASE) for i in ignore])]
 
-    if len(v)==1:
-      return '"' + self.parameter + '" IN ("' + str(v[0]) + '")'
+      # repair model
+      new_model = {}
+      for i in parameterIndices:
+        parameter = table[0][i]
+        new_model[parameter] = computeValues(table,i)
+
+      self.model = new_model
+      for w in self.widgets:
+        w.updatePlot()
+
+      self.db = sqlite3.connect(":memory:")
+      createTable(self.db, table)
+      insertData(self.db, table)
+
+    for w in self.widgets:
+      w.addHighlightedLines()
+
+    parameters = self.computeParameterValues()
+    if len(parameters)<1:
+      sql = 'SELECT * FROM `input` LIMIT 0'
     else:
-      return '"' + self.parameter + '" IN ' + str(v)
+      sql = 'SELECT * ' + self.computeSQL(parameters)
+    self.outputs.sql.set(sql)
 
-class SelectionEmitter(QtCore.QObject):
-  s_selection_changed = QtCore.Signal(name='s_selection_changed')
-  s_selection_changed_intermediate = QtCore.Signal(name='s_selection_changed_intermediate')
-
-  def __init__(self):
-    super().__init__()
-
-class _ParallelCoordinatesView(QtWidgets.QGraphicsView):
-
-  def __init__(self):
-    super().__init__()
-    self.axes = {}
-    self.lines = Lines()
-    self.emitter = SelectionEmitter()
-    self.emitter.s_selection_changed_intermediate.connect(self.resize)
-
-    self.header = []
-
-    self.setRenderHints(QtGui.QPainter.Antialiasing)
-    self.setDragMode(QtWidgets.QGraphicsView.DragMode.NoDrag)
-    self.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-    self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
-
-    self._scene = QtWidgets.QGraphicsScene(self)
-    self._scene.addItem(self.lines)
-    self.setScene(self._scene)
-
-  def removeAxes(self):
-    for a in self.axes:
-      axis = self.axes[a]
-      self._scene.removeItem(axis)
-    self.axes = {}
-    self.header = {}
-
-  def addAxes(self,header,values):
-    self.header = header
-
-    for i, (p,idx) in enumerate(self.header):
-      axis = Axis(p,values[i],self.emitter)
-      self.axes[p] = axis
-      self._scene.addItem(axis)
-
-  def removeLines(self):
-    self.lines.lines_normal = []
-    self.lines.lines_highlight = []
-    self.lines.path_normal = QtGui.QPainterPath()
-    self.lines.path_highlight = QtGui.QPainterPath()
-
-  def addLines(self, header, values, table, highlight=False):
-    n = len(header) - 1
-    if n<1: return
-
-    if highlight:
-      lines = self.lines.lines_highlight
-    else:
-      lines = self.lines.lines_normal
+    output_table = queryData(self.db, sql)
+    self.outputs.table.set(output_table)
 
-    dx = 1/n
-    for row_idx in range(1,len(table)):
-      path = []
-      x = 0
-      for header_idx, (p,column_idx) in enumerate(header):
-        v = values[header_idx]
-        vn = len(v) - 1
-        if vn < 1:
-          path.append( (x,0.5) )
+    # compositing output
+    compose = self.inputs.compose.get()
+    for w in self.widgets:
+      for a in w.axes:
+        w.axes[a].compose = a==compose
+        aw = w.axes[a].label.widget()
+        if w.axes[a].compose:
+          aw.setStyleSheet(aw._style+'font-weight:bold;')
         else:
-          path.append( (x,v.index(table[row_idx][column_idx])/vn) )
-        x += dx
+          aw.setStyleSheet(aw._style+'font-weight:normal;')
 
-      lines.append(path)
-
-  def scrollContentsBy(self,a,b):
-    return
-  def wheelEvent(self, event):
-    return
-  def fitInView(self):
-    return
-  def keyPressEvent(self,event):
-    return
-
-  def resizeEvent(self, event):
-    super().resizeEvent(event)
-    self.resize()
-
-  def resize(self):
-    n = len(self.header)
-    if n<1: return
-
-    view_rect = self.mapToScene(self.rect()).boundingRect()
-
-    margin = 50
-    w = view_rect.width()-2*margin
-    if n>1:
-      x = view_rect.x()+margin
-      aw = w/(n-1)
+    if compose != '':
+      idx = getColumnIndexFromTable(output_table,compose)
+      values = set()
+      for i in range(1,len(output_table)):
+        values.add(output_table[i][idx])
+      compose = (compose, {v:i for i,v in enumerate(values)})
     else:
-      x = view_rect.x() + view_rect.width()/2
-      aw = w
-    y = view_rect.y()
-    h = view_rect.height()
-
-    for (a,idx) in self.header:
-      axis = self.axes[a]
-      axis.update(x,y,h,aw)
-      x+=aw
-
-    a0 = self.axes[self.header[0][0]]
-    a1 = self.axes[self.header[n-1][0]]
-    x0 = a0.pos().x()
-    x1 = a1.pos().x()
-    y0 = a0.y0
-    y1 = a0.y1
-    self.lines.setBoundingRect(QtCore.QRectF(x0,y0,x1-x0,y1-y0))
-
-  def applyState(self,state):
-    for axis_name in state:
-      axis = self.axes[axis_name]
-      s = state[axis_name]
-      axis.selection_idx0 = s[0]
-      axis.selection_idx1 = s[1]
-      axis.compose = s[2]
-
-class ParallelCoordinatesView(Filter, FilterView):
-
-    def __init__(self):
-      FilterView.__init__(
-        self,
-        filter=self,
-        delete_filter_on_close = True
-      )
-
-      Filter.__init__(
-        self,
-        inputs={
-          'table': [[]],
-          'ignore': ['^file','^id'],
-          'state': {}
-        },
-        outputs={
-          'table': [[]],
-          'sql': 'SELECT * FROM input',
-          'compose': (None,{})
-        }
-      )
-
-    def generateWidgets(self):
-      self.pcp = _ParallelCoordinatesView()
-      self.content.layout().addWidget(self.pcp,1)
-      self.pcp.emitter.s_selection_changed.connect(self.updateState)
-
-    def updateState(self):
-      state = {}
-      for axis_name in self.pcp.axes:
-        axis = self.pcp.axes[axis_name]
-        if axis.selection_idx0 < axis.selection_idx1:
-          idx0, idx1 = axis.selection_idx0, axis.selection_idx1
-        else:
-          idx1, idx0 = axis.selection_idx0, axis.selection_idx1
-        state[axis_name] = (idx0,idx1,axis.compose)
-      self.inputs.state.set(state)
-
-    def _update(self):
-      table = self.inputs.table.get()
-      tableExtent = getTableExtent(table)
-      self.pcp.removeAxes()
-      self.pcp.removeLines()
-      self.pcp.resize()
-      if tableExtent[0]<2 or tableExtent[1]<1:
-        self.outputs.table.set([[]])
-        self.outputs.sql.set('SELECT * FROM input')
-        return 1
-
-      ignore = self.inputs.ignore.get()
-      header = [(p,idx) for idx,p in enumerate(table[0]) if not any([re.search(i, p, re.IGNORECASE) for i in ignore])]
-      header.sort()
-      values = computeValues(header,table)
-
-      self.pcp.addAxes(header,values)
-      self.pcp.addLines(header,values,table)
-      self.pcp.applyState(self.inputs.state.get())
-
       compose = (None,{})
-      sql = 'SELECT * FROM input WHERE '
-      for axis_name in self.pcp.axes:
-        axis = self.pcp.axes[axis_name]
-        axis_sql = axis.toSQL()
-        if len(axis_sql)>0:
-          sql += axis_sql+ ' AND '
-        if axis.compose:
-          valueMap = {}
-          for i,v in enumerate(axis.values):
-            valueMap[v] = i
-          compose = (axis_name,valueMap)
-      sql += ' '
-      sql = sql[:-6]
-
-      db = sqlite3.connect(":memory:")
-      createTable(db, table)
-      insertData(db, table)
-      output_table = queryData(db, sql)
-
-      header2 = [(p,output_table[0].index(p)) for (p,idx) in header]
-      self.pcp.addLines( header2, values, output_table, True )
-
-      self.pcp.resize()
-      self.outputs.table.set(output_table)
-      self.outputs.sql.set(sql)
-      self.outputs.compose.set(compose)
+    self.outputs.compose.set(compose)
 
-      return 1
+    return 1
```

### Comparing `pycinema-2.0.0/pycinema/theater/views/ParameterView.py` & `pycinema-3.0.0/pycinema/filters/ParametersView.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,282 +1,243 @@
+from copy import deepcopy
+import re
+import sqlite3
+
 from pycinema import isNumber, Filter, getTableExtent
-from pycinema.theater.views.FilterView import FilterView
+from pycinema.filters.TableQuery import executeSQL, createTable, insertData, queryData
+
+try:
+  from PySide6 import QtGui, QtCore, QtWidgets
+  from pycinema.theater.Icons import Icons
+except Exception:
+  pass
+
+try:
+  class Emitter(QtCore.QObject):
+    s_update = QtCore.Signal()
+    def __init__(self):
+      super().__init__()
+except NameError:
+  class Emitter():
+    def __init__(self):
+      pass
 
-from PySide6 import QtCore, QtWidgets
+def computeValues(table,idx):
+  vdic = set()
 
-import re
+  for j in range(1,len(table)):
+      vdic.add(table[j][idx])
 
-# ==============================================================================
-# SQL
-# ==============================================================================
-import sqlite3
-def executeSQL(db,sql):
-  try:
-    c = db.cursor()
-    c.execute(sql)
-  except sqlite3.Error as e:
-    print(e)
-
-def createTable(db, table):
-  sql = 'CREATE TABLE input(id INTEGER PRIMARY KEY AUTOINCREMENT';
-  header = table[0]
-  firstRow = table[1]
-  for i in range(0,len(header)):
-    if header[i].lower()=='id':
-      continue
-    sql = sql + ', ' + header[i] + ' TEXT';
-  sql =  sql + ')';
-  executeSQL(db,sql)
-
-def insertData(db, table):
-  sql = 'INSERT INTO input(';
-  for x in table[0]:
-    sql = sql + x + ', ';
-  sql = sql[0:-2] + ') VALUES\n';
-
-  for i in range(1, len(table)):
-    row = '('
-    for v in table[i]:
-      row += '"' + str(v) + '",'
-    sql += row[0:-1] + '),\n'
-  sql = sql[0:-2];
-  executeSQL(db,sql)
-
-def queryData(db, sqlQuery):
-  c = db.cursor()
-  try:
-    c.execute(sqlQuery)
-  except sqlite3.Error as er:
-    print('[SQL ERROR] %s' % (' '.join(er.args)))
-    return [[]]
-  res = c.fetchall()
-  columns = []
-  for d in c.description:
-    columns.append(d[0])
-  res.insert(0,columns)
-  return res
+  v_list = list(vdic)
+  isListOfNumbers = isNumber(table[1][idx])
+  if isListOfNumbers:
+    v_list = [(float(x),x) for x in v_list]
+  v_list.sort()
+  if isListOfNumbers:
+    v_list = [str(x[1]) for x in v_list]
+
+  return v_list
 
 # ==============================================================================
-# ParameterView
+# ParametersView
 # ==============================================================================
-class ParameterView(Filter, FilterView):
+class ParametersView(Filter):
 
     def __init__(self):
-
-        FilterView.__init__(
-          self,
-          filter=self,
-          delete_filter_on_close = True
-        )
-
+        self.emitter = Emitter()
         Filter.__init__(
           self,
           inputs={
             'table': [[]],
             'ignore': ['^file','^id'],
             'state': {}
           },
           outputs={
             'table': [[]],
             'sql': 'SELECT * FROM input',
             'compose': (None,{})
           }
         )
 
-    def generateWidgets(self):
-        self.widgets = QtWidgets.QFrame()
-        l = QtWidgets.QGridLayout()
-        l.setAlignment(QtCore.Qt.AlignTop)
-        l.setSpacing(0)
-        l.setContentsMargins(0,0,0,0)
-        self.widgets.setLayout(l)
-        self.content.layout().addWidget(self.widgets)
-
-        self.widgetsDict = {}
-
-    def widgetToSQL(self, wt):
-        v = None
-        t = wt['T'].currentText()
-        if t == 'S':
-            v = wt['values'][wt['S'].value()]
-        elif t == 'O':
-            v = wt['O'].selectedItems()
-
-        if type(v) is list:
-            v = ['"'+i.text()+'"' for i in v]
-            return '"' + wt['parameter'] + '" IN (' + ','.join(v) + ')'
-        else:
-            return '"' + wt['parameter'] + '"="' + v + '"'
-
-    def computeValues(self,table,idx):
-        vdic = set()
-
-        for j in range(1,len(table)):
-            vdic.add(table[j][idx])
-
-        v_list = list(vdic)
-        isListOfNumbers = isNumber(table[1][idx])
-        if isListOfNumbers:
-          v_list = [(float(x),x) for x in v_list]
-        v_list.sort()
-        if isListOfNumbers:
-          v_list = [x[1] for x in v_list]
-
-        return v_list
-
-    def addWidgetToLayout(self, wt, grid_layout, grid_idx):
-        wt['grid_idx'] = grid_idx
-        grid_layout.addWidget(wt['C'],grid_idx,0,QtCore.Qt.AlignTop)
-        grid_layout.addWidget(wt['T'],grid_idx,1,QtCore.Qt.AlignTop)
-        grid_layout.addWidget(wt['SF'],grid_idx,2,QtCore.Qt.AlignTop)
-        grid_layout.addWidget(wt['O'],grid_idx,2,QtCore.Qt.AlignTop)
-
-    def generateWidget(self,parameter, table, idx, states):
-
-        def on_change(name):
-          self.update()
-
-        def on_slider_change(name):
-          wt = self.widgetsDict[name]
-          wt['SL'].setText(wt['values'][wt['S'].value()])
-          self.update()
-
-        def on_type_change(name):
-          wt = self.widgetsDict[name]
-
-          t = wt['T'].currentText()
-          if t == 'S':
-              wt['SL'].setVisible(True)
-              wt['O'].setVisible(False)
-          elif t == 'O':
-              wt['SL'].setVisible(False)
-              wt['O'].setVisible(True)
-          self.update()
-
-        def make_callback(name,func):
-            return lambda: func(name)
+    def updateWidgets(self,widgets):
+      state = self.inputs.state.get()
 
-        wt = {}
-        wt['parameter'] = parameter
-
-        values = self.computeValues(table,idx)
-        wt['values'] = values
-
-        if parameter in states:
-            state = states[parameter]
+      def update_mode(p,v):
+        if self.ignore: return
+        new_state = deepcopy(self.inputs.state.get())
+        if v:
+          new_state[p]['M'] = 'O'
         else:
-            state = {
-              'C': False,
-              'T': 'S',
-              'S': 0,
-              'O': [0],
-            }
-
-        wt['C'] = QtWidgets.QPushButton(parameter)
-        wt['C'].setCheckable(True)
-        wt['C'].setChecked(state['C'])
-        wt['C'].toggled.connect( make_callback(parameter, on_change ) )
-
-        wt['T'] = QtWidgets.QComboBox()
-        wt['T'].addItems(["S", "O"])
-        wt['T'].setCurrentText(state['T'])
-        wt['T'].currentTextChanged.connect( make_callback(parameter, on_type_change ) )
-
-        wt['S'] = QtWidgets.QSlider(QtCore.Qt.Horizontal)
-        wt['S'].setMinimum(0)
-        wt['S'].setMaximum(len(values)-1)
-        wt['S'].setValue(state['S'])
-        wt['S'].valueChanged.connect( make_callback(parameter, on_slider_change ) )
-
-        wt['SL'] = QtWidgets.QLabel(values[state['S']])
-        wt['SL'].setVisible(state['T']=='S')
-
-        wt['SF'] = QtWidgets.QFrame()
-        wt['SF'].layout = QtWidgets.QHBoxLayout(wt['SF'])
-        wt['SF'].layout.addWidget(wt['S'])
-        wt['SF'].layout.addWidget(wt['SL'])
-
-        wt['O'] = QtWidgets.QListWidget()
-        wt['O'].insertItems(0,values)
-        wt['O'].setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
-        wt['O'].setMaximumHeight(60)
-        wt['O'].setVisible(state['T']=='O')
-        for oidx in state['O']:
-            wt['O'].item(oidx).setSelected(True)
-        wt['O'].itemSelectionChanged.connect( make_callback(parameter, on_change ) )
-
-        return wt
-
-    def updateWidgets(self):
-
-        table = self.inputs.table.get()
-        states = self.inputs.state.get()
-        ignore = self.inputs.ignore.get()
-
-        parameters = [p for p in table[0] if not any([re.search(i, p, re.IGNORECASE) for i in ignore])]
-        parameters.sort()
+          new_state[p]['M'] = 'S'
+          vv = new_state[p]['V']
+          if len(vv):
+            new_state[p]['V'] = [vv[0]]
+          else:
+            new_state[p]['V'] = [new_state[p]['O'][0]]
+
+        self.inputs.state.set(new_state)
+
+
+      def update_compositing(p,v):
+        if self.ignore: return
+        new_state = deepcopy(self.inputs.state.get())
+        new_state[p]['C'] = v
+        self.inputs.state.set(new_state)
+      def update_slider(p,v):
+        if self.ignore: return
+        new_state = deepcopy(self.inputs.state.get())
+        new_state[p]['V'] = [v]
+        self.inputs.state.set(new_state)
+      def update_options(p,o):
+        if self.ignore: return
+        new_state = deepcopy(self.inputs.state.get())
+        new_state[p]['V'] = [o.indexFromItem(i).row() for i in o.selectedItems()]
+        self.inputs.state.set(new_state)
+
+      def make_callback(p,func):
+        return lambda v: func(p,v)
+      def make_callback2(p,o,func):
+        return lambda: func(p,o)
+
+      # check if generation is necessary
+      requires_generation = any([s not in widgets.child_dict for s in state])
+      if requires_generation:
+        widgets.container.setParent(None)
+        widgets.container.deleteLater()
+        widgets.container = QtWidgets.QFrame()
+        widgets.layout().addWidget(widgets.container)
+
+        layout = QtWidgets.QGridLayout()
+        layout.setAlignment(QtCore.Qt.AlignTop)
+        layout.setSpacing(0)
+        layout.setContentsMargins(0,0,0,0)
+        widgets.container.setLayout(layout)
+        widgets.child_dict = {}
+
+        row_idx = 0
+        for p in state:
+          state_ = state[p]
+          l = QtWidgets.QPushButton(p)
+          l.setCheckable(True)
+          l.toggled.connect( make_callback(p,update_compositing) )
+          layout.addWidget(l,row_idx,0,QtCore.Qt.AlignVCenter)
+
+          m = QtWidgets.QPushButton()
+          m.setCheckable(True)
+          m.setIcon( Icons.toQIcon(Icons.icon_list) )
+          m.setCursor(QtCore.Qt.PointingHandCursor)
+          m.setToolTip('Toggle slider/list widget')
+          m.toggled.connect( make_callback(p,update_mode) )
+          layout.addWidget(m,row_idx,1,QtCore.Qt.AlignVCenter)
+
+          s = QtWidgets.QSlider(QtCore.Qt.Horizontal)
+          s.setMinimum(0)
+          s.setMaximum(len(state_['O'])-1)
+          s.valueChanged.connect( make_callback(p,update_slider) )
+
+          v = QtWidgets.QLabel()
+          mwidth = v.fontMetrics().boundingRect('m').width()
+          maxWidth = max(len(str(x)) for x in state_['O'])
+          v.setMinimumWidth(maxWidth*mwidth)
+
+          sv = QtWidgets.QFrame()
+          sv.setLayout(QtWidgets.QHBoxLayout())
+          sv.layout().addWidget(s)
+          sv.layout().addWidget(v)
+          layout.addWidget(sv,row_idx,2,QtCore.Qt.AlignVCenter)
+
+          o = QtWidgets.QListWidget()
+          o.insertItems(0,state_['O'])
+          o.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
+          # o.setMaximumHeight(1.2*mwidth*min(4,len(state_['O'])))
+          layout.addWidget(o,row_idx,2,QtCore.Qt.AlignVCenter)
+          o.itemSelectionChanged.connect( make_callback2(p, o, update_options ) )
+
+          widgets.child_dict[p] = {
+            'l': l,
+            'm': m,
+            's': s,
+            'v': v,
+            'o': o,
+            'sv': sv
+          }
+          row_idx += 1
 
-        existing_parameters = [p for p in self.widgetsDict]
-        existing_parameters.sort()
+      self.ignore = True
+      for p in state:
+        state_ = state[p]
+        child = widgets.child_dict[p]
+
+        child['l'].setChecked(state_['C'])
+        child['m'].setChecked(state_['M']!='S')
+        if len(state_['V']):
+          child['s'].setValue(state_['V'][0])
+        child['v'].setText(state_['O'][state_['V'][0]])
+        child['sv'].setVisible(state_['M']=='S')
+        child['o'].setVisible(state_['M']=='O')
+        child['o'].clearSelection()
+        for x in state_['V']:
+          child['o'].item(x).setSelected(True)
+      self.ignore = False
+      return
 
-        if parameters != existing_parameters and len(existing_parameters)<1:
-          grid_layout = self.widgets.layout()
-          grid_idx = 0
-          for parameter in parameters:
-              idx = table[0].index(parameter)
-              wt = self.generateWidget(parameter,table,idx,states)
-              self.widgetsDict[parameter] = wt
-              self.addWidgetToLayout(wt,grid_layout,grid_idx)
-              grid_idx += 1
+    def generateWidgets(self):
+        widgets = QtWidgets.QFrame()
+        widgets.setLayout(QtWidgets.QHBoxLayout())
+        widgets.container = QtWidgets.QWidget()
+        widgets.layout().addWidget(widgets.container)
+        widgets.child_dict = {}
+
+        self.emitter.s_update.connect(lambda: self.updateWidgets(widgets))
+        self.updateWidgets(widgets)
+        return widgets
 
     def _update(self):
-
         table = self.inputs.table.get()
         tableExtent = getTableExtent(table)
         if tableExtent[0]<1 or tableExtent[1]<1:
+          self.outputs.table.set([[]])
           self.outputs.sql.set('')
           self.outputs.compose.set((None,{}))
           return 0
 
-        # compute widgets
-        self.updateWidgets()
-
-        # export state
-        state = {}
-        for _,wt in self.widgetsDict.items():
-            state[wt['parameter']] = {
-              "C": wt['C'].isChecked(),
-              "T": wt['T'].currentText(),
-              "S": wt['S'].value(),
-              "O": [wt['O'].indexFromItem(i).row() for i in wt['O'].selectedItems()]
+        state = self.inputs.state.get()
+        if not bool(state):
+          state = {}
+          ignore = self.inputs.ignore.get()
+          parameterIndices = [idx for idx in range(0,tableExtent[1]) if not any([re.search(i, table[0][idx], re.IGNORECASE) for i in ignore])]
+          for i in parameterIndices:
+            state[table[0][i]] = {
+              'C': False,
+              'O': computeValues(table,i),
+              'V': [0],
+              'M': 'S'
             }
-        self.inputs.state.set(state, False)
+          self.inputs.state.set(state)
 
+        # sql output
         sql = 'SELECT * FROM input WHERE '
-        for _,wt in self.widgetsDict.items():
-            wsql = self.widgetToSQL(wt)
-            if len(wsql)>0:
-                sql += wsql+ ' AND '
+        for s in state:
+          sql += '"'+s+'" IN ("' +'","'.join([str(state[s]['O'][x]) for x in state[s]['V']])+ '") AND '
 
         sql += ' '
+        sql = sql[:-6]
+        self.outputs.sql.set(sql)
 
-        self.outputs.sql.set(sql[:-6])
-
+        # table output
         db = sqlite3.connect(":memory:")
         createTable(db, table)
         insertData(db, table)
-        output_table = queryData(db, self.outputs.sql.get())
+        output_table = queryData(db, sql)
         self.outputs.table.set(output_table)
 
-        compose = (None,{})
-        for _,wt in self.widgetsDict.items():
-            if wt['C'].isChecked():
-                valueMap = {}
-
-                for i,v in enumerate(wt['values']):
-                    valueMap[v] = i
-                compose = (wt['parameter'],valueMap)
-                break
-
+        # compositing output
+        compose = [(s, {v:i for i,v in enumerate(state[s]['O'])} ) for s in state if state[s]['C']]
+        if len(compose)<1:
+          compose = (None,{})
+        else:
+          compose = compose[0]
         self.outputs.compose.set(compose)
 
+        self.emitter.s_update.emit()
+
         return 1
```

### Comparing `pycinema-2.0.0/pycinema.egg-info/SOURCES.txt` & `pycinema-3.0.0/pycinema.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,85 @@
 setup.py
-doc/description.md
+doc/pycinema-description.md
 pycinema/Core.py
 pycinema/__init__.py
 pycinema/_version.py
 pycinema.egg-info/PKG-INFO
 pycinema.egg-info/SOURCES.txt
 pycinema.egg-info/dependency_links.txt
+pycinema.egg-info/not-zip-safe
 pycinema.egg-info/requires.txt
 pycinema.egg-info/top_level.txt
+pycinema/filters/CSVReader.py
+pycinema/filters/Calculator.py
 pycinema/filters/CinemaDatabaseReader.py
 pycinema/filters/CinemaDatabaseWriter.py
 pycinema/filters/ColorMapping.py
 pycinema/filters/ColorSource.py
 pycinema/filters/DepthCompositing.py
+pycinema/filters/GetColumn.py
 pycinema/filters/ImageAnnotation.py
 pycinema/filters/ImageBorder.py
 pycinema/filters/ImageCanny.py
 pycinema/filters/ImageConvertGrayscale.py
 pycinema/filters/ImageFilterPIL.py
 pycinema/filters/ImageReader.py
+pycinema/filters/ImageSort.py
+pycinema/filters/ImageView.py
+pycinema/filters/ImagesToTable.py
+pycinema/filters/InspectorView.py
+pycinema/filters/MLTFPredictor.py
+pycinema/filters/MLTFReader.py
 pycinema/filters/MaskCompositing.py
+pycinema/filters/ParallelCoordinates.py
+pycinema/filters/ParametersView.py
+pycinema/filters/Plot.py
+pycinema/filters/PlotLineItem.py
+pycinema/filters/Python.py
 pycinema/filters/Shader.py
 pycinema/filters/ShaderDemoScene.py
 pycinema/filters/ShaderFXAA.py
 pycinema/filters/ShaderIBS.py
 pycinema/filters/ShaderLineAO.py
 pycinema/filters/ShaderPBR.py
 pycinema/filters/ShaderPhong.py
 pycinema/filters/ShaderPointAO.py
 pycinema/filters/ShaderSSAO.py
+pycinema/filters/SqliteDatabaseReader.py
 pycinema/filters/TableEditor.py
 pycinema/filters/TableQuery.py
+pycinema/filters/TableView.py
 pycinema/filters/TableWriter.py
+pycinema/filters/TextEditor.py
+pycinema/filters/TextFileReader.py
+pycinema/filters/ValueSource.py
 pycinema/filters/__init__.py
 pycinema/ipy/CinemaDatabaseViewer.py
 pycinema/ipy/ColorMappingWidgets.py
 pycinema/ipy/ImageViewer.py
 pycinema/ipy/NumberWidget.py
 pycinema/ipy/ParameterWidgets.py
 pycinema/ipy/__init__.py
+pycinema/scripts/__init__.py
+pycinema/scripts/browse.py
+pycinema/scripts/discover.py
+pycinema/scripts/explore.py
+pycinema/scripts/view.py
 pycinema/theater/FilterBrowser.py
 pycinema/theater/Icons.py
+pycinema/theater/SplitFrame.py
+pycinema/theater/TabFrame.py
 pycinema/theater/Theater.py
 pycinema/theater/View.py
-pycinema/theater/ViewFrame.py
 pycinema/theater/ViewStyle.py
 pycinema/theater/__init__.py
 pycinema/theater/node_editor/Edge.py
 pycinema/theater/node_editor/InputText.py
 pycinema/theater/node_editor/Node.py
 pycinema/theater/node_editor/NodeEditorStyle.py
 pycinema/theater/node_editor/Port.py
 pycinema/theater/node_editor/__init__.py
-pycinema/theater/views/ColorMappingView.py
 pycinema/theater/views/FilterView.py
-pycinema/theater/views/ImageView.py
-pycinema/theater/views/InspectorView.py
 pycinema/theater/views/NodeEditorView.py
-pycinema/theater/views/ParallelCoordinatesView.py
-pycinema/theater/views/ParameterView.py
 pycinema/theater/views/SelectionView.py
-pycinema/theater/views/TableView.py
 pycinema/theater/views/__init__.py
 scripts/cinema
```

### Comparing `pycinema-2.0.0/setup.py` & `pycinema-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import setuptools
 
 # read the description file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'doc/description.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, 'doc/pycinema-description.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 exec(open("pycinema/_version.py").read())
 
 setuptools.setup(
     name="pycinema",
     version=__version__,
     author="David H. Rogers",
     author_email="dhr@lanl.gov",
     description="Cinema scientific toolset.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/cinemascience/pycinema",
     include_package_data=True,
-    packages=[  "pycinema", "pycinema.filters", "pycinema.theater", "pycinema.theater.node_editor", "pycinema.theater.views", "pycinema.ipy" ],
+    zip_safe=False,
+    packages=[  "pycinema", "pycinema.filters", "pycinema.scripts", "pycinema.theater", "pycinema.theater.node_editor", "pycinema.theater.views", "pycinema.ipy" ],
     install_requires=[
         "numpy==1.24.2",
         "scipy==1.10.0",
         "h5py==3.8.0",
         "matplotlib==3.6.0",
         "py==1.11.0",
         "Pillow==9.4.0",
         "moderngl<6",
         "opencv-python==4.7.0.68",
         "ipycanvas==0.13.1",
         "ipywidgets==8.0.6",
-        "PySide6>=6.0.0",
-        "python-igraph>=0.10.5"
+        "PySide6<=6.4.3",
+        "python-igraph>=0.10.5",
+        "requests>=2.31.0",
+        "pyqtgraph>=0.13.3",
+        "tensorflow==2.14.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     scripts=[
-        'doc/description.md',
+        'doc/pycinema-description.md',
         'scripts/cinema'
     ],
 )
```

