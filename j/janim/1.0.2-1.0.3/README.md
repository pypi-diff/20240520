# Comparing `tmp/janim-1.0.2.tar.gz` & `tmp/janim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-1.0.2.tar` & `janim-1.0.3.tar`

### file list

```diff
@@ -1,99 +1,97 @@
--rw-r--r--   0        0        0      165 2024-05-14 01:59:46.065562 janim-1.0.2/.gitignore
--rw-r--r--   0        0        0     1053 2024-04-17 15:49:03.633620 janim-1.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0      413 2024-05-14 01:59:46.073570 janim-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-1.0.2/.vscode/tasks.json
--rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.2/LICENSE
--rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-1.0.2/README.md
--rw-r--r--   0        0        0       71 2024-05-14 02:28:31.447277 janim-1.0.2/janim/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-17 03:59:08.847168 janim-1.0.2/janim/__main__.py
--rw-r--r--   0        0        0     4233 2024-05-14 01:59:46.170426 janim-1.0.2/janim/anims/animation.py
--rw-r--r--   0        0        0     6349 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/composition.py
--rw-r--r--   0        0        0     6034 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/creation.py
--rw-r--r--   0        0        0      815 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/display.py
--rw-r--r--   0        0        0     3454 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/fading.py
--rw-r--r--   0        0        0     3954 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/growing.py
--rw-r--r--   0        0        0    10342 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/indication.py
--rw-r--r--   0        0        0     1547 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/rotation.py
--rw-r--r--   0        0        0    25400 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/timeline.py
--rw-r--r--   0        0        0     9210 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/transform.py
--rw-r--r--   0        0        0     9946 2024-05-14 01:59:46.186425 janim-1.0.2/janim/anims/updater.py
--rw-r--r--   0        0        0     4505 2024-05-14 01:59:46.195654 janim-1.0.2/janim/camera/camera.py
--rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-1.0.2/janim/camera/camera_info.py
--rw-r--r--   0        0        0     6808 2024-05-14 01:59:46.203658 janim-1.0.2/janim/cli.py
--rw-r--r--   0        0        0     9221 2024-05-14 01:59:46.211660 janim-1.0.2/janim/components/component.py
--rw-r--r--   0        0        0     2408 2024-05-14 01:59:46.219687 janim-1.0.2/janim/components/data.py
--rw-r--r--   0        0        0     2609 2024-05-14 01:59:46.227662 janim-1.0.2/janim/components/depth.py
--rw-r--r--   0        0        0     1284 2024-05-14 01:59:46.235662 janim-1.0.2/janim/components/image.py
--rw-r--r--   0        0        0    30900 2024-05-14 01:59:46.249633 janim-1.0.2/janim/components/points.py
--rw-r--r--   0        0        0     2833 2024-05-14 01:59:46.265668 janim-1.0.2/janim/components/radius.py
--rw-r--r--   0        0        0     7922 2024-05-14 01:59:46.273667 janim-1.0.2/janim/components/rgbas.py
--rw-r--r--   0        0        0    22599 2024-05-14 01:59:46.281677 janim-1.0.2/janim/components/vpoints.py
--rw-r--r--   0        0        0      245 2024-05-14 01:59:46.289685 janim-1.0.2/janim/constants/__init__.py
--rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-1.0.2/janim/constants/alignment.py
--rw-r--r--   0        0        0     1542 2024-05-14 01:59:46.289685 janim-1.0.2/janim/constants/colors.py
--rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-1.0.2/janim/constants/coord.py
--rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-1.0.2/janim/constants/degrees.py
--rw-r--r--   0        0        0     4900 2024-05-14 02:28:31.447277 janim-1.0.2/janim/examples.py
--rw-r--r--   0        0        0     1723 2024-05-14 01:59:46.353641 janim-1.0.2/janim/exception.py
--rw-r--r--   0        0        0    40949 2024-05-14 01:59:46.370826 janim-1.0.2/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-1.0.2/janim/gui/application.py
--rw-r--r--   0        0        0      797 2024-04-17 03:59:08.853145 janim-1.0.2/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-1.0.2/janim/gui/export.png
--rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-1.0.2/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0      996 2024-05-14 01:59:46.378840 janim-1.0.2/janim/gui/glwidget.py
--rw-r--r--   0        0        0      903 2024-04-24 02:36:54.042754 janim-1.0.2/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-1.0.2/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8331 2024-05-14 01:59:46.386831 janim-1.0.2/janim/gui/selector.py
--rw-r--r--   0        0        0     1679 2024-05-14 01:59:46.402832 janim-1.0.2/janim/imports.py
--rw-r--r--   0        0        0     5727 2024-05-14 01:59:46.410834 janim-1.0.2/janim/items/audio.py
--rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-1.0.2/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8745 2024-05-14 01:59:46.425018 janim-1.0.2/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2165 2024-05-09 02:35:32.318443 janim-1.0.2/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-1.0.2/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8784 2024-05-14 01:59:46.430120 janim-1.0.2/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6729 2024-05-14 01:59:46.446128 janim-1.0.2/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     7917 2024-05-14 01:59:46.462124 janim-1.0.2/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5239 2024-05-14 01:59:46.470125 janim-1.0.2/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5277 2024-05-14 01:59:46.486125 janim-1.0.2/janim/items/image_item.py
--rw-r--r--   0        0        0    19084 2024-05-14 01:59:46.486125 janim-1.0.2/janim/items/item.py
--rw-r--r--   0        0        0     3262 2024-05-14 01:59:46.494125 janim-1.0.2/janim/items/points.py
--rw-r--r--   0        0        0     7660 2024-05-14 01:59:46.510125 janim-1.0.2/janim/items/relation.py
--rw-r--r--   0        0        0     2071 2024-05-14 01:59:46.518127 janim-1.0.2/janim/items/shape_matchers.py
--rw-r--r--   0        0        0     5955 2024-05-14 01:59:46.534124 janim-1.0.2/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-1.0.2/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4377 2024-05-14 01:59:46.542125 janim-1.0.2/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     3090 2024-04-17 03:59:08.856138 janim-1.0.2/janim/items/svg/typst.py
--rw-r--r--   0        0        0       40 2024-05-09 06:47:34.328454 janim-1.0.2/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    16153 2024-05-14 01:59:46.558125 janim-1.0.2/janim/items/text/text.py
--rw-r--r--   0        0        0     1094 2024-05-14 01:59:46.566125 janim-1.0.2/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5357 2024-05-14 01:59:46.582126 janim-1.0.2/janim/items/vitem.py
--rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-1.0.2/janim/logger.py
--rw-r--r--   0        0        0     3054 2024-04-29 03:26:21.783167 janim-1.0.2/janim/render/base.py
--rw-r--r--   0        0        0     8845 2024-05-14 01:59:46.614125 janim-1.0.2/janim/render/impl.py
--rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-1.0.2/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1250 2024-04-01 15:20:38.430742 janim-1.0.2/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-1.0.2/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-1.0.2/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-1.0.2/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6950 2024-04-12 03:01:12.197148 janim-1.0.2/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-1.0.2/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0     1013 2024-05-14 01:59:46.622126 janim-1.0.2/janim/render/texture.py
--rw-r--r--   0        0        0     6787 2024-04-17 03:59:08.857134 janim-1.0.2/janim/render/writer.py
--rw-r--r--   0        0        0      964 2024-05-14 01:59:46.638124 janim-1.0.2/janim/typing.py
--rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-1.0.2/janim/utils/bezier.py
--rw-r--r--   0        0        0     5515 2024-05-14 01:59:46.646128 janim-1.0.2/janim/utils/config.py
--rw-r--r--   0        0        0     5786 2024-05-14 01:59:46.662124 janim-1.0.2/janim/utils/data.py
--rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-1.0.2/janim/utils/dict_ops.py
--rw-r--r--   0        0        0     2483 2024-05-14 01:59:46.678125 janim-1.0.2/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2995 2024-05-14 01:59:46.694125 janim-1.0.2/janim/utils/font.py
--rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-1.0.2/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-1.0.2/janim/utils/iterables.py
--rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-1.0.2/janim/utils/paths.py
--rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-1.0.2/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2651 2024-05-14 01:59:46.710124 janim-1.0.2/janim/utils/refresh.py
--rw-r--r--   0        0        0     8342 2024-05-14 01:59:46.718125 janim-1.0.2/janim/utils/signal.py
--rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-1.0.2/janim/utils/simple_functions.py
--rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-1.0.2/janim/utils/space_ops.py
--rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-1.0.2/logo.png
--rw-r--r--   0        0        0     1018 2024-04-17 04:51:28.717344 janim-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-05-15 13:12:47.689581 janim-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1053 2024-05-15 13:12:47.693570 janim-1.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.3/LICENSE
+-rw-r--r--   0        0        0      966 2024-05-15 13:12:47.702546 janim-1.0.3/README.md
+-rw-r--r--   0        0        0       71 2024-05-20 03:02:24.964401 janim-1.0.3/janim/__init__.py
+-rw-r--r--   0        0        0     3147 2024-05-15 13:12:48.880157 janim-1.0.3/janim/__main__.py
+-rw-r--r--   0        0        0     4233 2024-05-15 13:12:48.880157 janim-1.0.3/janim/anims/animation.py
+-rw-r--r--   0        0        0     6347 2024-05-18 15:41:45.486818 janim-1.0.3/janim/anims/composition.py
+-rw-r--r--   0        0        0     6034 2024-05-15 13:12:48.882153 janim-1.0.3/janim/anims/creation.py
+-rw-r--r--   0        0        0      815 2024-05-15 13:12:48.882153 janim-1.0.3/janim/anims/display.py
+-rw-r--r--   0        0        0     3454 2024-05-15 13:12:48.883149 janim-1.0.3/janim/anims/fading.py
+-rw-r--r--   0        0        0     3954 2024-05-15 13:12:48.884148 janim-1.0.3/janim/anims/growing.py
+-rw-r--r--   0        0        0    10342 2024-05-15 13:12:48.884148 janim-1.0.3/janim/anims/indication.py
+-rw-r--r--   0        0        0     1547 2024-05-15 13:12:48.885147 janim-1.0.3/janim/anims/rotation.py
+-rw-r--r--   0        0        0    26783 2024-05-19 14:28:07.770496 janim-1.0.3/janim/anims/timeline.py
+-rw-r--r--   0        0        0     9210 2024-05-15 13:12:48.887139 janim-1.0.3/janim/anims/transform.py
+-rw-r--r--   0        0        0     9946 2024-05-19 14:26:49.275303 janim-1.0.3/janim/anims/updater.py
+-rw-r--r--   0        0        0     4505 2024-05-15 13:12:48.896116 janim-1.0.3/janim/camera/camera.py
+-rw-r--r--   0        0        0     2744 2024-05-15 13:12:48.903096 janim-1.0.3/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     6808 2024-05-15 13:12:48.913071 janim-1.0.3/janim/cli.py
+-rw-r--r--   0        0        0     9221 2024-05-15 13:12:48.913071 janim-1.0.3/janim/components/component.py
+-rw-r--r--   0        0        0     2408 2024-05-15 13:12:48.919053 janim-1.0.3/janim/components/data.py
+-rw-r--r--   0        0        0     2609 2024-05-15 13:12:48.919053 janim-1.0.3/janim/components/depth.py
+-rw-r--r--   0        0        0     1284 2024-05-15 13:12:48.926037 janim-1.0.3/janim/components/image.py
+-rw-r--r--   0        0        0    31079 2024-05-19 05:52:00.253534 janim-1.0.3/janim/components/points.py
+-rw-r--r--   0        0        0     2833 2024-05-15 13:12:48.933016 janim-1.0.3/janim/components/radius.py
+-rw-r--r--   0        0        0     7922 2024-05-15 13:12:48.941993 janim-1.0.3/janim/components/rgbas.py
+-rw-r--r--   0        0        0    22599 2024-05-15 13:12:48.941993 janim-1.0.3/janim/components/vpoints.py
+-rw-r--r--   0        0        0      245 2024-05-15 13:12:48.942989 janim-1.0.3/janim/constants/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-15 13:12:48.948973 janim-1.0.3/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1542 2024-05-15 13:12:48.948973 janim-1.0.3/janim/constants/colors.py
+-rw-r--r--   0        0        0      639 2024-05-19 23:59:21.996726 janim-1.0.3/janim/constants/coord.py
+-rw-r--r--   0        0        0      179 2024-05-15 13:12:48.961939 janim-1.0.3/janim/constants/degrees.py
+-rw-r--r--   0        0        0     4900 2024-05-15 13:12:48.962938 janim-1.0.3/janim/examples.py
+-rw-r--r--   0        0        0     1723 2024-05-15 13:12:49.008814 janim-1.0.3/janim/exception.py
+-rw-r--r--   0        0        0    41710 2024-05-20 02:25:11.810501 janim-1.0.3/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      330 2024-05-15 13:12:49.015794 janim-1.0.3/janim/gui/application.py
+-rw-r--r--   0        0        0      797 2024-05-15 13:12:49.024773 janim-1.0.3/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-05-15 13:12:49.034744 janim-1.0.3/janim/gui/export.png
+-rw-r--r--   0        0        0     1534 2024-05-15 13:12:49.035741 janim-1.0.3/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0     1465 2024-05-20 02:25:45.947783 janim-1.0.3/janim/gui/glwidget.py
+-rw-r--r--   0        0        0      903 2024-05-15 13:12:49.048708 janim-1.0.3/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5278 2024-05-15 13:12:49.058683 janim-1.0.3/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     8331 2024-05-15 13:12:49.074245 janim-1.0.3/janim/gui/selector.py
+-rw-r--r--   0        0        0     1710 2024-05-18 05:33:18.266011 janim-1.0.3/janim/imports.py
+-rw-r--r--   0        0        0     5727 2024-05-15 13:12:49.077235 janim-1.0.3/janim/items/audio.py
+-rw-r--r--   0        0        0     5362 2024-05-15 13:12:49.077235 janim-1.0.3/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8745 2024-05-15 13:12:49.078232 janim-1.0.3/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2165 2024-05-15 13:12:49.088209 janim-1.0.3/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8330 2024-05-15 13:12:49.097183 janim-1.0.3/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8784 2024-05-15 13:12:49.108152 janim-1.0.3/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6729 2024-05-15 13:12:49.109152 janim-1.0.3/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7917 2024-05-15 13:12:49.118125 janim-1.0.3/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5239 2024-05-15 13:12:49.119124 janim-1.0.3/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5242 2024-05-20 00:46:08.126552 janim-1.0.3/janim/items/image_item.py
+-rw-r--r--   0        0        0    19084 2024-05-15 13:12:49.121117 janim-1.0.3/janim/items/item.py
+-rw-r--r--   0        0        0     3262 2024-05-15 13:12:49.122116 janim-1.0.3/janim/items/points.py
+-rw-r--r--   0        0        0     7660 2024-05-15 13:12:49.123112 janim-1.0.3/janim/items/relation.py
+-rw-r--r--   0        0        0     2071 2024-05-15 13:12:49.131090 janim-1.0.3/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5955 2024-05-15 13:12:49.140067 janim-1.0.3/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1736 2024-05-15 13:12:49.148045 janim-1.0.3/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4377 2024-05-15 13:12:49.149042 janim-1.0.3/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     3090 2024-05-15 13:12:49.158019 janim-1.0.3/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       40 2024-05-15 13:12:49.165001 janim-1.0.3/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    16153 2024-05-15 13:12:49.165997 janim-1.0.3/janim/items/text/text.py
+-rw-r--r--   0        0        0     1094 2024-05-15 13:12:49.174974 janim-1.0.3/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5357 2024-05-15 13:12:49.174974 janim-1.0.3/janim/items/vitem.py
+-rw-r--r--   0        0        0      271 2024-05-15 13:12:49.182953 janim-1.0.3/janim/logger.py
+-rw-r--r--   0        0        0     3054 2024-05-15 13:12:49.192927 janim-1.0.3/janim/render/base.py
+-rw-r--r--   0        0        0     8857 2024-05-20 01:47:59.633622 janim-1.0.3/janim/render/impl.py
+-rw-r--r--   0        0        0      448 2024-05-15 13:12:49.208887 janim-1.0.3/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1250 2024-05-15 13:12:49.216861 janim-1.0.3/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      325 2024-05-15 13:12:49.225837 janim-1.0.3/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      180 2024-05-20 01:53:43.325091 janim-1.0.3/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      350 2024-05-15 13:12:49.247780 janim-1.0.3/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6950 2024-05-15 13:12:49.259747 janim-1.0.3/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      203 2024-05-15 13:12:49.269436 janim-1.0.3/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1073 2024-05-19 06:01:17.272817 janim-1.0.3/janim/render/texture.py
+-rw-r--r--   0        0        0     6971 2024-05-16 13:52:55.279071 janim-1.0.3/janim/render/writer.py
+-rw-r--r--   0        0        0      964 2024-05-15 13:12:49.278412 janim-1.0.3/janim/typing.py
+-rw-r--r--   0        0        0    17207 2024-05-15 13:12:49.289382 janim-1.0.3/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5515 2024-05-15 13:12:49.297361 janim-1.0.3/janim/utils/config.py
+-rw-r--r--   0        0        0     5786 2024-05-19 13:34:44.597026 janim-1.0.3/janim/utils/data.py
+-rw-r--r--   0        0        0      637 2024-05-15 13:12:49.317308 janim-1.0.3/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2483 2024-05-15 13:12:49.330273 janim-1.0.3/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     2995 2024-05-15 13:12:49.331270 janim-1.0.3/janim/utils/font.py
+-rw-r--r--   0        0        0     6369 2024-05-15 13:12:49.392575 janim-1.0.3/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5973 2024-05-15 13:12:49.403546 janim-1.0.3/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1870 2024-05-15 13:12:49.428480 janim-1.0.3/janim/utils/paths.py
+-rw-r--r--   0        0        0     2705 2024-05-15 13:12:49.435461 janim-1.0.3/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2651 2024-05-15 13:12:49.435461 janim-1.0.3/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8342 2024-05-15 13:12:49.436460 janim-1.0.3/janim/utils/signal.py
+-rw-r--r--   0        0        0     2000 2024-05-15 13:12:49.446431 janim-1.0.3/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0    10068 2024-05-15 13:12:49.456405 janim-1.0.3/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    18504 2024-05-15 13:12:49.457404 janim-1.0.3/logo.png
+-rw-r--r--   0        0        0     1030 2024-05-19 13:23:23.085515 janim-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.3/PKG-INFO
```

### Comparing `janim-1.0.2/.readthedocs.yaml` & `janim-1.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/LICENSE` & `janim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/README.md` & `janim-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/__main__.py` & `janim-1.0.3/janim/__main__.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/animation.py` & `janim-1.0.3/janim/anims/animation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/composition.py` & `janim-1.0.3/janim/anims/composition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,397 +1,397 @@
-00000000: 0d0a 6672 6f6d 206a 616e 696d 2e61 6e69  ..from janim.ani
-00000010: 6d73 2e61 6e69 6d61 7469 6f6e 2069 6d70  ms.animation imp
-00000020: 6f72 7420 416e 696d 6174 696f 6e0d 0a66  ort Animation..f
-00000030: 726f 6d20 6a61 6e69 6d2e 6578 6365 7074  rom janim.except
-00000040: 696f 6e20 696d 706f 7274 204e 6f74 416e  ion import NotAn
-00000050: 696d 6174 696f 6e45 7272 6f72 0d0a 6672  imationError..fr
-00000060: 6f6d 206a 616e 696d 2e75 7469 6c73 2e72  om janim.utils.r
-00000070: 6174 655f 6675 6e63 7469 6f6e 7320 696d  ate_functions im
-00000080: 706f 7274 2052 6174 6546 756e 632c 206c  port RateFunc, l
-00000090: 696e 6561 720d 0a0d 0a0d 0a63 6c61 7373  inear......class
-000000a0: 2041 6e69 6d47 726f 7570 2841 6e69 6d61   AnimGroup(Anima
-000000b0: 7469 6f6e 293a 0d0a 2020 2020 2727 270d  tion):..    '''.
-000000c0: 0a20 2020 20e5 8aa8 e794 bbe9 9b86 e590  .    ...........
-000000d0: 88ef bc88 e5b9 b6e5 8897 e689 a7e8 a18c  ................
-000000e0: efbc 890d 0a0d 0a20 2020 202d 20e8 8ba5  .......    - ...
-000000f0: e4b8 8de4 bca0 e585 a520 6060 6475 7261  ......... ``dura
-00000100: 7469 6f6e 6060 efbc 8ce5 8899 e5b0 86e7  tion``..........
-00000110: bb88 e6ad a2e6 97b6 e997 b4ef bc88 e5ad  ................
-00000120: 90e5 8aa8 e794 bbe7 bb93 e69d 9fe6 97b6  ................
-00000130: e997 b4e7 9a84 e69c 80e5 a4a7 e580 bcef  ................
-00000140: bc89 e4bd 9ce4 b8ba e8af a5e5 8aa8 e794  ................
-00000150: bbe9 9b86 e590 88e7 9a84 2060 6064 7572  .......... ``dur
-00000160: 6174 696f 6e60 600d 0a20 2020 202d 20e8  ation``..    - .
-00000170: 8ba5 e4bc a0e5 85a5 2060 6064 7572 6174  ........ ``durat
-00000180: 696f 6e60 60ef bc8c e588 99e4 bc9a e5b0  ion``...........
-00000190: 86e5 ad90 e58a a8e7 94bb e79a 84e6 97b6  ................
-000001a0: e997 b4e8 bf9b e8a1 8ce6 8b89 e4bc b8ef  ................
-000001b0: bc8c e4bd bfe5 be97 e7bb 88e6 ada2 e697  ................
-000001c0: b6e9 97b4 e4b8 8e20 6060 6475 7261 7469  ....... ``durati
-000001d0: 6f6e 6060 20e4 b880 e887 b40d 0a20 2020  on`` ........   
-000001e0: 202d 20e4 b894 e58f afe4 bba5 e4bd bfe7   - .............
-000001f0: 94a8 2060 6061 7460 6020 e8bf 9be8 a18c  .. ``at`` ......
-00000200: e680 bbe4 bd93 e581 8fe7 a7bb efbc 88e5  ................
-00000210: a682 2060 6061 743d 3160 6020 e588 99e6  .. ``at=1`` ....
-00000220: 98af e680 bbe4 bd93 e5bb b6e5 908e 2031  .............. 1
-00000230: 73ef bc89 0d0a 0d0a 2020 2020 e697 b6e9  s.......    ....
-00000240: 97b4 e7a4 bae4 be8b efbc 9a0d 0a0d 0a20  ............... 
-00000250: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-00000260: 3a3a 2070 7974 686f 6e0d 0a0d 0a20 2020  :: python....   
-00000270: 2020 2020 2041 6e69 6d47 726f 7570 280d       AnimGroup(.
-00000280: 0a20 2020 2020 2020 2020 2020 2041 6e69  .            Ani
-00000290: 6d31 2864 7572 6174 696f 6e3d 3329 2c0d  m1(duration=3),.
-000002a0: 0a20 2020 2020 2020 2020 2020 2041 6e69  .            Ani
-000002b0: 6d32 2864 7572 6174 696f 6e3d 3429 0d0a  m2(duration=4)..
-000002c0: 2020 2020 2020 2020 2920 2320 416e 696d          ) # Anim
-000002d0: 3120 e59c a820 307e 3373 20e6 89a7 e8a1  1 ... 0~3s .....
-000002e0: 8cef bc8c 416e 696d 3220 e59c a820 307e  ....Anim2 ... 0~
-000002f0: 3473 20e6 89a7 e8a1 8c0d 0a0d 0a20 2020  4s ..........   
-00000300: 2020 2020 2041 6e69 6d47 726f 7570 280d       AnimGroup(.
-00000310: 0a20 2020 2020 2020 2020 2020 2041 6e69  .            Ani
-00000320: 6d31 2864 7572 6174 696f 6e3d 3329 2c0d  m1(duration=3),.
-00000330: 0a20 2020 2020 2020 2020 2020 2041 6e69  .            Ani
-00000340: 6d32 2864 7572 6174 696f 6e3d 3429 2c0d  m2(duration=4),.
-00000350: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
-00000360: 6174 696f 6e3d 360d 0a20 2020 2020 2020  ation=6..       
-00000370: 2029 2023 2041 6e69 6d31 20e5 9ca8 2030   ) # Anim1 ... 0
-00000380: 7e34 2e35 7320 e689 a7e8 a18c efbc 8c41  ~4.5s .........A
-00000390: 6e69 6d32 20e5 9ca8 2030 7e36 7320 e689  nim2 ... 0~6s ..
-000003a0: a7e8 a18c 0d0a 0d0a 2020 2020 2020 2020  ........        
-000003b0: 416e 696d 4772 6f75 7028 0d0a 2020 2020  AnimGroup(..    
-000003c0: 2020 2020 2020 2020 416e 696d 3128 6475          Anim1(du
-000003d0: 7261 7469 6f6e 3d33 292c 0d0a 2020 2020  ration=3),..    
-000003e0: 2020 2020 2020 2020 416e 696d 3228 6475          Anim2(du
-000003f0: 7261 7469 6f6e 3d34 292c 0d0a 2020 2020  ration=4),..    
-00000400: 2020 2020 2020 2020 6174 3d31 2c0d 0a20          at=1,.. 
-00000410: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-00000420: 696f 6e3d 360d 0a20 2020 2020 2020 2029  ion=6..        )
-00000430: 2023 2041 6e69 6d31 20e5 9ca8 2031 7e35   # Anim1 ... 1~5
-00000440: 2e35 7320 e689 a7e8 a18c efbc 8c41 6e69  .5s .........Ani
-00000450: 6d32 20e5 9ca8 2031 7e37 7320 e689 a7e8  m2 ... 1~7s ....
-00000460: a18c 0d0a 2020 2020 2727 270d 0a20 2020  ....    '''..   
-00000470: 2064 6566 205f 5f69 6e69 745f 5f28 0d0a   def __init__(..
-00000480: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00000490: 2020 2020 2020 202a 616e 696d 733a 2041         *anims: A
-000004a0: 6e69 6d61 7469 6f6e 2c0d 0a20 2020 2020  nimation,..     
-000004b0: 2020 2064 7572 6174 696f 6e3a 2066 6c6f     duration: flo
-000004c0: 6174 207c 204e 6f6e 6520 3d20 4e6f 6e65  at | None = None
-000004d0: 2c0d 0a20 2020 2020 2020 2072 6174 655f  ,..        rate_
-000004e0: 6675 6e63 3a20 5261 7465 4675 6e63 203d  func: RateFunc =
-000004f0: 206c 696e 6561 722c 0d0a 2020 2020 2020   linear,..      
-00000500: 2020 5f67 6574 5f61 6e69 6d5f 6f62 6a65    _get_anim_obje
-00000510: 6374 733a 2062 6f6f 6c20 3d20 5472 7565  cts: bool = True
-00000520: 2c0d 0a20 2020 2020 2020 202a 2a6b 7761  ,..        **kwa
-00000530: 7267 730d 0a20 2020 2029 3a0d 0a20 2020  rgs..    ):..   
-00000540: 2020 2020 2069 6620 5f67 6574 5f61 6e69       if _get_ani
-00000550: 6d5f 6f62 6a65 6374 733a 0d0a 2020 2020  m_objects:..    
-00000560: 2020 2020 2020 2020 616e 696d 7320 3d20          anims = 
-00000570: 7365 6c66 2e5f 6765 745f 616e 696d 5f6f  self._get_anim_o
-00000580: 626a 6563 7473 2861 6e69 6d73 290d 0a20  bjects(anims).. 
-00000590: 2020 2020 2020 2073 656c 662e 616e 696d         self.anim
-000005a0: 7320 3d20 616e 696d 730d 0a20 2020 2020  s = anims..     
-000005b0: 2020 2073 656c 662e 6d61 7874 203d 2030     self.maxt = 0
-000005c0: 2069 6620 6e6f 7420 616e 696d 7320 656c   if not anims el
-000005d0: 7365 206d 6178 2861 6e69 6d2e 6c6f 6361  se max(anim.loca
-000005e0: 6c5f 7261 6e67 652e 656e 6420 666f 7220  l_range.end for 
-000005f0: 616e 696d 2069 6e20 616e 696d 7329 0d0a  anim in anims)..
-00000600: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
-00000610: 696f 6e20 6973 204e 6f6e 653a 0d0a 2020  ion is None:..  
-00000620: 2020 2020 2020 2020 2020 6475 7261 7469            durati
-00000630: 6f6e 203d 2073 656c 662e 6d61 7874 0d0a  on = self.maxt..
-00000640: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00000650: 292e 5f5f 696e 6974 5f5f 2864 7572 6174  ).__init__(durat
-00000660: 696f 6e3d 6475 7261 7469 6f6e 2c20 7261  ion=duration, ra
-00000670: 7465 5f66 756e 633d 7261 7465 5f66 756e  te_func=rate_fun
-00000680: 632c 202a 2a6b 7761 7267 7329 0d0a 2020  c, **kwargs)..  
-00000690: 2020 2020 2020 666f 7220 616e 696d 2069        for anim i
-000006a0: 6e20 7365 6c66 2e61 6e69 6d73 3a0d 0a20  n self.anims:.. 
-000006b0: 2020 2020 2020 2020 2020 2061 6e69 6d2e             anim.
-000006c0: 7061 7265 6e74 203d 2073 656c 660d 0a0d  parent = self...
-000006d0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-000006e0: 6f64 0d0a 2020 2020 6465 6620 5f67 6574  od..    def _get
-000006f0: 5f61 6e69 6d5f 6f62 6a65 6374 2861 6e69  _anim_object(ani
-00000700: 6d29 202d 3e20 416e 696d 6174 696f 6e3a  m) -> Animation:
-00000710: 0d0a 2020 2020 2020 2020 6174 7472 203d  ..        attr =
-00000720: 2067 6574 6174 7472 2861 6e69 6d2c 2027   getattr(anim, '
-00000730: 5f5f 616e 696d 5f5f 272c 204e 6f6e 6529  __anim__', None)
-00000740: 0d0a 2020 2020 2020 2020 6966 2061 7474  ..        if att
-00000750: 7220 6973 206e 6f74 204e 6f6e 6520 616e  r is not None an
-00000760: 6420 6361 6c6c 6162 6c65 2861 7474 7229  d callable(attr)
-00000770: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000780: 6574 7572 6e20 6174 7472 2829 0d0a 2020  eturn attr()..  
-00000790: 2020 2020 2020 7265 7475 726e 2061 6e69        return ani
-000007a0: 6d0d 0a0d 0a20 2020 2040 7374 6174 6963  m....    @static
-000007b0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-000007c0: 5f67 6574 5f61 6e69 6d5f 6f62 6a65 6374  _get_anim_object
-000007d0: 7328 616e 696d 733a 206c 6973 745b 416e  s(anims: list[An
-000007e0: 696d 6174 696f 6e5d 2920 2d3e 206c 6973  imation]) -> lis
-000007f0: 745b 416e 696d 6174 696f 6e5d 3a0d 0a20  t[Animation]:.. 
-00000800: 2020 2020 2020 2061 6e69 6d73 203d 205b         anims = [
-00000810: 0d0a 2020 2020 2020 2020 2020 2020 416e  ..            An
-00000820: 696d 4772 6f75 702e 5f67 6574 5f61 6e69  imGroup._get_ani
-00000830: 6d5f 6f62 6a65 6374 2861 6e69 6d29 0d0a  m_object(anim)..
-00000840: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00000850: 616e 696d 2069 6e20 616e 696d 730d 0a20  anim in anims.. 
-00000860: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-00000870: 2020 666f 7220 616e 696d 2069 6e20 616e    for anim in an
-00000880: 696d 733a 0d0a 2020 2020 2020 2020 2020  ims:..          
-00000890: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-000008a0: 6e63 6528 616e 696d 2c20 416e 696d 6174  nce(anim, Animat
-000008b0: 696f 6e29 3a0d 0a20 2020 2020 2020 2020  ion):..         
-000008c0: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-000008d0: 416e 696d 6174 696f 6e45 7272 6f72 2827  AnimationError('
-000008e0: e4bc a0e5 85a5 e4ba 86e9 9d9e e58a a8e7  ................
-000008f0: 94bb e5af b9e8 b1a1 efbc 8ce5 8faf e883  ................
-00000900: bde6 98af e4bd a0e5 bf98 e8ae b0e4 bdbf  ................
-00000910: e794 a820 2e61 6e69 6d20 e4ba 8627 290d  ... .anim ...').
-00000920: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00000930: 6e20 616e 696d 730d 0a0d 0a20 2020 2064  n anims....    d
-00000940: 6566 2066 6c61 7474 656e 2873 656c 6629  ef flatten(self)
-00000950: 202d 3e20 6c69 7374 5b41 6e69 6d61 7469   -> list[Animati
-00000960: 6f6e 5d3a 0d0a 2020 2020 2020 2020 7265  on]:..        re
-00000970: 7375 6c74 203d 205b 7365 6c66 5d0d 0a20  sult = [self].. 
-00000980: 2020 2020 2020 2066 6f72 2061 6e69 6d20         for anim 
-00000990: 696e 2073 656c 662e 616e 696d 733a 0d0a  in self.anims:..
-000009a0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000009b0: 7369 6e73 7461 6e63 6528 616e 696d 2c20  sinstance(anim, 
-000009c0: 416e 696d 4772 6f75 7029 3a0d 0a20 2020  AnimGroup):..   
-000009d0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-000009e0: 756c 742e 6578 7465 6e64 2861 6e69 6d2e  ult.extend(anim.
-000009f0: 666c 6174 7465 6e28 2929 0d0a 2020 2020  flatten())..    
-00000a00: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000a20: 6573 756c 742e 6170 7065 6e64 2861 6e69  esult.append(ani
-00000a30: 6d29 0d0a 0d0a 2020 2020 2020 2020 7265  m)....        re
-00000a40: 7475 726e 2072 6573 756c 740d 0a0d 0a20  turn result.... 
-00000a50: 2020 2064 6566 2063 6f6d 7075 7465 5f67     def compute_g
-00000a60: 6c6f 6261 6c5f 7261 6e67 6528 7365 6c66  lobal_range(self
-00000a70: 2c20 6174 3a20 666c 6f61 742c 2064 7572  , at: float, dur
-00000a80: 6174 696f 6e3a 2066 6c6f 6174 2920 2d3e  ation: float) ->
-00000a90: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00000aa0: 2727 270d 0a20 2020 2020 2020 20e8 aea1  '''..        ...
-00000ab0: e7ae 97e5 ad90 e58a a8e7 94bb e79a 84e6  ................
-00000ac0: 97b6 e997 b4e8 8c83 e59b b40d 0a0d 0a20  ............... 
-00000ad0: 2020 2020 2020 20e8 afa5 e696 b9e6 b395         .........
-00000ae0: e698 afe8 a2ab 203a 6d65 7468 3a60 7e2e  ...... :meth:`~.
-00000af0: 5469 6d65 6c69 6e65 2e70 7265 7061 7265  Timeline.prepare
-00000b00: 6020 e8b0 83e7 94a8 e4bb a5e8 aea1 e7ae  ` ..............
-00000b10: 97e7 9a84 0d0a 2020 2020 2020 2020 2727  ......        ''
-00000b20: 270d 0a20 2020 2020 2020 2073 7570 6572  '..        super
-00000b30: 2829 2e63 6f6d 7075 7465 5f67 6c6f 6261  ().compute_globa
-00000b40: 6c5f 7261 6e67 6528 6174 2c20 6475 7261  l_range(at, dura
-00000b50: 7469 6f6e 290d 0a0d 0a20 2020 2020 2020  tion)....       
-00000b60: 2066 6163 746f 7220 3d20 6475 7261 7469   factor = durati
-00000b70: 6f6e 202f 2073 656c 662e 6d61 7874 0d0a  on / self.maxt..
-00000b80: 0d0a 2020 2020 2020 2020 666f 7220 616e  ..        for an
-00000b90: 696d 2069 6e20 7365 6c66 2e61 6e69 6d73  im in self.anims
-00000ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
-00000bb0: 6e69 6d2e 636f 6d70 7574 655f 676c 6f62  nim.compute_glob
-00000bc0: 616c 5f72 616e 6765 280d 0a20 2020 2020  al_range(..     
-00000bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000be0: 676c 6f62 616c 5f72 616e 6765 2e61 7420  global_range.at 
-00000bf0: 2b20 616e 696d 2e6c 6f63 616c 5f72 616e  + anim.local_ran
-00000c00: 6765 2e61 7420 2a20 6661 6374 6f72 2c0d  ge.at * factor,.
-00000c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c20: 2061 6e69 6d2e 6c6f 6361 6c5f 7261 6e67   anim.local_rang
-00000c30: 652e 6475 7261 7469 6f6e 202a 2066 6163  e.duration * fac
-00000c40: 746f 720d 0a20 2020 2020 2020 2020 2020  tor..           
-00000c50: 2029 0d0a 0d0a 2020 2020 6465 6620 616e   )....    def an
-00000c60: 696d 5f70 7265 5f69 6e69 7428 7365 6c66  im_pre_init(self
-00000c70: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00000c80: 2020 2020 666f 7220 616e 696d 2069 6e20      for anim in 
-00000c90: 7365 6c66 2e61 6e69 6d73 3a0d 0a20 2020  self.anims:..   
-00000ca0: 2020 2020 2020 2020 2061 6e69 6d2e 616e           anim.an
-00000cb0: 696d 5f70 7265 5f69 6e69 7428 290d 0a0d  im_pre_init()...
-00000cc0: 0a20 2020 2064 6566 2061 6e69 6d5f 696e  .    def anim_in
-00000cd0: 6974 2873 656c 6629 202d 3e20 4e6f 6e65  it(self) -> None
-00000ce0: 3a0d 0a20 2020 2020 2020 2066 6f72 2061  :..        for a
-00000cf0: 6e69 6d20 696e 2073 656c 662e 616e 696d  nim in self.anim
-00000d00: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000d10: 616e 696d 2e61 6e69 6d5f 696e 6974 2829  anim.anim_init()
-00000d20: 0d0a 0d0a 2020 2020 6465 6620 6765 745f  ....    def get_
-00000d30: 616e 696d 5f74 2873 656c 662c 2061 6c70  anim_t(self, alp
-00000d40: 6861 3a20 666c 6f61 742c 2061 6e69 6d3a  ha: float, anim:
-00000d50: 2041 6e69 6d61 7469 6f6e 2920 2d3e 2066   Animation) -> f
-00000d60: 6c6f 6174 3a0d 0a20 2020 2020 2020 2072  loat:..        r
-00000d70: 6574 7572 6e20 616c 7068 6120 2a20 7365  eturn alpha * se
-00000d80: 6c66 2e6d 6178 7420 2d20 616e 696d 2e6c  lf.maxt - anim.l
-00000d90: 6f63 616c 5f72 616e 6765 2e61 740d 0a0d  ocal_range.at...
-00000da0: 0a20 2020 2064 6566 2061 6e69 6d5f 6f6e  .    def anim_on
-00000db0: 5f61 6c70 6861 2873 656c 662c 2061 6c70  _alpha(self, alp
-00000dc0: 6861 3a20 666c 6f61 7429 202d 3e20 4e6f  ha: float) -> No
-00000dd0: 6e65 3a0d 0a20 2020 2020 2020 2027 2727  ne:..        '''
-00000de0: 0d0a 2020 2020 2020 2020 e59c a8e8 afa5  ..        ......
-00000df0: e696 b9e6 b395 e4b8 adef bc8c 3a63 6c61  ............:cla
-00000e00: 7373 3a60 416e 696d 4772 6f75 7060 20e9  ss:`AnimGroup` .
-00000e10: 809a e8bf 8720 6060 616c 7068 6160 600d  ..... ``alpha``.
-00000e20: 0a20 2020 2020 2020 20e6 8da2 e7ae 97e5  .        .......
-00000e30: 87ba e5ad 90e5 8aa8 e794 bbe7 9a84 2060  .............. `
-00000e40: 606c 6f63 616c 5f74 6060 20e5 b9b6 e8b0  `local_t`` .....
-00000e50: 83e7 94a8 e5ad 90e5 8aa8 e794 bbe7 9a84  ................
-00000e60: 203a 6d65 7468 3a60 7e2e 416e 696d 6174   :meth:`~.Animat
-00000e70: 696f 6e2e 616e 696d 5f6f 6e60 20e6 96b9  ion.anim_on` ...
-00000e80: e6b3 950d 0a20 2020 2020 2020 2027 2727  .....        '''
-00000e90: 0d0a 2020 2020 2020 2020 676c 6f62 616c  ..        global
-00000ea0: 5f74 203d 2073 656c 662e 676c 6f62 616c  _t = self.global
-00000eb0: 5f74 5f63 7478 2e67 6574 2829 0d0a 0d0a  _t_ctx.get()....
-00000ec0: 2020 2020 2020 2020 666f 7220 616e 696d          for anim
-00000ed0: 2069 6e20 7365 6c66 2e61 6e69 6d73 3a0d   in self.anims:.
-00000ee0: 0a20 2020 2020 2020 2020 2020 2061 6e69  .            ani
-00000ef0: 6d5f 7420 3d20 7365 6c66 2e67 6574 5f61  m_t = self.get_a
-00000f00: 6e69 6d5f 7428 616c 7068 612c 2061 6e69  nim_t(alpha, ani
-00000f10: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
-00000f20: 6966 2061 6e69 6d2e 676c 6f62 616c 5f72  if anim.global_r
-00000f30: 616e 6765 2e61 7420 3c3d 2067 6c6f 6261  ange.at <= globa
-00000f40: 6c5f 7420 3c20 616e 696d 2e67 6c6f 6261  l_t < anim.globa
-00000f50: 6c5f 7261 6e67 652e 656e 643a 0d0a 2020  l_range.end:..  
-00000f60: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00000f70: 696d 2e61 6e69 6d5f 6f6e 2861 6e69 6d5f  im.anim_on(anim_
-00000f80: 7429 0d0a 0d0a 0d0a 636c 6173 7320 5375  t)......class Su
-00000f90: 6363 6573 7369 6f6e 2841 6e69 6d47 726f  ccession(AnimGro
-00000fa0: 7570 293a 0d0a 2020 2020 2727 270d 0a20  up):..    '''.. 
-00000fb0: 2020 20e5 8aa8 e794 bbe9 9b86 e590 88ef     .............
-00000fc0: bc88 e9a1 bae5 ba8f e689 a7e8 a18c efbc  ................
-00000fd0: 890d 0a0d 0a20 2020 202d 20e4 bc9a e5b0  .....    - .....
-00000fe0: 86e4 bca0 e585 a5e7 9a84 e58a a8e7 94bb  ................
-00000ff0: e4be 9de6 aca1 e689 a7e8 a18c efbc 8ce4  ................
-00001000: b88d e5b9 b6e8 a18c 0d0a 2020 2020 2d20  ..........    - 
-00001010: e58f afe4 bba5 e4bc a0e5 85a5 2060 6275  ............ `bu
-00001020: 6666 6020 e68c 87e5 ae9a e589 8de5 908e  ff` ............
-00001030: e58a a8e7 94bb e4b8 ade9 97b4 e79a 84e7  ................
-00001040: a9ba e799 bde6 97b6 e997 b40d 0a20 2020  .............   
-00001050: 202d 20e5 85b6 e4bd 99e4 b88e 2060 416e   - ......... `An
-00001060: 696d 4772 6f75 7060 20e7 9bb8 e590 8c0d  imGroup` .......
-00001070: 0a0d 0a20 2020 20e6 97b6 e997 b4e7 a4ba  ...    .........
-00001080: e4be 8bef bc9a 0d0a 0d0a 2020 2020 2e2e  ..........    ..
-00001090: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-000010a0: 7468 6f6e 0d0a 0d0a 2020 2020 2020 2020  thon....        
-000010b0: 5375 6363 6573 7369 6f6e 280d 0a20 2020  Succession(..   
-000010c0: 2020 2020 2020 2020 2041 6e69 6d31 2864           Anim1(d
-000010d0: 7572 6174 696f 6e3d 3329 2c0d 0a20 2020  uration=3),..   
-000010e0: 2020 2020 2020 2020 2041 6e69 6d32 2864           Anim2(d
-000010f0: 7572 6174 696f 6e3d 3429 0d0a 2020 2020  uration=4)..    
-00001100: 2020 2020 2920 2320 416e 696d 3120 e59c      ) # Anim1 ..
-00001110: a820 307e 3373 20e6 89a7 e8a1 8cef bc8c  . 0~3s .........
-00001120: 416e 696d 3220 e59c a820 337e 3773 20e6  Anim2 ... 3~7s .
-00001130: 89a7 e8a1 8c0d 0a0d 0a20 2020 2020 2020  .........       
-00001140: 2053 7563 6365 7373 696f 6e28 0d0a 2020   Succession(..  
-00001150: 2020 2020 2020 2020 2020 416e 696d 3128            Anim1(
-00001160: 6475 7261 7469 6f6e 3d32 292c 0d0a 2020  duration=2),..  
-00001170: 2020 2020 2020 2020 2020 416e 696d 3228            Anim2(
-00001180: 6174 3d31 2c20 6475 7261 7469 6f6e 3d32  at=1, duration=2
-00001190: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000011a0: 416e 696d 3328 6174 3d30 2e35 2c20 6475  Anim3(at=0.5, du
-000011b0: 7261 7469 6f6e 3d32 290d 0a20 2020 2020  ration=2)..     
-000011c0: 2020 2029 2023 2041 6e69 6d31 20e5 9ca8     ) # Anim1 ...
-000011d0: 2030 7e32 7320 e689 a7e8 a18c efbc 8c41   0~2s .........A
-000011e0: 6e69 6d32 20e5 9ca8 2033 7e35 7320 e689  nim2 ... 3~5s ..
-000011f0: a7e8 a18c efbc 8c41 6e69 6d33 20e5 9ca8  .......Anim3 ...
-00001200: 2035 2e35 7e37 2e35 7320 e689 a7e8 a18c   5.5~7.5s ......
-00001210: 0d0a 0d0a 2020 2020 2020 2020 5375 6363  ....        Succ
-00001220: 6573 7369 6f6e 280d 0a20 2020 2020 2020  ession(..       
-00001230: 2020 2020 2041 6e69 6d31 2864 7572 6174       Anim1(durat
-00001240: 696f 6e3d 3229 2c0d 0a20 2020 2020 2020  ion=2),..       
-00001250: 2020 2020 2041 6e69 6d32 2864 7572 6174       Anim2(durat
-00001260: 696f 6e3d 3229 2c0d 0a20 2020 2020 2020  ion=2),..       
-00001270: 2020 2020 2041 6e69 6d33 2864 7572 6174       Anim3(durat
-00001280: 696f 6e3d 3229 2c0d 0a20 2020 2020 2020  ion=2),..       
-00001290: 2020 2020 2062 7566 663d 302e 350d 0a20       buff=0.5.. 
-000012a0: 2020 2020 2020 2029 2023 2041 6e69 6d31         ) # Anim1
-000012b0: 20e5 9ca8 2030 7e32 7320 e689 a7e8 a18c   ... 0~2s ......
-000012c0: efbc 8c41 6e69 6d32 20e5 9ca8 2032 2e35  ...Anim2 ... 2.5
-000012d0: 7e34 2e35 7320 e689 a7e8 a18c efbc 8c41  ~4.5s .........A
-000012e0: 6e69 6d33 20e5 9ca8 2035 7e37 7320 e689  nim3 ... 5~7s ..
-000012f0: a7e8 a18c 0d0a 2020 2020 2727 270d 0a20  ......    '''.. 
-00001300: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001310: 7365 6c66 2c20 2a61 6e69 6d73 3a20 416e  self, *anims: An
-00001320: 696d 6174 696f 6e2c 2062 7566 663a 2066  imation, buff: f
-00001330: 6c6f 6174 203d 2030 2c20 2a2a 6b77 6172  loat = 0, **kwar
-00001340: 6773 293a 0d0a 2020 2020 2020 2020 616e  gs):..        an
-00001350: 696d 7320 3d20 7365 6c66 2e5f 6765 745f  ims = self._get_
-00001360: 616e 696d 5f6f 626a 6563 7473 2861 6e69  anim_objects(ani
-00001370: 6d73 290d 0a20 2020 2020 2020 2065 6e64  ms)..        end
-00001380: 5f74 696d 6520 3d20 300d 0a20 2020 2020  _time = 0..     
-00001390: 2020 2066 6f72 2061 6e69 6d20 696e 2061     for anim in a
-000013a0: 6e69 6d73 3a0d 0a20 2020 2020 2020 2020  nims:..         
-000013b0: 2020 2061 6e69 6d2e 6c6f 6361 6c5f 7261     anim.local_ra
-000013c0: 6e67 652e 6174 202b 3d20 656e 645f 7469  nge.at += end_ti
-000013d0: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
-000013e0: 656e 645f 7469 6d65 203d 2061 6e69 6d2e  end_time = anim.
-000013f0: 6c6f 6361 6c5f 7261 6e67 652e 656e 6420  local_range.end 
-00001400: 2b20 6275 6666 0d0a 2020 2020 2020 2020  + buff..        
-00001410: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-00001420: 282a 616e 696d 732c 205f 6765 745f 616e  (*anims, _get_an
-00001430: 696d 5f6f 626a 6563 7473 3d46 616c 7365  im_objects=False
-00001440: 2c20 2a2a 6b77 6172 6773 290d 0a0d 0a0d  , **kwargs).....
-00001450: 0a63 6c61 7373 2041 6c69 676e 6564 2841  .class Aligned(A
-00001460: 6e69 6d47 726f 7570 293a 0d0a 2020 2020  nimGroup):..    
-00001470: 2727 270d 0a20 2020 20e5 8aa8 e794 bbe9  '''..    .......
-00001480: 9b86 e590 88ef bc88 e5b9 b6e5 8897 e5af  ................
-00001490: b9e9 bd90 e689 a7e8 a18c efbc 890d 0a0d  ................
-000014a0: 0a20 2020 20e6 97b6 e997 b4e7 a4ba e4be  .    ...........
-000014b0: 8bef bc9a 0d0a 0d0a 2020 2020 2e2e 2063  ........    .. c
-000014c0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-000014d0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 416c  on....        Al
-000014e0: 6967 6e65 6428 0d0a 2020 2020 2020 2020  igned(..        
-000014f0: 2020 2020 416e 696d 3128 6475 7261 7469      Anim1(durati
-00001500: 6f6e 3d31 292c 0d0a 2020 2020 2020 2020  on=1),..        
-00001510: 2020 2020 416e 696d 3228 6475 7261 7469      Anim2(durati
-00001520: 6f6e 3d32 290d 0a20 2020 2020 2020 2029  on=2)..        )
-00001530: 2023 2041 6e69 6d31 20e5 928c 2041 6e69   # Anim1 ... Ani
-00001540: 6d32 20e9 83bd e59c a820 307e 3273 20e6  m2 ...... 0~2s .
-00001550: 89a7 e8a1 8c0d 0a0d 0a20 2020 2020 2020  .........       
-00001560: 2041 6c69 676e 6564 280d 0a20 2020 2020   Aligned(..     
-00001570: 2020 2020 2020 2041 6e69 6d31 2864 7572         Anim1(dur
-00001580: 6174 696f 6e3d 3129 2c0d 0a20 2020 2020  ation=1),..     
-00001590: 2020 2020 2020 2041 6e69 6d32 2864 7572         Anim2(dur
-000015a0: 6174 696f 6e3d 3229 2c0d 0a20 2020 2020  ation=2),..     
-000015b0: 2020 2020 2020 2064 7572 6174 696f 6e3d         duration=
-000015c0: 340d 0a20 2020 2020 2020 2029 2023 2041  4..        ) # A
-000015d0: 6e69 6d31 20e5 928c 2041 6e69 6d32 20e9  nim1 ... Anim2 .
-000015e0: 83bd e59c a820 307e 3473 20e6 89a7 e8a1  ..... 0~4s .....
-000015f0: 8c0d 0a20 2020 2027 2727 0d0a 2020 2020  ...    '''..    
-00001600: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001610: 662c 202a 616e 696d 733a 2041 6e69 6d61  f, *anims: Anima
-00001620: 7469 6f6e 2c20 6475 7261 7469 6f6e 3a20  tion, duration: 
-00001630: 666c 6f61 7420 7c20 4e6f 6e65 203d 204e  float | None = N
-00001640: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0d  one, **kwargs):.
-00001650: 0a20 2020 2020 2020 2061 6e69 6d73 203d  .        anims =
-00001660: 2073 656c 662e 5f67 6574 5f61 6e69 6d5f   self._get_anim_
-00001670: 6f62 6a65 6374 7328 616e 696d 7329 0d0a  objects(anims)..
-00001680: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
-00001690: 696f 6e20 6973 204e 6f6e 653a 0d0a 2020  ion is None:..  
-000016a0: 2020 2020 2020 2020 2020 6475 7261 7469            durati
-000016b0: 6f6e 203d 206d 6178 2861 6e69 6d2e 6c6f  on = max(anim.lo
-000016c0: 6361 6c5f 7261 6e67 652e 656e 6420 666f  cal_range.end fo
-000016d0: 7220 616e 696d 2069 6e20 616e 696d 7329  r anim in anims)
-000016e0: 0d0a 0d0a 2020 2020 2020 2020 7375 7065  ....        supe
-000016f0: 7228 292e 5f5f 696e 6974 5f5f 282a 616e  r().__init__(*an
-00001700: 696d 732c 2064 7572 6174 696f 6e3d 6475  ims, duration=du
-00001710: 7261 7469 6f6e 2c20 5f67 6574 5f61 6e69  ration, _get_ani
-00001720: 6d5f 6f62 6a65 6374 733d 4661 6c73 652c  m_objects=False,
-00001730: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
-00001740: 2020 6465 6620 636f 6d70 7574 655f 676c    def compute_gl
-00001750: 6f62 616c 5f72 616e 6765 2873 656c 662c  obal_range(self,
-00001760: 2061 743a 2066 6c6f 6174 2c20 6475 7261   at: float, dura
-00001770: 7469 6f6e 3a20 666c 6f61 7429 202d 3e20  tion: float) -> 
-00001780: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2041  None:..        A
-00001790: 6e69 6d61 7469 6f6e 2e63 6f6d 7075 7465  nimation.compute
-000017a0: 5f67 6c6f 6261 6c5f 7261 6e67 6528 7365  _global_range(se
-000017b0: 6c66 2c20 6174 2c20 6475 7261 7469 6f6e  lf, at, duration
-000017c0: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
-000017d0: 2061 6e69 6d20 696e 2073 656c 662e 616e   anim in self.an
-000017e0: 696d 733a 0d0a 2020 2020 2020 2020 2020  ims:..          
-000017f0: 2020 6661 6374 6f72 203d 2064 7572 6174    factor = durat
-00001800: 696f 6e20 2f20 616e 696d 2e6c 6f63 616c  ion / anim.local
-00001810: 5f72 616e 6765 2e65 6e64 0d0a 2020 2020  _range.end..    
-00001820: 2020 2020 2020 2020 616e 696d 2e63 6f6d          anim.com
-00001830: 7075 7465 5f67 6c6f 6261 6c5f 7261 6e67  pute_global_rang
-00001840: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-00001850: 2020 2020 7365 6c66 2e67 6c6f 6261 6c5f      self.global_
-00001860: 7261 6e67 652e 6174 202b 2061 6e69 6d2e  range.at + anim.
-00001870: 6c6f 6361 6c5f 7261 6e67 652e 6174 202a  local_range.at *
-00001880: 2066 6163 746f 722c 0d0a 2020 2020 2020   factor,..      
-00001890: 2020 2020 2020 2020 2020 616e 696d 2e6c            anim.l
-000018a0: 6f63 616c 5f72 616e 6765 2e64 7572 6174  ocal_range.durat
-000018b0: 696f 6e20 2a20 6661 6374 6f72 0d0a 2020  ion * factor..  
-000018c0: 2020 2020 2020 2020 2020 290d 0a                   )..
+00000000: 6672 6f6d 206a 616e 696d 2e61 6e69 6d73  from janim.anims
+00000010: 2e61 6e69 6d61 7469 6f6e 2069 6d70 6f72  .animation impor
+00000020: 7420 416e 696d 6174 696f 6e0d 0a66 726f  t Animation..fro
+00000030: 6d20 6a61 6e69 6d2e 6578 6365 7074 696f  m janim.exceptio
+00000040: 6e20 696d 706f 7274 204e 6f74 416e 696d  n import NotAnim
+00000050: 6174 696f 6e45 7272 6f72 0d0a 6672 6f6d  ationError..from
+00000060: 206a 616e 696d 2e75 7469 6c73 2e72 6174   janim.utils.rat
+00000070: 655f 6675 6e63 7469 6f6e 7320 696d 706f  e_functions impo
+00000080: 7274 2052 6174 6546 756e 632c 206c 696e  rt RateFunc, lin
+00000090: 6561 720d 0a0d 0a0d 0a63 6c61 7373 2041  ear......class A
+000000a0: 6e69 6d47 726f 7570 2841 6e69 6d61 7469  nimGroup(Animati
+000000b0: 6f6e 293a 0d0a 2020 2020 2727 270d 0a20  on):..    '''.. 
+000000c0: 2020 20e5 8aa8 e794 bbe9 9b86 e590 88ef     .............
+000000d0: bc88 e5b9 b6e5 8897 e689 a7e8 a18c efbc  ................
+000000e0: 890d 0a0d 0a20 2020 202d 20e8 8ba5 e4b8  .....    - .....
+000000f0: 8de4 bca0 e585 a520 6060 6475 7261 7469  ....... ``durati
+00000100: 6f6e 6060 efbc 8ce5 8899 e5b0 86e7 bb88  on``............
+00000110: e6ad a2e6 97b6 e997 b4ef bc88 e5ad 90e5  ................
+00000120: 8aa8 e794 bbe7 bb93 e69d 9fe6 97b6 e997  ................
+00000130: b4e7 9a84 e69c 80e5 a4a7 e580 bcef bc89  ................
+00000140: e4bd 9ce4 b8ba e8af a5e5 8aa8 e794 bbe9  ................
+00000150: 9b86 e590 88e7 9a84 2060 6064 7572 6174  ........ ``durat
+00000160: 696f 6e60 600d 0a20 2020 202d 20e8 8ba5  ion``..    - ...
+00000170: e4bc a0e5 85a5 2060 6064 7572 6174 696f  ...... ``duratio
+00000180: 6e60 60ef bc8c e588 99e4 bc9a e5b0 86e5  n``.............
+00000190: ad90 e58a a8e7 94bb e79a 84e6 97b6 e997  ................
+000001a0: b4e8 bf9b e8a1 8ce6 8b89 e4bc b8ef bc8c  ................
+000001b0: e4bd bfe5 be97 e7bb 88e6 ada2 e697 b6e9  ................
+000001c0: 97b4 e4b8 8e20 6060 6475 7261 7469 6f6e  ..... ``duration
+000001d0: 6060 20e4 b880 e887 b40d 0a20 2020 202d  `` ........    -
+000001e0: 20e4 b894 e58f afe4 bba5 e4bd bfe7 94a8   ...............
+000001f0: 2060 6061 7460 6020 e8bf 9be8 a18c e680   ``at`` ........
+00000200: bbe4 bd93 e581 8fe7 a7bb efbc 88e5 a682  ................
+00000210: 2060 6061 743d 3160 6020 e588 99e6 98af   ``at=1`` ......
+00000220: e680 bbe4 bd93 e5bb b6e5 908e 2031 73ef  ............ 1s.
+00000230: bc89 0d0a 0d0a 2020 2020 e697 b6e9 97b4  ......    ......
+00000240: e7a4 bae4 be8b efbc 9a0d 0a0d 0a20 2020  .............   
+00000250: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+00000260: 2070 7974 686f 6e0d 0a0d 0a20 2020 2020   python....     
+00000270: 2020 2041 6e69 6d47 726f 7570 280d 0a20     AnimGroup(.. 
+00000280: 2020 2020 2020 2020 2020 2041 6e69 6d31             Anim1
+00000290: 2864 7572 6174 696f 6e3d 3329 2c0d 0a20  (duration=3),.. 
+000002a0: 2020 2020 2020 2020 2020 2041 6e69 6d32             Anim2
+000002b0: 2864 7572 6174 696f 6e3d 3429 0d0a 2020  (duration=4)..  
+000002c0: 2020 2020 2020 2920 2320 416e 696d 3120        ) # Anim1 
+000002d0: e59c a820 307e 3373 20e6 89a7 e8a1 8cef  ... 0~3s .......
+000002e0: bc8c 416e 696d 3220 e59c a820 307e 3473  ..Anim2 ... 0~4s
+000002f0: 20e6 89a7 e8a1 8c0d 0a0d 0a20 2020 2020   ..........     
+00000300: 2020 2041 6e69 6d47 726f 7570 280d 0a20     AnimGroup(.. 
+00000310: 2020 2020 2020 2020 2020 2041 6e69 6d31             Anim1
+00000320: 2864 7572 6174 696f 6e3d 3329 2c0d 0a20  (duration=3),.. 
+00000330: 2020 2020 2020 2020 2020 2041 6e69 6d32             Anim2
+00000340: 2864 7572 6174 696f 6e3d 3429 2c0d 0a20  (duration=4),.. 
+00000350: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+00000360: 696f 6e3d 360d 0a20 2020 2020 2020 2029  ion=6..        )
+00000370: 2023 2041 6e69 6d31 20e5 9ca8 2030 7e34   # Anim1 ... 0~4
+00000380: 2e35 7320 e689 a7e8 a18c efbc 8c41 6e69  .5s .........Ani
+00000390: 6d32 20e5 9ca8 2030 7e36 7320 e689 a7e8  m2 ... 0~6s ....
+000003a0: a18c 0d0a 0d0a 2020 2020 2020 2020 416e  ......        An
+000003b0: 696d 4772 6f75 7028 0d0a 2020 2020 2020  imGroup(..      
+000003c0: 2020 2020 2020 416e 696d 3128 6475 7261        Anim1(dura
+000003d0: 7469 6f6e 3d33 292c 0d0a 2020 2020 2020  tion=3),..      
+000003e0: 2020 2020 2020 416e 696d 3228 6475 7261        Anim2(dura
+000003f0: 7469 6f6e 3d34 292c 0d0a 2020 2020 2020  tion=4),..      
+00000400: 2020 2020 2020 6174 3d31 2c0d 0a20 2020        at=1,..   
+00000410: 2020 2020 2020 2020 2064 7572 6174 696f           duratio
+00000420: 6e3d 360d 0a20 2020 2020 2020 2029 2023  n=6..        ) #
+00000430: 2041 6e69 6d31 20e5 9ca8 2031 7e35 2e35   Anim1 ... 1~5.5
+00000440: 7320 e689 a7e8 a18c efbc 8c41 6e69 6d32  s .........Anim2
+00000450: 20e5 9ca8 2031 7e37 7320 e689 a7e8 a18c   ... 1~7s ......
+00000460: 0d0a 2020 2020 2727 270d 0a20 2020 2064  ..    '''..    d
+00000470: 6566 205f 5f69 6e69 745f 5f28 0d0a 2020  ef __init__(..  
+00000480: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00000490: 2020 2020 202a 616e 696d 733a 2041 6e69       *anims: Ani
+000004a0: 6d61 7469 6f6e 2c0d 0a20 2020 2020 2020  mation,..       
+000004b0: 2064 7572 6174 696f 6e3a 2066 6c6f 6174   duration: float
+000004c0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c0d   | None = None,.
+000004d0: 0a20 2020 2020 2020 2072 6174 655f 6675  .        rate_fu
+000004e0: 6e63 3a20 5261 7465 4675 6e63 203d 206c  nc: RateFunc = l
+000004f0: 696e 6561 722c 0d0a 2020 2020 2020 2020  inear,..        
+00000500: 5f67 6574 5f61 6e69 6d5f 6f62 6a65 6374  _get_anim_object
+00000510: 733a 2062 6f6f 6c20 3d20 5472 7565 2c0d  s: bool = True,.
+00000520: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+00000530: 730d 0a20 2020 2029 3a0d 0a20 2020 2020  s..    ):..     
+00000540: 2020 2069 6620 5f67 6574 5f61 6e69 6d5f     if _get_anim_
+00000550: 6f62 6a65 6374 733a 0d0a 2020 2020 2020  objects:..      
+00000560: 2020 2020 2020 616e 696d 7320 3d20 7365        anims = se
+00000570: 6c66 2e5f 6765 745f 616e 696d 5f6f 626a  lf._get_anim_obj
+00000580: 6563 7473 2861 6e69 6d73 290d 0a20 2020  ects(anims)..   
+00000590: 2020 2020 2073 656c 662e 616e 696d 7320       self.anims 
+000005a0: 3d20 616e 696d 730d 0a20 2020 2020 2020  = anims..       
+000005b0: 2073 656c 662e 6d61 7874 203d 2030 2069   self.maxt = 0 i
+000005c0: 6620 6e6f 7420 616e 696d 7320 656c 7365  f not anims else
+000005d0: 206d 6178 2861 6e69 6d2e 6c6f 6361 6c5f   max(anim.local_
+000005e0: 7261 6e67 652e 656e 6420 666f 7220 616e  range.end for an
+000005f0: 696d 2069 6e20 616e 696d 7329 0d0a 2020  im in anims)..  
+00000600: 2020 2020 2020 6966 2064 7572 6174 696f        if duratio
+00000610: 6e20 6973 204e 6f6e 653a 0d0a 2020 2020  n is None:..    
+00000620: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
+00000630: 203d 2073 656c 662e 6d61 7874 0d0a 0d0a   = self.maxt....
+00000640: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00000650: 5f5f 696e 6974 5f5f 2864 7572 6174 696f  __init__(duratio
+00000660: 6e3d 6475 7261 7469 6f6e 2c20 7261 7465  n=duration, rate
+00000670: 5f66 756e 633d 7261 7465 5f66 756e 632c  _func=rate_func,
+00000680: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
+00000690: 2020 2020 666f 7220 616e 696d 2069 6e20      for anim in 
+000006a0: 7365 6c66 2e61 6e69 6d73 3a0d 0a20 2020  self.anims:..   
+000006b0: 2020 2020 2020 2020 2061 6e69 6d2e 7061           anim.pa
+000006c0: 7265 6e74 203d 2073 656c 660d 0a0d 0a20  rent = self.... 
+000006d0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+000006e0: 0d0a 2020 2020 6465 6620 5f67 6574 5f61  ..    def _get_a
+000006f0: 6e69 6d5f 6f62 6a65 6374 2861 6e69 6d29  nim_object(anim)
+00000700: 202d 3e20 416e 696d 6174 696f 6e3a 0d0a   -> Animation:..
+00000710: 2020 2020 2020 2020 6174 7472 203d 2067          attr = g
+00000720: 6574 6174 7472 2861 6e69 6d2c 2027 5f5f  etattr(anim, '__
+00000730: 616e 696d 5f5f 272c 204e 6f6e 6529 0d0a  anim__', None)..
+00000740: 2020 2020 2020 2020 6966 2061 7474 7220          if attr 
+00000750: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00000760: 6361 6c6c 6162 6c65 2861 7474 7229 3a0d  callable(attr):.
+00000770: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000780: 7572 6e20 6174 7472 2829 0d0a 2020 2020  urn attr()..    
+00000790: 2020 2020 7265 7475 726e 2061 6e69 6d0d      return anim.
+000007a0: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+000007b0: 7468 6f64 0d0a 2020 2020 6465 6620 5f67  thod..    def _g
+000007c0: 6574 5f61 6e69 6d5f 6f62 6a65 6374 7328  et_anim_objects(
+000007d0: 616e 696d 733a 206c 6973 745b 416e 696d  anims: list[Anim
+000007e0: 6174 696f 6e5d 2920 2d3e 206c 6973 745b  ation]) -> list[
+000007f0: 416e 696d 6174 696f 6e5d 3a0d 0a20 2020  Animation]:..   
+00000800: 2020 2020 2061 6e69 6d73 203d 205b 0d0a       anims = [..
+00000810: 2020 2020 2020 2020 2020 2020 416e 696d              Anim
+00000820: 4772 6f75 702e 5f67 6574 5f61 6e69 6d5f  Group._get_anim_
+00000830: 6f62 6a65 6374 2861 6e69 6d29 0d0a 2020  object(anim)..  
+00000840: 2020 2020 2020 2020 2020 666f 7220 616e            for an
+00000850: 696d 2069 6e20 616e 696d 730d 0a20 2020  im in anims..   
+00000860: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
+00000870: 666f 7220 616e 696d 2069 6e20 616e 696d  for anim in anim
+00000880: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000890: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+000008a0: 6528 616e 696d 2c20 416e 696d 6174 696f  e(anim, Animatio
+000008b0: 6e29 3a0d 0a20 2020 2020 2020 2020 2020  n):..           
+000008c0: 2020 2020 2072 6169 7365 204e 6f74 416e       raise NotAn
+000008d0: 696d 6174 696f 6e45 7272 6f72 2827 e4bc  imationError('..
+000008e0: a0e5 85a5 e4ba 86e9 9d9e e58a a8e7 94bb  ................
+000008f0: e5af b9e8 b1a1 efbc 8ce5 8faf e883 bde6  ................
+00000900: 98af e4bd a0e5 bf98 e8ae b0e4 bdbf e794  ................
+00000910: a820 2e61 6e69 6d20 e4ba 8627 290d 0a0d  . .anim ...')...
+00000920: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000930: 616e 696d 730d 0a0d 0a20 2020 2064 6566  anims....    def
+00000940: 2066 6c61 7474 656e 2873 656c 6629 202d   flatten(self) -
+00000950: 3e20 6c69 7374 5b41 6e69 6d61 7469 6f6e  > list[Animation
+00000960: 5d3a 0d0a 2020 2020 2020 2020 7265 7375  ]:..        resu
+00000970: 6c74 203d 205b 7365 6c66 5d0d 0a20 2020  lt = [self]..   
+00000980: 2020 2020 2066 6f72 2061 6e69 6d20 696e       for anim in
+00000990: 2073 656c 662e 616e 696d 733a 0d0a 2020   self.anims:..  
+000009a0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+000009b0: 6e73 7461 6e63 6528 616e 696d 2c20 416e  nstance(anim, An
+000009c0: 696d 4772 6f75 7029 3a0d 0a20 2020 2020  imGroup):..     
+000009d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000009e0: 742e 6578 7465 6e64 2861 6e69 6d2e 666c  t.extend(anim.fl
+000009f0: 6174 7465 6e28 2929 0d0a 2020 2020 2020  atten())..      
+00000a00: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000a10: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00000a20: 756c 742e 6170 7065 6e64 2861 6e69 6d29  ult.append(anim)
+00000a30: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+00000a40: 726e 2072 6573 756c 740d 0a0d 0a20 2020  rn result....   
+00000a50: 2064 6566 2063 6f6d 7075 7465 5f67 6c6f   def compute_glo
+00000a60: 6261 6c5f 7261 6e67 6528 7365 6c66 2c20  bal_range(self, 
+00000a70: 6174 3a20 666c 6f61 742c 2064 7572 6174  at: float, durat
+00000a80: 696f 6e3a 2066 6c6f 6174 2920 2d3e 204e  ion: float) -> N
+00000a90: 6f6e 653a 0d0a 2020 2020 2020 2020 2727  one:..        ''
+00000aa0: 270d 0a20 2020 2020 2020 20e8 aea1 e7ae  '..        .....
+00000ab0: 97e5 ad90 e58a a8e7 94bb e79a 84e6 97b6  ................
+00000ac0: e997 b4e8 8c83 e59b b40d 0a0d 0a20 2020  .............   
+00000ad0: 2020 2020 20e8 afa5 e696 b9e6 b395 e698       ...........
+00000ae0: afe8 a2ab 203a 6d65 7468 3a60 7e2e 5469  .... :meth:`~.Ti
+00000af0: 6d65 6c69 6e65 2e70 7265 7061 7265 6020  meline.prepare` 
+00000b00: e8b0 83e7 94a8 e4bb a5e8 aea1 e7ae 97e7  ................
+00000b10: 9a84 0d0a 2020 2020 2020 2020 2727 270d  ....        '''.
+00000b20: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00000b30: 2e63 6f6d 7075 7465 5f67 6c6f 6261 6c5f  .compute_global_
+00000b40: 7261 6e67 6528 6174 2c20 6475 7261 7469  range(at, durati
+00000b50: 6f6e 290d 0a0d 0a20 2020 2020 2020 2066  on)....        f
+00000b60: 6163 746f 7220 3d20 6475 7261 7469 6f6e  actor = duration
+00000b70: 202f 2073 656c 662e 6d61 7874 0d0a 0d0a   / self.maxt....
+00000b80: 2020 2020 2020 2020 666f 7220 616e 696d          for anim
+00000b90: 2069 6e20 7365 6c66 2e61 6e69 6d73 3a0d   in self.anims:.
+00000ba0: 0a20 2020 2020 2020 2020 2020 2061 6e69  .            ani
+00000bb0: 6d2e 636f 6d70 7574 655f 676c 6f62 616c  m.compute_global
+00000bc0: 5f72 616e 6765 280d 0a20 2020 2020 2020  _range(..       
+00000bd0: 2020 2020 2020 2020 2073 656c 662e 676c           self.gl
+00000be0: 6f62 616c 5f72 616e 6765 2e61 7420 2b20  obal_range.at + 
+00000bf0: 616e 696d 2e6c 6f63 616c 5f72 616e 6765  anim.local_range
+00000c00: 2e61 7420 2a20 6661 6374 6f72 2c0d 0a20  .at * factor,.. 
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00000c20: 6e69 6d2e 6c6f 6361 6c5f 7261 6e67 652e  nim.local_range.
+00000c30: 6475 7261 7469 6f6e 202a 2066 6163 746f  duration * facto
+00000c40: 720d 0a20 2020 2020 2020 2020 2020 2029  r..            )
+00000c50: 0d0a 0d0a 2020 2020 6465 6620 616e 696d  ....    def anim
+00000c60: 5f70 7265 5f69 6e69 7428 7365 6c66 2920  _pre_init(self) 
+00000c70: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+00000c80: 2020 666f 7220 616e 696d 2069 6e20 7365    for anim in se
+00000c90: 6c66 2e61 6e69 6d73 3a0d 0a20 2020 2020  lf.anims:..     
+00000ca0: 2020 2020 2020 2061 6e69 6d2e 616e 696d         anim.anim
+00000cb0: 5f70 7265 5f69 6e69 7428 290d 0a0d 0a20  _pre_init().... 
+00000cc0: 2020 2064 6566 2061 6e69 6d5f 696e 6974     def anim_init
+00000cd0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0d  (self) -> None:.
+00000ce0: 0a20 2020 2020 2020 2066 6f72 2061 6e69  .        for ani
+00000cf0: 6d20 696e 2073 656c 662e 616e 696d 733a  m in self.anims:
+00000d00: 0d0a 2020 2020 2020 2020 2020 2020 616e  ..            an
+00000d10: 696d 2e61 6e69 6d5f 696e 6974 2829 0d0a  im.anim_init()..
+00000d20: 0d0a 2020 2020 6465 6620 6765 745f 616e  ..    def get_an
+00000d30: 696d 5f74 2873 656c 662c 2061 6c70 6861  im_t(self, alpha
+00000d40: 3a20 666c 6f61 742c 2061 6e69 6d3a 2041  : float, anim: A
+00000d50: 6e69 6d61 7469 6f6e 2920 2d3e 2066 6c6f  nimation) -> flo
+00000d60: 6174 3a0d 0a20 2020 2020 2020 2072 6574  at:..        ret
+00000d70: 7572 6e20 616c 7068 6120 2a20 7365 6c66  urn alpha * self
+00000d80: 2e6d 6178 7420 2d20 616e 696d 2e6c 6f63  .maxt - anim.loc
+00000d90: 616c 5f72 616e 6765 2e61 740d 0a0d 0a20  al_range.at.... 
+00000da0: 2020 2064 6566 2061 6e69 6d5f 6f6e 5f61     def anim_on_a
+00000db0: 6c70 6861 2873 656c 662c 2061 6c70 6861  lpha(self, alpha
+00000dc0: 3a20 666c 6f61 7429 202d 3e20 4e6f 6e65  : float) -> None
+00000dd0: 3a0d 0a20 2020 2020 2020 2027 2727 0d0a  :..        '''..
+00000de0: 2020 2020 2020 2020 e59c a8e8 afa5 e696          ........
+00000df0: b9e6 b395 e4b8 adef bc8c 3a63 6c61 7373  ..........:class
+00000e00: 3a60 416e 696d 4772 6f75 7060 20e9 809a  :`AnimGroup` ...
+00000e10: e8bf 8720 6060 616c 7068 6160 600d 0a20  ... ``alpha``.. 
+00000e20: 2020 2020 2020 20e6 8da2 e7ae 97e5 87ba         .........
+00000e30: e5ad 90e5 8aa8 e794 bbe7 9a84 2060 606c  ............ ``l
+00000e40: 6f63 616c 5f74 6060 20e5 b9b6 e8b0 83e7  ocal_t`` .......
+00000e50: 94a8 e5ad 90e5 8aa8 e794 bbe7 9a84 203a  .............. :
+00000e60: 6d65 7468 3a60 7e2e 416e 696d 6174 696f  meth:`~.Animatio
+00000e70: 6e2e 616e 696d 5f6f 6e60 20e6 96b9 e6b3  n.anim_on` .....
+00000e80: 950d 0a20 2020 2020 2020 2027 2727 0d0a  ...        '''..
+00000e90: 2020 2020 2020 2020 676c 6f62 616c 5f74          global_t
+00000ea0: 203d 2073 656c 662e 676c 6f62 616c 5f74   = self.global_t
+00000eb0: 5f63 7478 2e67 6574 2829 0d0a 0d0a 2020  _ctx.get()....  
+00000ec0: 2020 2020 2020 666f 7220 616e 696d 2069        for anim i
+00000ed0: 6e20 7365 6c66 2e61 6e69 6d73 3a0d 0a20  n self.anims:.. 
+00000ee0: 2020 2020 2020 2020 2020 2061 6e69 6d5f             anim_
+00000ef0: 7420 3d20 7365 6c66 2e67 6574 5f61 6e69  t = self.get_ani
+00000f00: 6d5f 7428 616c 7068 612c 2061 6e69 6d29  m_t(alpha, anim)
+00000f10: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000f20: 2061 6e69 6d2e 676c 6f62 616c 5f72 616e   anim.global_ran
+00000f30: 6765 2e61 7420 3c3d 2067 6c6f 6261 6c5f  ge.at <= global_
+00000f40: 7420 3c20 616e 696d 2e67 6c6f 6261 6c5f  t < anim.global_
+00000f50: 7261 6e67 652e 656e 643a 0d0a 2020 2020  range.end:..    
+00000f60: 2020 2020 2020 2020 2020 2020 616e 696d              anim
+00000f70: 2e61 6e69 6d5f 6f6e 2861 6e69 6d5f 7429  .anim_on(anim_t)
+00000f80: 0d0a 0d0a 0d0a 636c 6173 7320 5375 6363  ......class Succ
+00000f90: 6573 7369 6f6e 2841 6e69 6d47 726f 7570  ession(AnimGroup
+00000fa0: 293a 0d0a 2020 2020 2727 270d 0a20 2020  ):..    '''..   
+00000fb0: 20e5 8aa8 e794 bbe9 9b86 e590 88ef bc88   ...............
+00000fc0: e9a1 bae5 ba8f e689 a7e8 a18c efbc 890d  ................
+00000fd0: 0a0d 0a20 2020 202d 20e4 bc9a e5b0 86e4  ...    - .......
+00000fe0: bca0 e585 a5e7 9a84 e58a a8e7 94bb e4be  ................
+00000ff0: 9de6 aca1 e689 a7e8 a18c efbc 8ce4 b88d  ................
+00001000: e5b9 b6e8 a18c 0d0a 2020 2020 2d20 e58f  ........    - ..
+00001010: afe4 bba5 e4bc a0e5 85a5 2060 6275 6666  .......... `buff
+00001020: 6020 e68c 87e5 ae9a e589 8de5 908e e58a  ` ..............
+00001030: a8e7 94bb e4b8 ade9 97b4 e79a 84e7 a9ba  ................
+00001040: e799 bde6 97b6 e997 b40d 0a20 2020 202d  ...........    -
+00001050: 20e5 85b6 e4bd 99e4 b88e 2060 416e 696d   ......... `Anim
+00001060: 4772 6f75 7060 20e7 9bb8 e590 8c0d 0a0d  Group` .........
+00001070: 0a20 2020 20e6 97b6 e997 b4e7 a4ba e4be  .    ...........
+00001080: 8bef bc9a 0d0a 0d0a 2020 2020 2e2e 2063  ........    .. c
+00001090: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+000010a0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 5375  on....        Su
+000010b0: 6363 6573 7369 6f6e 280d 0a20 2020 2020  ccession(..     
+000010c0: 2020 2020 2020 2041 6e69 6d31 2864 7572         Anim1(dur
+000010d0: 6174 696f 6e3d 3329 2c0d 0a20 2020 2020  ation=3),..     
+000010e0: 2020 2020 2020 2041 6e69 6d32 2864 7572         Anim2(dur
+000010f0: 6174 696f 6e3d 3429 0d0a 2020 2020 2020  ation=4)..      
+00001100: 2020 2920 2320 416e 696d 3120 e59c a820    ) # Anim1 ... 
+00001110: 307e 3373 20e6 89a7 e8a1 8cef bc8c 416e  0~3s .........An
+00001120: 696d 3220 e59c a820 337e 3773 20e6 89a7  im2 ... 3~7s ...
+00001130: e8a1 8c0d 0a0d 0a20 2020 2020 2020 2053  .......        S
+00001140: 7563 6365 7373 696f 6e28 0d0a 2020 2020  uccession(..    
+00001150: 2020 2020 2020 2020 416e 696d 3128 6475          Anim1(du
+00001160: 7261 7469 6f6e 3d32 292c 0d0a 2020 2020  ration=2),..    
+00001170: 2020 2020 2020 2020 416e 696d 3228 6174          Anim2(at
+00001180: 3d31 2c20 6475 7261 7469 6f6e 3d32 292c  =1, duration=2),
+00001190: 0d0a 2020 2020 2020 2020 2020 2020 416e  ..            An
+000011a0: 696d 3328 6174 3d30 2e35 2c20 6475 7261  im3(at=0.5, dura
+000011b0: 7469 6f6e 3d32 290d 0a20 2020 2020 2020  tion=2)..       
+000011c0: 2029 2023 2041 6e69 6d31 20e5 9ca8 2030   ) # Anim1 ... 0
+000011d0: 7e32 7320 e689 a7e8 a18c efbc 8c41 6e69  ~2s .........Ani
+000011e0: 6d32 20e5 9ca8 2033 7e35 7320 e689 a7e8  m2 ... 3~5s ....
+000011f0: a18c efbc 8c41 6e69 6d33 20e5 9ca8 2035  .....Anim3 ... 5
+00001200: 2e35 7e37 2e35 7320 e689 a7e8 a18c 0d0a  .5~7.5s ........
+00001210: 0d0a 2020 2020 2020 2020 5375 6363 6573  ..        Succes
+00001220: 7369 6f6e 280d 0a20 2020 2020 2020 2020  sion(..         
+00001230: 2020 2041 6e69 6d31 2864 7572 6174 696f     Anim1(duratio
+00001240: 6e3d 3229 2c0d 0a20 2020 2020 2020 2020  n=2),..         
+00001250: 2020 2041 6e69 6d32 2864 7572 6174 696f     Anim2(duratio
+00001260: 6e3d 3229 2c0d 0a20 2020 2020 2020 2020  n=2),..         
+00001270: 2020 2041 6e69 6d33 2864 7572 6174 696f     Anim3(duratio
+00001280: 6e3d 3229 2c0d 0a20 2020 2020 2020 2020  n=2),..         
+00001290: 2020 2062 7566 663d 302e 350d 0a20 2020     buff=0.5..   
+000012a0: 2020 2020 2029 2023 2041 6e69 6d31 20e5       ) # Anim1 .
+000012b0: 9ca8 2030 7e32 7320 e689 a7e8 a18c efbc  .. 0~2s ........
+000012c0: 8c41 6e69 6d32 20e5 9ca8 2032 2e35 7e34  .Anim2 ... 2.5~4
+000012d0: 2e35 7320 e689 a7e8 a18c efbc 8c41 6e69  .5s .........Ani
+000012e0: 6d33 20e5 9ca8 2035 7e37 7320 e689 a7e8  m3 ... 5~7s ....
+000012f0: a18c 0d0a 2020 2020 2727 270d 0a20 2020  ....    '''..   
+00001300: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00001310: 6c66 2c20 2a61 6e69 6d73 3a20 416e 696d  lf, *anims: Anim
+00001320: 6174 696f 6e2c 2062 7566 663a 2066 6c6f  ation, buff: flo
+00001330: 6174 203d 2030 2c20 2a2a 6b77 6172 6773  at = 0, **kwargs
+00001340: 293a 0d0a 2020 2020 2020 2020 616e 696d  ):..        anim
+00001350: 7320 3d20 7365 6c66 2e5f 6765 745f 616e  s = self._get_an
+00001360: 696d 5f6f 626a 6563 7473 2861 6e69 6d73  im_objects(anims
+00001370: 290d 0a20 2020 2020 2020 2065 6e64 5f74  )..        end_t
+00001380: 696d 6520 3d20 300d 0a20 2020 2020 2020  ime = 0..       
+00001390: 2066 6f72 2061 6e69 6d20 696e 2061 6e69   for anim in ani
+000013a0: 6d73 3a0d 0a20 2020 2020 2020 2020 2020  ms:..           
+000013b0: 2061 6e69 6d2e 6c6f 6361 6c5f 7261 6e67   anim.local_rang
+000013c0: 652e 6174 202b 3d20 656e 645f 7469 6d65  e.at += end_time
+000013d0: 0d0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+000013e0: 645f 7469 6d65 203d 2061 6e69 6d2e 6c6f  d_time = anim.lo
+000013f0: 6361 6c5f 7261 6e67 652e 656e 6420 2b20  cal_range.end + 
+00001400: 6275 6666 0d0a 2020 2020 2020 2020 7375  buff..        su
+00001410: 7065 7228 292e 5f5f 696e 6974 5f5f 282a  per().__init__(*
+00001420: 616e 696d 732c 205f 6765 745f 616e 696d  anims, _get_anim
+00001430: 5f6f 626a 6563 7473 3d46 616c 7365 2c20  _objects=False, 
+00001440: 2a2a 6b77 6172 6773 290d 0a0d 0a0d 0a63  **kwargs)......c
+00001450: 6c61 7373 2041 6c69 676e 6564 2841 6e69  lass Aligned(Ani
+00001460: 6d47 726f 7570 293a 0d0a 2020 2020 2727  mGroup):..    ''
+00001470: 270d 0a20 2020 20e5 8aa8 e794 bbe9 9b86  '..    .........
+00001480: e590 88ef bc88 e5b9 b6e5 8897 e5af b9e9  ................
+00001490: bd90 e689 a7e8 a18c efbc 890d 0a0d 0a20  ............... 
+000014a0: 2020 20e6 97b6 e997 b4e7 a4ba e4be 8bef     .............
+000014b0: bc9a 0d0a 0d0a 2020 2020 2e2e 2063 6f64  ......    .. cod
+000014c0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
+000014d0: 0d0a 0d0a 2020 2020 2020 2020 416c 6967  ....        Alig
+000014e0: 6e65 6428 0d0a 2020 2020 2020 2020 2020  ned(..          
+000014f0: 2020 416e 696d 3128 6475 7261 7469 6f6e    Anim1(duration
+00001500: 3d31 292c 0d0a 2020 2020 2020 2020 2020  =1),..          
+00001510: 2020 416e 696d 3228 6475 7261 7469 6f6e    Anim2(duration
+00001520: 3d32 290d 0a20 2020 2020 2020 2029 2023  =2)..        ) #
+00001530: 2041 6e69 6d31 20e5 928c 2041 6e69 6d32   Anim1 ... Anim2
+00001540: 20e9 83bd e59c a820 307e 3273 20e6 89a7   ...... 0~2s ...
+00001550: e8a1 8c0d 0a0d 0a20 2020 2020 2020 2041  .......        A
+00001560: 6c69 676e 6564 280d 0a20 2020 2020 2020  ligned(..       
+00001570: 2020 2020 2041 6e69 6d31 2864 7572 6174       Anim1(durat
+00001580: 696f 6e3d 3129 2c0d 0a20 2020 2020 2020  ion=1),..       
+00001590: 2020 2020 2041 6e69 6d32 2864 7572 6174       Anim2(durat
+000015a0: 696f 6e3d 3229 2c0d 0a20 2020 2020 2020  ion=2),..       
+000015b0: 2020 2020 2064 7572 6174 696f 6e3d 340d       duration=4.
+000015c0: 0a20 2020 2020 2020 2029 2023 2041 6e69  .        ) # Ani
+000015d0: 6d31 20e5 928c 2041 6e69 6d32 20e9 83bd  m1 ... Anim2 ...
+000015e0: e59c a820 307e 3473 20e6 89a7 e8a1 8c0d  ... 0~4s .......
+000015f0: 0a20 2020 2027 2727 0d0a 2020 2020 6465  .    '''..    de
+00001600: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00001610: 202a 616e 696d 733a 2041 6e69 6d61 7469   *anims: Animati
+00001620: 6f6e 2c20 6475 7261 7469 6f6e 3a20 666c  on, duration: fl
+00001630: 6f61 7420 7c20 4e6f 6e65 203d 204e 6f6e  oat | None = Non
+00001640: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+00001650: 2020 2020 2020 2061 6e69 6d73 203d 2073         anims = s
+00001660: 656c 662e 5f67 6574 5f61 6e69 6d5f 6f62  elf._get_anim_ob
+00001670: 6a65 6374 7328 616e 696d 7329 0d0a 2020  jects(anims)..  
+00001680: 2020 2020 2020 6966 2064 7572 6174 696f        if duratio
+00001690: 6e20 6973 204e 6f6e 653a 0d0a 2020 2020  n is None:..    
+000016a0: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
+000016b0: 203d 206d 6178 2861 6e69 6d2e 6c6f 6361   = max(anim.loca
+000016c0: 6c5f 7261 6e67 652e 656e 6420 666f 7220  l_range.end for 
+000016d0: 616e 696d 2069 6e20 616e 696d 7329 0d0a  anim in anims)..
+000016e0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
+000016f0: 292e 5f5f 696e 6974 5f5f 282a 616e 696d  ).__init__(*anim
+00001700: 732c 2064 7572 6174 696f 6e3d 6475 7261  s, duration=dura
+00001710: 7469 6f6e 2c20 5f67 6574 5f61 6e69 6d5f  tion, _get_anim_
+00001720: 6f62 6a65 6374 733d 4661 6c73 652c 202a  objects=False, *
+00001730: 2a6b 7761 7267 7329 0d0a 0d0a 2020 2020  *kwargs)....    
+00001740: 6465 6620 636f 6d70 7574 655f 676c 6f62  def compute_glob
+00001750: 616c 5f72 616e 6765 2873 656c 662c 2061  al_range(self, a
+00001760: 743a 2066 6c6f 6174 2c20 6475 7261 7469  t: float, durati
+00001770: 6f6e 3a20 666c 6f61 7429 202d 3e20 4e6f  on: float) -> No
+00001780: 6e65 3a0d 0a20 2020 2020 2020 2041 6e69  ne:..        Ani
+00001790: 6d61 7469 6f6e 2e63 6f6d 7075 7465 5f67  mation.compute_g
+000017a0: 6c6f 6261 6c5f 7261 6e67 6528 7365 6c66  lobal_range(self
+000017b0: 2c20 6174 2c20 6475 7261 7469 6f6e 290d  , at, duration).
+000017c0: 0a0d 0a20 2020 2020 2020 2066 6f72 2061  ...        for a
+000017d0: 6e69 6d20 696e 2073 656c 662e 616e 696d  nim in self.anim
+000017e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000017f0: 6661 6374 6f72 203d 2064 7572 6174 696f  factor = duratio
+00001800: 6e20 2f20 616e 696d 2e6c 6f63 616c 5f72  n / anim.local_r
+00001810: 616e 6765 2e65 6e64 0d0a 2020 2020 2020  ange.end..      
+00001820: 2020 2020 2020 616e 696d 2e63 6f6d 7075        anim.compu
+00001830: 7465 5f67 6c6f 6261 6c5f 7261 6e67 6528  te_global_range(
+00001840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001850: 2020 7365 6c66 2e67 6c6f 6261 6c5f 7261    self.global_ra
+00001860: 6e67 652e 6174 202b 2061 6e69 6d2e 6c6f  nge.at + anim.lo
+00001870: 6361 6c5f 7261 6e67 652e 6174 202a 2066  cal_range.at * f
+00001880: 6163 746f 722c 0d0a 2020 2020 2020 2020  actor,..        
+00001890: 2020 2020 2020 2020 616e 696d 2e6c 6f63          anim.loc
+000018a0: 616c 5f72 616e 6765 2e64 7572 6174 696f  al_range.duratio
+000018b0: 6e20 2a20 6661 6374 6f72 0d0a 2020 2020  n * factor..    
+000018c0: 2020 2020 2020 2020 290d 0a                      )..
```

### Comparing `janim-1.0.2/janim/anims/creation.py` & `janim-1.0.3/janim/anims/creation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/display.py` & `janim-1.0.3/janim/anims/display.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/fading.py` & `janim-1.0.3/janim/anims/fading.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/growing.py` & `janim-1.0.3/janim/anims/growing.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/indication.py` & `janim-1.0.3/janim/anims/indication.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/rotation.py` & `janim-1.0.3/janim/anims/rotation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/timeline.py` & `janim-1.0.3/janim/anims/timeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from collections import defaultdict
 from contextvars import ContextVar
 from dataclasses import dataclass
 from typing import Callable, Iterable, Self, overload
 
 import moderngl as mgl
 import numpy as np
+from PIL import Image
 
 from janim.anims.animation import Animation, TimeRange
 from janim.anims.composition import AnimGroup
 from janim.anims.display import Display
 from janim.anims.updater import updater_params_ctx
 from janim.camera.camera import Camera
 from janim.constants import BLACK, DEFAULT_DURATION, DOWN, SMALL_BUFF, UP
@@ -81,15 +82,15 @@
             self.token = config_ctx_var.set(lst)
             return self
 
         def __exit__(self, exc_type, exc_value, tb) -> None:
             config_ctx_var.reset(self.token)
 
     @classmethod
-    def _with_config(cls) -> _WithConfig:
+    def with_config(cls) -> _WithConfig:
         '''
         使用定义在 :class:`Timeline` 子类中的 config
         '''
         return cls._WithConfig(cls)
 
     # endregion
 
@@ -176,15 +177,15 @@
         '''
         pass    # pragma: no cover
 
     def build(self, *, quiet=False) -> TimelineAnim:
         '''
         构建动画并返回
         '''
-        with self._with_config(), ContextSetter(self.ctx_var, self):
+        with self.with_config(), ContextSetter(self.ctx_var, self):
 
             self.config_getter = ConfigGetter(config_ctx_var.get())
             self.camera = Camera()
 
             self._build_frame = inspect.currentframe()
 
             if not quiet:   # pragma: no cover
@@ -729,7 +730,43 @@
                         reverse=True
                     )
                     for render_call in render_calls:
                         render_call.func()
 
         except Exception:
             traceback.print_exc()
+
+    capture_ctx: mgl.Context | None = None
+    capture_fbo: mgl.Framebuffer | None = None
+
+    def capture(self) -> Image.Image:
+        if TimelineAnim.capture_ctx is None:
+            TimelineAnim.capture_ctx = mgl.create_standalone_context(require=430)
+            TimelineAnim.capture_ctx.enable(mgl.BLEND)
+            TimelineAnim.capture_ctx.blend_func = (
+                mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
+                mgl.ONE, mgl.ONE
+            )
+            TimelineAnim.capture_ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
+
+            pw, ph = self.cfg.pixel_width, self.cfg.pixel_height
+            TimelineAnim.capture_fbo = TimelineAnim.capture_ctx.framebuffer(
+                color_attachments=TimelineAnim.capture_ctx.texture(
+                    (pw, ph),
+                    components=4,
+                    samples=0,
+                ),
+                depth_attachment=TimelineAnim.capture_ctx.depth_renderbuffer(
+                    (pw, ph),
+                    samples=0
+                )
+            )
+
+        fbo = TimelineAnim.capture_fbo
+        fbo.use()
+        fbo.clear(*self.cfg.background_color.rgb)
+        self.render_all(TimelineAnim.capture_ctx)
+
+        return Image.frombytes(
+            "RGBA", fbo.size, fbo.read(components=4),
+            "raw", "RGBA", 0, -1
+        )
```

### Comparing `janim-1.0.2/janim/anims/transform.py` & `janim-1.0.3/janim/anims/transform.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/anims/updater.py` & `janim-1.0.3/janim/anims/updater.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/camera/camera.py` & `janim-1.0.3/janim/camera/camera.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/camera/camera_info.py` & `janim-1.0.3/janim/camera/camera_info.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/cli.py` & `janim-1.0.3/janim/cli.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/component.py` & `janim-1.0.3/janim/components/component.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/data.py` & `janim-1.0.3/janim/components/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/depth.py` & `janim-1.0.3/janim/components/depth.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/image.py` & `janim-1.0.3/janim/components/image.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/points.py` & `janim-1.0.3/janim/components/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,17 +531,21 @@
         '''
         将物件缩放指定倍数
 
         如果传入的倍数是可遍历的对象，那么则将其中的各个元素作为坐标各分量缩放的倍数，
         例如传入 ``scale_factor`` 为 ``(2, 0.5, 1)`` 则是在 ``x`` 方向上缩放为两倍，在 ``y`` 方向上压缩为原来的一半，在 ``z`` 方向上保持不变
         '''
         if isinstance(scale_factor, Iterable):
-            scale_factor = np.array(scale_factor).clip(min=min_scale_factor)
+            sgn = np.sign(scale_factor)
+            scale_factor = sgn * abs(np.array(scale_factor)).clip(min=min_scale_factor)
         else:
-            scale_factor = max(scale_factor, min_scale_factor)
+            if scale_factor >= 0:
+                scale_factor = max(scale_factor, min_scale_factor)
+            else:
+                scale_factor = min(scale_factor, -min_scale_factor)
 
         self.apply_points_fn(
             lambda points: scale_factor * points,
             about_point=about_point,
             about_edge=about_edge,
             root_only=root_only
         )
```

### Comparing `janim-1.0.2/janim/components/radius.py` & `janim-1.0.3/janim/components/radius.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/rgbas.py` & `janim-1.0.3/janim/components/rgbas.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/components/vpoints.py` & `janim-1.0.3/janim/components/vpoints.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/constants/colors.py` & `janim-1.0.3/janim/constants/colors.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/examples.py` & `janim-1.0.3/janim/examples.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/exception.py` & `janim-1.0.3/janim/exception.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/gui/anim_viewer.py` & `janim-1.0.3/janim/gui/anim_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,15 +402,19 @@
 
         self.setup_audio_player()
         self.play_timer.duration = 1 / self.anim.cfg.preview_fps
         progress = int(progress * self.anim.cfg.preview_fps / preview_fps)
 
         self.anim.anim_on(self.timeline_view.progress_to_time(progress))
 
+        self.fixed_ratio_widget.set_src_size((self.anim.cfg.pixel_width,
+                                              self.anim.cfg.pixel_height))
+
         self.glw.anim = self.anim
+        self.glw.update_clear_color()
         self.glw.update()
 
         range = self.timeline_view.range
         self.timeline_view.set_anim(self.anim)
         self.timeline_view.set_progress(progress)
         self.timeline_view.range = range
 
@@ -590,15 +594,15 @@
         self.labels_info: list[TimelineView.LabelInfo] = []
         self.max_row = 0
 
         self.flatten = self.anim.user_anim.flatten()[1:]
         self._sorted_anims = None
 
         stack: list[Animation] = []
-        for anim in self.flatten:
+        for anim in self.get_sorted_anims():
             # 可能会因为浮点误差导致 <= 中的相等判断错误，所以 +1e-5
             while stack and stack[-1].global_range.end <= anim.global_range.at + 1e-5:
                 stack.pop()
 
             self.labels_info.append(TimelineView.LabelInfo(anim, len(stack)))
             self.max_row = max(self.max_row, len(stack))
             stack.append(anim)
@@ -1003,15 +1007,16 @@
 
                 self.paint_label(p,
                                  info.range,
                                  audio_rect.y(),
                                  self.audio_height,
                                  info.audio.filename,
                                  QColor(152, 255, 191),
-                                 QColor(152, 255, 191, 128))
+                                 QColor(152, 255, 191, 128),
+                                 False)
 
             p.setFont(orig_font)
 
         # 绘制动画区段
         bottom_rect = self.bottom_rect
         p.setClipRect(bottom_rect)
 
@@ -1021,15 +1026,16 @@
 
             self.paint_label(p,
                              info.anim.global_range,
                              bottom_rect.y() + self.label_y(info.row),
                              self.label_height,
                              info.anim.__class__.__name__,
                              Qt.PenStyle.NoPen,
-                             QColor(*info.anim.label_color).lighter())
+                             QColor(*info.anim.label_color).lighter(),
+                             True)
 
         p.setClipping(False)
 
         # 绘制当前进度指示
         p.setPen(QPen(Qt.GlobalColor.white, 2))
         p.setRenderHint(QPainter.RenderHint.Antialiasing, True)
         self.paint_line(p, self.progress_to_time(self._progress))
@@ -1070,49 +1076,60 @@
         p: QPainter,
         time_range: TimeRange,
         y: float,
         height: float,
         txt: str,
         stroke: QPen | QColor,
         fill: QBrush | QColor,
+        is_anim_lable: bool
     ) -> None:
         range = self.time_range_to_pixel_range(time_range)
         rect = QRectF(range.left, y, range.width, height)
 
         # 标记是否应当绘制文字
-        draw_txt = True
+        out_of_boundary = False
 
-        # 使得超出底端的区段也能看到一条边
-        max_y = self.height() - self.range_tip_height - 4
-        if rect.y() > max_y:
-            rect.setY(max_y)
-            rect.setBottom(self.height() + 2)
-            draw_txt = False
+        if is_anim_lable:
+            # 使得超出底端的区段也能看到一条边
+            max_y = self.height() - self.range_tip_height - 4
+            if rect.y() > max_y:
+                rect.moveTop(max_y)
+                rect.setHeight(4)
+                out_of_boundary = True
+
+            # 使得超出顶端的区段也能看到一条边
+            top_margin = self.audio_height if self.anim.timeline.has_audio() else 0
+            min_bottom = top_margin + 4
+            if rect.bottom() < min_bottom:
+                rect.moveTop(top_margin)
+                rect.setHeight(4)
+                out_of_boundary = True
 
         # 这里的判断使得区段过窄时也能看得见
         if rect.width() > 5:
             x_adjust = 2
         elif rect.width() > 1:
             x_adjust = (rect.width() - 1) / 2
         else:
             x_adjust = 0
 
         # 绘制背景部分
-        rect.adjust(x_adjust, 2, -x_adjust, -2)
+        if not out_of_boundary:
+            rect.adjust(x_adjust, 2, -x_adjust, -2)
         p.setPen(stroke)
         p.setBrush(fill)
         p.drawRect(rect)
 
         # 使得在区段的左侧有一部分在显示区域外时，
         # 文字仍然对齐到屏幕的左端，而不是跑到屏幕外面去
         if rect.x() < 0:
             rect.setX(0)
 
         # 绘制文字
-        if draw_txt:
+        if not out_of_boundary:
             rect.adjust(1, 1, -1, -1)
             p.setPen(Qt.GlobalColor.black)
             p.drawText(
                 rect,
                 Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop,
                 txt
             )
```

### Comparing `janim-1.0.2/janim/gui/audio_player.py` & `janim-1.0.3/janim/gui/audio_player.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/gui/export.png` & `janim-1.0.3/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/gui/fixed_ratio_widget.py` & `janim-1.0.3/janim/gui/fixed_ratio_widget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 
+from PySide6.QtCore import QSize
 from PySide6.QtGui import QResizeEvent
 from PySide6.QtWidgets import QWidget
 
 
 class FixedRatioWidget(QWidget):
     '''
     使得传入的 ``inside`` 控件可以以固定比例塞在该控件中
     '''
     def __init__(self, inside: QWidget, src_size: tuple[float, float], parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.inside = inside
         self.inside.setParent(self)
         self.src_size = src_size
 
-    def resizeEvent(self, event: QResizeEvent) -> None:
-        super().resizeEvent(event)
+    def set_src_size(self, size: tuple[float, float]) -> None:
+        self.src_size = size
+        self.update_inner_size(self.size())
 
-        wnd_width, wnd_height = event.size().toTuple()
+    def update_inner_size(self, wnd_size: QSize) -> None:
+        wnd_width, wnd_height = wnd_size.toTuple()
         w, h = get_proportional_scale_size(*self.src_size, wnd_width, wnd_height)
         self.inside.setGeometry(
             (wnd_width - w) // 2,
             (wnd_height - h) // 2,
             w, h
         )
 
+    def resizeEvent(self, event: QResizeEvent) -> None:
+        super().resizeEvent(event)
+        self.update_inner_size(event.size())
+
 
 def get_proportional_scale_size(src_width, src_height, tg_width, tg_height):
     '''
     根据 ``(tg_width, tg_height)`` 的目标大小信息，
     得到 ``(src_width, src_height)`` 在进行等比缩放后能塞进目标区域的最大大小
     '''
     factor1 = tg_width / src_width
```

### Comparing `janim-1.0.2/janim/gui/glwidget.py` & `janim-1.0.3/janim/gui/glwidget.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,23 +12,35 @@
     窗口中央的渲染界面
     '''
     rendered = Signal()
 
     def __init__(self, anim: TimelineAnim, parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.anim = anim
+        self.needs_update_clear_color = False
 
     def set_time(self, time: float) -> None:
         self.anim.anim_on(time)
         self.update()
 
     def initializeGL(self) -> None:
         self.ctx = mgl.create_context()
         self.ctx.enable(mgl.BLEND)
+        self.ctx.blend_func = (
+            mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
+            mgl.ONE, mgl.ONE
+        )
+        self.ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
+
         self.qfuncs = self.context().functions()
+        self.update_clear_color()
 
-        self.ctx.clear(*self.anim.cfg.background_color.rgb)
+    def update_clear_color(self) -> None:
+        self.needs_update_clear_color = True
 
     def paintGL(self) -> None:
+        if self.needs_update_clear_color:
+            self.qfuncs.glClearColor(*self.anim.cfg.background_color.rgb, 0.)
+            self.needs_update_clear_color = False
         self.qfuncs.glClear(0x00004000 | 0x00000100)    # GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT
         self.anim.render_all(self.ctx)
         self.rendered.emit()
```

### Comparing `janim-1.0.2/janim/gui/precise_timer.py` & `janim-1.0.3/janim/gui/precise_timer.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/gui/richtext_editor.py` & `janim-1.0.3/janim/gui/richtext_editor.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/gui/selector.py` & `janim-1.0.3/janim/gui/selector.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/imports.py` & `janim-1.0.3/janim/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,7 +39,8 @@
 from janim.utils.config import Config
 from janim.utils.file_ops import *
 from janim.utils.iterables import *
 from janim.utils.paths import *
 from janim.utils.rate_functions import *
 from janim.utils.simple_functions import *
 from janim.utils.space_ops import *
+from janim.exception import *
```

### Comparing `janim-1.0.2/janim/items/audio.py` & `janim-1.0.3/janim/items/audio.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/boolean_ops.py` & `janim-1.0.3/janim/items/boolean_ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import numpy as np
 import pathops
 
 from janim.exception import BooleanOpsError
+from janim.items.item import Item
 from janim.items.vitem import VItem
 from janim.utils.bezier import PathBuilder
 
 # Boolean operations between 2D mobjects
 # Borrowed from from https://github.com/ManimCommunity/manim/
 
 
@@ -65,21 +66,30 @@
     def __init__(self, *vitems: VItem, **kwargs):
         if len(vitems) < 2:
             raise BooleanOpsError("At least 2 items needed for Union.")
         super().__init__(**kwargs)
         outpen = pathops.Path()
         pathops.union(
             [
-                _convert_vitem_to_skia_path(vmobject)
-                for vmobject in vitems
+                _convert_vitem_to_skia_path(vitem)
+                for vitem in vitems
             ],
             outpen.getPen()
         )
         _convert_skia_path_to_vitem(outpen, self)
 
+    @staticmethod
+    def from_item(item: Item, **kwargs) -> Union:
+        lst = [
+            sub
+            for sub in item.walk_self_and_descendants()
+            if isinstance(sub, VItem)
+        ]
+        return Union(*lst, **kwargs)
+
 
 class Difference(VItem):
     '''
     差集
 
     传入 ``subitem`` 和 ``clip``，返回 ``subitem`` 裁去 ``clip`` 区域的轮廓线
     '''
@@ -96,35 +106,44 @@
 
 class Intersection(VItem):
     '''
     交集
 
     传入两个及以上 :class:`~.VItem`，返回它们区域交集的外轮廓
     '''
-    def __init__(self, *vmobjects: VItem, **kwargs):
-        if len(vmobjects) < 2:
+    def __init__(self, *vitems: VItem, **kwargs):
+        if len(vitems) < 2:
             raise BooleanOpsError("At least 2 items needed for Intersection.")
         super().__init__(**kwargs)
         outpen = pathops.Path()
         pathops.intersection(
-            [_convert_vitem_to_skia_path(vmobjects[0])],
-            [_convert_vitem_to_skia_path(vmobjects[1])],
+            [_convert_vitem_to_skia_path(vitems[0])],
+            [_convert_vitem_to_skia_path(vitems[1])],
             outpen.getPen(),
         )
         new_outpen = outpen
-        for _i in range(2, len(vmobjects)):
+        for _i in range(2, len(vitems)):
             new_outpen = pathops.Path()
             pathops.intersection(
                 [outpen],
-                [_convert_vitem_to_skia_path(vmobjects[_i])],
+                [_convert_vitem_to_skia_path(vitems[_i])],
                 new_outpen.getPen(),
             )
             outpen = new_outpen
         _convert_skia_path_to_vitem(outpen, self)
 
+    @staticmethod
+    def from_item(item: Item) -> Union:
+        lst = [
+            sub
+            for sub in item.walk_self_and_descendants()
+            if isinstance(sub, VItem)
+        ]
+        return Intersection(*lst)
+
 
 class Exclusion(VItem):
     '''
     补集
 
     传入两个及以上 :class:`~.VItem`，返回它们的区域经过 XOR 运算后的外轮廓
     '''
```

### Comparing `janim-1.0.2/janim/items/coordinate/coordinate_systems.py` & `janim-1.0.3/janim/items/coordinate/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/coordinate/functions.py` & `janim-1.0.3/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/coordinate/number_line.py` & `janim-1.0.3/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/geometry/arc.py` & `janim-1.0.3/janim/items/geometry/arc.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/geometry/arrow.py` & `janim-1.0.3/janim/items/geometry/arrow.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/geometry/line.py` & `janim-1.0.3/janim/items/geometry/line.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/geometry/polygon.py` & `janim-1.0.3/janim/items/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/image_item.py` & `janim-1.0.3/janim/items/image_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import moderngl as mgl
 import numpy as np
 
 from janim.components.component import CmptInfo
 from janim.components.image import Cmpt_Image
 from janim.components.rgbas import Cmpt_Rgbas
 from janim.constants import DL, DR, OUT, UL, UR
-from janim.items.item import Item
 from janim.items.points import Points
 from janim.render.impl import ImageItemRenderer
 from janim.render.texture import get_img_from_file
 from janim.utils.config import Config
 from janim.utils.data import AlignedData
 from janim.utils.simple_functions import clip
 from janim.utils.space_ops import cross, det, get_norm, z_to_vector
```

### Comparing `janim-1.0.2/janim/items/item.py` & `janim-1.0.3/janim/items/item.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/points.py` & `janim-1.0.3/janim/items/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/relation.py` & `janim-1.0.3/janim/items/relation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/shape_matchers.py` & `janim-1.0.3/janim/items/shape_matchers.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/svg/brace.py` & `janim-1.0.3/janim/items/svg/brace.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/svg/brace.svg` & `janim-1.0.3/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/svg/svg_item.py` & `janim-1.0.3/janim/items/svg/svg_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/svg/typst.py` & `janim-1.0.3/janim/items/svg/typst.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/text/text.py` & `janim-1.0.3/janim/items/text/text.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/value_tracker.py` & `janim-1.0.3/janim/items/value_tracker.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/items/vitem.py` & `janim-1.0.3/janim/items/vitem.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/render/base.py` & `janim-1.0.3/janim/render/base.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/render/impl.py` & `janim-1.0.3/janim/render/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,16 +220,16 @@
             bytes = new_points.astype('f4').tobytes()
 
             assert len(bytes) == self.vbo_points.size
 
             self.vbo_points.write(bytes)
             self.prev_points = new_points
 
-        if self.prev_img is None or item.image != self.prev_img:
+        if self.prev_img is None or item.image.img is not self.prev_img:
             self.texture = get_texture_from_img(item.image.get())
             self.texture.build_mipmaps()
-            self.prev_img = item.image
+            self.prev_img = item.image.img
 
         self.prog['image'] = 0
         self.texture.filter = item.image.get_filter()
         self.texture.use(0)
         self.vao.render(mgl.TRIANGLE_STRIP)
```

### Comparing `janim-1.0.2/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.0.3/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/render/shaders/vitem.frag.glsl` & `janim-1.0.3/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/render/texture.py` & `janim-1.0.3/janim/render/texture.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,9 +31,11 @@
         return texture
     ctx = Renderer.data_ctx.get().ctx
     texture = ctx.texture(
         size=img.size,
         components=len(img.getbands()),
         data=img.tobytes()
     )
+    texture.repeat_x = False
+    texture.repeat_y = False
     img_to_texture_map[id(img)] = texture
     return texture
```

### Comparing `janim-1.0.2/janim/render/writer.py` & `janim-1.0.3/janim/render/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     - 最后结束 ffmpeg 的调用，完成 _temp 文件的输出
     - 将 _temp 文件改名，删去 "_temp" 后缀，完成视频输出
     '''
     def __init__(self, anim: TimelineAnim):
         self.anim = anim
         self.ctx = mgl.create_standalone_context()
         self.ctx.enable(mgl.BLEND)
+        self.ctx.blend_func = (
+            mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
+            mgl.ONE, mgl.ONE
+        )
+        self.ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
 
         pw, ph = anim.cfg.pixel_width, anim.cfg.pixel_height
         self.fbo = self.ctx.framebuffer(
             color_attachments=self.ctx.texture(
                 (pw, ph),
                 components=4,
                 samples=0,
```

### Comparing `janim-1.0.2/janim/typing.py` & `janim-1.0.3/janim/typing.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/bezier.py` & `janim-1.0.3/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/config.py` & `janim-1.0.3/janim/utils/config.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/data.py` & `janim-1.0.3/janim/utils/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/dict_ops.py` & `janim-1.0.3/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/file_ops.py` & `janim-1.0.3/janim/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/font.py` & `janim-1.0.3/janim/utils/font.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/font_manager.py` & `janim-1.0.3/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/iterables.py` & `janim-1.0.3/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/paths.py` & `janim-1.0.3/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/rate_functions.py` & `janim-1.0.3/janim/utils/rate_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/refresh.py` & `janim-1.0.3/janim/utils/refresh.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/signal.py` & `janim-1.0.3/janim/utils/signal.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/simple_functions.py` & `janim-1.0.3/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/janim/utils/space_ops.py` & `janim-1.0.3/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.2/PKG-INFO` & `janim-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 1.0.2
+Version: 1.0.3
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
```

