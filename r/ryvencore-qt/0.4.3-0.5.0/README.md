# Comparing `tmp/ryvencore-qt-0.4.3.tar.gz` & `tmp/ryvencore_qt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryvencore-qt-0.4.3.tar", last modified: Fri Oct 27 21:53:14 2023, max compression
+gzip compressed data, was "ryvencore_qt-0.5.0.tar", last modified: Mon May 20 15:51:14 2024, max compression
```

## Comparing `ryvencore-qt-0.4.3.tar` & `ryvencore_qt-0.5.0.tar`

### file list

```diff
@@ -1,138 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.087465 ryvencore-qt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-10-27 21:53:14.087465 ryvencore-qt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.043464 ryvencore-qt-0.4.3/ryvencore_qt/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.047464 ryvencore-qt-0.4.3/ryvencore_qt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.047464 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.051464 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/
--rw-r--r--   0 runner    (1001) docker     (127)   102416 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   111664 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   109800 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   102444 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   111808 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   101032 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   102688 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   112712 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.059464 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   138520 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155420 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   140724 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   159688 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   139684 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   158172 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   147416 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170376 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   166604 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145936 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168408 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   142980 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   164976 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   144776 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   141612 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   161360 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   148440 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171772 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.067464 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)   191284 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155056 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191568 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155288 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   193360 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   156884 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   161376 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   193160 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   156984 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191984 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   156156 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   192740 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   191792 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   155568 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/node_collapse_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/node_expand_icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.075464 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25091 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/code_block_picture.png
--rw-r--r--   0 runner    (1001) docker     (127)    23985 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/code_block_picture2.png
--rw-r--r--   0 runner    (1001) docker     (127)    17618 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/code_block_picture3.png
--rw-r--r--   0 runner    (1001) docker     (127)    20454 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/function_picture.png
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/function_picture_.png
--rw-r--r--   0 runner    (1001) docker     (127)    71305 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    19733 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/macro_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86801 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/macro_node_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    20715 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/macro_script_picture.png
--rw-r--r--   0 runner    (1001) docker     (127)  2383140 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/opencv_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/script_picture.png
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/script_picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/script_picture_old.png
--rw-r--r--   0 runner    (1001) docker     (127)    18389 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/variable_picture.png
--rw-r--r--   0 runner    (1001) docker     (127)    41046 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/warning.png
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/resources/warning.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.075464 ryvencore-qt-0.4.3/ryvencore_qt/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/Design.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/GUIBase.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/GlobalAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/SessionGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.079464 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/
--rw-r--r--   0 runner    (1001) docker     (127)     9894 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowCommands.py
--rw-r--r--   0 runner    (1001) docker     (127)    58050 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    46630 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowView.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowViewProxyWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowViewZoomWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.079464 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/connections/ConnectionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.079464 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/drawings/
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/drawings/DrawingObject.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/drawings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.083464 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.087465 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeGUI.py
--rw-r--r--   0 runner    (1001) docker     (127)    18859 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItemAction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItemWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/PortItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/WidgetBaseClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.087465 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/EditVal_Dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/FlowsListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/FlowsList_FlowWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/ListWidget_NameLineEdit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/VariablesListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/VarsList_VarWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-27 21:53:14.047464 ryvencore-qt-0.4.3/ryvencore_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-10-27 21:53:14.000000 ryvencore-qt-0.4.3/ryvencore_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2023-10-27 21:53:14.000000 ryvencore-qt-0.4.3/ryvencore_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-27 21:53:14.000000 ryvencore-qt-0.4.3/ryvencore_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-27 21:53:14.000000 ryvencore-qt-0.4.3/ryvencore_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-27 21:53:14.000000 ryvencore-qt-0.4.3/ryvencore_qt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2023-10-27 21:53:14.087465 ryvencore-qt-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-27 21:52:59.000000 ryvencore-qt-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.673915 ryvencore_qt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-20 15:51:14.673915 ryvencore_qt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.645915 ryvencore_qt-0.5.0/ryvencore_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.645915 ryvencore_qt-0.5.0/ryvencore_qt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.645915 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.649915 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/
+-rw-r--r--   0 runner    (1001) docker     (127)   102416 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   111664 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   109800 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   102444 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   111808 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   101032 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   102688 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   112712 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.653915 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   138520 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155420 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   140724 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   159688 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   139684 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   158172 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   147416 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170376 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   166604 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145936 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168408 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   142980 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   164976 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   144776 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   141612 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   161360 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   148440 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171772 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.661915 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191284 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155056 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191568 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155288 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   193360 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   156884 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   161376 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   193160 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   156984 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191984 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   156156 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   192740 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   191792 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   155568 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/node_collapse_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/node_expand_icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.665915 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25091 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/code_block_picture.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23985 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/code_block_picture2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/code_block_picture3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/function_picture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/function_picture_.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71305 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/macro_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86801 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/macro_node_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20715 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/macro_script_picture.png
+-rw-r--r--   0 runner    (1001) docker     (127)  2383140 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/opencv_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/script_picture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/script_picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/script_picture_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18389 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/variable_picture.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41046 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/resources/warning.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.665915 ryvencore_qt-0.5.0/ryvencore_qt/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/Design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/GUIBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/GlobalAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/SessionGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.669915 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowCommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58277 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56039 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowViewProxyWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowViewZoomWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.669915 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/connections/ConnectionAnimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/connections/ConnectionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.669915 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/drawings/
+-rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/drawings/DrawingObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/drawings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.669915 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.673915 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeGUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeInspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19750 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItemAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItemWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/PortItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/WidgetBaseClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.673915 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/EditVal_Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/FlowsListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/FlowsList_FlowWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/ListWidget_NameLineEdit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/VariablesListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/VarsList_VarWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:51:14.673915 ryvencore_qt-0.5.0/ryvencore_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-20 15:51:14.000000 ryvencore_qt-0.5.0/ryvencore_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-20 15:51:14.000000 ryvencore_qt-0.5.0/ryvencore_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:51:14.000000 ryvencore_qt-0.5.0/ryvencore_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 15:51:14.000000 ryvencore_qt-0.5.0/ryvencore_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 15:51:14.000000 ryvencore_qt-0.5.0/ryvencore_qt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-20 15:51:14.673915 ryvencore_qt-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 15:51:10.000000 ryvencore_qt-0.5.0/setup.py
```

### Comparing `ryvencore-qt-0.4.3/LICENSE` & `ryvencore_qt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/PKG-INFO` & `ryvencore_qt-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ryvencore-qt
-Version: 0.4.3
+Version: 0.5.0
 Summary: Qt frontend for ryvencore; Library for building Visual Node Editors
 Home-page: https://github.com/leon-thomm/ryvencore-qt
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.6
+Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ryvencore==0.4.*
-Requires-Dist: PySide2
+Requires-Dist: ryvencore==0.5.*
 Requires-Dist: QtPy
 Requires-Dist: waiting
 Requires-Dist: textdistance
 
 
 <p align="center">
   <img src="./img/logo.png" alt="drawing" width="70%"/>
```

### Comparing `ryvencore-qt-0.4.3/README.md` & `ryvencore_qt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/__init__.py` & `ryvencore_qt-0.5.0/ryvencore_qt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 import ryvencore
 
 from .src.SessionGUI import SessionGUI
 from .src.flows.nodes.NodeGUI import NodeGUI
 
 # customer base classes
 from ryvencore import Node
-from .src.flows.nodes.WidgetBaseClasses import NodeMainWidget, NodeInputWidget
+from .src.flows.nodes.WidgetBaseClasses import NodeMainWidget, NodeInputWidget, NodeInspectorWidget
 
 # gui classes
 from .src.widgets import *
 from .src.flows.FlowTheme import flow_themes
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/asap/OFL.txt` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/asap/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/OFL.txt` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/node_collapse_icon.svg` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/node_collapse_icon.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/node_expand_icon.svg` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/node_expand_icon.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/code_block_picture.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/code_block_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/code_block_picture2.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/code_block_picture2.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/code_block_picture3.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/code_block_picture3.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/function_picture.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/function_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/function_picture_.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/function_picture_.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/logo.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/logo.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/macro_icon.svg` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/macro_icon.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/macro_node_icon.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/macro_node_icon.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/macro_script_picture.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/macro_script_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/opencv_example.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/opencv_example.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/script_picture.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/script_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/script_picture.svg` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/script_picture.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/script_picture_old.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/script_picture_old.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/variable_picture.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/variable_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/pics/warning.png` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/pics/warning.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/resources/warning.svg` & `ryvencore_qt-0.5.0/ryvencore_qt/resources/warning.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/Design.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/Design.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 import json
+from typing import Optional, List, Tuple
 
 from qtpy.QtCore import QObject, Signal
 from qtpy.QtGui import QFontDatabase
 
 from .flows.FlowTheme import FlowTheme, flow_themes
 from .GlobalAttributes import Location
 
 
 class Design(QObject):
     """Design serves as a container for the stylesheet and flow themes, and sends signals to notify GUI elements
-    on change of the flow theme. A configuration for the flow themes can be loaded from a json file."""
+    on change of the flow theme. A configuration for the flow themes can be loaded from a json file.
+    """
 
     global_stylesheet = ''
 
     flow_theme_changed = Signal(str)
     performance_mode_changed = Signal(str)
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
 
-        self.flow_themes = flow_themes
-        self.flow_theme: FlowTheme = None
-        self.default_flow_size = None
-        self.performance_mode: str = None
-        self.node_item_shadows_enabled: bool = None
-        self.animations_enabled: bool = None
-        self.node_selection_stylesheet: str = None
+        self.flow_themes: List[FlowTheme] = flow_themes
+        self.flow_theme: FlowTheme
+        self.default_flow_size: Tuple[int, int]
+        self.performance_mode: str
+        self.node_item_shadows_enabled: bool
+        self.animations_enabled: bool
+        self.node_selection_stylesheet: str
 
         # load standard default values
         self._default_flow_theme = self.flow_themes[-1]
         self.set_performance_mode('pretty')
         self.set_animations_enabled(True)
-        self.default_flow_size = [1000, 700]
+        self.default_flow_size = (1000, 700)
         self.set_flow_theme(self._default_flow_theme)
 
     @staticmethod
     def register_fonts():
         db = QFontDatabase()
-        db.addApplicationFont(
-            Location.PACKAGE_PATH + '/resources/fonts/poppins/Poppins-Medium.ttf'
-        )
-        db.addApplicationFont(
-            Location.PACKAGE_PATH + '/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf'
-        )
-        db.addApplicationFont(
-            Location.PACKAGE_PATH + '/resources/fonts/asap/Asap-Regular.ttf'
-        )
+        db.addApplicationFont(Location.PACKAGE_PATH + '/resources/fonts/poppins/Poppins-Medium.ttf')
+        db.addApplicationFont(Location.PACKAGE_PATH + '/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf')
+        db.addApplicationFont(Location.PACKAGE_PATH + '/resources/fonts/asap/Asap-Regular.ttf')
 
     def load_from_config(self, filepath: str):
         """Loads design configs from a config json file"""
 
         f = open(filepath, 'r')
         data = f.read()
         f.close()
@@ -78,37 +74,35 @@
     def available_flow_themes(self) -> dict:
         return {theme.name: theme for theme in self.flow_themes}
 
     def flow_theme_by_name(self, name: str) -> FlowTheme:
         for theme in self.flow_themes:
             if theme.name.casefold() == name.casefold():
                 return theme
-        return None
+        raise ValueError(f'Flow theme with name "{name}" not found')
 
-    def set_flow_theme(self, theme: FlowTheme = None, name: str = ''):
+    def set_flow_theme(self, theme: Optional[FlowTheme] = None, name: Optional[str] = None):
         """You can either specify the theme by name, or directly provide a FlowTheme object"""
-        if theme:
+        if theme is not None:
             self.flow_theme = theme
-        elif name and name != '':
+        elif name is not None and name != '':
             self.flow_theme = self.flow_theme_by_name(name)
         else:
             return
 
         self.node_selection_stylesheet = self.flow_theme.build_node_selection_stylesheet()
 
         self.flow_theme_changed.emit(self.flow_theme.name)
 
-
     def set_performance_mode(self, new_mode: str):
-        self.performance_mode = new_mode
         if new_mode == 'fast':
             self.node_item_shadows_enabled = False
         else:
             self.node_item_shadows_enabled = True
-
+        self.performance_mode = new_mode
         self.performance_mode_changed.emit(self.performance_mode)
 
     def set_animations_enabled(self, b: bool):
         self.animations_enabled = b
 
     def set_node_item_shadows(self, b: bool):
         self.node_item_shadows_enabled = b
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/GUIBase.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/GUIBase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from ryvencore.Base import Base
+from typing import Any, Dict, Optional
 
+from ryvencore.Base import Base
+from qtpy.QtWidgets import QGraphicsObject, QGraphicsItem
+from qtpy.QtCore import QObject
 
+  
 class GUIBase:
     """Base class for GUI items that represent specific core components"""
 
     # every frontend GUI object that represents some specific component from the core
     # is stored there under the the global id of the represented component.
     # used for completing data (serialization)
-    FRONTEND_COMPONENT_ASSIGNMENTS = {}  # component global id : GUI object
+    FRONTEND_COMPONENT_ASSIGNMENTS: Dict[int, Any] = {}  # component global id : GUI object
 
     @staticmethod
     def get_complete_data_function(session):
         """
         generates a function that searches through generated data by the core and calls
         complete_data() on frontend components that represent them to add frontend data
         """
@@ -38,16 +42,44 @@
                     item = analyze(item)
                     obj[i] = item
 
             return obj
 
         return analyze
 
-    def __init__(self, representing_component: Base = None):
+    def __init__(self, representing_component: Optional[Base] = None):
         """parameter `representing` indicates representation of a specific core component"""
         if representing_component is not None:
             GUIBase.FRONTEND_COMPONENT_ASSIGNMENTS[representing_component.global_id] = self
 
     # OVERRIDE
     def complete_data(self, data: dict) -> dict:
         """completes the data dict of the represented core component by adding all frontend data"""
         return data
+    
+    def on_move(self):
+        """virtual function for when a GUI is moved in the view"""
+        pass
+
+# if the __doc__ is incorrect, this class should be removed
+class QGraphicsItemAnimated(QGraphicsObject):
+    """
+    Serves as a proxy for animating any kind fo QGraphicsItem.
+    This was created because there is no apparent way to animate
+    a QGraphicsItem that isn't a QObject.
+    """
+    
+    def __init__(self, item: QGraphicsItem, parent = None) -> None:
+        super().__init__(parent)
+        self.item = item
+        
+        # for delete purposes
+        # perhaps this could be implemented in an item change where the scene
+        # is none and calling a delete later 
+        self.item.setParentItem(self)
+        self.item.setVisible(False)
+    
+    def boundingRect(self):
+        return self.item.boundingRect()
+    
+    def paint(self, painter, option, widget):
+        return self.item.paint(painter, option, widget)
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/SessionGUI.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/SessionGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Dict
 
 from qtpy.QtCore import QObject, Signal, Qt
 from qtpy.QtWidgets import QWidget, QApplication
 
 import ryvencore
 
 from .flows.FlowView import FlowView
@@ -32,15 +32,15 @@
 
         self.core_session = ryvencore.Session(gui=True, load_addons=True)
         setattr(self.core_session, 'gui', self)
 
         self.gui_parent = gui_parent
 
         # flow views
-        self.flow_views = {}  # {Flow : FlowView}
+        self.flow_views: Dict[ryvencore.Flow, FlowView] = {}
 
         # register complete_data function
         ryvencore.set_complete_data_func(self.get_complete_data_function(self))
 
         # load design
         app = QApplication.instance()
         app.setAttribute(Qt.AA_UseHighDpiPixmaps)
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowTheme.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowTheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional, Tuple, List
+
 from qtpy.QtCore import Qt, QPointF, QPoint, QRectF, QMargins, QMarginsF
 from qtpy.QtGui import QColor, QPainter, QBrush, QRadialGradient, QLinearGradient, QPen, QPainterPath, QFont, QPolygon
 from qtpy.QtWidgets import QStyle, QStyleOption
 
 from ..utils import pythagoras
 
 
@@ -34,20 +36,20 @@
     exec_conn_pen_style = Qt.SolidLine
 
     data_conn_color = QColor('#ffffff')
     data_conn_width = 1.5
     data_conn_pen_style = Qt.DashLine
 
     flow_background_brush = QBrush(QColor('#333333'))
-    flow_background_grid = None
+    flow_background_grid: Optional[Tuple[str, QColor, int, int, int]] = None
     flow_highlight_pen_color = QColor('#245d75')
 
     node_item_shadow_color = QColor('#2b2b2b')
 
-    EXPORT = []
+    EXPORT: List[str] = []
 
     def __init__(self):
         pass
 
     def load(self, data: dict):
         if data and self.name in data.keys():
             imported = {}
@@ -127,15 +129,15 @@
 
         painter.drawRoundedRect(rect, 10, 10)
 
     @staticmethod
     def paint_NI_title_label_default(painter: QPainter, node_style: str, title: str, color: QColor, pen_w: float,
                                      font: QFont, node_item_bounding_rect):
         pen = QPen(color)
-        pen.setWidth(pen_w)
+        pen.setWidth(pen_w)  # type: ignore
 
         painter.setPen(pen)
         painter.setFont(font)
 
         text_rect = node_item_bounding_rect
         text_rect.setTop(text_rect.top())
 
@@ -194,15 +196,15 @@
             return QColor(r, g, b)
         elif len(h) == 8:
             r, g, b, a = tuple(
                 int(h[i:i + 2], 16) for i in (0, 2, 4, 6)
             )
             return QColor(r, g, b, a)
 
-        return None
+        raise ValueError(f'Invalid hex color string: {hex_str}')
 
     @staticmethod
     def col(c: QColor, alpha=255):
         return QColor(c.red(), c.green(), c.blue(), alpha)
 
     @staticmethod
     def _parse_pen_style(s: str):
@@ -275,15 +277,19 @@
 
         painter.drawEllipse(rect)
 
     def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter: QPainter, c: QColor, w, h, bounding_rect, title_rect):
 
         # main rect
-        header_color = QColor(c.red() / 10 + 100, c.green() / 10 + 100, c.blue() / 10 + 100)
+        header_color = QColor(
+            int(c.red() / 10 + 100),
+            int(c.green() / 10 + 100),
+            int(c.blue() / 10 + 100),
+        )
         if selected:
             header_color = header_color.lighter()
         body_gradient = QRadialGradient(bounding_rect.topLeft(), pythagoras(h, w))
         body_gradient.setColorAt(0, self.col(header_color, alpha=200))
         body_gradient.setColorAt(1, self.col(header_color, alpha=0))
 
         painter.setBrush(body_gradient)
@@ -375,23 +381,23 @@
         else:
             c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Source Code Pro", 10, QFont.Bold), bounding_rect)
 
     def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
-        color = QColor('#FFFFFF') if type_ == 'exec' else node_color
+        color = QColor('#FFFFFF') if type_ == 'exec' else QColor(node_color)
         pen = QPen(color)
         pen.setWidth(2)
         painter.setPen(pen)
         if connected or \
                 option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
-            r = node_color.red()
-            g = node_color.green()
-            b = node_color.blue()
+            r = color.red()
+            g = color.green()
+            b = color.blue()
             brush = QBrush(QColor(r, g, b, 100))
             painter.setBrush(brush)
         else:
             painter.setBrush(Qt.NoBrush)
 
         painter.drawEllipse(rect)
 
@@ -565,29 +571,29 @@
         else:
             c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Source Code Pro", 10, QFont.Bold), bounding_rect)
 
     def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
-        color = QColor('#FFFFFF') if type_ == 'exec' else node_color
+        color = QColor('#FFFFFF') if type_ == 'exec' else QColor(node_color)
 
         if type_ == 'exec':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
                 brush = QBrush(QColor(255, 255, 255, 100))
                 painter.setBrush(brush)
             else:
                 painter.setBrush(Qt.NoBrush)
         elif type_ == 'data':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
-                r = node_color.red()
-                g = node_color.green()
-                b = node_color.blue()
+                r = color.red()
+                g = color.green()
+                b = color.blue()
                 brush = QBrush(QColor(r, g, b, 100))
                 painter.setBrush(brush)
             else:
                 painter.setBrush(Qt.NoBrush)
 
         pen = QPen(color)
         pen.setWidth(1)
@@ -875,35 +881,35 @@
         color = None
         if not connected:
             color = QColor('#53585c')
         else:
             if type_ == 'exec':
                 color = QColor('#dddddd')
             else:
-                color = node_color
+                color = QColor(node_color)
 
         if type_ == 'exec':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
                 brush = QBrush(QColor(255, 255, 255, 100))
                 painter.setBrush(brush)
             else:
                 painter.setBrush(Qt.NoBrush)
         elif type_ == 'data':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
-                r = node_color.red()
-                g = node_color.green()
-                b = node_color.blue()
+                r = color.red()
+                g = color.green()
+                b = color.blue()
                 brush = QBrush(QColor(r, g, b, 100))
                 painter.setBrush(brush)
             else:
                 painter.setBrush(Qt.NoBrush)
 
-        brush = QBrush(QColor(color))
+        brush = QBrush(color)
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
 
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
         # painter.drawEllipse(QRectF(padding+w/8, padding+h/8, 3*w/4, 3*h/4))
 
     def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
@@ -994,53 +1000,55 @@
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
     def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
 
         c = None
         if not connected:
-            c = QColor('#53585c')
+            c = '#53585c'
         else:
             if type_ == 'exec':
-                c = QColor('#cccccc')
+                c = '#cccccc'
             else:
                 c = node_color
+        color = QColor(c)
 
-        self.paint_PI_label_default(painter, label_str, c, QFont("Courier New", 10, QFont.Bold), bounding_rect)
+        self.paint_PI_label_default(painter, label_str, color, QFont("Courier New", 10, QFont.Bold), bounding_rect)
 
     def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
-        color = None
+        color_str = None
         if not connected:
-            color = QColor('#53585c')
+            color_str = '#53585c'
         else:
             if type_ == 'exec':
-                color = QColor('#dddddd')
+                color_str = '#dddddd'
             else:
-                color = node_color
+                color_str = node_color
 
+        color = QColor(color_str)
         if type_ == 'exec':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
                 brush = QBrush(QColor(255, 255, 255, 100))
                 painter.setBrush(brush)
             else:
                 painter.setBrush(Qt.NoBrush)
         elif type_ == 'data':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
-                r = node_color.red()
-                g = node_color.green()
-                b = node_color.blue()
+                r = color.red()
+                g = color.green()
+                b = color.blue()
                 brush = QBrush(QColor(r, g, b, 100))
                 painter.setBrush(brush)
             else:
                 painter.setBrush(Qt.NoBrush)
 
-        brush = QBrush(QColor(color))
+        brush = QBrush(color)
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
 
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
         # painter.drawEllipse(QRectF(padding+w/8, padding+h/8, 3*w/4, 3*h/4))
 
     def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
@@ -1433,15 +1441,15 @@
 
     def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = QColor('#FFFFFF')
         self.paint_PI_label_default(painter, label_str, c, QFont("Segoe UI", 8, QFont.Normal), bounding_rect)
 
     def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
-        color = QColor('#FFFFFF') if type_ == 'exec' else node_color
+        color = QColor('#FFFFFF') if type_ == 'exec' else QColor(node_color)
 
         # add = 2
         # padd = padding + add
         outer_ellipse_rect = rect.marginsRemoved(QMarginsF(2, 2, 2, 2))  # QRectF(padd, padd, w - 2*padd, h - 2*padd)
         # add = 4
         # padd = padding + add
         inner_ellipse_rect = rect.marginsRemoved(QMarginsF(4, 4, 4, 4))  # QRectF(padd, padd, w - 2*padd, h - 2*padd)
@@ -1468,15 +1476,15 @@
 
             pen = QPen(color)
             pen.setWidth(1)
             painter.setPen(pen)
 
             if connected:
                 # draw inner ellipse
-                brush = QBrush(QColor(node_color.red(), node_color.green(), node_color.blue(), 200))
+                brush = QBrush(QColor(color.red(), color.green(), color.blue(), 200))
                 painter.setBrush(brush)
                 painter.drawEllipse(inner_ellipse_rect)
 
             # draw outer ellipse
             painter.setBrush(Qt.NoBrush)
             painter.drawEllipse(outer_ellipse_rect)
 
@@ -1607,15 +1615,15 @@
                       painter, c, w, h, bounding_rect, background_color=None):
 
         painter.setBrush(QBrush(self.node_small_bg_col))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 4, 4)
 
 
-flow_themes = [
+flow_themes: List[FlowTheme] = [
     FlowTheme_Toy(),
     FlowTheme_DarkTron(),
     FlowTheme_Ghost(),
     FlowTheme_Blender(),
     FlowTheme_Simple(),
     FlowTheme_Ueli(),
     FlowTheme_PureDark(),
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowView.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowView.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,129 @@
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from ..SessionGUI import SessionGUI
+
 import json
 
-from typing import Tuple
+from typing import Tuple, Optional
 
-from qtpy.QtCore import Qt, QPointF, QPoint, QRectF, QSizeF, Signal, QTimer, QTimeLine, QEvent
-from qtpy.QtGui import QPainter, QPen, QColor, QKeySequence, QTabletEvent, QImage, QGuiApplication, QFont, QTouchEvent
-from qtpy.QtWidgets import QGraphicsView, QGraphicsScene, QShortcut, QMenu, QGraphicsItem, QUndoStack
+from qtpy.QtCore import (
+    Qt,
+    QPointF,
+    QPoint,
+    QRectF,
+    QSizeF,
+    Signal,
+    QTimer,
+    QTimeLine,
+    QEvent,
+)
+from qtpy.QtGui import (
+    QPainter,
+    QPen,
+    QColor,
+    QKeySequence,
+    QTabletEvent,
+    QDropEvent,
+    QContextMenuEvent,
+    QImage,
+    QGuiApplication,
+    QFont,
+    QTouchEvent,
+    QTransform,
+)
+from qtpy.QtWidgets import (
+    QGraphicsView,
+    QGraphicsScene,
+    QShortcut,
+    QMenu,
+    QGraphicsItem,
+    QPushButton,
+    QHBoxLayout,
+    QWidget,
+)
+
+# for compatibility between qt5 and qt6
+try:
+    from qtpy.QtGui import QUndoStack
+except ImportError:
+    from qtpy.QtWidgets import QUndoStack  # type: ignore
 
 from ryvencore.Flow import Flow
 from ryvencore.Node import Node
 from ryvencore.NodePort import NodePort, NodeInput, NodeOutput
-#from ryvencore.Connection import Connection, DataConnection
+
+# from ryvencore.Connection import Connection, DataConnection
 from ryvencore.InfoMsgs import InfoMsgs
 from ryvencore.RC import PortObjPos
 from ryvencore.utils import node_from_identifier
 
 from ..GUIBase import GUIBase
 from ..utils import *
-from .FlowCommands import MoveComponents_Command, PlaceNode_Command, \
-    PlaceDrawing_Command, RemoveComponents_Command, ConnectPorts_Command, Paste_Command, FlowUndoCommand
-from .FlowViewProxyWidget import FlowViewProxyWidget
+from .FlowCommands import (
+    MoveComponents_Command,
+    PlaceNode_Command,
+    PlaceDrawing_Command,
+    RemoveComponents_Command,
+    ConnectPorts_Command,
+    Paste_Command,
+    FlowUndoCommand,
+    SelectComponents_Command,
+)
+from .FlowViewProxyWidget import *
 from .FlowViewStylusModesWidget import FlowViewStylusModesWidget
 from .node_list_widget.NodeListWidget import NodeListWidget
 from .nodes.NodeGUI import NodeGUI
 from .nodes.NodeItem import NodeItem
 from .nodes.PortItem import PortItemPin, PortItem
-from .connections.ConnectionItem import default_cubic_connection_path, ConnectionItem, DataConnectionItem, \
-    ExecConnectionItem
+from .connections.ConnectionItem import (
+    default_cubic_connection_path,
+    ConnectionItem,
+    DataConnectionItem,
+    ExecConnectionItem,
+)
 from .drawings.DrawingObject import DrawingObject
 
+from ..Design import Design
+from enum import Enum
+
+
+class _SelectionMode(Enum):
+    """
+    Determines how selection change events will be handled.
+    If INSTANT, then they happen instantly.
+    If UNDO, the event is pushed unto the undo stack
+    """
+
+    INSTANT = 1
+    UNDOABLE_CLICK = 2
+    UNDOABLE_RUBBERBANDDRAG = 3
+
 
 class FlowView(GUIBase, QGraphicsView):
     """Manages the GUI of flows"""
 
     nodes_selection_changed = Signal(list)
     node_placed = Signal(Node)
 
     create_node_request = Signal(object, dict)
     remove_node_request = Signal(Node)
 
     check_connection_validity_request = Signal((NodeOutput, NodeInput), bool)
     connect_request = Signal(NodePort, NodePort)
 
-    #get_nodes_data_request = Signal(list)
-    #get_connections_data_request = Signal(list)
+    # get_nodes_data_request = Signal(list)
+    # get_connections_data_request = Signal(list)
     get_flow_data_request = Signal()
 
     viewport_update_mode_changed = Signal(str)
 
-    def __init__(self, session_gui, flow, parent=None):
+    def __init__(self, session_gui: SessionGUI, flow: Flow, parent=None) -> None:
         GUIBase.__init__(self, representing_component=flow)
         QGraphicsView.__init__(self, parent=parent)
 
         # UNDO STACK
         self._undo_stack = QUndoStack(self)
         self._undo_action = self._undo_stack.createUndoAction(self, 'undo')
         self._undo_action.setShortcuts(QKeySequence.Undo)
@@ -59,52 +131,57 @@
         self._redo_action.setShortcuts(QKeySequence.Redo)
 
         # SHORTCUTS
         self._init_shortcuts()
 
         # GENERAL ATTRIBUTES
         self.session_gui = session_gui
+        self.design: Design = session_gui.design  # type hinting and quicker access
 
         self.flow: Flow = flow
-        self.node_items: dict = {}  # {Node: NodeItem}
-        self.node_items__cache: dict = {}
-        self.connection_items: dict = {}  # {Connection: ConnectionItem}
-        self.connection_items__cache: dict = {}
+        self.node_items: Dict = {}  # {Node: NodeItem}
+        self.node_items__cache: Dict = {}
+        self.connection_items: Dict = {}  # {Connection: ConnectionItem}
+        self.connection_items__cache: Dict = {}
+        self.selection_mode: _SelectionMode = _SelectionMode.UNDOABLE_CLICK
 
         # PRIVATE FIELDS
+        self._loaded_state: Optional[Dict] = None # h and v scrollbars are changed on import, so we need to defer
         self._tmp_data = None
-        self._selected_pin: PortItemPin = None
+        self._selected_pin: Optional[PortItemPin] = None
         self._dragging_connection = False
-        self._temp_connection_ports = None
+        self._temp_connection_ports: Optional[Tuple[NodeOutput, NodeInput]] = None
         self._waiting_for_connection_request: bool = False
         self.mouse_event_taken = False  # for stylus - see tablet event
-        self._last_mouse_move_pos: QPointF = None
+        self._last_mouse_move_pos: Optional[QPointF] = None
         self._node_place_pos = QPointF()
         self._left_mouse_pressed_in_flow = False
         self._right_mouse_pressed_in_flow = False
-        self._mouse_press_pos: QPointF = None
-        self._auto_connection_pin = None  # stores the gate that we may try to auto connect to a newly placed NI
+        self._mouse_press_pos: Optional[QPointF] = None
+        self._multi_selection = False
+        self._current_selected: List[QGraphicsItem] = []
+        self._auto_connection_pin: Optional[PortItemPin] = None  # stores the gate that we may try to auto connect to a newly placed NI
         self._panning = False
-        self._pan_last_x = None
-        self._pan_last_y = None
+        self._pan_last_x: Optional[int] = None
+        self._pan_last_y: Optional[int] = None
         self._current_scale = 1
         self._total_scale_div = 1
         self._zoom_data = {
             'viewport pos': None,
             'scene pos': None,
             'delta': 0,
         }
 
         # CONNECTIONS TO FLOW
         self.create_node_request.connect(self.flow.create_node)
         self.remove_node_request.connect(self.flow.remove_node)
         self.check_connection_validity_request.connect(self.flow.check_connection_validity)
         # TODO: need to check if the 2 lines below are used
-        #self.get_nodes_data_request.connect(self.flow.gen_nodes_data)
-        #self.get_connections_data_request.connect(self.flow.gen_conns_data)
+        # self.get_nodes_data_request.connect(self.flow.gen_nodes_data)
+        # self.get_connections_data_request.connect(self.flow.gen_conns_data)
         self.get_flow_data_request.connect(self.flow.data)
 
         # CONNECTIONS FROM FLOW
         self.flow.node_added.sub(self.add_node)
         self.flow.node_removed.sub(self.remove_node)
         self.flow.connection_added.sub(self.add_connection)
         self.flow.connection_removed.sub(self.remove_connection)
@@ -117,22 +194,29 @@
 
         self.setScene(scene)
         self.setCacheMode(QGraphicsView.CacheBackground)
         self.setViewportUpdateMode(QGraphicsView.BoundingRectViewportUpdate)
         self.setRenderHint(QPainter.Antialiasing)
         self.setTransformationAnchor(QGraphicsView.AnchorUnderMouse)
         self.setDragMode(QGraphicsView.RubberBandDrag)
-        scene.selectionChanged.connect(self._scene_selection_changed)
+        self._watch_scene_selection()
         self.setAcceptDrops(True)
 
         self.centerOn(QPointF(self.viewport().width() / 2, self.viewport().height() / 2))
 
         self.scene_rect_width = self.mapFromScene(self.sceneRect()).boundingRect().width()
         self.scene_rect_height = self.mapFromScene(self.sceneRect()).boundingRect().height()
 
+        # for proper background painting
+        # we could probably use the no cache flag
+        on_pan = lambda scroll: self.resetCachedContent()
+        
+        self.horizontalScrollBar().valueChanged.connect(on_pan)
+        self.verticalScrollBar().valueChanged.connect(on_pan)
+        
         # NODE LIST WIDGET
         self._node_list_widget = NodeListWidget(self.session_gui)
         self._node_list_widget.setMinimumWidth(260)
         self._node_list_widget.setFixedHeight(300)
         self._node_list_widget.escaped.connect(self.hide_node_list_widget)
         self._node_list_widget.node_chosen.connect(self.create_node__cmd)
 
@@ -148,28 +232,58 @@
         # self._zoom_proxy.setFlag(QGraphicsItem.ItemIgnoresTransformations, True)
         # self._zoom_proxy.setZValue(1001)
         # self._zoom_widget = FlowViewZoomWidget(self)
         # self._zoom_proxy.setWidget(self._zoom_widget)
         # self.scene().addItem(self._zoom_proxy)
         # self.set_zoom_proxy_pos()
 
+        def init_proxy_widget(widget: QWidget, proxy: FlowViewProxyWidget):
+            proxy.setFlag(QGraphicsItem.ItemIgnoresTransformations, True)
+            proxy.setZValue(1001)
+            proxy.setWidget(widget)
+            self.scene().addItem(proxy)
+            return proxy
+
         # STYLUS
         self.stylus_mode = ''
         self._current_drawing = None
         self._drawing = False
-        self.drawings = []
-        self._stylus_modes_proxy = FlowViewProxyWidget(self)
-        self._stylus_modes_proxy.setFlag(QGraphicsItem.ItemIgnoresTransformations, True)
-        self._stylus_modes_proxy.setZValue(1001)
+        self.drawings: List[DrawingObject] = []
         self._stylus_modes_widget = FlowViewStylusModesWidget(self)
-        self._stylus_modes_proxy.setWidget(self._stylus_modes_widget)
-        self.scene().addItem(self._stylus_modes_proxy)
+        self._stylus_modes_proxy = init_proxy_widget(
+            self._stylus_modes_widget, FlowViewProxyWidget(self)
+        )
         self.set_stylus_proxy_pos()
         self.setAttribute(Qt.WA_TabletTracking)
 
+        # MENU
+        self._menu = QMenu()
+        
+        # just to add some space for the button
+        menu_layout_widget = self._create_no_background_widget("FlowMenu")
+        # just to add some space for the button
+        menu_layout_widget.setLayout(QHBoxLayout())
+        menu_button = QPushButton("Menu")
+        self._menu_button = menu_button
+        menu_layout_widget.layout().addWidget(menu_button)
+
+        def menu_button_clicked():
+            # prob not entirely correct, since menu is part of a layout
+            # but since it's the first item, it's the same
+            menu_pos = self._menu_button.pos()
+            menu_pos = self.mapToGlobal(menu_pos) + QPoint(8, self._menu_button.height() + 10)
+            self._menu.exec_(menu_pos)
+
+        menu_button.clicked.connect(menu_button_clicked)
+
+        menu_layout_proxy = init_proxy_widget(menu_layout_widget, FlowViewProxyWidget(self))
+        self._menu_widget = menu_button
+        self._menu_layout_proxy = menu_layout_proxy
+        self.set_menu_proxy_pos()
+
         # # TOUCH GESTURES
         # recognizer = PanGestureRecognizer()
         # pan_gesture_id = QGestureRecognizer.registerRecognizer(recognizer) <--- CRASH HERE
         # self.grabGesture(pan_gesture_id)
         self.viewport().setAttribute(Qt.WA_AcceptTouchEvents)
         self.last_pinch_points_dist = 0
 
@@ -190,27 +304,43 @@
 
         # CATCH UP ON FLOW
         for node in self.flow.nodes:
             self.add_node(node)
         for c in [(o, i) for o, conns in self.flow.graph_adj.items() for i in conns]:
             self.add_connection(c)
 
+    def menu(self) -> QMenu:
+        """The menu for this flow view"""
+        return self._menu
+
+    def _create_no_background_widget(self, name: str):
+        result = QWidget()
+        result.setObjectName(name)
+        result.setStyleSheet(
+            f'''
+        QWidget#{name} {{
+            background: transparent; 
+        }}
+                '''
+        )
+        return result
+
     def _init_shortcuts(self):
         place_new_node_shortcut = QShortcut(QKeySequence('Shift+P'), self)
         place_new_node_shortcut.activated.connect(self._place_new_node_by_shortcut)
         move_selected_components_left_shortcut = QShortcut(QKeySequence('Shift+Left'), self)
         move_selected_components_left_shortcut.activated.connect(self._move_selected_comps_left)
         move_selected_components_up_shortcut = QShortcut(QKeySequence('Shift+Up'), self)
         move_selected_components_up_shortcut.activated.connect(self._move_selected_comps_up)
         move_selected_components_right_shortcut = QShortcut(QKeySequence('Shift+Right'), self)
         move_selected_components_right_shortcut.activated.connect(self._move_selected_comps_right)
         move_selected_components_down_shortcut = QShortcut(QKeySequence('Shift+Down'), self)
         move_selected_components_down_shortcut.activated.connect(self._move_selected_comps_down)
         select_all_shortcut = QShortcut(QKeySequence('Ctrl+A'), self)
-        select_all_shortcut.activated.connect(self.select_all)
+        select_all_shortcut.activated.connect(self._select_all_action)
         copy_shortcut = QShortcut(QKeySequence.Copy, self)
         copy_shortcut.activated.connect(self._copy)
         cut_shortcut = QShortcut(QKeySequence.Cut, self)
         cut_shortcut.activated.connect(self._cut)
         paste_shortcut = QShortcut(QKeySequence.Paste, self)
         paste_shortcut.activated.connect(self._paste)
 
@@ -220,46 +350,29 @@
         redo_shortcut.activated.connect(self._redo_activated)
 
     def _theme_changed(self, t):
         self._node_list_widget.setStyleSheet(self.session_gui.design.node_selection_stylesheet)
         for n, ni in self.node_items.items():
             ni.widget.rebuild_ui()
 
-        # TODO: repaint background. how?
-        self.viewport().update()
-        self.scene().update(self.sceneRect())
+        # https://doc.qt.io/qtforpython-5/PySide2/QtWidgets/QGraphicsView.html#PySide2.QtWidgets.PySide2.QtWidgets.QGraphicsView.resetCachedContent
+        self.resetCachedContent()
+        self.update()
 
     def _perf_mode_changed(self, mode):
-
         # set widget value update rule for port inputs, because this takes up quite a bit of performance
-        update_widget_value = (mode == 'pretty')
+        update_widget_value = mode == 'pretty'
         for n, ni in self.node_items.items():
             for inp in ni.inputs:
-                inp.update_widget_value = (update_widget_value and inp.widget)
+                inp.update_widget_value = update_widget_value and inp.widget
 
         self.viewport().update()
         self.scene().update(self.sceneRect())
 
-    def _scene_selection_changed(self):
-        self.nodes_selection_changed.emit(self.selected_nodes())
-
-    def contextMenuEvent(self, event):
-        QGraphicsView.contextMenuEvent(self, event)
-        # in the case of the menu already being shown by a widget under the mouse, the event is accepted here
-        if event.isAccepted():
-            return
-
-        for i in self.items(event.pos()):
-            if isinstance(i, NodeItem):
-                ni: NodeItem = i
-                menu: QMenu = ni.get_context_menu()
-                menu.exec_(event.globalPos())
-                event.accept()
-
-    def _push_undo(self, cmd: FlowUndoCommand):
+    def push_undo(self, cmd: FlowUndoCommand):
         self._undo_stack.push(cmd)
         cmd.activate()
 
     def _undo_activated(self):
         """Triggered by ctrl+z"""
         self._undo_stack.undo()
         self.viewport().update()
@@ -268,51 +381,59 @@
         """Triggered by ctrl+y"""
         self._undo_stack.redo()
         self.viewport().update()
 
     def mousePressEvent(self, event):
         # InfoMsgs.write('mouse press event received, point:', event.pos())
 
+        self._set_selection_mode(_SelectionMode.UNDOABLE_CLICK)
+
         # to catch tablet events (for some reason, it results in a mousePrEv too)
         if self.mouse_event_taken:
             self.mouse_event_taken = False
             return
 
-        QGraphicsView.mousePressEvent(self, event)
+        # this allows to chain the selection event when multi-selecting
+        hover_item = self.itemAt(event.pos())
+        if hover_item is None:
+            self._set_selection_mode(_SelectionMode.UNDOABLE_RUBBERBANDDRAG)
+
+        if event.button() != Qt.RightButton:
+            QGraphicsView.mousePressEvent(self, event)
 
         # don't process the event if it has been processed by a specific component in the scene
         # this includes node items, node port pins, proxy widgets etc.
         if self.mouse_event_taken:
             self.mouse_event_taken = False
+            self._set_selection_mode(_SelectionMode.UNDOABLE_CLICK)
             return
 
         if event.button() == Qt.LeftButton:
             if self._node_list_widget_proxy.isVisible():
                 self.hide_node_list_widget()
 
         elif event.button() == Qt.RightButton:
             self._right_mouse_pressed_in_flow = True
             event.accept()
 
         self._mouse_press_pos = self.mapToScene(event.pos())
 
     def mouseMoveEvent(self, event):
-
-        QGraphicsView.mouseMoveEvent(self, event)
-
         if self._right_mouse_pressed_in_flow:  # PAN
-
             if not self._panning:
                 self._panning = True
                 self._pan_last_x = event.x()
                 self._pan_last_y = event.y()
 
             self.pan(event.pos())
             event.accept()
 
+        else:
+            QGraphicsView.mouseMoveEvent(self, event)
+
         self._last_mouse_move_pos = self.mapToScene(event.pos())
 
         if self._dragging_connection:
             self.viewport().repaint()
 
     def mouseReleaseEvent(self, event):
         # there might be a proxy widget meant to receive the event instead of the flow
@@ -322,38 +443,36 @@
         for item in self.items(event.pos()):
             if isinstance(item, NodeItem):
                 node_item_at_event_pos = item
 
         if self.mouse_event_taken:
             self.mouse_event_taken = False
             self.viewport().repaint()
+            self._set_selection_mode(_SelectionMode.UNDOABLE_CLICK)
             return
 
         elif self._panning:
             self._panning = False
 
         elif event.button() == Qt.RightButton:
             self._right_mouse_pressed_in_flow = False
-            if self._mouse_press_pos == self._last_mouse_move_pos:
+            if self._mouse_press_pos == self._last_mouse_move_pos and not self.itemAt(event.pos()):
                 self.show_place_node_widget(event.pos())
+                self._set_selection_mode(_SelectionMode.UNDOABLE_CLICK)
                 return
 
         if self._dragging_connection:
-
             # connection dropped over port item
             port_items = {i: isinstance(i, PortItem) for i in self.items(event.pos())}
             if any(port_items.values()):
-
-                p_i = list(port_items.keys())[list(port_items.values()).index(True)]  # gets the first PortItem
+                # gets the first PortItem
+                p_i = list(port_items.keys())[list(port_items.values()).index(True)]
 
                 # the validity of the connection is checked in connect_node_ports__cmd
-                self.connect_node_ports__cmd(
-                    self._selected_pin.port,
-                    p_i.port
-                )
+                self.connect_node_ports__cmd(self._selected_pin.port, p_i.port)
 
             # connection dropped above NodeItem -> auto connect
             elif node_item_at_event_pos:
                 # find node item
                 ni_under_drop = None
                 for item in self.items(event.pos()):
                     if isinstance(item, NodeItem):
@@ -367,45 +486,50 @@
                 self.show_place_node_widget(event.pos())
 
             self._dragging_connection = False
             self._selected_pin = None
 
         # if event.button() == Qt.LeftButton:
         #     self._left_mouse_pressed_in_flow = False
-        elif event.button() == Qt.RightButton:
+        elif event.button() != Qt.RightButton:
+            if self.selection_mode == _SelectionMode.UNDOABLE_RUBBERBANDDRAG:
+                self._select__cmd()
+
+        else:
             self._right_mouse_pressed_in_flow = False
 
+        self._set_selection_mode(_SelectionMode.UNDOABLE_CLICK)
         self.viewport().repaint()
 
     def keyPressEvent(self, event):
         QGraphicsView.keyPressEvent(self, event)
-
         if event.isAccepted():
             return
 
         if event.key() == Qt.Key_Escape:  # do I need that... ?
             self.clearFocus()
             self.setFocus()
             return True
 
-        elif event.key() == Qt.Key_Delete:
+        elif event.key() == Qt.Key_Delete and self.selection_mode != _SelectionMode.UNDOABLE_RUBBERBANDDRAG:
             self.remove_selected_components__cmd()
 
     def wheelEvent(self, event):
-
         if event.modifiers() & Qt.ControlModifier:
             event.accept()
 
-            self._zoom_data['viewport pos'] = event.posF()
-            self._zoom_data['scene pos'] = pointF_mapped(self.mapToScene(event.pos()), event.posF())
+            view_pos = event.position()
+            self._zoom_data['viewport pos'] = view_pos
+            self._zoom_data['scene pos'] = self.mapToScene(view_pos.toPoint())
 
-            self._zoom_data['delta'] += event.delta()
+            y_delta = event.angleDelta().y()
+            self._zoom_data['delta'] += y_delta
 
-            if self._zoom_data['delta'] * event.delta() < 0:
-                self._zoom_data['delta'] = event.delta()
+            if self._zoom_data['delta'] * y_delta < 0:
+                self._zoom_data['delta'] = y_delta
 
             anim = QTimeLine(100, self)
             anim.setUpdateInterval(10)
             anim.valueChanged.connect(self._scaling_time)
             anim.start()
 
         else:
@@ -421,68 +545,75 @@
 
     def viewportEvent(self, event: QEvent) -> bool:
         """handling some touch features here"""
 
         if event.type() == QEvent.TouchBegin:
             self.setDragMode(QGraphicsView.NoDrag)
             return True
+
         elif event.type() == QEvent.TouchUpdate:
-            event: QTouchEvent
             if len(event.touchPoints()) == 2:
-
                 tp0, tp1 = event.touchPoints()[0], event.touchPoints()[1]
 
                 p0, p1 = tp0.pos(), tp1.pos()
                 # sp0, sp1 = tp0.scenePos(), tp1.scenePos()
 
                 pinch_points_dist = points_dist(p0, p1)
 
                 if self.last_pinch_points_dist == 0:
                     self.last_pinch_points_dist = pinch_points_dist
 
                 center = middle_point(p0, p1)
                 self.zoom(
                     p_abs=center,
                     p_mapped=self.mapToScene(center.toPoint()),
-                    angle=((pinch_points_dist / self.last_pinch_points_dist)**10 - 1) * 100,
+                    angle=((pinch_points_dist / self.last_pinch_points_dist) ** 10 - 1) * 100,
                 )
 
                 self.last_pinch_points_dist = pinch_points_dist
 
             return True
 
         elif event.type() == QEvent.TouchEnd:
             self.last_pinch_points_dist = 0
             self.setDragMode(QGraphicsView.RubberBandDrag)
             return True
 
         else:
             return super().viewportEvent(event)
 
-    def tabletEvent(self, event):
+    def tabletEvent(self, event: QTabletEvent) -> None:
         """tabletEvent gets called by stylus operations.
         LeftButton: std, no button pressed
         RightButton: upper button pressed"""
 
         # if in edit mode and not panning or starting a pan, pass on to std mouseEvent handlers above
-        if self.stylus_mode == 'edit' and not self._panning and not \
-                (event.type() == QTabletEvent.TabletPress and event.button() == Qt.RightButton):
+        if (
+            self.stylus_mode == 'edit'
+            and not self._panning
+            and not (event.type() == QTabletEvent.TabletPress and event.button() == Qt.RightButton)
+        ):
             return  # let the mousePress/Move/Release-Events handle it
 
-        scaled_event_pos: QPointF = event.posF() / self._current_scale
+        scaled_event_pos: QPointF = event.posF()
+        scaled_event_pos /= self._current_scale  # type: ignore
+        # mypy thinks the above results in a float, but it doesn't
 
         if event.type() == QTabletEvent.TabletPress:
             self.mouse_event_taken = True
 
             if event.button() == Qt.LeftButton:
                 if self.stylus_mode == 'comment':
                     view_pos = self.mapToScene(self.viewport().pos())
                     new_drawing = self._create_and_place_drawing__cmd(
                         view_pos + scaled_event_pos,
-                        data={**self._stylus_modes_widget.get_pen_settings(), 'viewport pos': view_pos}
+                        data={
+                            **self._stylus_modes_widget.get_pen_settings(),
+                            'viewport pos': view_pos,
+                        },
                     )
                     self._current_drawing = new_drawing
                     self._drawing = True
             elif event.button() == Qt.RightButton:
                 self._panning = True
                 self._pan_last_x = event.x()
                 self._pan_last_y = event.y()
@@ -495,23 +626,27 @@
             elif event.pointerType() == QTabletEvent.Eraser:
                 if self.stylus_mode == 'comment':
                     for i in self.items(event.pos()):
                         if isinstance(i, DrawingObject):
                             self.remove_drawing(i)
                             break
             elif self.stylus_mode == 'comment' and self._drawing:
+                assert self._current_drawing is not None
                 if self._current_drawing.append_point(scaled_event_pos):
-                    self._current_drawing.stroke_weights.append(event.pressure()*self._stylus_modes_widget.pen_width())
+                    self._current_drawing.stroke_weights.append(
+                        event.pressure() * self._stylus_modes_widget.pen_width()
+                    )
                 self._current_drawing.update()
                 self.viewport().update()
 
         elif event.type() == QTabletEvent.TabletRelease:
             if self._panning:
                 self._panning = False
             if self.stylus_mode == 'comment' and self._drawing:
+                assert self._current_drawing is not None
                 self._current_drawing.finish()
                 InfoMsgs.write('drawing finished')
                 self._current_drawing = None
                 self._drawing = False
 
     """
     --> https://forum.qt.io/topic/121473/qgesturerecognizer-registerrecognizer-crashes-using-pyside2
@@ -533,33 +668,48 @@
         if event.mimeData().hasFormat('application/json'):
             event.acceptProposedAction()
 
     def dragMoveEvent(self, event):
         if event.mimeData().hasFormat('application/json'):
             event.acceptProposedAction()
 
-    def dropEvent(self, event):
-
+    def dropEvent(self, event: QDropEvent):
         try:
             text = str(event.mimeData().data('application/json'), 'utf-8')
-            data: dict = json.loads(text)
+            data: Dict = json.loads(text)
 
             if data['type'] == 'node':
                 self._node_place_pos = self.mapToScene(event.pos())
                 self.create_node__cmd(
-                    node_from_identifier(data['node identifier'], self.session_gui.core_session.nodes)
+                    node_from_identifier(
+                        data['node identifier'],
+                        list(self.session_gui.core_session.nodes)
+                    )
                 )
+            # without this keyPressed function isn't called if we don't click in the view
+            self.setFocus()
         except Exception:
             pass
+    
+    def contextMenuEvent(self, event: QContextMenuEvent):
+        QGraphicsView.contextMenuEvent(self, event)
+        # in the case of the menu already being shown by a widget under the mouse, the event is accepted here
+        if event.isAccepted():
+            return
+        
+        for i in self.items(event.pos()):
+            if isinstance(i, NodeItem):
+                ni: NodeItem = i
+                menu: QMenu = ni.get_context_menu()
+                menu.exec_(event.globalPos())
+                event.accept()
 
     # PAINTING
     def drawBackground(self, painter, rect):
-
         painter.setBrush(self.session_gui.design.flow_theme.flow_background_brush)
-        painter.drawRect(rect.intersected(self.sceneRect()))
         painter.setPen(Qt.NoPen)
         painter.drawRect(self.sceneRect())
 
         if self.session_gui.design.performance_mode == 'pretty':
             theme = self.session_gui.design.flow_theme
             if theme.flow_background_grid and self._current_scale >= 0.7:
                 if theme.flow_background_grid[0] == 'points':
@@ -568,40 +718,45 @@
                     diff_x = theme.flow_background_grid[3]
                     diff_y = theme.flow_background_grid[4]
 
                     pen = QPen(color)
                     pen.setWidthF(pen_width)
                     painter.setPen(pen)
 
-                    for x in range(diff_x, self.sceneRect().toRect().width(), diff_x):
-                        for y in range(diff_y, self.sceneRect().toRect().height(), diff_y):
+                    points_rect = rect.toRect()
+                    top_left = points_rect.topLeft()
+                    for x in range(
+                        diff_x + top_left.x(), points_rect.width() + top_left.x(), diff_x
+                    ):
+                        for y in range(
+                            diff_y + top_left.y(), points_rect.height() + top_left.y(), diff_y
+                        ):
                             painter.drawPoint(x, y)
 
-        self.set_stylus_proxy_pos()  # has to be called here instead of in drawForeground to prevent lagging
+        # has to be called here instead of in drawForeground to prevent lagging
+        self.set_stylus_proxy_pos()
+        self.set_menu_proxy_pos()
         # self.set_zoom_proxy_pos()
 
     def drawForeground(self, painter, rect):
-
         # DRAW CURRENTLY DRAGGED CONNECTION
         if self._dragging_connection:
             pen = QPen(QColor('#101520'))
             pen.setWidth(3)
             pen.setStyle(Qt.DotLine)
             painter.setPen(pen)
 
             pin_pos = self._selected_pin.get_scene_center_pos()
             spp = self._selected_pin.port
             cursor_pos = self._last_mouse_move_pos
 
             pos1 = pin_pos if spp.io_pos == PortObjPos.OUTPUT else cursor_pos
             pos2 = pin_pos if spp.io_pos == PortObjPos.INPUT else cursor_pos
 
-            painter.drawPath(
-                default_cubic_connection_path(pos1, pos2)
-            )
+            painter.drawPath(default_cubic_connection_path(pos1, pos2))
 
         # # DRAW SELECTED NIs BORDER
         # for ni in self.selected_node_items():
         #     pen = QPen(self.session.design.flow_theme.flow_highlight_pen_color)
         #     pen.setWidth(3)
         #     painter.setPen(pen)
         #     painter.setBrush(Qt.NoBrush)
@@ -629,17 +784,19 @@
             painter.drawEllipse(p_o.pos().x(), p_o.pos().y(), 2, 2)
 
     def get_viewport_img(self) -> QImage:
         """Returns a clear image of the viewport"""
 
         self.hide_proxies()
         img = QImage(
-            self.viewport().rect().width(),
-            self.viewport().height(),
-            QImage.Format_ARGB32
+            size=QSizeF(
+                self.viewport().rect().width(),
+                self.viewport().height(),
+            ),
+            format=QImage.Format_ARGB32,
         )
         img.fill(Qt.transparent)
 
         painter = QPainter(img)
         painter.setRenderHint(QPainter.Antialiasing)
         self.render(painter, self.viewport().rect(), self.viewport().rect())
         self.show_proxies()
@@ -647,17 +804,21 @@
 
     def get_whole_scene_img(self) -> QImage:
         """Returns an image of the whole scene, scaled accordingly to current scale factor.
         Due to a bug this only works from the viewport position down and right, so the user has to scroll to
         the top left corner in order to get the full scene"""
 
         self.hide_proxies()
-        img = QImage(self.sceneRect().width() / self._total_scale_div,
-                     self.sceneRect().height() / self._total_scale_div,
-                     QImage.Format_RGB32)
+        img = QImage(
+            size=QSizeF(
+                self.sceneRect().width() / self._total_scale_div,
+                self.sceneRect().height() / self._total_scale_div,
+            ),
+            format=QImage.Format_RGB32,
+        )
         img.fill(Qt.transparent)
 
         painter = QPainter(img)
         painter.setRenderHint(QPainter.Antialiasing)
         rect = QRectF()
         rect.setLeft(-self.viewport().pos().x())
         rect.setTop(-self.viewport().pos().y())
@@ -671,40 +832,64 @@
     # PROXY POSITIONS
 
     # def set_zoom_proxy_pos(self):
     #     self._zoom_proxy.setPos(self.mapToScene(self.viewport().width() - self._zoom_widget.width(), 0))
 
     def set_stylus_proxy_pos(self):
         self._stylus_modes_proxy.setPos(
-            self.mapToScene(self.viewport().width() - self._stylus_modes_widget.width(), 0))
-            # self.mapToScene(self.viewport().width() - self._stylus_modes_widget.width() - self._zoom_widget.width(), 0))
-
+            self.mapToScene(self.viewport().width() - self._stylus_modes_widget.width(), 0)
+        )
+        # self.mapToScene(self.viewport().width() - self._stylus_modes_widget.width() - self._zoom_widget.width(), 0))
+    
+    def set_menu_proxy_pos(self):
+        self._menu_layout_proxy.setPos(self.mapToScene(0, 0))
+        
     def hide_proxies(self):
         self._stylus_modes_proxy.hide()
+        self._menu_layout_proxy.hide()
         # self._zoom_proxy.hide()
 
     def show_proxies(self):
         self._stylus_modes_proxy.show()
+        self._menu_layout_proxy.show()
         # self._zoom_proxy.show()
 
     # PLACE NODE WIDGET
     def show_place_node_widget(self, pos, nodes=None):
         """Opens the place node dialog in the scene."""
 
         # calculating position
         self._node_place_pos = self.mapToScene(pos)
         dialog_pos = QPoint(pos.x() + 1, pos.y() + 1)
 
         # ensure that the node_list_widget stays in the viewport
-        if dialog_pos.x() + self._node_list_widget.width() / self._total_scale_div > self.viewport().width():
-            dialog_pos.setX(dialog_pos.x() - (
-                    dialog_pos.x() + self._node_list_widget.width() / self._total_scale_div - self.viewport().width()))
-        if dialog_pos.y() + self._node_list_widget.height() / self._total_scale_div > self.viewport().height():
-            dialog_pos.setY(dialog_pos.y() - (
-                    dialog_pos.y() + self._node_list_widget.height() / self._total_scale_div - self.viewport().height()))
+        if (
+            dialog_pos.x() + self._node_list_widget.width() / self._total_scale_div
+            > self.viewport().width()
+        ):
+            dialog_pos.setX(
+                dialog_pos.x()
+                - (
+                    dialog_pos.x()
+                    + self._node_list_widget.width() / self._total_scale_div
+                    - self.viewport().width()
+                )
+            )
+        if (
+            dialog_pos.y() + self._node_list_widget.height() / self._total_scale_div
+            > self.viewport().height()
+        ):
+            dialog_pos.setY(
+                dialog_pos.y()
+                - (
+                    dialog_pos.y()
+                    + self._node_list_widget.height() / self._total_scale_div
+                    - self.viewport().height()
+                )
+            )
         dialog_pos = self.mapToScene(dialog_pos)
 
         # open nodes dialog
         # the dialog emits 'node_chosen' which is connected to self.place_node__cmd
         self._node_list_widget.update_list(
             nodes if nodes is not None else self.session_gui.core_session.nodes
         )
@@ -731,16 +916,20 @@
             point_in_viewport = QPointF(viewport_x, viewport_y).toPoint()
             self._node_place_pos = self.mapToScene(point_in_viewport)
 
         self.show_place_node_widget(point_in_viewport)
 
     # PAN
     def pan(self, new_pos):
-        self.horizontalScrollBar().setValue(self.horizontalScrollBar().value() - (new_pos.x() - self._pan_last_x))
-        self.verticalScrollBar().setValue(self.verticalScrollBar().value() - (new_pos.y() - self._pan_last_y))
+        self.horizontalScrollBar().setValue(
+            self.horizontalScrollBar().value() - (new_pos.x() - self._pan_last_x)
+        )
+        self.verticalScrollBar().setValue(
+            self.verticalScrollBar().value() - (new_pos.y() - self._pan_last_y)
+        )
         self._pan_last_x = new_pos.x()
         self._pan_last_y = new_pos.y()
 
     # ZOOM
     def zoom_in(self, amount):
         local_viewport_center = QPoint(self.viewport().width() / 2, self.viewport().height() / 2)
         self.zoom(local_viewport_center, self.mapToScene(local_viewport_center), amount)
@@ -755,54 +944,53 @@
         by = 0
         velocity = 2 * (1 / self._current_scale) + 0.5
         if velocity > 3:
             velocity = 3
         if self._current_scale < 1:
             velocity *= self._current_scale
 
-        zoom_dir_IN = angle>0
+        zoom_dir_IN = angle > 0
         if zoom_dir_IN:
-            by = 1 + (angle / 4000)*velocity
+            by = 1 + (angle / 4000) * velocity
         else:
-            by = 1 - (-angle / 4000)*velocity
+            by = 1 - (-angle / 4000) * velocity
 
         if zoom_dir_IN:
             if self._current_scale * by < 3:
                 self.scale(by, by)
                 self._current_scale *= by
         else:
-            if self.scene_rect_width * by >= self.viewport().size().width() and self.scene_rect_height * by >= self.viewport().size().height():
+            if (
+                self.scene_rect_width * by >= self.viewport().size().width()
+                and self.scene_rect_height * by >= self.viewport().size().height()
+            ):
                 self.scale(by, by)
                 self._current_scale *= by
 
         w = self.viewport().width()
         h = self.viewport().height()
         wf = self.mapToScene(QPoint(w - 1, 0)).x() - self.mapToScene(QPoint(0, 0)).x()
         hf = self.mapToScene(QPoint(0, h - 1)).y() - self.mapToScene(QPoint(0, 0)).y()
         lf = p_mapped.x() - p_abs.x() * wf / w
         tf = p_mapped.y() - p_abs.y() * hf / h
 
         self.ensureVisible(lf, tf, wf, hf, 0, 0)
 
-        target_rect = QRectF(QPointF(lf, tf),
-                             QSizeF(wf, hf))
+        target_rect = QRectF(QPointF(lf, tf), QSizeF(wf, hf))
         self._total_scale_div = target_rect.width() / self.viewport().width()
 
         self.ensureVisible(target_rect, 0, 0)
 
     # NODES
     def create_node__cmd(self, node_class):
-        self._push_undo(
-            PlaceNode_Command(self, node_class, self._node_place_pos)
-        )
-
-    def add_node(self, node):
+        self.push_undo(PlaceNode_Command(self, node_class, self._node_place_pos))
 
+    def add_node(self, node: Node):
         # create item
-        item: NodeItem = None
+        item: NodeItem
 
         if node in self.node_items__cache.keys():  # load from cache
             # print('using a cached item')
             item = self.node_items__cache[node]
             self._add_node_item(item)
 
         else:  # create new item
@@ -824,20 +1012,21 @@
             else:
                 pos = self._node_place_pos
 
             self._add_node_item(item, pos)
 
         # auto connect
         if self._auto_connection_pin:
-            self.auto_connect(self._auto_connection_pin.port,
-                              node)
+            self.auto_connect(self._auto_connection_pin.port, node)
 
     def _add_node_item(self, item: NodeItem, pos=None):
         self.node_items[item.node] = item
 
+        self._set_selection_mode(_SelectionMode.INSTANT)
+
         self.scene().addItem(item)
         if pos:
             item.setPos(pos)
 
         # select new item
         self.clear_selection()
         item.setSelected(True)
@@ -845,14 +1034,15 @@
     def remove_node(self, node):
         item = self.node_items[node]
         self._remove_node_item(item)
         del self.node_items[node]
 
     def _remove_node_item(self, item: NodeItem):
         # store item in case the remove action gets undone later
+        self._set_selection_mode(_SelectionMode.INSTANT)
         self.node_items__cache[item.node] = item
         self.scene().removeItem(item)
 
     # CONNECTIONS
     def connect_node_ports__cmd(self, p1: NodePort, p2: NodePort):
         # Need to check order of ports since Flow.check_connection_validity needs (NodeOutput, NodeInput)
         if isinstance(p1, NodeOutput) and isinstance(p2, NodeInput):
@@ -869,78 +1059,87 @@
             self.connection_request_valid(False)
 
     def connection_request_valid(self, valid: bool):
         """
         Triggered after the abstract flow evaluated validity of pending connect request.
         This can also lead to a disconnect!
         """
+        
+        # TODO: this stuff is too complicated, simplify
 
         if self._waiting_for_connection_request:
             self._waiting_for_connection_request = False
         else:
             return
 
+        assert self._temp_connection_ports is not None
+
         if valid:
+            out: NodeOutput
+            inp: NodeInput
             out, inp = self._temp_connection_ports
-            if out.io_pos == PortObjPos.INPUT:
-                out, inp = inp, out
 
             if self.flow.graph_adj_rev[inp] not in (None, out): # out connected to something else
                 # remove existing connection
-                self._push_undo(
+                self.push_undo(
                     ConnectPorts_Command(self, out=self.flow.graph_adj_rev[inp], inp=inp)
                 )
 
             if self.flow.connected_output(inp) == out:
                 # if the exact connection exists, we want to remove it by command
-                self._push_undo(
+                self.push_undo(
                     ConnectPorts_Command(self, out=self.flow.connected_output(inp), inp=inp)
                 )
             else:
-                self._push_undo(
-                    ConnectPorts_Command(self, out=out, inp=inp)
-                )
+                self.push_undo(ConnectPorts_Command(self, out=out, inp=inp))
 
     def add_connection(self, c: Tuple[NodeOutput, NodeInput]):
         out, inp = c
 
-        #TODO: need to verify that connection_items_cache still works fine with new connection object
-        item: ConnectionItem = None
+        # TODO: need to verify that connection_items_cache still works fine with new connection object
+        item: ConnectionItem
         if c in self.connection_items__cache.keys():
             item = self.connection_items__cache[c]
-
         else:
             if inp.type_ == 'data':
                 # item = self.CLASSES['data conn item'](c, self.session.design)
                 item = DataConnectionItem(c, self.session_gui.design)
             else:
                 # item = self.CLASSES['exec conn item'](c, self.session.design)
                 item = ExecConnectionItem(c, self.session_gui.design)
 
         self._add_connection_item(item)
 
         item.out_item.port_connected()
         item.inp_item.port_connected()
+        # for updating the visual state
+        for i in c:
+            self.node_items[i.node].update()
 
     def _add_connection_item(self, item: ConnectionItem):
+        self._set_selection_mode(_SelectionMode.INSTANT)
         self.connection_items[item.connection] = item
         self.scene().addItem(item)
-        item.setZValue(10)
+        item.recompute()
+        item.setZValue(-1)
         # self.viewport().repaint()
 
     def remove_connection(self, c: Tuple[NodeOutput, NodeInput]):
         item = self.connection_items[c]
         self._remove_connection_item(item)
 
         item.out_item.port_disconnected()
         item.inp_item.port_disconnected()
-
+        # for updating the visual state
+        for i in c:
+            self.node_items[i.node].update()
         del self.connection_items[c]
 
     def _remove_connection_item(self, item: ConnectionItem):
+        self._set_selection_mode(_SelectionMode.INSTANT)
         self.connection_items__cache[item.connection] = item
         self.scene().removeItem(item)
 
     def auto_connect(self, p: NodePort, n: Node):
         if p.io_pos == PortObjPos.OUTPUT:
             for inp in n.inputs:
                 if p.type_ == inp.type_:
@@ -962,17 +1161,18 @@
     # DRAWINGS
     def create_drawing(self, data=None) -> DrawingObject:
         """Creates and returns a new DrawingObject."""
 
         new_drawing = DrawingObject(self, data)
         return new_drawing
 
-    def add_drawing(self, drawing_obj, posF=None):
+    def add_drawing(self, drawing_obj: DrawingObject, posF=None):
         """Adds a DrawingObject to the scene."""
 
+        self._set_selection_mode(_SelectionMode.INSTANT)
         self.scene().addItem(drawing_obj)
         if posF:
             drawing_obj.setPos(posF)
         self.drawings.append(drawing_obj)
 
     def add_drawings(self, drawings):
         """Adds a list of DrawingObjects to the scene."""
@@ -980,15 +1180,15 @@
         for d in drawings:
             self.add_drawing(d)
 
     def remove_drawing(self, drawing: DrawingObject):
         """Removes a drawing from the scene."""
 
         # TODO https://github.com/leon-thomm/ryvencore/issues/4
-
+        self._set_selection_mode(_SelectionMode.INSTANT)
         self.scene().removeItem(drawing)
         self.drawings.remove(drawing)
 
     def place_drawings_from_data(self, drawings_data: list, offset_pos=QPoint(0, 0)):
         """Creates and places drawings from drawings. The same list is returned by the data_() method
         at 'drawings'."""
 
@@ -1001,164 +1201,210 @@
             new_drawings.append(new_drawing)
 
         return new_drawings
 
     def _create_and_place_drawing__cmd(self, posF, data=None):
         new_drawing_obj = self.create_drawing(data)
         place_command = PlaceDrawing_Command(self, posF, new_drawing_obj)
-        self._push_undo(place_command)
+        self.push_undo(place_command)
         return new_drawing_obj
 
     # ADDING/REMOVING COMPONENTS
     def add_component(self, e: QGraphicsItem):
         if isinstance(e, NodeItem):
             self.add_node(e.node)
-            self.add_node_item(e)
         elif isinstance(e, DrawingObject):
             self.add_drawing(e)
 
-    def remove_components(self, comps: [QGraphicsItem]):
+    def remove_components(self, comps: List[QGraphicsItem]):
         for c in comps:
             self.remove_component(c)
 
     def remove_component(self, e: QGraphicsItem):
         if isinstance(e, NodeItem):
             self.remove_node(e.node)
-            self.remove_node_item(e)
         elif isinstance(e, DrawingObject):
             self.remove_drawing(e)
 
     def remove_selected_components__cmd(self):
-        self._push_undo(
-            RemoveComponents_Command(self, self.scene().selectedItems())
-        )
+        if self._current_selected:
+            self.push_undo(RemoveComponents_Command(self, self._current_selected))
 
         self.viewport().update()
 
     # MOVING COMPONENTS
-    def _move_selected_copmonents__cmd(self, x, y):
-        new_rel_pos = QPointF(x, y)
+    def _move_selected_copmonents__cmd(self, pos_diff: QPointF, already_moved=False):
 
         # if one node item would leave the scene (f.ex. pos.x < 0), stop
         left = False
         for i in self.scene().selectedItems():
-            new_pos = i.pos() + new_rel_pos
+            new_pos = i.pos() + pos_diff
             w = i.boundingRect().width()
             h = i.boundingRect().height()
-            if new_pos.x() - w / 2 < 0 or \
-                    new_pos.x() + w / 2 > self.scene().width() or \
-                    new_pos.y() - h / 2 < 0 or \
-                    new_pos.y() + h / 2 > self.scene().height():
+            if (
+                new_pos.x() - w / 2 < 0
+                or new_pos.x() + w / 2 > self.scene().width()
+                or new_pos.y() - h / 2 < 0
+                or new_pos.y() + h / 2 > self.scene().height()
+            ):
                 left = True
                 break
 
         if not left:
             # moving the items
-            items_group = self.scene().createItemGroup(self.scene().selectedItems())
-            items_group.moveBy(new_rel_pos.x(), new_rel_pos.y())
-            self.scene().destroyItemGroup(items_group)
+            if not already_moved:
+                items_group = self.scene().createItemGroup(self.scene().selectedItems())
+                items_group.moveBy(pos_diff.x(), pos_diff.y())
+                self.scene().destroyItemGroup(items_group)
 
             # saving the command
-            self._push_undo(
-                MoveComponents_Command(self, self.scene().selectedItems(), p_from=-new_rel_pos, p_to=QPointF(0, 0))
+            self.push_undo(
+                MoveComponents_Command(
+                    self,
+                    self.scene().selectedItems(),
+                    p_from=-pos_diff,
+                    p_to=QPointF(0, 0),
+                )
             )
 
         self.viewport().repaint()
 
     def _move_selected_comps_left(self):
-        self._move_selected_copmonents__cmd(-40, 0)
+        self._move_selected_copmonents__cmd(QPointF(-40, 0))
 
     def _move_selected_comps_up(self):
-        self._move_selected_copmonents__cmd(0, -40)
+        self._move_selected_copmonents__cmd(QPointF(0, -40))
 
     def _move_selected_comps_right(self):
-        self._move_selected_copmonents__cmd(+40, 0)
+        self._move_selected_copmonents__cmd(QPointF(+40, 0))
 
     def _move_selected_comps_down(self):
-        self._move_selected_copmonents__cmd(0, +40)
+        self._move_selected_copmonents__cmd(QPointF(0, +40))
 
     # SELECTION
-    def selected_components_moved(self, pos_diff):
-        items_list = self.scene().selectedItems()
+    def _scene_selection_changed(self):
+        if self.selection_mode == _SelectionMode.INSTANT:
+            self._current_selected = self.scene().selectedItems()
+            self.emit_selected_items()
+        elif self.selection_mode == _SelectionMode.UNDOABLE_CLICK:
+            self._select__cmd()
 
-        self._push_undo(
-            MoveComponents_Command(self, items_list, p_from=-pos_diff, p_to=QPointF(0, 0))
-        )
+    def _watch_scene_selection(self):
+        self.scene().selectionChanged.connect(self._scene_selection_changed)
+
+    def _unwatch_scene_selection(self):
+        self.scene().selectionChanged.disconnect(self._scene_selection_changed)
+
+    def emit_selected_items(self):
+        """Emits signals indicating selection changes."""
+
+        self.nodes_selection_changed.emit(self.selected_nodes())
+
+    def _set_selection_mode(self, mode: _SelectionMode):
+        self.selection_mode = mode
+
+    def _select__cmd(self):
+        items = self.scene().selectedItems()
+        if items != self._current_selected:
+            self.push_undo(
+                SelectComponents_Command(self, items, self._current_selected)
+            )
 
-    def selected_node_items(self) -> [NodeItem]:
+    def selected_node_items(self, item_list: Optional[List[NodeItem]] = None) -> List[NodeItem]:
         """Returns a list of the currently selected NodeItems."""
 
-        selected_NIs = []
-        for i in self.scene().selectedItems():
-            if isinstance(i, NodeItem):
-                selected_NIs.append(i)
-        return selected_NIs
+        search_list = item_list if item_list is not None else self.scene().selectedItems()
+        return [node_item for node_item in search_list if isinstance(node_item, NodeItem)]
 
-    def selected_nodes(self) -> [Node]:
-        return [item.node for item in self.selected_node_items()]
+    def selected_nodes(self, item_list: Optional[List[NodeItem]] = None) -> List[Node]:
+        """Returns a list of the currently selected nodes."""
+        
+        return [node_item.node for node_item in self.selected_node_items(item_list)]
 
-    def selected_drawings(self) -> [DrawingObject]:
+    def selected_drawings(self) -> List[DrawingObject]:
         """Returns a list of the currently selected drawings."""
 
-        selected_drawings = []
-        for i in self.scene().selectedItems():
-            if isinstance(i, DrawingObject):
-                selected_drawings.append(i)
-        return selected_drawings
+        return [
+            drawing
+            for drawing in self.scene().selectedItems()
+            if isinstance(drawing, DrawingObject)
+        ]
 
-    def select_all(self):
+    def select_items(self, items: list):
+        """
+        Selects a list of items in the scene.
+        It always clears the current selection
+        Does not cause any command to be pushed to the undo stack.
+        Emits signals indicating selection changes.
+        """
+        
+        self._unwatch_scene_selection()
+        self._current_selected = items
         for i in self.scene().items():
-            if i.ItemIsSelectable:
+            if i.flags() & QGraphicsItem.ItemIsSelectable != 0:
+                i.setSelected(False)
+                
+        for i in items:
+            if i.flags() & QGraphicsItem.ItemIsSelectable != 0:
                 i.setSelected(True)
+        self.emit_selected_items()
         self.viewport().repaint()
+        self._watch_scene_selection()
 
-    def clear_selection(self):
-        self.scene().clearSelection()
+    def select_all(self):
+        self.select_items(self.scene().items())
 
-    def select_components(self, comps):
-        self.scene().clearSelection()
-        for c in comps:
-            c.setSelected(True)
+    def clear_selection(self):
+        self.select_items([])
 
     # ACTIONS
+    def _select_all_action(self):  # ctrl+a
+        all_items = self.scene().items()
+        if all_items != self._current_selected:
+            self.push_undo(SelectComponents_Command(self, all_items, self._current_selected))
+
     def _copy(self):  # ctrl+c
         data = {
             'nodes': self._get_nodes_data(self.selected_nodes()),
             'connections': self._get_connections_data(self.selected_nodes()),
             'output data': self._get_output_data(self.selected_nodes()),
-            'drawings': self._get_drawings_data(self.selected_drawings())
+            'drawings': self._get_drawings_data(self.selected_drawings()),
         }
         QGuiApplication.clipboard().setText(json.dumps(data))
 
     def _cut(self):  # ctrl+x
         data = {
             'nodes': self._get_nodes_data(self.selected_nodes()),
             'connections': self._get_connections_data(self.selected_nodes()),
-            'drawings': self._get_drawings_data(self.selected_drawings())
+            'drawings': self._get_drawings_data(self.selected_drawings()),
         }
         QGuiApplication.clipboard().setText(json.dumps(data))
         self.remove_selected_components__cmd()
 
-    def _paste(self):
+    def _paste(self):  # ctrl+v
         data = {}
         try:
             data = json.loads(QGuiApplication.clipboard().text())
         except Exception as e:
             return
 
         self.clear_selection()
 
         # calculate offset
         positions = []
         for d in data['drawings']:
-            positions.append({'x': d['pos x'],
-                              'y': d['pos y']})
+            positions.append({
+                'x': d['pos x'], 
+                'y': d['pos y']
+            })
         for n in data['nodes']:
-            positions.append({'x': n['pos x'],
-                              'y': n['pos y']})
+            positions.append({
+                'x': n['pos x'], 
+                'y': n['pos y']
+            })
 
         offset_for_middle_pos = QPointF(0, 0)
         if len(positions) > 0:
             rect = QRectF(positions[0]['x'], positions[0]['y'], 0, 0)
             for p in positions:
                 x = p['x']
                 y = p['y']
@@ -1169,24 +1415,24 @@
                 if y < rect.top():
                     rect.setTop(y)
                 if y > rect.bottom():
                     rect.setBottom(y)
 
             offset_for_middle_pos = self._last_mouse_move_pos - rect.center()
 
-        self._push_undo(
-            Paste_Command(self, data, offset_for_middle_pos)
-        )
+        self.push_undo(Paste_Command(self, data, offset_for_middle_pos))
 
     # DATA
-    def complete_data(self, data: dict):
-
+    def complete_data(self, data: Dict):
         data['flow view'] = {
             'drawings': self._get_drawings_data(self.drawings),
-            'view size': [self.sceneRect().size().width(), self.sceneRect().size().height()]
+            'view size': [
+                self.sceneRect().size().width(),
+                self.sceneRect().size().height(),
+            ],
         }
 
         return data
 
     def _get_nodes_data(self, nodes):
         """generates the data for the specified list of nodes"""
         f_complete_data = self.session_gui.core_session.complete_data
@@ -1202,7 +1448,43 @@
         f_complete_data = self.session_gui.core_session.complete_data
         return f_complete_data(self.flow._gen_output_data(nodes))
 
     def _get_drawings_data(self, drawings):
         """generates the data for a list of drawings"""
 
         return [d.data() for d in drawings]
+
+    def save_state(self) -> dict:
+        """Save the state of the view in a json-compliant dict"""
+        transform = self.transform()
+        return {
+            'm11': transform.m11(),  # Horizontal scaling
+            'm12': transform.m12(),  # Horizontal shearing
+            'm13': transform.m13(),  # Horizontal projection
+            'm21': transform.m21(),  # Vertical shearing
+            'm22': transform.m22(),  # Vertical scaling
+            'm23': transform.m23(),  # Vertical projection
+            'm31': transform.m31(),  # Horizontal translation
+            'm32': transform.m32(),  # Vertical translation
+            'm33': transform.m33(),  # Perspective division
+            'v_scroll': self.horizontalScrollBar().value(),
+            'h_scroll': self.verticalScrollBar().value(),
+        }
+    
+    def load(self, state: Dict):
+        """Load the state of the view"""
+        transform = QTransform(
+            state['m11'], state['m12'], state['m13'],
+            state['m21'], state['m22'], state['m23'],
+            state['m31'], state['m32'], state['m33']
+        )
+        
+        self.setTransform(transform)
+        self.horizontalScrollBar().setValue(state['v_scroll'])
+        self.verticalScrollBar().setValue(state['h_scroll'])
+        
+        self._loaded_state = state
+    
+    def reload(self):
+        if self._loaded_state is not None:
+            self.load(self._loaded_state)
+
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/FlowViewZoomWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/FlowViewZoomWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/connections/ConnectionItem.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/connections/ConnectionItem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,119 @@
 # import math
-from qtpy.QtCore import QMarginsF
-from qtpy.QtCore import QRectF, QPointF, Qt
+from typing import List, Any, Tuple
+from qtpy.QtCore import QPointF, Qt
 from qtpy.QtGui import QPainter, QColor, QRadialGradient, QPainterPath, QPen
-from qtpy.QtWidgets import QGraphicsPathItem, QGraphicsItem, QStyleOptionGraphicsItem
+from qtpy.QtWidgets import (
+    QGraphicsPathItem,
+    QGraphicsItem,
+    QStyleOptionGraphicsItem,
+    QGraphicsEllipseItem,
+)
 
 from ...GUIBase import GUIBase
 from ...utils import sqrt
 from ...utils import pythagoras
+from ...flows.nodes.PortItem import PortItem
+from .ConnectionAnimation import ConnPathItemsAnimation, ConnPathItemsAnimationScaled
+
+from ryvencore_qt.src.Design import Design
+from ryvencore.NodePort import NodeInput, NodeOutput
 
 
 class ConnectionItem(GUIBase, QGraphicsPathItem):
     """The GUI representative for a connection. The classes ExecConnectionItem and DataConnectionItem will be ready
     for reimplementation later, so users can add GUI for the enhancements of DataConnection and ExecConnection,
     like input fields for weights."""
 
-    def __init__(self, connection, session_design):
+    def __init__(self, connection: Tuple[NodeOutput, NodeInput], session_design: Design):
         QGraphicsPathItem.__init__(self)
 
         self.setAcceptHoverEvents(True)
 
         self.connection = connection
         out, inp = self.connection
 
         out_port_index = out.node.outputs.index(out)
         inp_port_index = inp.node.inputs.index(inp)
-        self.out_item = out.node.gui.item.outputs[out_port_index]
-        self.inp_item = inp.node.gui.item.inputs[inp_port_index]
+        assert hasattr(out.node, 'gui') and hasattr(inp.node, 'gui')
+        self.out_item: PortItem = out.node.gui.item.outputs[out_port_index]
+        self.inp_item: PortItem = inp.node.gui.item.inputs[inp_port_index]
 
         self.session_design = session_design
         self.session_design.flow_theme_changed.connect(self.recompute)
         self.session_design.performance_mode_changed.connect(self.recompute)
 
         # for rendering flow pictures
         self.setCacheMode(QGraphicsItem.DeviceCoordinateCache)
+        self.setFlag(QGraphicsItem.ItemIsSelectable)
+
+        diam = 12.5
+        self.num_dots = 40
+        self.dots = [
+            QGraphicsEllipseItem(-diam / 2, -diam / 2, diam, diam, self) 
+            for _ in range(self.num_dots)
+        ]
+        for dot in self.dots:
+            dot.setVisible(False)
+
+        # TODO: the connection animation is currently unused because we need a 
+        #       signel for when the node output is updated
+        self.items_path_animation = ConnPathItemsAnimation(self.dots, self)
+        self.connection_animation = ConnPathItemsAnimationScaled(self.items_path_animation)
 
         self.recompute()
 
-    def recompute(self):
-        """Updates scene position and recomputes path, pen and gradient"""
+    def __str__(self):
+        out, inp = self.connection
+        node_in_name = f'{inp.node.gui.item}'
+        node_in_index = inp.node.inputs.index(inp)
+        node_out_name = f'{out.node.gui.item}'
+        node_out_index = out.node.outputs.index(out)
+        return f'{node_out_index}->{node_in_index} ({node_out_name}, {node_in_name})'
+
+    def paint(self, painter: QPainter, option: QStyleOptionGraphicsItem, widget = None):
+        # draw path
+        painter.setBrush(self.brush())
+        painter.setPen(self.pen())
+        painter.drawPath(self.path())
+        # return super().paint(painter, option, widget)
+
+    def recompute(self) -> None:
+        """Updates scene position and recomputes path, pen, gradient and dots"""
+
+        # dots
+        self.items_path_animation.recompute()
 
         # position
         self.setPos(self.out_pos())
 
         # path
-        self.setPath(
-            self.connection_path(
-                QPointF(0, 0),
-                self.inp_pos()-self.scenePos()
-            )
-        )
+        p1: QPointF = QPointF(self.out_item.pin.width_no_padding() * 0.5, 0)
+        p2: QPointF = self.inp_pos() - self.scenePos() - QPointF(self.inp_item.pin.width_no_padding() * 0.5, 0)
+        self.setPath(self.connection_path(p1, p2))
 
         # pen
-        pen = self.get_pen()
+        pen: QPen = self.get_pen()
 
         # brush
         self.setBrush(Qt.NoBrush)
 
         #   gradient
         if self.session_design.performance_mode == 'pretty':
             c = pen.color()
             w = self.path().boundingRect().width()
             h = self.path().boundingRect().height()
             gradient = QRadialGradient(
-                self.boundingRect().center(),
+                self.boundingRect().center(), 
                 pythagoras(w, h) / 2
             )
 
-            c_r = c.red()
-            c_g = c.green()
-            c_b = c.blue()
+            c_r: int = c.red()
+            c_g: int = c.green()
+            c_b: int = c.blue()
 
             # this offset will be 1 if inp.x >> out.x and 0 if inp.x < out.x
             # hence, no fade for the gradient if the connection goes backwards
             offset_mult: float = max(
                 0,
                 min(
                     (self.inp_pos().x() - self.out_pos().x()) / 200,
@@ -92,107 +133,126 @@
             gradient.setColorAt(0.0, QColor(c_r, c_g, c_b, 255))
             gradient.setColorAt(0.75, QColor(c_r, c_g, c_b, 255 - round(55 * offset_mult)))
             gradient.setColorAt(0.95, QColor(c_r, c_g, c_b, 255 - round(255 * offset_mult)))
 
             pen.setBrush(gradient)
 
         self.setPen(pen)
-    
+
     def out_pos(self) -> QPointF:
         """The current global scene position of the pin of the output port"""
 
         return self.out_item.pin.get_scene_center_pos()
-    
+
     def inp_pos(self) -> QPointF:
         """The current global scene position of the pin of the input port"""
 
         return self.inp_item.pin.get_scene_center_pos()
 
+    def itemChange(self, change, value):
+        if change == QGraphicsItem.ItemSelectedHasChanged or (
+            change == QGraphicsItem.ItemVisibleHasChanged and self.isVisible()
+        ):
+            self.set_highlighted(self.isSelected())
+        return QGraphicsItem.itemChange(self, change, value)
+
     def set_highlighted(self, b: bool):
         pen: QPen = self.pen()
 
         if b:
             pen.setWidthF(self.pen_width() * 2)
         else:
             pen.setWidthF(self.pen_width())
             self.recompute()
 
         self.setPen(pen)
 
     def get_pen(self) -> QPen:
-        pass
+        raise NotImplementedError
 
     def pen_width(self) -> int:
-        pass
+        raise NotImplementedError
+
+    def get_style_color(self):
+        raise NotImplementedError
 
     def flow_theme(self):
         return self.session_design.flow_theme
 
     def hoverEnterEvent(self, event):
         self.set_highlighted(True)
         super().hoverEnterEvent(event)
 
     def hoverLeaveEvent(self, event):
-        self.set_highlighted(False)
+        if not self.isSelected():
+            self.set_highlighted(False)
         super().hoverLeaveEvent(event)
 
+    # uncomment to test connection animation:
+    # 
+    # def mouseReleaseEvent(self, event) -> None:
+    #    self.connection_animation.toggle()
+        
     @staticmethod
     def dist(p1: QPointF, p2: QPointF) -> float:
         """Returns the diagonal distance between the points using pythagoras"""
 
-        dx = p2.x()-p1.x()
-        dy = p2.y()-p1.y()
+        dx = p2.x() - p1.x()
+        dy = p2.y() - p1.y()
         return sqrt((dx**2) + (dy**2))
 
-
     @staticmethod
     def connection_path(p1: QPointF, p2: QPointF) -> QPainterPath:
         """Returns the painter path for drawing the connection, using the usual cubic connection path by default"""
 
         return default_cubic_connection_path(p1, p2)
 
 
 class ExecConnectionItem(ConnectionItem):
-
     def pen_width(self):
         return self.flow_theme().exec_conn_width
 
     def get_pen(self):
         theme = self.flow_theme()
         pen = QPen(theme.exec_conn_color, theme.exec_conn_width)
         pen.setStyle(theme.exec_conn_pen_style)
         pen.setCapStyle(Qt.RoundCap)
         return pen
 
+    def get_style_color(self):
+        return self.flow_theme().exec_conn_color
 
-class DataConnectionItem(ConnectionItem):
 
+class DataConnectionItem(ConnectionItem):
     def pen_width(self):
         return self.flow_theme().data_conn_width
 
     def get_pen(self):
         theme = self.flow_theme()
         pen = QPen(theme.data_conn_color, theme.data_conn_width)
         pen.setStyle(theme.data_conn_pen_style)
         pen.setCapStyle(Qt.RoundCap)
         return pen
 
+    def get_style_color(self):
+        return self.flow_theme().data_conn_color
 
-def default_cubic_connection_path(p1: QPointF, p2: QPointF):
+
+def default_cubic_connection_path(p1: QPointF, p2: QPointF) -> QPainterPath:
     """Returns the nice looking QPainterPath from p1 to p2"""
 
     path = QPainterPath()
 
     path.moveTo(p1)
 
     dx = p2.x() - p1.x()
     adx = abs(dx)
     dy = p2.y() - p1.y()
     ady = abs(dy)
-    distance = sqrt((dx ** 2) + (dy ** 2))
+    distance = sqrt((dx**2) + (dy**2))
     x1, y1 = p1.x(), p1.y()
     x2, y2 = p2.x(), p2.y()
 
     if ((x1 < x2 - 30) or distance < 100) and (x1 < x2):
         # STANDARD FORWARD
         path.cubicTo(x1 + ((x2 - x1) / 2), y1,
                      x1 + ((x2 - x1) / 2), y2,
@@ -206,9 +266,9 @@
                      x2 - 100 - (x1 - x2) / 10, y2,
                      x2, y2)
     else:
         # STANDARD BACKWARDS
         path.cubicTo(x1 + 100 + (x1 - x2) / 3, y1,
                      x2 - 100 - (x1 - x2) / 3, y2,
                      x2, y2)
-    
+
     return path
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/drawings/DrawingObject.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/drawings/DrawingObject.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,78 @@
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from ..FlowView import FlowView
+
+from typing import Dict, Optional
+
 from qtpy.QtWidgets import QGraphicsItem
 from qtpy.QtGui import QPen, QPainter, QColor, QPainterPath
 from qtpy.QtCore import Qt, QRectF, QPointF, QLineF
-
-from ...utils import MovementEnum
-
+from ...utils import MovementEnum, generate_name
 
 class DrawingObject(QGraphicsItem):
     """GUI implementation for 'drawing objects' in the scene, written by hand using a stylus pen"""
 
-    def __init__(self, flow_view, load_data=None):
+    def __init__(self, flow_view: FlowView, load_data: Optional[Dict] = None):
         super(DrawingObject, self).__init__()
 
         self.setFlags(QGraphicsItem.ItemIsSelectable | QGraphicsItem.ItemIsMovable |
                       QGraphicsItem.ItemSendsScenePositionChanges)
         self.setAcceptHoverEvents(True)
         self.setCacheMode(QGraphicsItem.DeviceCoordinateCache)  # for rendering flow pictures
 
         self.flow_view = flow_view
         self.color = None
         self.base_stroke_weight = None
-        self.type = 'pen'  # so far the only available, but I already save it so I could add more types in the future
+        self.type_ = 'pen'  # so far the only available, but I already save it so I could add more types in the future
         self.points = []
         self.stroke_weights = []
         self.pen_stroke_weight = 0  # approx. avg of self.stroke_weights
         self.rect = None
-        self.path: QPainterPath = None
+        self.path: Optional[QPainterPath] = None
         self.width = -1
         self.height = -1
         self.finished = False
 
         # viewport_pos enables global floating points for precise pen positions
-        self.viewport_pos: QPointF = load_data['viewport pos'] if 'viewport pos' in load_data else None
+        self.viewport_pos: Optional[QPointF] = None
         # if the drawing gets loaded, its correct global floating pos is already correct (gets set by flow then)
 
         self.movement_state = None  # ugly - should get replaced later, see NodeItem, same issue
         self.movement_pos_from = None
 
-        if 'points' in load_data:
-            p_c = load_data['points']
-            for p in p_c:
-                if type(p) == list:
-                    x = p[0]
-                    y = p[1]
-                    w = p[2]
-                    self.points.append(QPointF(x, y))
-                    self.stroke_weights.append(w)
-                elif type(p) == dict:  # backwards compatibility
-                    x = p['x']
-                    y = p['y']
-                    w = p['w']
-                    self.points.append(QPointF(x, y))
-                    self.stroke_weights.append(w)
-            self.finished = True
-
-        self.color = QColor(load_data['color'])
-        self.base_stroke_weight = load_data['base stroke weight']
-
-
+        if load_data is not None: 
+            if 'viewport pos' in load_data:
+                self.viewport_pos = load_data['viewport pos']
+
+            if 'points' in load_data:
+                p_c = load_data['points']
+                for p in p_c:
+                    if type(p) == list:
+                        x = p[0]
+                        y = p[1]
+                        w = p[2]
+                        self.points.append(QPointF(x, y))
+                        self.stroke_weights.append(w)
+                    elif type(p) == dict:  # backwards compatibility
+                        x = p['x']
+                        y = p['y']
+                        w = p['w']
+                        self.points.append(QPointF(x, y))
+                        self.stroke_weights.append(w)
+                self.finished = True
+
+            self.color = QColor(load_data['color'])
+            self.base_stroke_weight = load_data['base stroke weight']
+
+    def __str__(self):
+        return generate_name(self, 'Drawing')
+    
     def paint(self, painter, option, widget=None):
 
         if not self.finished:
             for i in range(1, len(self.points)):
                 pen = QPen()
                 pen.setColor(self.color)
                 pen_width = (self.stroke_weights[i] + 0.2) * self.base_stroke_weight
@@ -172,24 +184,27 @@
         self.movement_pos_from = self.pos()
         return QGraphicsItem.mousePressEvent(self, event)
 
     def mouseReleaseEvent(self, event):
         """Used for Moving-Commands in Flow - may be replaced later with a nicer determination of a move action."""
 
         if self.movement_state == MovementEnum.position_changed:
-            self.flow_view.selected_components_moved(self.pos() - self.movement_pos_from)
+            self.flow_view._move_selected_copmonents__cmd(
+                pos_diff=self.pos() - self.movement_pos_from,
+                already_moved=True,
+            )
         self.movement_state = None
         return QGraphicsItem.mouseReleaseEvent(self, event)
 
     def data_(self):
         drawing_dict = {
             'pos x': self.pos().x(),
             'pos y': self.pos().y(),
             'color': self.color.name(),
-            'type': self.type,
+            'type': self.type_,
             'base stroke weight': self.base_stroke_weight
         }
         points_list = []
         for i in range(len(self.points)):
             p = self.points[i]
             points_list.append([p.x(), p.y(), self.stroke_weights[i]])
         drawing_dict['points'] = points_list
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 import json
 
 from qtpy.QtWidgets import QLineEdit, QWidget, QLabel, QGridLayout, QHBoxLayout, QSpacerItem, QSizePolicy, QStyleOption, QStyle
 from qtpy.QtGui import QFont, QPainter, QColor, QDrag
-from qtpy.QtCore import Signal, Qt, QMimeData
+from qtpy.QtCore import Signal, Qt, QMimeData, QByteArray
 
 
 class NodeWidget(QWidget):
 
     chosen = Signal()
     custom_focused_from_inside = Signal()
 
+    @staticmethod
+    def _create_mime_data(node) -> QMimeData:
+        mime_data = QMimeData()
+        mime_data.setData('application/json', QByteArray(bytes(json.dumps(
+                {
+                    'type': 'node',
+                    'node identifier': node.identifier,
+                }
+            ), encoding='utf-8')))
+        return mime_data
+    
     def __init__(self, parent, node):
         super(NodeWidget, self).__init__(parent)
 
         self.custom_focused = False
         self.node = node
 
         self.left_mouse_pressed_on_me = False
@@ -96,15 +107,14 @@
         f'background-color: rgba(255,255,255,80);'
     ) if self.custom_focused else ''}
 }}
 QLabel {{
     background: transparent;
 }}
 QLineEdit {{
-    color: white;
     background: transparent;
     border: none;
     padding: 2px;
 }}
         '''
 
         self.setStyleSheet(new_style_sheet)
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/node_list_widget/utils.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/node_list_widget/utils.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeGUI.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeGUI.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from queue import Queue
-from typing import List, Dict, Tuple, Optional, Union
+from typing import List, Dict, Tuple, Optional, Union, Type
 
 from qtpy.QtCore import QObject, Signal
 
+from .WidgetBaseClasses import NodeMainWidget, NodeInputWidget, NodeInspectorWidget
+from .NodeInspector import NodeInspectorDefaultWidget
+
 
 class NodeGUI(QObject):
     """
     Interface class between nodes and their GUI representation.
     """
 
     # customizable gui attributes
-    description_html: str = None
-    main_widget_class: list = None
+    description_html: Optional[str] = None
+    main_widget_class: Optional[Type[NodeMainWidget]] = None
     main_widget_pos: str = 'below ports'
-    input_widget_classes: dict = {}
+    input_widget_classes: Dict[str, Type[NodeInputWidget]] = {}
+    inspector_widget_class: Type[NodeInspectorWidget] = NodeInspectorDefaultWidget
+    wrap_inspector_in_default: bool = False
     init_input_widgets: dict = {}
     style: str = 'normal'
     color: str = '#c69a15'
-    display_title: str = None
-    icon: str = None
+    display_title: Optional[str] = None
+    icon: Optional[str] = None
 
     # qt signals
     updating = Signal()
     update_error = Signal(object)
     input_added = Signal(int, object)
     output_added = Signal(int, object)
     input_removed = Signal(int, object)
@@ -58,14 +63,24 @@
         self.node.updating.sub(self._on_updating)
         self.node.update_error.sub(self._on_update_error)
         self.node.input_added.sub(self._on_new_input_added)
         self.node.output_added.sub(self._on_new_output_added)
         self.node.input_removed.sub(self._on_input_removed)
         self.node.output_removed.sub(self._on_output_removed)
 
+        # create the inspector widget
+        inspector_params = (self.node, self)
+        if self.wrap_inspector_in_default:
+            self.inspector_widget = NodeInspectorDefaultWidget(
+                child=self.inspector_widget_class((self.node, self)),
+                params=inspector_params,
+            )
+        else:
+            self.inspector_widget = self.inspector_widget_class(inspector_params)
+
     def initialized(self):
         """
         *VIRTUAL*
 
         Called after the node GUI has been fully initialized.
         The Node has been created already (including all ports) and loaded.
         No connections have been made to ports of the node yet.
@@ -179,24 +194,26 @@
     serialization
     """
 
     def data(self):
         return {
             'actions': self._serialize_actions(self.actions),
             'display title': self.display_title,
+            'inspector widget': self.inspector_widget.get_state(),
         }
 
     def load(self, data):
         if 'actions' in data:   # otherwise keep default
             self.actions = self._deserialize_actions(data['actions'])
         if 'display title' in data:
             self.display_title = data['display title']
-
         if 'special actions' in data:   # backward compatibility
             self.actions = self._deserialize_actions(data['special actions'])
+        if 'inspector widget' in data:
+            self.inspector_widget.set_state(data['inspector widget'])
 
     """
     GUI access methods
     """
 
     def set_display_title(self, t: str):
         self.display_title = t
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,60 @@
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from ..FlowView import FlowView
+
 import traceback
-from typing import Optional, Tuple
+from typing import Optional, Tuple, List
 
 from qtpy.QtWidgets import QGraphicsItem, QGraphicsObject, QMenu, QGraphicsDropShadowEffect
 from qtpy.QtCore import Qt, QRectF, QObject, QPointF
 from qtpy.QtGui import QColor
 
 from .NodeErrorIndicator import NodeErrorIndicator
 from .NodeGUI import NodeGUI
 from ...GUIBase import GUIBase
-from ryvencore.NodePort import NodeInput, NodeOutput
 from .NodeItemAction import NodeItemAction
 from .NodeItemAnimator import NodeItemAnimator
 from .NodeItemWidget import NodeItemWidget
 from .PortItem import InputPortItem, OutputPortItem
-from ...utils import serialize, deserialize
-from ...utils import MovementEnum
+from ...utils import serialize, deserialize, MovementEnum, generate_name
+
+from ryvencore_qt.src.Design import Design
+
+from ryvencore import Node
+from ryvencore.NodePort import NodeInput, NodeOutput
 
 
 class NodeItem(GUIBase, QGraphicsObject):  # QGraphicsItem, QObject):
     """The GUI representative for nodes. Unlike the Node class, this class is not subclassed individually and works
     the same for every node."""
 
-    def __init__(self, node, node_gui, flow_view, design):
+    def __init__(self, node: Node, node_gui: NodeGUI, flow_view: FlowView, design: Design):
         GUIBase.__init__(self, representing_component=node)
         QGraphicsObject.__init__(self)
 
         self.node = node
         self.node_gui = node_gui
         self.node_gui.item = self
         self.flow_view = flow_view
-        self.session_design = design
-        self.movement_state = None
-        self.movement_pos_from = None
-        self.painted_once = False
-        self.inputs = []
-        self.outputs = []
+        self.session_design: Design = design
+        self.movement_state: Optional[MovementEnum] = None
+        self.movement_pos_from: Optional[QPointF] = None
+        self.painted_once: bool = False
+        self.inputs: List[InputPortItem] = []
+        self.outputs: List[OutputPortItem] = []
         self.color = QColor(self.node_gui.color)  # manipulated by self.animator
 
         self.collapsed = False
         self.hovered = False
         self.hiding_unconnected_ports = False
         self.displaying_error = False
 
-        self.personal_logs = []
-
         # 'initializing' will be set to False below. It's needed for the ports setup, to prevent shape updating stuff
         self.initializing = True
 
         # self.temp_state_data = None
         self.init_data = self.node.load_data
 
         # CONNECT TO NODE
@@ -129,14 +136,19 @@
         # self.update_shape() gets called when the item is being drawn the first time (see paint event in NI painter)
         # https://forum.qt.io/topic/117179/force-qgraphicsitem-to-update-immediately-wait-for-update-event
 
         self.update_design()  # load current design, update QGraphicsItem
 
         self.update()  # ... not sure if I need that
 
+    def __str__(self):
+        name = self.node.__class__.title if self.node else f'{NodeItem.__name__}'
+        obj = self.node if self.node else self
+        return generate_name(obj, name)
+    
     # UI STUFF
 
     def node_updating(self):
         if self.session_design.animations_enabled:
             if not self.animator.running():
                 self.animator.start()
             elif self.animator.fading_out():
@@ -168,15 +180,15 @@
         self.setToolTip(html)
         self.setCursor(Qt.SizeAllCursor)
 
     def on_node_input_added(self, index, inp: NodeInput):
         insert = index if index == len(self.node.inputs) - 1 else None
         self.add_new_input(inp, insert)
 
-    def add_new_input(self, inp: NodeInput, insert: int = None):
+    def add_new_input(self, inp: NodeInput, insert: Optional[int] = None):
 
         if inp in self.node_gui.input_widgets:
             widget_name = self.node_gui.input_widgets[inp]['name']
             widget_class = self.node_gui.input_widget_classes[widget_name]
             widget_pos = self.node_gui.input_widgets[inp]['pos']
             widget = (widget_class, widget_pos)
         else:
@@ -196,19 +208,21 @@
             self.update_shape()
             self.update()
 
     def on_node_input_removed(self, index, inp: NodeInput):
         self.remove_input(inp)
 
     def remove_input(self, inp: NodeInput):
-        item = None
+        item: InputPortItem
         for inp_item in self.inputs:
             if inp_item.port == inp:
                 item = inp_item
                 break
+        else:
+            return
 
         # index = self.node.inputs.index(inp)
         # item = self.inputs[index]
 
         # for some reason, I have to remove all widget items manually from the scene too. setting the items to
         # ownedByLayout(True) does not work, I don't know why.
         self.scene().removeItem(item.pin)
@@ -223,15 +237,15 @@
             self.update_shape()
             self.update()
 
     def on_node_output_added(self, index, out: NodeOutput):
         insert = index if index == len(self.node.outputs) - 1 else None
         self.add_new_output(out, insert)
 
-    def add_new_output(self, out: NodeOutput, insert: int = None):
+    def add_new_output(self, out: NodeOutput, insert: Optional[int] = None):
 
         # create item
         # out.item = OutputPortItem(out.node, self, out)
         item = OutputPortItem(self.node_gui, self, out)
 
         if insert is not None:
             self.outputs.insert(insert, item)
@@ -244,19 +258,21 @@
             self.update_shape()
             self.update()
 
     def on_node_output_removed(self, index, out: NodeOutput):
         self.remove_output(out)
 
     def remove_output(self, out: NodeOutput):
-        item = None
+        item: OutputPortItem
         for out_item in self.outputs:
             if out_item.port == out:
                 item = out_item
                 break
+        else:
+            return
 
         # index = self.node.outputs.index(out)
         # item = self.outputs[index]
 
         # see remove_input() for info!
         self.scene().removeItem(item.pin)
         self.scene().removeItem(item.label)
@@ -298,23 +314,25 @@
         h = self.widget.layout().geometry().height()
         rect.setLeft(-w / 2)
         rect.setTop(-h / 2)
         rect.setWidth(w)
         rect.setHeight(h)
         return rect
 
-    def get_left_body_header_vertex_scene_pos(self):
+    def get_left_body_header_vertex_scene_pos(self) -> QPointF:
+        assert self.widget.header_widget is not None
         return self.mapToScene(
             QPointF(
                 -self.boundingRect().width() / 2,
                 -self.boundingRect().height() / 2 + self.widget.header_widget.rect().height()
             )
         )
 
-    def get_right_body_header_vertex_scene_pos(self):
+    def get_right_body_header_vertex_scene_pos(self) -> QPointF:
+        assert self.widget.header_widget is not None
         return self.mapToScene(
             QPointF(
                 +self.boundingRect().width() / 2,
                 -self.boundingRect().height() / 2 + self.widget.header_widget.rect().height()
             )
         )
 
@@ -420,14 +438,17 @@
             if self.movement_state == MovementEnum.mouse_clicked:
                 self.movement_state = MovementEnum.position_changed
 
             self.update_conn_pos()
 
         return QGraphicsItem.itemChange(self, change, value)
 
+    def on_move(self):
+        self.update_conn_pos()
+    
     def update_conn_pos(self):
         """Updates the scene positions of connections"""
 
         for o in self.node.outputs:
             for i in self.node.flow.connected_inputs(o):
                 # c.item.recompute()
 
@@ -472,15 +493,18 @@
 
     def mouseReleaseEvent(self, event):
         """Used for Moving-Commands in FlowView - may be replaced later by a nicer determination of a moving action."""
 
         self.flow_view.mouse_event_taken = True
 
         if self.movement_state == MovementEnum.position_changed:
-            self.flow_view.selected_components_moved(self.pos() - self.movement_pos_from)
+            self.flow_view._move_selected_copmonents__cmd(
+                pos_diff=self.pos() - self.movement_pos_from,
+                already_moved=True,
+            )
         self.movement_state = None
         return QGraphicsItem.mouseReleaseEvent(self, event)
 
     # ACTIONS
 
     def get_actions(self, actions_dict, menu):
         actions = []
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItemAction.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItemAction.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,53 @@
-from qtpy.QtCore import QObject, QPropertyAnimation, Property
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .NodeItem import NodeItem
+
+from qtpy.QtCore import QObject, QPropertyAnimation, Property, QParallelAnimationGroup, QTimeLine
 from qtpy.QtGui import QColor
 from qtpy.QtWidgets import QGraphicsItem
 
-
 class NodeItemAnimator(QObject):
 
-    def __init__(self, node_item):
+    def __init__(self, node_item: NodeItem):
         super(NodeItemAnimator, self).__init__()
 
-        self.node_item = node_item
+        self.node_item: QGraphicsItem = node_item
         self.animation_running = False
 
-        self.title_activation_animation = QPropertyAnimation(self, b"p_title_color")
+        # title color
+        self.title_activation_animation = QPropertyAnimation(self, b"p_title_color")  # type: ignore
         self.title_activation_animation.setDuration(700)
-        self.title_activation_animation.finished.connect(self.finished)
-        self.body_activation_animation = QPropertyAnimation(self, b"p_body_color")
+        # body color
+        self.body_activation_animation = QPropertyAnimation(self, b"p_body_color")  # type: ignore
         self.body_activation_animation.setDuration(700)
+        # transform
+        self.scale_animation = QPropertyAnimation(self.node_item, b'scale')  # type: ignore
+        self.scale_animation.setDuration(700)
+        self.scalar = 1.04
+        
+        self.animation = QParallelAnimationGroup()
+        self.animation.addAnimation(self.title_activation_animation)
+        self.animation.addAnimation(self.body_activation_animation)
+        self.animation.addAnimation(self.scale_animation)
+        self.animation.finished.connect(self.finished)
 
     def start(self):
         self.animation_running = True
-        self.title_activation_animation.start()
-        self.body_activation_animation.start()
+        self.animation.start()
 
     def stop(self):
         # reset color values. it would just freeze without
         self.title_activation_animation.setCurrentTime(self.title_activation_animation.duration())
         self.body_activation_animation.setCurrentTime(self.body_activation_animation.duration())
-
-        self.title_activation_animation.stop()
-        self.body_activation_animation.stop()
+        self.scale_animation.setCurrentTime(self.scale_animation.duration())
+        
+        self.animation.stop()
 
     def finished(self):
         self.animation_running = False
 
     def running(self):
         return self.animation_running
 
@@ -43,32 +58,37 @@
         self.title_activation_animation.setKeyValueAt(0, self.get_title_color())
         self.title_activation_animation.setKeyValueAt(0.3, self.get_body_color().lighter().lighter())
         self.title_activation_animation.setKeyValueAt(1, self.get_title_color())
 
         self.body_activation_animation.setKeyValueAt(0, self.get_body_color())
         self.body_activation_animation.setKeyValueAt(0.3, self.get_body_color().lighter())
         self.body_activation_animation.setKeyValueAt(1, self.get_body_color())
+        
+        self.scale_animation.setKeyValueAt(0, 1)
+        self.scale_animation.setKeyValueAt(0.3, self.scalar)
+        self.scale_animation.setKeyValueAt(1, 1)
 
     def fading_out(self):
         return self.title_activation_animation.currentTime()/self.title_activation_animation.duration() >= 0.3
 
     def set_animation_max(self):
         self.title_activation_animation.setCurrentTime(0.3*self.title_activation_animation.duration())
         self.body_activation_animation.setCurrentTime(0.3*self.body_activation_animation.duration())
 
+    # BODY COLOR
     def get_body_color(self):
         return self.node_item.color
 
     def set_body_color(self, val):
         self.node_item.color = val
         QGraphicsItem.update(self.node_item)
 
     p_body_color = Property(QColor, get_body_color, set_body_color)
 
-
+    # TITLE COLOR
     def get_title_color(self):
         return self.node_item.widget.title_label.color
 
     def set_title_color(self, val):
         self.node_item.widget.title_label.color = val
         # QGraphicsItem.update(self.node_item)
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItemWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItemWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,72 @@
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .NodeGUI import NodeGUI
+    from .NodeItem import NodeItem
+    from ..FlowView import FlowView
+
 from qtpy.QtCore import QPointF, QRectF, Qt, QSizeF
-from qtpy.QtWidgets import QGraphicsWidget, QGraphicsLinearLayout, QSizePolicy
+from qtpy.QtWidgets import QGraphicsWidget, QGraphicsLinearLayout, QSizePolicy, QWidget
+
+from typing import Optional
 
 from .NodeItem_CollapseButton import NodeItem_CollapseButton
 from ..FlowViewProxyWidget import FlowViewProxyWidget
 # from .Node import Node
 from .NodeItem_Icon import NodeItem_Icon
 from .NodeItem_TitleLabel import TitleLabel
 from .PortItem import InputPortItem, OutputPortItem
 
+from ryvencore import Flow
+
 
 class NodeItemWidget(QGraphicsWidget):
     """The QGraphicsWidget managing all GUI components of a NodeItem in widgets and layouts."""
 
-    def __init__(self, node_gui, node_item):
+    def __init__(self, node_gui: NodeGUI, node_item: NodeItem) -> None:
         super().__init__(parent=node_item)
 
-        self.node_gui = node_gui
-        self.node_item = node_item
-        self.flow_view = self.node_item.flow_view
-        self.flow = self.flow_view.flow
+        self.node_gui: NodeGUI = node_gui
+        self.node_item: NodeItem = node_item
+        self.flow_view: FlowView = self.node_item.flow_view
+        self.flow: Flow = self.flow_view.flow
 
         self.body_padding = 6
         self.header_padding = (0, 0, 0, 0)  # theme dependent and hence updated in setup_layout()!
 
         self.icon = NodeItem_Icon(node_gui, node_item) if node_gui.icon else None
-        self.collapse_button = NodeItem_CollapseButton(node_gui, node_item) if node_gui.style == 'normal' else None
         self.title_label = TitleLabel(node_gui, node_item)
-        self.main_widget_proxy: FlowViewProxyWidget = None
+        self.main_widget_proxy: Optional[FlowViewProxyWidget] = None
         if self.node_item.main_widget:
+            assert isinstance(self.node_item.main_widget, QWidget)
             self.main_widget_proxy = FlowViewProxyWidget(self.flow_view)
             self.main_widget_proxy.setWidget(self.node_item.main_widget)
-        self.header_layout: QGraphicsWidget = None
-        self.header_widget: QGraphicsWidget = None
-        self.body_layout: QGraphicsLinearLayout = None
-        self.body_widget: QGraphicsWidget = None
-        self.inputs_layout: QGraphicsLinearLayout = None
-        self.outputs_layout: QGraphicsLinearLayout = None
+        self.header_layout: Optional[QGraphicsWidget]
+        self.header_widget: Optional[QGraphicsWidget]
+        self.collapse_button: Optional[NodeItem_CollapseButton]
+        self.body_layout: QGraphicsLinearLayout
+        self.body_widget: QGraphicsWidget
+        self.inputs_layout: QGraphicsLinearLayout
+        self.outputs_layout: QGraphicsLinearLayout
         self.setLayout(self.setup_layout())
 
     def setup_layout(self) -> QGraphicsLinearLayout:
 
         self.header_padding = self.node_item.session_design.flow_theme.header_padding
 
         #   main layout
         layout = QGraphicsLinearLayout(Qt.Vertical)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
 
         if self.node_gui.style == 'normal':
+            self.collapse_button = NodeItem_CollapseButton(self.node_gui, self.node_item)
+
             self.header_widget = QGraphicsWidget()
             # self.header_widget.setContentsMargins(0, 0, 0, 0)
             self.header_widget.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
             self.header_layout = QGraphicsLinearLayout(Qt.Horizontal)
             self.header_layout.setSpacing(5)
             self.header_layout.setContentsMargins(
                 *self.header_padding
@@ -66,14 +81,17 @@
             self.header_layout.setAlignment(self.collapse_button, Qt.AlignVCenter | Qt.AlignRight)
 
             self.header_widget.setLayout(self.header_layout)
             # layout.addItem(self.header_layout)
             layout.addItem(self.header_widget)
             # layout.setAlignment(self.title_label, Qt.AlignTop)
         else:
+            self.collapse_button = None
+            self.header_widget = None
+            self.header_layout = None
             self.setZValue(self.title_label.zValue() + 1)
 
         #   inputs
         self.inputs_layout = QGraphicsLinearLayout(Qt.Vertical)
         self.inputs_layout.setSpacing(2)
 
         #   outputs
@@ -142,14 +160,16 @@
         # makes extended node items shrink according to resizing input widgets
         if not self.node_item.initializing:
             self.rebuild_ui()
         # strangely, this only works for small node items without this, not for normal ones
 
         mw = self.node_item.main_widget
         if mw is not None:  # maybe the main_widget got resized
+            assert self.main_widget_proxy is not None
+
             # self.main_widget_proxy.setMaximumSize(mw.size())
 
             # self.main_widget_proxy.setMaximumSize(mw.maximumSize())
 
             self.main_widget_proxy.setMaximumSize(QSizeF(mw.size()))
             self.main_widget_proxy.setMinimumSize(QSizeF(mw.size()))
 
@@ -187,14 +207,15 @@
                 self.title_label.setPos(
                     QPointF(-self.title_label.boundingRect().width() / 2,
                             -self.title_label.boundingRect().height() / 2)
                 )
 
 
     def add_main_widget_to_layout(self):
+        assert self.main_widget_proxy is not None
         if self.node_gui.main_widget_pos == 'between ports':
             self.body_layout.insertItem(1, self.main_widget_proxy)
             self.body_layout.insertStretch(2)
 
         elif self.node_gui.main_widget_pos == 'below ports':
             self.layout().addItem(self.main_widget_proxy)
             self.layout().setAlignment(self.main_widget_proxy, Qt.AlignHCenter)
@@ -235,20 +256,20 @@
 
         # just a temporary workaround for the issues discussed here:
         # https://forum.qt.io/topic/116268/qgraphicslayout-not-properly-resizing-to-change-of-content
         self.rebuild_ui()
 
     def collapse(self):
         self.body_widget.hide()
-        if self.main_widget_proxy:
+        if self.main_widget_proxy is not None:
             self.main_widget_proxy.hide()
 
     def expand(self):
         self.body_widget.show()
-        if self.main_widget_proxy:
+        if self.main_widget_proxy is not None:
             self.main_widget_proxy.show()
 
     def hide_unconnected_ports(self):
         for inp in self.node_item.node.inputs:
             if self.flow.connected_output(inp) is None:
                 inp.hide()
         for out in self.node_item.node.outputs:
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/PortItem.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/PortItem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,52 @@
-from typing import Tuple
+# prevent circular imports
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from .NodeGUI import NodeGUI
+    from .NodeItem import NodeItem
+    from ..FlowView import FlowView
+
+from typing import Tuple, Optional
 
 from qtpy.QtWidgets import QGraphicsGridLayout, QGraphicsWidget, QGraphicsLayoutItem
 from qtpy.QtCore import Qt, QRectF, QPointF, QSizeF
 from qtpy.QtGui import QFontMetricsF, QFont
 
-from ...GUIBase import GUIBase
-from .PortItemInputWidgets import Data_IW_S, Data_IW_M, Data_IW_L, Float_IW, Integer_IW, \
-    Choice_IW, Boolean_IW, String_IW_S, String_IW_M, String_IW_L
 from ryvencore import serialize, Data
 from ryvencore.NodePort import NodeOutput, NodeInput, NodePort
 from ryvencore.utils import deserialize
-from ...utils import get_longest_line, shorten
 
+from ...GUIBase import GUIBase
+from ...utils import get_longest_line, shorten
 from ..FlowViewProxyWidget import FlowViewProxyWidget
-
+from .WidgetBaseClasses import NodeInputWidget
 
 # utils
 
 
 def is_connected(port):
     if isinstance(port, NodeOutput):
         is_connected = len(port.node.flow.connected_inputs(port)) > 0
     else:
         is_connected = port.node.flow.connected_output(port) is not None
     return is_connected
 
+
 def val(port):
     if isinstance(port, NodeOutput):
         return port.val.payload if isinstance(port.val, Data) else None
     else:
         conn_out = port.node.flow.connected_output(port)
         if conn_out:
             return conn_out.val.payload if conn_out.val is not None else None
         else:
             return None
 
+
 def connections(port):
     if isinstance(port, NodeOutput):
         return [(port, i) for i in port.node.flow.connected_inputs(port)]
     else:
         conn_out = port.node.flow.connected_output(port)
         if conn_out:
             return [(port.node.flow.connected_output(port), port)]
@@ -48,24 +56,24 @@
 
 # main classes
 
 
 class PortItem(GUIBase, QGraphicsWidget):
     """The GUI representative for ports of nodes, also handling mouse events for connections."""
 
-    def __init__(self, node_gui, node_item, port, flow_view):
+    def __init__(self, node_gui: NodeGUI, node_item: NodeItem, port: NodePort, flow_view: FlowView):
         GUIBase.__init__(self, representing_component=port)
         QGraphicsWidget.__init__(self)
 
         self.setGraphicsItem(self)
 
-        self.node_gui = node_gui
-        self.node_item = node_item
+        self.node_gui: NodeGUI = node_gui
+        self.node_item: NodeItem = node_item
         self.port: NodePort = port
-        self.flow_view = flow_view
+        self.flow_view: FlowView = flow_view
 
         # self.port.has_been_connected.connect(self.port_connected)
         # self.port.has_been_disconnected.connect(self.port_disconnected)
 
         self.pin = PortItemPin(self.port, self, self.node_gui, self.node_item)
 
         self.label = PortItemLabel(self.port, self, self.node_gui, self.node_item)
@@ -92,31 +100,39 @@
         pass
 
     def port_disconnected(self):
         pass
 
 
 class InputPortItem(PortItem):
-    def __init__(self, node_gui, node_item, port, input_widget: Tuple[type, str] = None):
+    def __init__(self, node_gui, node_item, port, input_widget: Optional[Tuple[type, str]] = None):
+        self.port: NodeInput
         super().__init__(node_gui, node_item, port, node_gui.flow_view())
 
-        self.proxy = None   # widget proxy
-        self.widget = None  # widget
+        self.proxy = None  # widget proxy
+        self.widget: Optional[NodeInputWidget] = None  # widget
         if input_widget is not None:
             self.create_widget(input_widget[0], input_widget[1])
 
-        self.update_widget_value = self.widget is not None  # modified by FlowView when performance mode changes
+        self.update_widget_value = (
+            self.widget is not None
+        )  # modified by FlowView when performance mode changes
 
         # catch up to missed connections
         if self.port.node.flow.connected_output(self.port) is not None:
             self.port_connected()
 
-        if self.port.type_ == 'data' and self.port.load_data is not None and self.port.load_data['has widget']:
+        if (
+            self.port.type_ == 'data'
+            and self.port.load_data is not None
+            and self.port.load_data['has widget']
+        ):
             c_d = self.port.load_data['widget data']
             if c_d is not None:
+                assert self.widget is not None
                 self.widget.set_state(deserialize(c_d))
             else:
                 # this is a little feature that lets us prevent loading of input widgets
                 # which is occasionally useful, e.g. when changing an input widget class:
                 # to prevent loading of the input widget, 'widget data' must be None
                 pass
 
@@ -137,15 +153,14 @@
                 l.addItem(self.proxy, 0, 2)
             else:
                 print('Unknown input widget position:', self.widget.position)
 
             l.setAlignment(self.proxy, Qt.AlignCenter)
 
     def create_widget(self, widget_class, widget_pos):
-
         if widget_class is None:
             return
 
         if self.port.type_ != 'data':
             # TODO: how about input widgets for exec inputs?
             return
 
@@ -246,87 +261,100 @@
         self.node_item.session_design.flow_theme.paint_PI(
             node_gui=self.node_gui,
             painter=painter,
             option=option,
             node_color=self.node_gui.color,
             type_=self.port.type_,
             connected=is_connected(self.port),
-            rect=QRectF(self.padding, self.padding, self.width-2*self.padding, self.height-2*self.padding)
+            rect=QRectF(
+                self.padding, self.padding, self.width_no_padding(), self.height_no_padding()
+            ),
         )
 
     def mousePressEvent(self, event):
         if event.button() == Qt.LeftButton:  # DRAG NEW CONNECTION
             self.flow_view.mouse_event_taken = True
             self.flow_view._selected_pin = self
             self.flow_view._dragging_connection = True
             event.accept()  # don't pass the ev ent to anything below
         else:
             return QGraphicsWidget.mousePressEvent(self, event)
 
-
     def moveEvent(self, event):
         super().moveEvent(event)
 
         # update connections
         conn_items = self.flow_view.connection_items
         for c in self.port.connections:
             i = conn_items[c]
 
             # if the items are grouped (which means they move together), don't recompute
             if i.out.group() is None or i.out.group() != i.inp.group():  # not entirely sure if this is working
                 i.recompute()
 
-
     def hoverEnterEvent(self, event):
         if self.port.type_ == 'data':  # and self.parent_port_instance.io_pos == PortPos.OUTPUT:
             self.setToolTip(shorten(str(val(self.port)), 1000, line_break=True))
 
         # highlight connections
         items = self.flow_view.connection_items
         for c in connections(self.port):
             items[c].set_highlighted(True)
 
         self.hovered = True
 
         QGraphicsWidget.hoverEnterEvent(self, event)
 
     def hoverLeaveEvent(self, event):
-
         # un-highlight connections
         items = self.flow_view.connection_items
         for c in connections(self.port):
             items[c].set_highlighted(False)
 
         self.hovered = False
 
         QGraphicsWidget.hoverLeaveEvent(self, event)
 
-    def get_scene_center_pos(self):
+    def width_no_padding(self):
+        """The width without the padding"""
+        return self.width - 2 * self.padding
+
+    def height_no_padding(self):
+        """The height without the padding"""
+        return self.height - 2 * self.padding
+
+    def get_scene_center_pos(self) -> QPointF:
         if not self.node_item.collapsed:
-            return QPointF(self.scenePos().x() + self.boundingRect().width()/2,
-                           self.scenePos().y() + self.boundingRect().height()/2)
+            return QPointF(
+                self.scenePos().x() + self.boundingRect().width() / 2,
+                self.scenePos().y() + self.boundingRect().height() / 2,
+            )
         else:
+            # mypy seems buggy here, it things below methods return Any,
+            # but they are annotated to return QPointF
             if isinstance(self.port_item, InputPortItem):
-                return self.node_item.get_left_body_header_vertex_scene_pos()
+                return self.node_item.get_left_body_header_vertex_scene_pos()  # type: ignore
             else:
-                return self.node_item.get_right_body_header_vertex_scene_pos()
+                return self.node_item.get_right_body_header_vertex_scene_pos()  # type: ignore
 
 
 class PortItemLabel(QGraphicsWidget):
     def __init__(self, port, port_item, node_gui, node_item):
         super(PortItemLabel, self).__init__(node_item)
         self.setGraphicsItem(self)
 
         self.port = port
         self.port_item = port_item
         self.node_gui = node_gui
         self.node_item = node_item
 
         self.font = QFont("Source Code Pro", 10, QFont.Bold)
-        font_metrics = QFontMetricsF(self.font)  # approximately! the designs can use different fonts
+        font_metrics = QFontMetricsF(
+            self.font
+        )  # approximately! the designs can use different fonts
         self.width = font_metrics.width(get_longest_line(self.port.label_str))
         self.height = font_metrics.height() * (self.port.label_str.count('\n') + 1)
         self.port_local_pos = None
 
     def boundingRect(self):
         return QRectF(QPointF(0, 0), self.geometry().size())
 
@@ -337,14 +365,15 @@
 
     def sizeHint(self, which, constraint=...):
         return QSizeF(self.width, self.height)
 
     def paint(self, painter, option, widget=None):
         self.node_item.session_design.flow_theme.paint_PI_label(
             self.node_gui,
-            painter, option,
+            painter,
+            option,
             self.port.type_,
             is_connected(self.port),
             self.port.label_str,
             self.node_gui.color,
-            self.boundingRect()
+            self.boundingRect(),
         )
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __str__(self):
         return self.__class__.__name__
 
 
 class Data_IW(DType_IW_Base, QLineEdit):  # virtual
 
-    base_width = None  # specified by subclasses
+    base_width: int  # specified by subclasses
 
     def __init__(self, params):
         DType_IW_Base.__init__(self, params)
         QLineEdit.__init__(self)
 
         # dtype = self.input.dtype
         # self.last_val = None
@@ -106,26 +106,26 @@
 
 
 # -----------------------------------
 
 
 class String_IW(DType_IW_Base, QLineEdit):  # virtual
 
-    width = None  # specified by subclasses
+    width_: int   # specified by subclasses
 
     def __init__(self, params):
         DType_IW_Base.__init__(self, params)
         QLineEdit.__init__(self)
 
         # dtype = self.input.dtype
         # self.last_val = None
 
         self.setFont(QFont('source code pro', 10))
         self.setText(self.dtype.val)
-        self.setFixedWidth(self.width)
+        self.setFixedWidth(self.width_)
         self.setToolTip(self.dtype.doc)
 
         self.editingFinished.connect(self.editing_finished)
 
     def editing_finished(self):
         """updates the input"""
         self.change_val(self.get_val())
@@ -151,23 +151,23 @@
         # just show value, DO NOT UPDATE
         self.val_update_event(data['text'])
 
 
 # custom sized classes for qss access:
 
 class String_IW_S(String_IW):
-    width = 30
+    width_ = 30
 
 
 class String_IW_M(String_IW):
-    width = 70
+    width_ = 70
 
 
 class String_IW_L(String_IW):
-    width = 150
+    width_ = 150
 
 
 # -----------------------------------
 
 
 class Integer_IW(DType_IW_Base, QSpinBox):
     def __init__(self, params):
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/utils.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from typing import List, Dict
 
 from qtpy.QtCore import QPointF, QByteArray
 
 from ryvencore.utils import serialize, deserialize
 from .GlobalAttributes import *
 
-
+def generate_name(obj, name):
+   return f'{name}:[{id(obj)}]'
+    
 def pythagoras(a, b):
     return sqrt(a ** 2 + b ** 2)
 
 
 def get_longest_line(s: str):
     lines = s.split('\n')
     lines = [line.replace('\n', '') for line in lines]
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/EditVal_Dialog.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/EditVal_Dialog.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/FlowsListWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/FlowsListWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/FlowsList_FlowWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/FlowsList_FlowWidget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from qtpy.QtWidgets import QWidget, QHBoxLayout, QLabel, QMenu, QAction
-from qtpy.QtGui import QIcon, QImage
-from qtpy.QtCore import Qt, QEvent, QBuffer, QByteArray
+from qtpy.QtGui import QIcon, QImage, QMouseEvent
+from qtpy.QtCore import Qt, QEvent, QBuffer, QByteArray, QIODevice
 
 from ..GlobalAttributes import Location
 from .ListWidget_NameLineEdit import ListWidget_NameLineEdit
 
 
 class FlowsList_FlowWidget(QWidget):
     """A QWidget representing a single Flow for the FlowsListWidget."""
@@ -46,41 +46,42 @@
 
         main_layout.addWidget(self.title_line_edit)
 
         self.setLayout(main_layout)
 
 
 
-    def mouseDoubleClickEvent(self, event):
+    def mouseDoubleClickEvent(self, event: QMouseEvent):
         if event.button() == Qt.LeftButton:
             if self.title_line_edit.geometry().contains(event.pos()):
                 self.title_line_edit_double_clicked()
                 return
 
 
-    def event(self, event):
+    def event(self, event: QEvent):
         if event.type() == QEvent.ToolTip:
 
             # generate preview img as QImage
             img: QImage = self.flow_view.get_viewport_img().scaledToHeight(200)
 
             # store the img data in QBuffer to load it directly from memory
             buffer = QBuffer()
-            img.save(buffer, 'PNG')
+            img.save(device=buffer, format='PNG')  # type: ignore
+            # QBuffer inherits QIODevice, but mypy doesn't know that
 
             # generate html from data in memory
             html = f"<img src='data:image/png;base64, { bytes( buffer.data().toBase64() ).decode() }'>"
 
             # show tooltip
             self.setToolTip(html)
 
         return QWidget.event(self, event)
 
 
-    def contextMenuEvent(self, event):
+    def contextMenuEvent(self, event: QEvent):
         menu: QMenu = QMenu(self)
 
         delete_action = QAction('delete')
         delete_action.triggered.connect(self.action_delete_triggered)
 
         actions = [delete_action]
         for a in actions:
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/LogWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/LogWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/VariablesListWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/VariablesListWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt/src/widgets/VarsList_VarWidget.py` & `ryvencore_qt-0.5.0/ryvencore_qt/src/widgets/VarsList_VarWidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qtpy.QtWidgets import QWidget, QHBoxLayout, QLabel, QMenu, QAction
-from qtpy.QtGui import QIcon, QDrag
+from qtpy.QtGui import QIcon, QDrag, QMouseEvent
 from qtpy.QtCore import QMimeData, Qt, QEvent, QByteArray
 
 import json
 
 from ..GlobalAttributes import Location
 from .ListWidget_NameLineEdit import ListWidget_NameLineEdit
 from ..utils import shorten
@@ -50,46 +50,46 @@
 
         main_layout.addWidget(self.name_line_edit)
 
         self.setLayout(main_layout)
 
 
 
-    def mouseDoubleClickEvent(self, event):
+    def mouseDoubleClickEvent(self, event: QMouseEvent):
         if event.button() == Qt.LeftButton:
             if self.name_line_edit.geometry().contains(event.pos()):
                 self.name_line_edit_double_clicked()
                 return
 
 
-    def mousePressEvent(self, event):
+    def mousePressEvent(self, event: QMouseEvent):
         if event.button() == Qt.LeftButton:
             drag = QDrag(self)
             mime_data = QMimeData()
             data_text = self.get_drag_data()
             data = QByteArray(bytes(data_text, 'utf-8'))
             mime_data.setData('text/plain', data)
             drag.setMimeData(mime_data)
             drop_action = drag.exec_()
             return
 
 
-    def event(self, event):
+    def event(self, event: QEvent):
         if event.type() == QEvent.ToolTip:
             val_str = ''
             try:
                 val_str = str(self.var.get())
             except Exception as e:
                 val_str = "couldn't stringify value"
             self.setToolTip('val type: '+str(type(self.var.get()))+'\nval: '+shorten(val_str, 3000, line_break=True))
 
         return QWidget.event(self, event)
 
 
-    def contextMenuEvent(self, event):
+    def contextMenuEvent(self, event: QEvent):
         menu: QMenu = QMenu(self)
 
         delete_action = QAction('delete')
         delete_action.triggered.connect(self.action_delete_triggered)
 
         edit_value_action = QAction('edit value')
         edit_value_action.triggered.connect(self.action_edit_val_triggered)
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt.egg-info/PKG-INFO` & `ryvencore_qt-0.5.0/ryvencore_qt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ryvencore-qt
-Version: 0.4.3
+Version: 0.5.0
 Summary: Qt frontend for ryvencore; Library for building Visual Node Editors
 Home-page: https://github.com/leon-thomm/ryvencore-qt
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.6
+Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ryvencore==0.4.*
-Requires-Dist: PySide2
+Requires-Dist: ryvencore==0.5.*
 Requires-Dist: QtPy
 Requires-Dist: waiting
 Requires-Dist: textdistance
 
 
 <p align="center">
   <img src="./img/logo.png" alt="drawing" width="70%"/>
```

### Comparing `ryvencore-qt-0.4.3/ryvencore_qt.egg-info/SOURCES.txt` & `ryvencore_qt-0.5.0/ryvencore_qt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 ryvencore_qt/__init__.py
+ryvencore_qt/py.typed
 ryvencore_qt.egg-info/PKG-INFO
 ryvencore_qt.egg-info/SOURCES.txt
 ryvencore_qt.egg-info/dependency_links.txt
 ryvencore_qt.egg-info/requires.txt
 ryvencore_qt.egg-info/top_level.txt
 ryvencore_qt/resources/__init__.py
 ryvencore_qt/resources/node_collapse_icon.svg
@@ -86,24 +86,26 @@
 ryvencore_qt/src/flows/FlowCommands.py
 ryvencore_qt/src/flows/FlowTheme.py
 ryvencore_qt/src/flows/FlowView.py
 ryvencore_qt/src/flows/FlowViewProxyWidget.py
 ryvencore_qt/src/flows/FlowViewStylusModesWidget.py
 ryvencore_qt/src/flows/FlowViewZoomWidget.py
 ryvencore_qt/src/flows/__init__.py
+ryvencore_qt/src/flows/connections/ConnectionAnimation.py
 ryvencore_qt/src/flows/connections/ConnectionItem.py
 ryvencore_qt/src/flows/connections/__init__.py
 ryvencore_qt/src/flows/drawings/DrawingObject.py
 ryvencore_qt/src/flows/drawings/__init__.py
 ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py
 ryvencore_qt/src/flows/node_list_widget/NodeWidget.py
 ryvencore_qt/src/flows/node_list_widget/__init__.py
 ryvencore_qt/src/flows/node_list_widget/utils.py
 ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py
 ryvencore_qt/src/flows/nodes/NodeGUI.py
+ryvencore_qt/src/flows/nodes/NodeInspector.py
 ryvencore_qt/src/flows/nodes/NodeItem.py
 ryvencore_qt/src/flows/nodes/NodeItemAction.py
 ryvencore_qt/src/flows/nodes/NodeItemAnimator.py
 ryvencore_qt/src/flows/nodes/NodeItemWidget.py
 ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py
 ryvencore_qt/src/flows/nodes/NodeItem_Icon.py
 ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py
```

### Comparing `ryvencore-qt-0.4.3/setup.cfg` & `ryvencore_qt-0.5.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ryvencore-qt
-version = v0.4.3
+version = v0.5.0
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Qt frontend for ryvencore; Library for building Visual Node Editors
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/leon-thomm/ryvencore-qt
@@ -14,18 +14,17 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.6, <3.11
+python_requires = >=3.6, <3.13
 install_requires = 
-	ryvencore ==0.4.*
-	PySide2
+	ryvencore ==0.5.*
 	QtPy
 	waiting
 	textdistance
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

