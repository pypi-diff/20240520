# Comparing `tmp/eomaps-8.2.tar.gz` & `tmp/eomaps-8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eomaps-8.2.tar", last modified: Mon May 13 12:48:01 2024, max compression
+gzip compressed data, was "eomaps-8.2.1.tar", last modified: Mon May 20 19:21:31 2024, max compression
```

## Comparing `eomaps-8.2.tar` & `eomaps-8.2.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.208550 eomaps-8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 12:47:51.000000 eomaps-8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-13 12:48:01.208550 eomaps-8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-05-13 12:47:51.000000 eomaps-8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.192550 eomaps-8.2/eomaps/
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54662 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_blit_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    54772 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    48810 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_maps_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/annotation_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    49570 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    79174 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/cb_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    57530 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/compass.py
--rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)   146187 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/inset_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)    38892 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.196550 eomaps-8.2/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.200550 eomaps-8.2/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/edit_layout.png
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_active.png
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/info.png
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/info_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/info_hoover.png
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/layers.png
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/layers_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/open.png
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/open_hover.png
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/peek_top_active.png
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/icons/plus_hoover.png
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/signal_container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/eomaps/qtcompanion/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)    62338 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)    46849 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20418 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/peek.py
--rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/save.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/qtcompanion/widgets/wms.py
--rw-r--r--   0 runner    (1001) docker     (127)    51631 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    57249 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/scalebar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/eomaps/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/scripts/open.py
--rw-r--r--   0 runner    (1001) docker     (127)    83217 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    91116 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18151 2024-05-13 12:47:51.000000 eomaps-8.2/eomaps/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/eomaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 12:48:01.000000 eomaps-8.2/eomaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-13 12:47:51.000000 eomaps-8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:48:01.208550 eomaps-8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:48:01.204550 eomaps-8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_WMS_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    44313 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_basic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_doc_codeblocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_doc_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_layout_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_plot_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_raster_aggregaton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-13 12:47:51.000000 eomaps-8.2/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.879175 eomaps-8.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-20 19:21:22.000000 eomaps-8.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-20 19:21:31.879175 eomaps-8.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-05-20 19:21:22.000000 eomaps-8.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.867174 eomaps-8.2.1/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54836 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/_blit_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54800 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52395 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/_maps_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50349 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/annotation_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49570 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79174 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57681 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28800 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147115 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/inset_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38892 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.867174 eomaps-8.2.1/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.875175 eomaps-8.2.1/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/edit_layout.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/edit_layout_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/edit_layout_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/info.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/info_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/info_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/layers.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/layers_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86617 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/open_hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/peek_top_active.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/icons/plus_hoover.png
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/signal_container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.875175 eomaps-8.2.1/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23702 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19962 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62338 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46849 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15167 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20418 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51631 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57249 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/scalebar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.875175 eomaps-8.2.1/eomaps/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/scripts/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83447 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91116 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-20 19:21:22.000000 eomaps-8.2.1/eomaps/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.879175 eomaps-8.2.1/eomaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-20 19:21:31.000000 eomaps-8.2.1/eomaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-20 19:21:31.000000 eomaps-8.2.1/eomaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:21:31.000000 eomaps-8.2.1/eomaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 19:21:31.000000 eomaps-8.2.1/eomaps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 19:21:31.000000 eomaps-8.2.1/eomaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:21:31.000000 eomaps-8.2.1/eomaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-20 19:21:22.000000 eomaps-8.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:21:31.879175 eomaps-8.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:31.879175 eomaps-8.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_WMS_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44313 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_basic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_doc_codeblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_doc_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_layout_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_plot_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_raster_aggregaton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-20 19:21:22.000000 eomaps-8.2.1/tests/test_widgets.py
```

### Comparing `eomaps-8.2/LICENSE` & `eomaps-8.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/PKG-INFO` & `eomaps-8.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eomaps
-Version: 8.2
+Version: 8.2.1
 Summary: A library to create interactive maps of geographical datasets.
 Author-email: Raphael Quast <raphael.quast@geo.tuwien.ac.at>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, The EOmaps authors.
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eomaps Version: 8.2 Summary: A library to create
+Metadata-Version: 2.1 Name: eomaps Version: 8.2.1 Summary: A library to create
 interactive maps of geographical datasets. Author-email: Raphael Quast
 geo.tuwien.ac.at> License: BSD 3-Clause License Copyright (c) 2021, The EOmaps
 authors. Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `eomaps-8.2/README.md` & `eomaps-8.2.1/README.md`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/NE_features.json` & `eomaps-8.2.1/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/__init__.py` & `eomaps-8.2.1/eomaps/__init__.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/_blit_manager.py` & `eomaps-8.2.1/eomaps/_blit_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,15 +570,19 @@
             l = str(l)  # w make sure we convert non-string layer names to string!
 
             # get artists defined on the layer itself
             # Note: it's possible to create explicit multi-layers and attach
             # artists that are only visible if both layers are visible! (e.g. "l1|l2")
             artists.extend(self._bg_artists.get(l, []))
 
-            if l == self._unmanaged_artists_layer:
+            # make sure to also trigger drawing unmanaged artists on inset-maps!
+            if l in (
+                self._unmanaged_artists_layer,
+                f"__inset_{self._unmanaged_artists_layer}",
+            ):
                 artists.extend(self._get_unmanaged_artists())
 
         # make the list unique but maintain order (dicts keep order for python>3.7)
         artists = dict.fromkeys(artists)
         # sort artists by zorder (respecting inset-map priority)
         artists = sorted(artists, key=self._bg_artists_sort)
```

### Comparing `eomaps-8.2/eomaps/_containers.py` & `eomaps-8.2.1/eomaps/_containers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/_data_manager.py` & `eomaps-8.2.1/eomaps/_data_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,15 +677,15 @@
 
         # don't re-draw while the layout-editor is active!
         if self.m.parent._layout_editor.modifier_pressed:
             return False
 
         # don't re-draw if the layer of the dataset is not requested
         # (note multi-layers trigger re-draws of individual layers as well)
-        if layer not in ["all", self.layer]:
+        if not self.m.BM._layer_is_subset(layer, self.layer):
             return False
 
         # don't re-draw if the collection has been hidden in the companion-widget
         if self.m.coll in self.m.BM._hidden_artists:
             return False
 
         # re-draw if the data has never been plotted
@@ -887,15 +887,14 @@
             props = self.get_props()
             if props is None or props["x0"] is None or props["y0"] is None:
                 # fail-fast in case the data is completely outside the extent
                 return
 
             s = self._get_datasize(**props)
             self._print_datasize_warnings(s)
-
             # stop here in case we are dealing with a pick-only dataset
             if self._only_pick:
                 return
 
             if props["x0"].size < 1 or props["y0"].size < 1:
                 # keep original data if too low amount of data is attempted
                 # to be plotted
@@ -936,17 +935,17 @@
             # before a layer has been fetched (e.g. before m.coll is defined)
             # (=lazily initialize the picker when the layer is fetched)
             while len(self._on_next_fetch) > 0:
                 self._on_next_fetch.pop(-1)()
 
             self.m.cb.pick._set_artist(coll)
 
-        except Exception:
+        except Exception as ex:
             _log.exception(
-                f"EOmaps: Unable to plot the data for the layer '{layer}'!",
+                f"EOmaps: Unable to plot the data for the layer '{layer}'!\n{ex}",
                 exc_info=_log.getEffectiveLevel() <= logging.DEBUG,
             )
 
     def data_in_extent(self, extent):
         # check if the data extent collides with the map extent
         x0, x1, y0, y1 = extent
         if x0 > self._x0max or self._x0min > x1:
```

### Comparing `eomaps-8.2/eomaps/_maps_base.py` & `eomaps-8.2.1/eomaps/_maps_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,102 @@
 
         if use_interactive_mode is not None:
             cls._use_interactive_mode = use_interactive_mode
 
         if log_level is not None:
             set_loglevel(log_level)
 
+    def apply_webagg_fix(cls):
+        """
+        Apply fix to avoid slow updates and lags due to event-accumulation in webagg backend.
+
+        (e.g. when using `matplotlib.use("webagg")`)
+
+        - Events that occur while draws are pending are dropped and only the
+          last event of each type that occured during the wait is finally executed.
+
+        Note
+        ----
+
+        Using this fix is **experimental** and will monkey-patch matplotlibs
+        `FigureCanvasWebAggCore` and `FigureManagerWebAgg` to avoid event accumulation!
+
+        You MUST call this function at the very beginning of the script to ensure
+        changes are applied correctly!
+
+        There might be unwanted side-effects for callbacks that require all events
+        to be executed consecutively independent of the draw-state (e.g. typing text).
+
+        """
+        from matplotlib.backends.backend_webagg_core import (
+            FigureCanvasWebAggCore,
+            FigureManagerWebAgg,
+        )
+
+        def handle_ack(self, event):
+            self._ack_cnt += 1  # count the number of received images
+
+        def refresh_all(self):
+            if self.web_sockets:
+                diff = self.canvas.get_diff_image()
+                if diff is not None:
+                    for s in self.web_sockets:
+                        s.send_binary(diff)
+
+                    self._send_cnt += 1  # count the number of sent images
+
+        def handle_event(self, event):
+            if not hasattr(self, "_event_cache"):
+                self._event_cache = dict()
+
+            cnt_equal = self._ack_cnt == self.manager._send_cnt
+
+            # always process ack and draw events
+            # process other events only if "ack count" equals "send count"
+            # (e.g. if we received and handled all pending images)
+            if cnt_equal or event["type"] in ["ack", "draw"]:
+                # immediately process all cached events
+                for cache_event_type, cache_event in self._event_cache.items():
+                    getattr(
+                        self,
+                        "handle_{0}".format(cache_event_type),
+                        self.handle_unknown_event,
+                    )(cache_event)
+                self._event_cache.clear()
+
+                # reset counters to avoid overflows (just a precaution to avoid overflows)
+                if cnt_equal:
+                    self._ack_cnt, self.manager._send_cnt = 0, 0
+
+                # process event
+                e_type = event["type"]
+                handler = getattr(
+                    self, "handle_{0}".format(e_type), self.handle_unknown_event
+                )
+            else:
+                # ignore events in case we have a pending image that is on the way to be processed
+                # cache the latest event of each type so we can process it once we are ready
+                self._event_cache[event["type"]] = event
+
+                # a final savety precaution in case send count is lower than ack count
+                # (e.g. we wait for an image but there was no image sent)
+                if self.manager._send_cnt < self._ack_cnt:
+                    # reset counts... they seem to be incorrect
+                    self._ack_cnt, self.manager._send_cnt = 0, 0
+                return
+
+            return handler(event)
+
+        FigureCanvasWebAggCore._ack_cnt = 0
+        FigureCanvasWebAggCore.handle_ack = handle_ack
+        FigureCanvasWebAggCore.handle_event = handle_event
+
+        FigureManagerWebAgg._send_cnt = 0
+        FigureManagerWebAgg.refresh_all = refresh_all
+
 
 class MapsBase(metaclass=_MapsMeta):
     def __init__(
         self,
         crs=None,
         layer="base",
         f=None,
```

### Comparing `eomaps-8.2/eomaps/_webmap.py` & `eomaps-8.2.1/eomaps/_webmap.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/annotation_editor.py` & `eomaps-8.2.1/eomaps/annotation_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/callbacks.py` & `eomaps-8.2.1/eomaps/callbacks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/cb_container.py` & `eomaps-8.2.1/eomaps/cb_container.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/colorbar.py` & `eomaps-8.2.1/eomaps/colorbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,14 +627,16 @@
     Note
     ----
     To add a colorbar to a map, use
     :py:meth:`Maps.add_colorbar <eomaps.eomaps.Maps.add_colorbar>`.
 
     """
 
+    max_n_classify_bins_to_label = 30
+
     def __init__(self, *args, inherit_position=True, layer=None, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._layer = layer
 
         self._inherit_position = inherit_position
         self._dynamic_shade_indicator = False
@@ -1193,17 +1195,19 @@
 
     def _set_tick_formatter(self):
         if "format" in self._cb_kwargs:
             self.cb.set_ticks(self.cb.get_ticks())
             return
 
         if self._m._classified:
-            self.cb.set_ticks(
-                np.unique(np.clip(self._m.classify_specs._bins, self._vmin, self._vmax))
+            unique_bins = np.unique(
+                np.clip(self._m.classify_specs._bins, self._vmin, self._vmax)
             )
+            if len(unique_bins) <= self.max_n_classify_bins_to_label:
+                self.cb.set_ticks(unique_bins)
 
         if self.orientation == "horizontal":
             if self._m._classified:
                 self.ax_cb.xaxis.set_major_formatter(self._classified_cb_tick_formatter)
             else:
                 self.ax_cb.xaxis.set_major_formatter(self._default_cb_tick_formatter)
         else:
```

### Comparing `eomaps-8.2/eomaps/compass.py` & `eomaps-8.2.1/eomaps/compass.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/draw.py` & `eomaps-8.2.1/eomaps/draw.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/eomaps.py` & `eomaps-8.2.1/eomaps/eomaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,25 +359,39 @@
 
     @property
     def coll(self):
         """The collection representing the dataset plotted by m.plot_map()."""
         return self._coll
 
     @property
+    def _shape_assigned(self):
+        """Return True if the shape is explicitly assigned and False otherwise"""
+        # the shape is considered assigned if an explicit shape is set
+        # or if the data has been plotted with the default shape
+
+        q = self._shape is None or (
+            getattr(self._shape, "_is_default", False) and not self._data_plotted
+        )
+
+        return not q
+
+    @property
     def shape(self):
         """
         The shape that is used to represent the dataset if `m.plot_map()` is called.
 
         By default "ellipses" is used for datasets < 500k datapoints and for plots
         where no explicit data is assigned, and otherwise "shade_raster" is used
         for 2D datasets and "shade_points" is used for unstructured datasets.
 
         """
-        if self._shape is None:
+
+        if not self._shape_assigned:
             self._set_default_shape()
+            self._shape._is_default = True
 
         return self._shape
 
     @property
     def colorbar(self):
         """
         Get the **most recently added** colorbar of this Maps-object.
@@ -527,15 +541,15 @@
         """
         m2 = Maps(f=self.f, ax=ax, **kwargs)
 
         if inherit_data:
             m2.inherit_data(self)
         if inherit_classification:
             m2.inherit_classification(self)
-        if inherit_shape:
+        if inherit_shape and self._shape_assigned:
             getattr(m2.set_shape, self.shape.name)(**self.shape._initargs)
 
         if np.allclose(self.ax.bbox.bounds, m2.ax.bbox.bounds):
             _log.warning(
                 "EOmaps:The new map overlaps exactly with the parent map! "
                 "Use `ax=...` or the LayoutEditor to adjust the position of the map."
             )
@@ -658,15 +672,15 @@
             layer=layer,
         )
 
         if inherit_data:
             m.inherit_data(self)
         if inherit_classification:
             m.inherit_classification(self)
-        if inherit_shape:
+        if inherit_shape and self._shape_assigned:
             getattr(m.set_shape, self.shape.name)(**self.shape._initargs)
 
         # make sure the new layer does not attempt to reset the extent if
         # it has already been set on the parent layer
         m._set_extent_on_plot = self._set_extent_on_plot
 
         # re-initialize all sliders and buttons to include the new layer
@@ -2761,16 +2775,17 @@
                 raise TypeError(
                     "EOmaps: You cannot provide an explicit norm for the dataset if a "
                     "classification scheme is used!"
                 )
         else:
             if "norm" in kwargs:
                 norm = kwargs.pop("norm")
-                norm.vmin = self._vmin
-                norm.vmax = self._vmax
+                if not isinstance(norm, str):  # to allow datashader "eq_hist" norm
+                    norm.vmin = self._vmin
+                    norm.vmax = self._vmax
             else:
                 norm = plt.Normalize(vmin=self._vmin, vmax=self._vmax)
 
         # todo remove duplicate attributes
         self.classify_specs._cbcmap = cbcmap
         self.classify_specs._norm = norm
         self.classify_specs._bins = bins
@@ -3495,16 +3510,23 @@
 
             if vmin < min(bins):
                 bins = [vmin, *bins]
 
             if vmax > max(bins):
                 bins = [*bins, vmax]
 
-            cbcmap = cmap
-            norm = mpl.colors.BoundaryNorm(bins, cmap.N)
+            # TODO Always use resample once mpl>3.6 is pinned
+            if hasattr(cmap, "resampled") and len(bins) > cmap.N:
+                # Resample colormap to contain enough color-values
+                # as needed by the boundary-norm.
+                cbcmap = cmap.resampled(len(bins))
+            else:
+                cbcmap = cmap
+
+            norm = mpl.colors.BoundaryNorm(bins, cbcmap.N)
 
             self._emit_signal("cmapsChanged")
 
             if cmap._rgba_bad:
                 cbcmap.set_bad(cmap._rgba_bad)
             if cmap._rgba_over:
                 cbcmap.set_over(cmap._rgba_over)
```

### Comparing `eomaps-8.2/eomaps/grid.py` & `eomaps-8.2.1/eomaps/grid.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/helpers.py` & `eomaps-8.2.1/eomaps/helpers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/inset_maps.py` & `eomaps-8.2.1/eomaps/inset_maps.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/layout_editor.py` & `eomaps-8.2.1/eomaps/layout_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/logo.png` & `eomaps-8.2.1/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/mapsgrid.py` & `eomaps-8.2.1/eomaps/mapsgrid.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/ne_features.py` & `eomaps-8.2.1/eomaps/ne_features.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/projections.py` & `eomaps-8.2.1/eomaps/projections.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/app.py` & `eomaps-8.2.1/eomaps/qtcompanion/app.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/base.py` & `eomaps-8.2.1/eomaps/qtcompanion/base.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/edit_layout.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/edit_layout.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_active.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/edit_layout_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/edit_layout_hover.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/edit_layout_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/eye_closed.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/eye_closed.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/eye_open.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/eye_open.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/info.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/info.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/info_checked.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/info_checked.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/info_hoover.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/info_hoover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/layers.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/layers.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/layers_hover.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/layers_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/logo.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/open.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/open.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/open_hover.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/open_hover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/peek_circle.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/peek_circle_active.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/plus.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/plus.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/icons/plus_hoover.png` & `eomaps-8.2.1/eomaps/qtcompanion/icons/plus_hoover.png`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/signal_container.py` & `eomaps-8.2.1/eomaps/qtcompanion/signal_container.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/annotate.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/annotate.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/click_callbacks.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/draw.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/draw.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/editor.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/extent.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/extent.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/files.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/files.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/layer.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/layer.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/peek.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/peek.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/save.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/save.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/utils.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/qtcompanion/widgets/wms.py` & `eomaps-8.2.1/eomaps/qtcompanion/widgets/wms.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/reader.py` & `eomaps-8.2.1/eomaps/reader.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/scalebar.py` & `eomaps-8.2.1/eomaps/scalebar.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/scripts/open.py` & `eomaps-8.2.1/eomaps/scripts/open.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/shapes.py` & `eomaps-8.2.1/eomaps/shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,14 +422,19 @@
     def _get_radius(m, radius, radius_crs):
         if (isinstance(radius, str) and radius == "estimate") or radius is None:
             if m._estimated_radius is None:
                 # make sure props are defined otherwise we can't estimate the radius!
                 if m._data_manager.x0 is None:
                     m._data_manager.set_props(None)
 
+                # check if the first element of x0 is nonzero...
+                # (to avoid slow performance of np.any for large arrays)
+                if not np.any(m._data_manager.x0.take(0)):
+                    return None
+
                 _log.info("EOmaps: Estimating shape radius...")
                 radiusx, radiusy = Shapes._estimate_radius(m, radius_crs)
 
                 if radiusx == radiusy:
                     _log.info(
                         "EOmaps: radius = "
                         f"{np.format_float_scientific(radiusx, precision=4)}"
```

### Comparing `eomaps-8.2/eomaps/utilities.py` & `eomaps-8.2.1/eomaps/utilities.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/webmap_containers.py` & `eomaps-8.2.1/eomaps/webmap_containers.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/eomaps/widgets.py` & `eomaps-8.2.1/eomaps/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 from contextlib import contextmanager
 
 import numpy as np
-import matplotlib.pyplot as plt
 
 from . import _log
 from ._blit_manager import LayerParser
 
 try:
     import ipywidgets
 except ImportError:
     _log.warning("EOmaps-widgets are missing the required dependency 'ipywidgets'!")
 
 
-def _check_backend():
-    backend = plt.get_backend()
-    if "ipympl" not in backend.lower():
-        _log.warning(
-            "EOmaps-widgets only work with the 'ipympl (widget)' backend! "
-            "Make sure you have 'ipympl' installed and use the magic-command "
-            "'%matplotlib widget' to switch to the interactive jupyter backend!"
-        )
-
-
 @contextmanager
 def _force_full(m):
     """A contextmanager to force a full update of the figure (to avoid glitches)"""
     force_full = getattr(m.BM, "_mpl_backend_force_full", False)
 
     try:
         m.BM._mpl_backend_force_full = True
@@ -96,16 +85,14 @@
 
     """
 
     _description = "Layers"
     _widget_cls = None
 
     def __init__(self, m, layers=None, **kwargs):
-        _check_backend()
-
         self._m = m
         self._set_layers_options(layers)
 
         self._set_default_kwargs(kwargs)
         self._widget_cls.__init__(self, options=self._options, **kwargs)
 
         if hasattr(self, "change_handler"):
@@ -332,16 +319,14 @@
     kwargs:
         Additional kwargs passed to the used `ipywidgets.FloatSlider`.
 
     """
 
     def __init__(self, m, layer, **kwargs):
         self._m = m
-        _check_backend()
-
         self._layer = self._parse_layer(layer)
 
         kwargs.setdefault("description", self._layer)
 
         super().__init__(**kwargs)
         self.on_click(self.click_handler)
 
@@ -382,16 +367,14 @@
     kwargs:
         Additional kwargs passed to the used `ipywidgets.FloatSlider`.
 
     """
 
     def __init__(self, m, layer, **kwargs):
         self._m = m
-        _check_backend()
-
         self._layer = layer
 
         kwargs.setdefault("value", 0)
         kwargs.setdefault("min", 0)
         kwargs.setdefault("max", 1)
         kwargs.setdefault("step", 0.01)
         kwargs.setdefault("description", f"Overlay\n'{layer}':")
@@ -445,16 +428,14 @@
     """
 
     _cid = None
     _widget_cls = None
 
     def __init__(self, m, widget_kwargs=None, **kwargs):
         self._m = m
-        _check_backend()
-
         self._kwargs = kwargs
 
         if widget_kwargs is None:
             widget_kwargs = dict()
 
         widget_kwargs.setdefault("value", False)
         widget_kwargs.setdefault("description", self._description)
```

### Comparing `eomaps-8.2/eomaps.egg-info/PKG-INFO` & `eomaps-8.2.1/eomaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eomaps
-Version: 8.2
+Version: 8.2.1
 Summary: A library to create interactive maps of geographical datasets.
 Author-email: Raphael Quast <raphael.quast@geo.tuwien.ac.at>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, The EOmaps authors.
         
         Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eomaps Version: 8.2 Summary: A library to create
+Metadata-Version: 2.1 Name: eomaps Version: 8.2.1 Summary: A library to create
 interactive maps of geographical datasets. Author-email: Raphael Quast
 geo.tuwien.ac.at> License: BSD 3-Clause License Copyright (c) 2021, The EOmaps
 authors. Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `eomaps-8.2/eomaps.egg-info/SOURCES.txt` & `eomaps-8.2.1/eomaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/pyproject.toml` & `eomaps-8.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.package-data]
 eomaps = ["logo.png", "NE_features.json", "qtcompanion/icons/*"]
 
 
 [project]
 name = "eomaps"
-version = "8.2"
+version = "8.2.1"
 description = "A library to create interactive maps of geographical datasets."
 readme = "README.md"
 license = {file = "LICENSE"}
 
 requires-python = ">=3.8"
 
 authors = [
```

### Comparing `eomaps-8.2/tests/test_WMS_capabilities.py` & `eomaps-8.2.1/tests/test_WMS_capabilities.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_basic_functions.py` & `eomaps-8.2.1/tests/test_basic_functions.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_callbacks.py` & `eomaps-8.2.1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_config.py` & `eomaps-8.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_doc_codeblocks.py` & `eomaps-8.2.1/tests/test_doc_codeblocks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_doc_notebooks.py` & `eomaps-8.2.1/tests/test_doc_notebooks.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_drawer.py` & `eomaps-8.2.1/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_examples.py` & `eomaps-8.2.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_from_file.py` & `eomaps-8.2.1/tests/test_from_file.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_layout_editor.py` & `eomaps-8.2.1/tests/test_layout_editor.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_plot_shapes.py` & `eomaps-8.2.1/tests/test_plot_shapes.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_raster_aggregaton.py` & `eomaps-8.2.1/tests/test_raster_aggregaton.py`

 * *Files identical despite different names*

### Comparing `eomaps-8.2/tests/test_widgets.py` & `eomaps-8.2.1/tests/test_widgets.py`

 * *Files identical despite different names*

